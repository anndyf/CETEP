
# Funções em Python 🐍

As **funções** são blocos de código reutilizáveis que executam uma tarefa específica. Elas ajudam a organizar e reutilizar o código com mais clareza e eficiência.

---

## 📌 Estrutura Básica

```python
def nome_da_funcao(param1, param2):
    # bloco de código
    return resultado
```

---

## ✅ Componentes Principais

| Componente       | Descrição                                                                 |
|------------------|--------------------------------------------------------------------------|
| `def`            | Palavra-chave para declarar uma função                                   |
| `nome_da_funcao` | Nome que identifica a função (deve seguir as regras de nomes em Python)  |
| `param1, param2` | Parâmetros (opcionais) que a função pode receber                         |
| `return`         | (opcional) Indica o valor que a função devolve                          |

---

## 🧪 Exemplo Simples

```python
def somar(a, b):
    return a + b

resultado = somar(5, 3)
print("Resultado:", resultado)  # Resultado: 8
```

---

## 🔄 Exemplo com `return`

```python
def calcular_area_retangulo(base, altura):
    area = base * altura
    return area

# Chamando a função
resultado = calcular_area_retangulo(5, 3)
print("Área do retângulo:", resultado)  # Área do retângulo: 15
```

---

## ℹ️ Funções Sem Parâmetros

```python
def saudacao():
    print("Olá! Bem-vindo ao mundo Python.")

saudacao()
```

---

## 🔁 Parâmetros Opcionais

```python
def apresentar(nome, saudacao="Olá"):
    print(f"{saudacao}, {nome}!")

apresentar("Andressa")
apresentar("João", "Oi")
```

---

## 📦 Funções com `*args` e `**kwargs`

```python
def listar_nomes(*args):
    for nome in args:
        print(nome)

listar_nomes("Ana", "Beatriz", "Carlos")

def mostrar_info(**kwargs):
    for chave, valor in kwargs.items():
        print(f"{chave}: {valor}")

mostrar_info(nome="Ana", idade=22)
```

---

## 🧠 Boas Práticas

- Escolha nomes descritivos para suas funções
- Evite funções muito longas: separe tarefas em subfunções

---

## 🧰 Recursos Úteis

- [Documentação Oficial do Python – Funções](https://docs.python.org/3/tutorial/controlflow.html#defining-functions)
- [PEP 8 – Guia de estilo para Python](https://peps.python.org/pep-0008/)

---

📝 *Esta página foi criada para auxiliar estudantes iniciantes na compreensão de funções em Python. Sinta-se à vontade para copiar, adaptar ou contribuir!*
