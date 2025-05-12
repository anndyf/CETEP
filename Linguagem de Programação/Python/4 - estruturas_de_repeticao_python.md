
# Estruturas de Repetição em Python 🔁

As **estruturas de repetição** permitem executar um bloco de código várias vezes, de forma controlada. Em Python, usamos principalmente os comandos `for` e `while`.

---

## 🔂 Tipos de Laços

| Estrutura | Quando usar                                                              |
|-----------|---------------------------------------------------------------------------|
| `for`     | Quando se sabe previamente o número de repetições                         |
| `while`   | Quando a repetição depende de uma condição que pode mudar ao longo do tempo |

---

## 🔁 Estrutura `for`

A estrutura `for` é usada para percorrer elementos de uma sequência (como listas, strings, intervalos).

### 📌 Exemplo com `range()`

```python
for i in range(5):
    print("Repetição:", i)
```

**Saída**:
```
Repetição: 0
Repetição: 1
Repetição: 2
Repetição: 3
Repetição: 4
```

---

### 🔍 Varredura de Lista com `for`

```python
nomes = ["Ana", "Beatriz", "Carlos"]

for nome in nomes:
    print("Nome encontrado:", nome)
```

---

## 🔄 Estrutura `while`

Executa um bloco de código enquanto a condição for verdadeira.

### 📌 Exemplo com `while`

```python
contador = 0
while contador < 5:
    print("Contador:", contador)
    contador += 1
```

---

## 📋 Exemplo: Menu com `while`

```python
opcao = ""

while opcao != "3":
    print("\nMENU")
    print("1 - Dizer Olá")
    print("2 - Mostrar Números")
    print("3 - Sair")

    opcao = input("Escolha uma opção: ")

    if opcao == "1":
        print("Olá, usuário!")
    elif opcao == "2":
        for i in range(1, 6):
            print(i)
    elif opcao == "3":
        print("Saindo do programa...")
    else:
        print("Opção inválida. Tente novamente.")
```

---

## ❌ Usando `break` para interromper o laço

```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

**Saída**: `0 1 2 3 4`

---

## 🔃 Usando `continue` para pular uma repetição

```python
for i in range(5):
    if i == 2:
        continue
    print(i)
```

**Saída**: `0 1 3 4`

---

## 🔐 Loop Infinito (com `while`)

```python
while True:
    comando = input("Digite 'sair' para encerrar: ")
    if comando == "sair":
        break
```

---

## 🧠 Boas Práticas

- Use `for` com `range()` para contagem
- Use `for` para percorrer listas e strings
- Use `while` para menus e repetições condicionais
- Evite loops infinitos sem controle
- Comente loops mais complexos para facilitar o entendimento

---

## 🧰 Recursos Úteis

- [Documentação Oficial – For Statements](https://docs.python.org/3/tutorial/controlflow.html#for-statements)
- [Função `range()`](https://docs.python.org/3/library/functions.html#func-range)
- [Comando `while`](https://docs.python.org/3/reference/compound_stmts.html#the-while-statement)
