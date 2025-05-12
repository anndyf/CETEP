
# HTML Básico 🌐

HTML (HyperText Markup Language) é a **linguagem de marcação** usada para criar e estruturar conteúdo na web.

---

## 📌 Estrutura Básica

A estrutura de um documento HTML é composta por várias partes essenciais:

- `<!DOCTYPE html>`: Informa ao navegador que o documento usa HTML5.
- `<html>`: Elemento raiz de todo documento HTML.
- `<head>`: Contém metadados, título da página, links para estilos e scripts.
- `<body>`: Contém o conteúdo visível da página (textos, imagens, botões etc).

```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha Página</title>
  </head>
  <body>
    <h1>Bem-vindo ao meu site!</h1>
    <p>Essa é uma página HTML simples.</p>
  </body>
</html>
```

---

## 📝 Títulos e Parágrafos

- `<h1>` a `<h6>`: Representam títulos (do maior para o menor).
- `<p>`: Define um parágrafo de texto.

```html
<h1>Título Principal</h1>
<h2>Subtítulo</h2>
<p>Este é um parágrafo explicativo.</p>
```

---

## 🔗 Links

- `<a href="">`: Cria um link para outra página ou site.

```html
<a href="https://www.exemplo.com">Clique aqui para visitar</a>
```

---

## 🖼️ Imagens

- `<img>`: Exibe uma imagem.

Atributos:
- `src`: caminho da imagem
- `alt`: descrição (acessibilidade)
- `width` / `height`: define tamanho

```html
<img src="foto.jpg" alt="Imagem de exemplo" width="300">
```

---

## 📋 Listas

- `<ul>`: Lista não ordenada
- `<ol>`: Lista ordenada
- `<li>`: Item da lista

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
</ul>

<ol>
  <li>Iniciar</li>
  <li>Configurar</li>
</ol>
```

---

## 🧩 Tabelas

- `<table>`: Define a tabela
- `<tr>`: Linha
- `<th>`: Cabeçalho da coluna
- `<td>`: Dado da célula

```html
<table border="1">
  <tr>
    <th>Produto</th>
    <th>Preço</th>
  </tr>
  <tr>
    <td>Notebook</td>
    <td>R$ 3.000</td>
  </tr>
</table>
```

---

## 🧾 Formulários

- `<form>`: Delimita o formulário
- `<input>`: Campo de entrada
- `<label>`: Rótulo do campo
- `<textarea>`: Área de texto
- `<button>`: Botão
- `action`: define para onde os dados serão enviados
- `method`: `GET` ou `POST`

```html
<form action="/enviar" method="post">
  <label for="nome">Nome:</label>
  <input type="text" id="nome" name="nome" required>

  <br><br>

  <label for="mensagem">Mensagem:</label><br>
  <textarea id="mensagem" name="mensagem" rows="4" cols="30"></textarea>

  <br><br>

  <button type="submit">Enviar</button>
</form>
```

---

## 🧠 Boas Práticas

- Sempre declare `<!DOCTYPE html>` no topo.
- Use `alt` para imagens (acessibilidade).
- Indente o código HTML para melhor legibilidade.
- Use `label` para associar texto aos campos de entrada.

---

## 🧰 Recursos Úteis

- [HTML Básico – MDN Web Docs](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
- [Tutorial de HTML – W3Schools](https://www.w3schools.com/html/)
