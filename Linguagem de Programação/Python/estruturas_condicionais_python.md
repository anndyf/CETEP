
# Estruturas Condicionais em Python ⚖️

As **estruturas condicionais** são usadas para tomar decisões no código, executando diferentes blocos de código dependendo do valor de uma condição.

---

## 🔍 Estrutura Básica

```python
if condição:
    # bloco se a condição for verdadeira
elif outra_condição:
    # bloco se a outra condição for verdadeira
else:
    # bloco se nenhuma das condições anteriores for verdadeira
```

---

## ✅ Exemplo Simples

```python
idade = 18

if idade >= 18:
    print("Você é maior de idade.")
else:
    print("Você é menor de idade.")
```

---

## 🔄 Exemplo com `elif`

```python
nota = 75

if nota >= 90:
    print("Aprovado com excelência!")
elif nota >= 60:
    print("Aprovado.")
else:
    print("Reprovado.")
```

---

## 📦 Condicional com múltiplas condições

```python
usuario = "admin"
senha = "123"

if usuario == "admin" and senha == "123":
    print("Acesso permitido.")
else:
    print("Acesso negado.")
```

---

## 🔃 Condicional com entrada do usuário

```python
numero = int(input("Digite um número: "))

if numero % 2 == 0:
    print("Número par.")
else:
    print("Número ímpar.")
```

---

## 📋 Condicional dentro de laço

```python
for i in range(1, 6):
    if i % 2 == 0:
        print(i, "é par")
    else:
        print(i, "é ímpar")
```

---

## 🧠 Boas Práticas

- Use identação correta para que os blocos funcionem corretamente
- Use `elif` quando houver múltiplas alternativas
- Evite excesso de `if` aninhado; prefira lógica clara e organizada
- Comente decisões importantes no código

---

## 🧰 Recursos Úteis

- [Documentação Oficial – if Statements](https://docs.python.org/3/tutorial/controlflow.html#if-statements)
- [Operadores Lógicos em Python](https://docs.python.org/3/library/stdtypes.html#boolean-operations-and-or-not)
