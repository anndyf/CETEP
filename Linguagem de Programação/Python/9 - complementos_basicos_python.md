
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
