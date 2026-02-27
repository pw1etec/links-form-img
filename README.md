# 🌐 Desenvolvimento Web - Teoria

Este documento contém conceitos fundamentais sobre elementos essenciais da Web, abordando texto, hyperlinks, imagens, vetores SVG, conteúdos embutidos, tabelas e formulários.

## 📝 Texto e Hyperlinks

O HTML permite estruturar o conteúdo textual de uma página com diversas tags:

- **`<p>`**: 📝 Define um parágrafo, usado para estruturar blocos de texto.
  - Atributo útil: `lang` (define o idioma do texto, exemplo: `lang="pt-br"`).

- **`<h1>` - `<h6>`**: 🏷️ Definem títulos de diferentes níveis, sendo `<h1>` o mais importante e `<h6>` o menos importante.
  - Atributo útil: `id` (define um identificador único para referência no CSS ou JavaScript).

- **`<strong>`** e **`<em>`**: 🔠 Destacam textos em negrito e itálico, respectivamente, para dar ênfase.
  - Atributo útil: `title` (exibe um texto ao passar o mouse sobre o elemento).

- **`<a href="URL">`**: 🔗 Cria um hyperlink para outra página ou recurso externo.
  - Atributos úteis: `target="_blank"` (abre o link em uma nova aba) e `rel="noopener noreferrer"` (melhora a segurança para links externos).

Exemplo de um hyperlink:

```html
<a href="https://www.example.com" target="_blank">Visite o site</a>
```
[docs elemento a](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/a)

## 🖼️ Imagens, Vetores SVG e Outros Conteúdos Embutidos

As imagens e outros recursos multimídia são essenciais para a Web:

- **`<img>`**: 🖼️ Insere imagens na página, podendo incluir atributos como `alt` para acessibilidade.
  - Atributos úteis: `src` (define o caminho da imagem) e `alt` (texto alternativo para acessibilidade).

- **`<svg>`**: 📐 Define gráficos vetoriais escaláveis que não perdem qualidade ao serem redimensionados.
  - Atributo útil: `viewBox` (define a área visível do SVG).

- **`<iframe>`**: 🎥 Embute conteúdos de outras páginas, como vídeos do YouTube ou mapas interativos.
  - Atributo útil: `allowfullscreen` (permite exibição em tela cheia para vídeos).

Exemplo de imagem com texto alternativo:

```html
<img src="imagem.jpg" alt="Descrição da imagem">
```
[docs elemento img](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/img)

## 📊 Tabelas

As tabelas são usadas para exibir dados tabulares de maneira organizada:

- **`<table>`**: 📋 Define uma tabela.
  - Atributo útil: `border` (define a borda da tabela).

- **`<tr>`**: ➡️ Define uma linha dentro da tabela.
  - Atributo útil: `align` (alinhamento horizontal das células, pode ser `left`, `center` ou `right`).

- **`<th>`**: 🔠 Define uma célula de cabeçalho, geralmente usada para indicar títulos das colunas.
  - Atributo útil: `scope` (indica se o cabeçalho pertence a uma coluna ou linha).

- **`<td>`**: 📦 Define uma célula de dados dentro de uma linha.
  - Atributo útil: `colspan` (define quantas colunas a célula ocupa).

Exemplo de tabela:

```html
<table border="1">
  <tr>
    <th>Nome</th>
    <th>Idade</th>
  </tr>
  <tr>
    <td>Ana</td>
    <td>25</td>
  </tr>
</table>
```
[docs elemento table](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/table)

## 📝 Formulários

Os formulários permitem a interação do usuário com a página, permitindo entradas de dados:

- **`<form>`**: 📝 Define um formulário que agrupa campos de entrada.
  - Atributos úteis: `action` (define para onde os dados serão enviados) e `method` (define o método de envio: `GET` ou `POST`).

- **`<input>`**: 📌 Define um campo de entrada de diversos tipos (texto, senha, email, etc.).
  - Atributos úteis: `type` (define o tipo do campo) e `placeholder` (exibe um texto de exemplo dentro do campo).

- **`<textarea>`**: ✍️ Define uma área de texto maior para inserção de múltiplas linhas.
  - Atributo útil: `rows` (define a quantidade de linhas visíveis no campo).

- **`<button>`**: 🔘 Cria um botão para submissão do formulário.
  - Atributo útil: `type` (pode ser `submit`, `reset` ou `button`).

- **`<fieldset>`**: 📦 Agrupa elementos relacionados dentro do formulário.
  - Atributo útil: `disabled` (desabilita todos os campos dentro do `<fieldset>`).

- **`<legend>`**: 🏷️ Define um título descritivo para um `<fieldset>`.
  - Atributo útil: `align` (define o alinhamento do texto da legenda, pode ser `left`, `center` ou `right`).

Exemplo de formulário com `<fieldset>` e `<legend>`:

```html
<form action="submit.php" method="post">
  <fieldset>
    <legend>Informações Pessoais</legend>
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome" placeholder="Digite seu nome">
    
    <label for="email">E-mail:</label>
    <input type="email" id="email" name="email" placeholder="Digite seu e-mail">
  </fieldset>
  <button type="submit">Enviar</button>
</form>
```
[doc eleemento form](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form)

---

Este material serve como base teórica para as aulas de Desenvolvimento Web. Pratique implementando esses conceitos em seus próprios projetos! 🚀
