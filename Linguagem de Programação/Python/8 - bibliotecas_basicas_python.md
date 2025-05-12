
# Bibliotecas Básicas em Python 📚

As bibliotecas em Python são conjuntos de funções e recursos prontos para facilitar tarefas específicas. Abaixo estão algumas das bibliotecas mais comuns para iniciantes.

---

## 🔣 `math` – Funções Matemáticas

```python
import math

print(math.sqrt(25))     # Raiz quadrada
print(math.pow(2, 3))    # Potência
print(math.pi)           # Constante pi
```

---

## 🎲 `random` – Valores Aleatórios

```python
import random

print(random.randint(1, 10))              # Inteiro aleatório entre 1 e 10
print(random.choice(["maçã", "uva", "kiwi"]))  # Escolhe item da lista
```

---

## 🗂️ Outras Bibliotecas Úteis

| Biblioteca | Uso comum                                |
|------------|-------------------------------------------|
| `datetime` | Manipulação de datas e horários          |
| `os`       | Acesso a pastas, arquivos e comandos do sistema |
| `time`     | Medir tempo de execução, pausas          |

---

### Exemplo com `datetime`

```python
import datetime

hoje = datetime.date.today()
print("Data de hoje:", hoje)
```

---

### Exemplo com `os`

```python
import os

print("Diretório atual:", os.getcwd())
```

---

### Exemplo com `time`

```python
import time

print("Esperando 2 segundos...")
time.sleep(2)
print("Fim")
```

---

## ✅ Boas Práticas

- Importe apenas o necessário (`from math import sqrt` se quiser só a raiz)
- Explore a documentação oficial das bibliotecas
