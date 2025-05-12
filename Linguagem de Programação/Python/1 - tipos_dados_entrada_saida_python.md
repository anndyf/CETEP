
# Tipos de Dados, Entrada e Saída em Python 📥📤

Python é uma linguagem de tipagem dinâmica, ou seja, você não precisa declarar o tipo das variáveis — o interpretador identifica automaticamente.

---

## 🔤 Tipos de Dados Principais

| Tipo       | Exemplo       | Descrição                                |
|------------|---------------|--------------------------------------------|
| `int`      | `10`, `-3`    | Números inteiros                          |
| `float`    | `3.14`, `-2.7`| Números decimais (ponto flutuante)        |
| `str`      | `"Python"`    | Texto (string de caracteres)              |
| `bool`     | `True`, `False`| Valores booleanos (lógico)               |
| `list`     | `[1, 2, 3]`   | Lista de elementos                        |
| `dict`     | `{"nome": "Ana", "idade": 20}` | Dicionário (chave-valor)    |

---

## ✅ Atribuição de Variáveis

```python
nome = "João"
idade = 25
altura = 1.75
maior_de_idade = True
```

---

## 🔍 Verificando o Tipo

```python
print(type(nome))      # <class 'str'>
print(type(idade))     # <class 'int'>
print(type(altura))    # <class 'float'>
print(type(maior_de_idade))  # <class 'bool'>
```

---

## 🎤 Entrada de Dados com `input()`

A função `input()` lê **valores digitados pelo usuário** como texto (`str`).

```python
nome = input("Digite seu nome: ")
print("Olá,", nome)
```

---

### 🧮 Convertendo para números

```python
idade = int(input("Digite sua idade: "))
altura = float(input("Digite sua altura: "))
```

---

## 📤 Saída de Dados com `print()`

```python
nome = "Maria"
idade = 30

print("Nome:", nome)
print(f"{nome} tem {idade} anos.")  # f-string
```

---

## 🔁 Exemplo Completo

```python
nome = input("Nome: ")
idade = int(input("Idade: "))
altura = float(input("Altura: "))

print(f"{nome} tem {idade} anos e {altura}m de altura.")
```

---
## ➕ Operadores Aritméticos

| Operador | Significado            | Exemplo    | Resultado |
|----------|------------------------|------------|-----------|
| `+`      | Soma                   | `2 + 3`    | `5`       |
| `-`      | Subtração              | `7 - 4`    | `3`       |
| `*`      | Multiplicação          | `3 * 2`    | `6`       |
| `/`      | Divisão (float)        | `5 / 2`    | `2.5`     |
| `//`     | Divisão inteira        | `5 // 2`   | `2`       |
| `%`      | Resto da divisão       | `5 % 2`    | `1`       |
| `**`     | Potência               | `2 ** 3`   | `8`       |

---

## 🔁 Operadores de Comparação

| Operador | Significado           | Exemplo     | Resultado |
|----------|-----------------------|-------------|-----------|
| `==`     | Igual                 | `3 == 3`    | `True`    |
| `!=`     | Diferente             | `4 != 5`    | `True`    |
| `>`      | Maior que             | `5 > 2`     | `True`    |
| `<`      | Menor que             | `3 < 1`     | `False`   |
| `>=`     | Maior ou igual        | `4 >= 4`    | `True`    |
| `<=`     | Menor ou igual        | `6 <= 3`    | `False`   |

---
## 🧠 Boas Práticas

- Use `f-strings` para formatar mensagens com variáveis.
- Sempre converta os dados de entrada (`input`) quando precisar de números.
- Teste o tipo das variáveis se necessário usando `type()`.

---

## 🧰 Recursos Úteis

- [Função `input()` – Documentação Python](https://docs.python.org/3/library/functions.html#input)
- [Função `print()` – Documentação Python](https://docs.python.org/3/library/functions.html#print)
- [Tipos de dados em Python – W3Schools](https://www.w3schools.com/python/python_datatypes.asp)
