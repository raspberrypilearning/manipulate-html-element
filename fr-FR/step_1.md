En JavaScript, tu peux voir et modifier le contenu d'un élément HTML en utilisant diverses propriétés DOM.

### .innerHTML

`.innerHTML` refers to the text content as well as the CSS styling, attributes, and HTML tags of an element.

In this example, the HTML element has the attribute `id="myDiv"`.

## --- code ---

language: html
filename: index.html
line_numbers:
--------------------------------------------------

<div id="myDiv">
<p>Il s'agit du contenu original.</p>
</div>

\--- /code ---

Le contenu `HTML` de cet élément peut être modifié.

## --- code ---

language: js
filename: scripts.js
line_numbers:
--------------------------------------------------

// Mise à jour du contenu de l'élément HTML
document.querySelector(#myDiv).innerHTML = "<p>Nouveau contenu avec les balises <strong>HTML</strong> !</p>";

\--- /code ---

### .innerText

`.innerText` fait référence au contenu du texte ainsi qu'au style CSS mais **pas** aux balises et attributs d'un élément.

## --- code ---

language: html
filename: index.html
line_numbers:
--------------------------------------------------

<div id="myDiv">
  <p>Il s'agit du contenu original.</p>
</div>

\--- /code ---

## --- code ---

language: js
filename: scripts.js
line_numbers:
--------------------------------------------------

// Mise à jour du contenu de l'élément HTML
document.querySelector(#myDiv).innerText = "Nouveau contenu de texte sans balises HTML !";

\--- /code ---

### .textContent

`.textContent` fait uniquement référence au contenu du texte d'un élément HTML.

## --- code ---

language: html
filename: index.html
line_numbers:
--------------------------------------------------

<div id="myDiv">
  <p>Il s'agit du contenu original.</p>
</div>

\--- /code ---

## --- code ---

language: js
filename: scripts.js
line_numbers:
--------------------------------------------------

// Mise à jour du contenu de l'élément HTML
document.querySelector(#myDiv).textContent = "Nouveau contenu de texte avec les balises HTML <strong>préservées</strong> !";

\--- /code ---
