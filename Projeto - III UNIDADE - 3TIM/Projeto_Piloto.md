# Projeto Flask para Iniciantes: Lista de Tarefas Simples (To-Do List)

Este guia detalhado é o ponto de partida perfeito para estudantes de programação que querem aprender a construir suas primeiras aplicações web usando **Flask**, um micro-framework Python.

## 🎯 Visão Geral do Projeto

Vamos criar uma **Lista de Tarefas (To-Do List)** simples que roda no seu navegador. Este projeto cobre os conceitos essenciais do desenvolvimento web com Flask:

1.  **Rotas (`@app.route`)**: Como definir os URLs da sua aplicação.
2.  **Templates (Jinja2)**: Como usar arquivos HTML dinâmicos.
3.  **Requisições (`request`)**: Como receber dados de formulários do usuário.

---

## 🛠️ Passo 1: Configuração do Ambiente

Siga estes passos para preparar seu ambiente de desenvolvimento.

### 1. Requisitos

Certifique-se de ter o **Python 3.x** e o **pip** instalados no seu sistema.

### 2. Criar e Ativar o Ambiente Virtual

É crucial isolar as dependências do seu projeto.

```bash
# Crie a pasta do projeto e navegue até ela
mkdir meu_projeto_flask
cd meu_projeto_flask

# Crie o ambiente virtual (venv)
python3 -m venv venv

# Ative o ambiente virtual
# No macOS/Linux:
source venv/bin/activate
# No Windows:
venv\Scripts\activate
````

### 3\. Instalar o Flask

Com o ambiente virtual ativo, instale a biblioteca Flask:

```bash
pip install Flask
```

-----

## 💻 Passo 2: Criando o Arquivo Principal (`app.py`)

Crie o arquivo **`app.py`** na pasta raiz do projeto. Ele contém toda a lógica da nossa aplicação.

```python
# app.py

from flask import Flask, render_template, request, redirect, url_for

# Inicializa a aplicação Flask
app = Flask(__name__)

# Lista simples na memória para armazenar as tarefas.
# ATENÇÃO: Se o servidor for reiniciado, os dados serão perdidos!
tarefas = []

@app.route('/')
def index():
    """
    Rota principal: Exibe a lista de tarefas.
    Renderiza o template 'index.html', passando a lista de tarefas para exibição.
    """
    return render_template('index.html', tarefas=tarefas)

@app.route('/adicionar', methods=['POST'])
def adicionar_tarefa():
    """
    Rota para adicionar uma nova tarefa (acessada via formulário POST).
    """
    # Obtém o valor do campo 'tarefa' do formulário
    nova_tarefa = request.form.get('tarefa')
    
    if nova_tarefa:
        tarefas.append(nova_tarefa)
    
    # Redireciona o usuário de volta para a página inicial
    return redirect(url_for('index'))

@app.route('/remover/<int:tarefa_id>')
def remover_tarefa(tarefa_id):
    """
    Rota para remover uma tarefa específica, identificada pelo seu ID (índice na lista).
    """
    # Verifica se o ID está dentro dos limites da lista
    if 0 <= tarefa_id < len(tarefas):
        tarefas.pop(tarefa_id)
        
    return redirect(url_for('index'))

if __name__ == '__main__':
    # Roda a aplicação. 'debug=True' é ótimo para desenvolvimento, pois
    # reinicia o servidor automaticamente quando você salva o arquivo.
    app.run(debug=True)
```

-----

## 🖼️ Passo 3: Criando a Interface (Templates)

O Flask precisa de uma pasta chamada **`templates`** para encontrar seus arquivos HTML. Crie essa pasta e, dentro dela, o arquivo **`index.html`**.

**Estrutura de pastas:**

```
meu_projeto_flask/
├── venv/
├── templates/
│   └── index.html  <-- CRIE ESTE ARQUIVO AQUI
└── app.py
```

### Código do `index.html`

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha Lista de Tarefas Flask</title>
    <style>
        body { font-family: 'Arial', sans-serif; max-width: 600px; margin: 40px auto; padding: 20px; background: #f4f4f4; border-radius: 8px; box-shadow: 0 0 10px rgba(0,0,0,0.1); }
        h1 { text-align: center; color: #333; }
        ul { list-style: none; padding: 0; }
        li { background: #fff; padding: 12px; margin-bottom: 8px; border-radius: 4px; display: flex; justify-content: space-between; align-items: center; border-left: 5px solid #007bff; }
        .remover-btn { color: #dc3545; text-decoration: none; font-weight: bold; font-size: 0.9em; transition: color 0.2s; }
        .remover-btn:hover { color: #c82333; }
        form { margin-top: 25px; display: flex; gap: 10px; }
        input[type="text"] { flex-grow: 1; padding: 10px; border: 1px solid #ccc; border-radius: 4px; }
        button { padding: 10px 15px; border: none; background-color: #28a745; color: white; border-radius: 4px; cursor: pointer; transition: background-color 0.2s; }
        button:hover { background-color: #218838; }
    </style>
</head>
<body>

    <h1>Minha Lista de Tarefas</h1>

    <form action="{{ url_for('adicionar_tarefa') }}" method="POST">
        <input type="text" name="tarefa" placeholder="Digite uma nova tarefa..." required>
        <button type="submit">Adicionar</button>
    </form>

    <ul>
        {% for tarefa in tarefas %}
            <li>
                <span>{{ tarefa }}</span>
                <a href="{{ url_for('remover_tarefa', tarefa_id=loop.index0) }}" class="remover-btn">Remover</a>
            </li>
        {% else %}
            <li>Nenhuma tarefa adicionada ainda. Use o campo acima para começar!</li>
        {% endfor %}
    </ul>

</body>
</html>
```

-----

## 🚀 Passo 4: Rodando a Aplicação

Com os arquivos `app.py` e `templates/index.html` prontos, inicie o servidor\!

1.  Certifique-se de que seu **ambiente virtual (`(venv)`)** está ativo.
2.  Execute o arquivo Python:

<!-- end list -->

```bash
python app.py
```

3.  Abra seu navegador e acesse o endereço: **`http://127.0.0.1:5000/`**

Pronto\! Sua primeira aplicação web Flask está funcionando.

