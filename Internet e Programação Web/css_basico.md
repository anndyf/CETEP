
# CSS Básico 🎨

**CSS (Cascading Style Sheets)** é a linguagem usada para estilizar elementos HTML, controlando cores, tamanhos, espaçamentos, posicionamento e muito mais.

---

## 🧭 Como Usar CSS

A melhor prática é **usar um arquivo CSS externo**. Isso separa o conteúdo (HTML) da aparência (CSS), facilitando a manutenção do código.

### ✅ Recomendado: CSS Externo

1. Crie um arquivo chamado `estilos.css`:

```css
body {
  background-color: #f0f0f0;
  font-family: Arial, sans-serif;
}

h1 {
  color: blue;
  text-align: center;
}
```

2. No HTML, faça o link:

```html
<head>
  <link rel="stylesheet" href="estilos.css">
</head>
```

---

## 🚫 Outras formas (menos recomendadas)

### ❌ CSS Inline (evite)

```html
<p style="color: red;">Texto em vermelho</p>
```

### ⚠️ CSS Interno (útil apenas para testes)

```html
<head>
  <style>
    p { color: green; }
  </style>
</head>
```

---

## 🎯 Seletores Básicos

| Seletor         | Exemplo           | Descrição                              |
|------------------|--------------------|------------------------------------------|
| `*`             | `* {}`            | Aplica a todos os elementos              |
| `tag`           | `p {}`            | Aplica a todas as tags `<p>`             |
| `.classe`       | `.destaque {}`    | Aplica a elementos com class             |
| `#id`           | `#menu {}`        | Aplica ao elemento com id específico     |

---

## ✨ Propriedades Comuns

```css
/* Cores e texto */
color: red;
background-color: yellow;
font-size: 16px;
font-family: Arial, sans-serif;
text-align: center;

/* Espaçamento */
margin: 10px;
padding: 20px;

/* Bordas */
border: 2px solid black;
border-radius: 8px;

/* Tamanho */
width: 300px;
height: 150px;
```

---

## 🧱 Box Model (Modelo de Caixa)

Todo elemento HTML é uma "caixa" composta por:

- `content`: conteúdo (texto, imagem, etc.)
- `padding`: espaço interno
- `border`: borda ao redor
- `margin`: espaço externo

```css
.caixa {
  width: 200px;
  padding: 10px;
  border: 1px solid black;
  margin: 20px;
}
```

---

## 🧪 Exemplo Completo com Arquivo Externo

### HTML (`index.html`)

```html
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="estilos.css">
</head>
<body>
  <div class="cartao">
    <h2>Sobre mim</h2>
    <p>Sou estudante de programação!</p>
  </div>
</body>
</html>
```

### CSS (`estilos.css`)

```css
.cartao {
  background-color: #fff;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 10px;
  width: 300px;
}
```

---

## 🧠 Boas Práticas

- Sempre use CSS externo em projetos reais.
- Organize seu CSS por seções ou componentes.
- Use classes ao invés de IDs para estilizar.
- Evite repetir estilos desnecessários.

---

## 🧰 Recursos Úteis

- [Guia de CSS – MDN Web Docs](https://developer.mozilla.org/pt-BR/docs/Web/CSS)
- [Tutorial de CSS – W3Schools](https://www.w3schools.com/css/)
