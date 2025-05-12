
# Strings em Python ✍️

**Strings** são sequências de caracteres usadas para representar textos. Em Python, strings podem ser delimitadas por aspas simples `'` ou duplas `"`.

---

## 📌 Criando Strings

```python
mensagem1 = "Olá, mundo!"
mensagem2 = 'Python é incrível'
```

---

## 🔍 Acessando Caracteres

```python
texto = "Python"
print(texto[0])   # P
print(texto[-1])  # n (último caractere)
```

---

## 🔁 Percorrendo uma String

```python
for letra in texto:
    print(letra)
```

---

## ➕ Concatenando Strings

```python
nome = "Ana"
sobrenome = "Silva"
nome_completo = nome + " " + sobrenome
print(nome_completo)
```

---

## 🧮 Tamanho da String

```python
frase = "Aprender Python"
print(len(frase))  # 15
```

---

## 🔢 Conversão de Tipos para String

```python
idade = 20
texto = "Você tem " + str(idade) + " anos."
print(texto)
```

---

## ❓ Verificação de Substrings

```python
frase = "Aprender Python é divertido"
print("Python" in frase)   # True
print("Java" not in frase) # True
```

---

## ✂️ Fatiamento (Slicing)

```python
texto = "Programação"
print(texto[0:4])   # 'Prog'
print(texto[:5])    # 'Progr'
print(texto[5:])    # 'amação'
```

---

## 🔗 Juntando Strings com `join()`

```python
letras = ['P', 'y', 't', 'h', 'o', 'n']
texto = ''.join(letras)
print(texto)  # Python
```

---

## 🔣 `.split()` com separador

```python
frase = "um,dois,tres"
partes = frase.split(",")
print(partes)  # ['um', 'dois', 'tres']
```

---

## 🎯 Métodos Úteis

| Método               | Descrição                                |
|----------------------|-------------------------------------------|
| `lower()`            | Converte para minúsculas                  |
| `upper()`            | Converte para maiúsculas                  |
| `capitalize()`       | Primeira letra maiúscula                  |
| `strip()`            | Remove espaços extras                     |
| `replace("a", "e")`  | Substitui caracteres                      |
| `split()`            | Divide a string em lista                  |
| `find("texto")`      | Retorna o índice do texto (ou -1)         |

---

## 🧪 Exemplo Completo

```python
frase = "   Python é divertido!   "

print(frase.strip())                # Remove espaços
print(frase.upper())                # Tudo maiúsculo
print(frase.lower())                # Tudo minúsculo
print(frase.replace("divertido", "poderoso"))  # Substitui palavra
```

---

## 🔡 f-strings (formatação moderna)

```python
nome = "Carlos"
idade = 28

print(f"{nome} tem {idade} anos.")
```

---

## 🧠 Boas Práticas

- Prefira `f-strings` para montar mensagens.
- Use métodos como `.strip()` ao receber textos de entrada.
- Evite concatenações dentro de laços — prefira `join()` se necessário.
- Use slicing e `in` para manipular strings com clareza.

---

## 🧰 Recursos Úteis

- [Strings – Documentação Oficial Python](https://docs.python.org/3/library/stdtypes.html#text-sequence-type-str)
- [W3Schools – Python Strings](https://www.w3schools.com/python/python_strings.asp)
