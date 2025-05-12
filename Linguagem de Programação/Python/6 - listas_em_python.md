
# Listas em Python 📋

As **listas** são estruturas de dados que armazenam **múltiplos valores em uma única variável**, podendo conter qualquer tipo de dado, inclusive outras listas.

---

## 📌 Criando uma Lista

```python
nomes = ["Ana", "Bruno", "Carlos"]
numeros = [1, 2, 3, 4, 5]
misturada = [1, "Python", True, 3.14]
```

---

## 🔍 Acessando Elementos

```python
print(nomes[0])   # Ana
print(nomes[1])   # Bruno
print(nomes[-1])  # Carlos (último elemento)
```

---

## 🔁 Percorrendo Listas com `for`

```python
for nome in nomes:
    print("Olá,", nome)
```

---

## ➕ Adicionando Elementos

```python
nomes.append("Daniela")     # Adiciona no final
nomes.insert(1, "Eduarda")  # Insere na posição 1
```

---

## ❌ Removendo Elementos

```python
nomes.remove("Carlos")  # Remove pelo valor
nomes.pop()             # Remove o último elemento
del nomes[0]            # Remove pelo índice
```

---

## 🎯 Outros Métodos Úteis

| Método           | Ação                                     |
|------------------|------------------------------------------|
| `append(valor)`  | Adiciona ao final                        |
| `insert(pos, v)` | Insere na posição indicada               |
| `remove(valor)`  | Remove o primeiro valor correspondente   |
| `pop()`          | Remove o último valor                    |
| `len(lista)`     | Retorna o tamanho da lista               |
| `sort()`         | Ordena em ordem crescente                |
| `reverse()`      | Inverte a ordem da lista                 |

---

## 🧪 Exemplo Completo

```python
frutas = ["maçã", "banana", "laranja"]

frutas.append("uva")
frutas.remove("banana")

for fruta in frutas:
    print(fruta)

print("Total de frutas:", len(frutas))
```

---

## 🧠 Boas Práticas

- Use nomes significativos para listas.
- Prefira `for` para percorrer listas.
- Combine listas com estruturas condicionais e repetição para mais poder.

---

## 🧰 Recursos Úteis

- [Listas – Documentação Oficial Python](https://docs.python.org/3/tutorial/datastructures.html)
- [Python List Methods – W3Schools](https://www.w3schools.com/python/python_lists.asp)
