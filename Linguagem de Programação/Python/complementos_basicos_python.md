
# Complementos Básicos em Python 🧰

Este material reúne conceitos adicionais que enriquecem a base de quem está começando a programar em Python.

---

## 📦 Tuplas e Dicionários

### Tuplas (imutáveis)

```python
cores = ("vermelho", "verde", "azul")
print(cores[1])  # verde
```

### Dicionários (chave-valor)

```python
pessoa = {"nome": "Maria", "idade": 25}
print(pessoa["nome"])  # Maria
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

## 🛠️ Tratamento de Erros (`try/except`)

```python
try:
    numero = int(input("Digite um número: "))
    print("Número digitado:", numero)
except ValueError:
    print("Entrada inválida. Digite um número inteiro.")
```

---

## 💬 Comentários no Código

```python
# Isso é um comentário
print("Olá!")  # Comentário após código
```

---

## ✅ Boas Práticas

- Comente trechos importantes do código.
- Use operadores com clareza para evitar ambiguidade.
- Trate entradas com `try/except` para evitar falhas em tempo de execução.
