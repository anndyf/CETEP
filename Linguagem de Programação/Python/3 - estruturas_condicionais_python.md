
# Estruturas Condicionais em Python 🔀

As **estruturas condicionais** permitem ao programa **tomar decisões** com base em condições. São amplamente usadas em praticamente todo código Python.

---

## ⚙️ Quando Usar?

| Comando   | Quando usar                                                                 |
|-----------|------------------------------------------------------------------------------|
| `if`      | Quando você quer testar uma **condição principal**                          |
| `elif`    | Quando deseja **testar novas condições** se o `if` anterior for falso        |
| `else`    | Quando nenhuma das condições anteriores for verdadeira (opcional)            |

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

## ✅ Estrutura Básica

```python
if condicao1:
    # código executado se condicao1 for verdadeira
elif condicao2:
    # código executado se condicao2 for verdadeira
else:
    # código executado se nenhuma condição acima for verdadeira
```

---

## 🧪 Exemplo Simples

```python
nota = 7

if nota >= 9:
    print("Excelente")
elif nota >= 6:
    print("Aprovado")
else:
    print("Reprovado")
```

---

## 🔍 Somente `if`

Use apenas `if` quando há **uma única condição a ser testada**.

```python
idade = 18

if idade >= 18:
    print("Você é maior de idade.")
```

---

## 🔄 `if` + `else`

Use `else` quando você quer **uma ação alternativa** caso o `if` seja falso.

```python
senha = "admin"

if senha == "admin":
    print("Acesso permitido.")
else:
    print("Senha incorreta.")
```

---

## 🔁 `if`, `elif`, `else`

Use `elif` quando há **várias possibilidades** mutuamente exclusivas.

```python
numero = 0

if numero > 0:
    print("Número positivo")
elif numero < 0:
    print("Número negativo")
else:
    print("Número é zero")
```

---

## 🔂 Condições Aninhadas (evitar excesso)

```python
idade = 17
tem_autorizacao = True

if idade < 18:
    if tem_autorizacao:
        print("Entrada permitida com autorização.")
    else:
        print("Entrada não permitida.")
else:
    print("Entrada permitida.")
```

---

## ✅ Boas Práticas

- Evite muitos `if` aninhados — prefira lógica mais clara.
- Sempre use indentação correta.
- Use comparações diretas (`==`, `>`, `<`, `!=`, etc.).
- Para múltiplas comparações, considere o uso de operadores lógicos (`and`, `or`).

---

## 🧰 Recursos Úteis

- [Python: if Statements](https://docs.python.org/3/tutorial/controlflow.html#if-statements)
- [Operadores Lógicos em Python](https://www.w3schools.com/python/python_conditions.asp)
