
# Aula 2 – Estilização com CSS Externo (com código)
 
🎯 Objetivo: Aplicar estilos com CSS externo, deixando o site visualmente organizado e moderno.

---

## 🎨 Passo 1: Criar o Arquivo CSS

Crie um arquivo chamado `style.css` na mesma pasta do `index.html`.

---

## 🔗 Passo 2: Conectar o CSS no HTML

```html
<head>
  ...
  <link rel="stylesheet" href="style.css">
</head>
```

---

## 💅 Etapa 3: Estilo Global

```css
body {
  font-family: Arial, sans-serif;
  margin: 0;
  background-color: #f9f9f9;
  color: #333;
}
```

---

## 💠 Etapa 4: Estilo do Cabeçalho e Menu

```css
header {
  background-color: #0077cc;
  color: white;
  padding: 20px 0;
  text-align: center;
}

nav {
  background-color: #005fa3;
}

.menu {
  list-style: none;
  display: flex;
  justify-content: center;
  padding: 0;
  margin: 0;
}

.menu li {
  margin: 0 15px;
}

.menu a {
  color: white;
  text-decoration: none;
  font-weight: bold;
  padding: 10px;
  display: inline-block;
}

.menu a:hover {
  background-color: #004f87;
  border-radius: 5px;
}
```

---

## 🧱 Etapa 5: Estilo das Seções e Rodapé

```css
main {
  max-width: 900px;
  margin: auto;
  padding: 20px;
}

section {
  background-color: white;
  padding: 20px;
  margin: 20px 0;
  border-left: 5px solid #0077cc;
  border-radius: 5px;
  box-shadow: 0 0 5px rgba(0,0,0,0.1);
}

footer {
  background-color: #0077cc;
  color: white;
  text-align: center;
  padding: 15px;
}
```

---

✅ **Resultado Esperado**: Um site com visual organizado, menu funcional, cores harmônicas e conteúdo bem dividido.
