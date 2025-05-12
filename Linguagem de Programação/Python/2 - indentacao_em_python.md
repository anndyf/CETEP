
# Indentação em Python 🧱

A **indentação** é fundamental em Python e define os blocos de código. Diferente de outras linguagens que usam chaves (`{}`) ou palavras-chave para marcar blocos, o Python **usa a identação obrigatória** com espaços ou tabulações.

---

## 🧾 O que é Indentação?

Indentação é o **recuo do código** em relação à margem esquerda. Em Python, ela **não é opcional**: é usada para indicar o início e o fim de blocos, como em funções, condicionais, laços, etc.

---

## ⚠️ Regras Gerais

- O **nível de indentação** deve ser **consistente** no bloco.
- **4 espaços** por nível é a convenção recomendada (PEP 8).
- Misturar **espaços e tabulações** pode causar erros.

---

## ✅ Exemplo Correto

```python
if True:
    print("Indentado corretamente")
    print("Esse também está no mesmo bloco")
```

---

## ❌ Exemplo Incorreto

```python
if True:
print("Erro! Não está indentado.")
```

**Resultado**:
```
IndentationError: expected an indented block
```

---

## 🧪 Uso em `if`, `for`, `while`, `def` e mais

### Condicional:

```python
if x > 10:
    print("Maior que 10")
```

### Laço:

```python
for i in range(3):
    print(i)
```

### Função:

```python
def saudacao():
    print("Olá!")
```

---

## 🔁 Blocos Aninhados

```python
idade = 18

if idade >= 18:
    print("Maior de idade")
    if idade >= 60:
        print("Idoso")
```

---

## 🧠 Boas Práticas

- Use sempre 4 espaços para cada nível de indentação.
- Não misture tabulação e espaço.
- Configure seu editor para **inserir 4 espaços** ao pressionar "Tab".

---

## 🧰 Recursos Úteis

- [Guia PEP 8 – Estilo de Código Python](https://peps.python.org/pep-0008/#indentation)
- [Erro IndentationError – Documentação Python](https://docs.python.org/3/tutorial/errors.html)

