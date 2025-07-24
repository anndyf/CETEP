
# Criando um Sistema de Login com CustomTkinter

Neste passo a passo, você aprenderá a criar uma interface gráfica simples com `CustomTkinter`, incluindo campos de usuário, senha e validação de login.

---

## Pré-requisitos

Antes de começar, certifique-se de que o Python está instalado em seu computador.

1. Atualize o gerenciador de pacotes `pip`:
```bash
pip install --upgrade pip
```

2. Instale a biblioteca `customtkinter`:
```bash
pip install customtkinter
```

---

## Passo a Passo

### 1. Importe a biblioteca
```python
import customtkinter as ctk
```
**Explicação:** Importa a biblioteca `customtkinter` com o apelido `ctk`, facilitando o uso de seus componentes gráficos.

---

### 2. Defina o tema da interface
```python
ctk.set_appearance_mode("dark")
```
**Explicação:** Define a aparência da interface no modo escuro, o que deixa o visual mais moderno e confortável para os olhos.

---

### 3. Crie a janela principal
```python
app = ctk.CTk()
app.title("Sistema de Login")
app.geometry("400x300")
```
**Explicação:**  
- `ctk.CTk()` cria a janela principal da aplicação.  
- `title()` define o título da janela.  
- `geometry()` define o tamanho da janela (largura x altura).

---

### 4. Adicione o campo de usuário
```python
label_usuario = ctk.CTkLabel(app, text="Usuário:")
label_usuario.pack(pady=10)
```
**Explicação:** Cria um rótulo (label) com o texto "Usuário:" e o posiciona com um espaçamento vertical de 10 pixels.

```python
campo_usuario = ctk.CTkEntry(app, placeholder_text="Digite seu usuário")
campo_usuario.pack(pady=10)
```
**Explicação:** Cria um campo de entrada com um texto auxiliar ("placeholder") e posiciona com espaçamento vertical.

---

### 5. Adicione o campo de senha
```python
label_senha = ctk.CTkLabel(app, text="Senha:")
label_senha.pack(pady=10)
```
**Explicação:** Cria um rótulo (label) com o texto "Senha:" e o posiciona com espaçamento.

```python
campo_senha = ctk.CTkEntry(app, placeholder_text="Digite sua senha", show="*")
campo_senha.pack(pady=10)
```
**Explicação:** Cria um campo de entrada para senha, onde os caracteres ficam ocultos (por causa do `show="*"`).

---

### 6. Adicione o campo de feedback
```python
resultado_login = ctk.CTkLabel(app, text="")
resultado_login.pack(pady=10)
```
**Explicação:** Cria um rótulo que inicialmente está vazio, mas será usado para exibir o resultado do login (sucesso ou erro).

---

### 7. Crie a função de validação de login
```python
def validar_login():
    usuario = campo_usuario.get()
    senha = campo_senha.get()

    if usuario == "admin" and senha == "1234":
        resultado_login.configure(text="Login bem-sucedido!", text_color="green")
    else:
        resultado_login.configure(text="Usuário ou senha inválidos.", text_color="red")
```
**Explicação:**  
- `campo_usuario.get()` e `campo_senha.get()` pegam os textos digitados nos campos.  
- A estrutura `if` compara os dados com os valores esperados.  
- O `configure` atualiza o texto e a cor do rótulo de feedback.

---

### 8. Adicione o botão de login
```python
botao_login = ctk.CTkButton(app, text="Login", command=validar_login)
botao_login.pack(pady=20)
```
**Explicação:**  
- Cria um botão com o texto "Login".  
- O parâmetro `command=validar_login` faz com que, ao clicar, a função de validação seja executada.  
- `pack(pady=20)` posiciona o botão com espaçamento.

---

### 9. Execute o aplicativo
```python
app.mainloop()
```
**Explicação:** Inicia o loop principal da interface, mantendo a janela aberta e interativa.

---

## Resultado

Você terá uma interface funcional com validação de login e feedback visual. Ideal para introdução ao desenvolvimento de interfaces gráficas em Python!
