# 🐍 Guia de Instalação do Flask no VS Code com Ambiente Virtual

Este guia mostra como configurar um projeto Flask no **Visual Studio Code** com **ambiente virtual**, explicando a importância e sugerindo uma estrutura de pastas organizada.

---

## 🔹 1. Pré-requisitos

- **Python** instalado (recomenda-se versão 3.8+).  
  Verifique no terminal:
  ```bash
  python3 --version
  ```

- **Visual Studio Code** instalado.  
  - Extensão recomendada: **Python (Microsoft)**  

---

## 🔹 2. Criar e ativar um ambiente virtual

Um **ambiente virtual** (venv) permite isolar as bibliotecas de cada projeto, evitando conflitos entre versões diferentes de pacotes.  

No terminal, dentro da pasta do projeto:

```bash
# Criar ambiente virtual
python3 -m venv venv
```

Ativar o ambiente virtual:

- **Linux / MacOS**
  ```bash
  source venv/bin/activate
  ```

- **Windows (PowerShell)**
  ```powershell
  .\venv\Scripts\activate
  ```

Quando ativo, você verá algo como `(venv)` no início da linha do terminal.  

Para desativar:
```bash
deactivate
```

---

## 🔹 3. Instalar o Flask no ambiente virtual

Com o ambiente virtual ativo, instale o Flask:

```bash
pip install flask
```

Verifique se foi instalado corretamente:

```bash
pip show flask
```

---

## 🔹 4. Criar um projeto Flask básico

Estrutura de pastas sugerida:

```
meu_projeto/
│── venv/              # Ambiente virtual
│── app/               # Código principal do Flask
│   ├── __init__.py    # Inicializa o app Flask
│   ├── routes.py      # Rotas da aplicação
│── static/            # Arquivos estáticos (CSS, JS, imagens)
│── templates/         # Templates HTML (Jinja2)
│── requirements.txt   # Lista de dependências do projeto
│── run.py             # Arquivo principal para rodar o app
```

### Exemplo de `run.py`:

```python
from app import app

if __name__ == "__main__":
    app.run(debug=True)
```

### Exemplo de `app/__init__.py`:

```python
from flask import Flask

app = Flask(__name__)

from app import routes
```

### Exemplo de `app/routes.py`:

```python
from app import app

@app.route("/")
def home():
    return "Olá, Flask no VS Code!"
```

---

## 🔹 5. Gerenciar dependências

Para salvar as bibliotecas usadas no projeto:

```bash
pip freeze > requirements.txt
```

Para instalar em outro ambiente:

```bash
pip install -r requirements.txt
```

---

## 🔹 6. Rodar o servidor Flask

No terminal (com `venv` ativo):

```bash
python run.py
```

Acesse no navegador:  
👉 `http://127.0.0.1:5000/`

---

## ✅ Por que usar ambiente virtual?

- Isola bibliotecas por projeto.  
- Evita conflitos de versões.  
- Facilita a portabilidade (via `requirements.txt`).  
- É a prática recomendada para desenvolvimento Python.  
