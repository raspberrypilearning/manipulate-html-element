在 JavaScript 中，你可以使用各种 DOM 属性查看和更改 HTML 元素的内容。

### .innerHTML

`.innerHTML` 指的是元素的文本内容以及 CSS 样式、属性和 HTML 标签。

在此示例中，HTML元素具有属性 `id="myDiv"`。

## --- code ---

language: html
filename: index.html
line_numbers:
--------------------------------------------------

<div id="myDiv">
<p>这是原文内容。</p>
</div>

\--- /code ---

此元素的 `HTML` 内容可以更改。

## --- code ---

language: js
filename: scripts.js
line_numbers:
--------------------------------------------------

// 更新 HTML 元素内容
document.querySelector(#myDiv).innerHTML = "<p>带有 <strong>HTML</strong> 标签的新内容！</p>";

\--- /code ---

### .innerText

`.innerText` 指的是文本内容以及 CSS 样式，但**不是**元素的标签和属性。

## --- code ---

language: html
filename: index.html
line_numbers:
--------------------------------------------------

<div id="myDiv">
  <p>这是原文内容。</p>
</div>

\--- /code ---

## --- code ---

language: js
filename: scripts.js
line_numbers:
--------------------------------------------------

// 更新 HTML 元素内容
document.querySelector(#myDiv).innerText = "没有 HTML 标签的新文本内容！";

\--- /code ---

### .textContent

`.textContent` 仅指 HTML 元素的文本内容。

## --- code ---

language: html
filename: index.html
line_numbers:
--------------------------------------------------

<div id="myDiv">
  <p>这是原文内容。</p>
</div>

\--- /code ---

## --- code ---

language: js
filename: scripts.js
line_numbers:
--------------------------------------------------

// 更新 HTML 元素内容
document.querySelector(#myDiv).textContent = "带有 HTML 标签 <strong>的新文本内容保留</strong>！";

\--- /code ---
