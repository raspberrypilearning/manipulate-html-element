In JavaScript kun je de inhoud van een HTML-element bekijken en wijzigen met behulp van verschillende DOM-eigenschappen.

### .innerHTML

`.innerHTML` verwijst naar de tekstinhoud evenals de CSS styling, attributen en HTML tags van een element.

In dit voorbeeld heeft het HTML-element het kenmerk `id="myDiv"`.

## --- code ---

language: html
filename: index.html
line_numbers:
--------------------------------------------------

<div id="myDiv">
<p>Dit is de originele inhoud.</p>
</div>

\--- /code ---

De `HTML`-inhoud van dit element kan worden gewijzigd.

## --- code ---

language: js
filename: scripts.js
line_numbers:
--------------------------------------------------

// Werk de inhoud van het HTML-element bij
document.querySelector(#myDiv).innerHTML = "<p>Nieuwe inhoud met <strong>HTML</strong> tags!</p>";

\--- /code ---

### .innerText

`.innerText` verwijst zowel naar de tekstinhoud als naar de CSS-stijl, maar **niet** naar de tags en attributen van een element.

## --- code ---

language: html
filename: index.html
line_numbers:
--------------------------------------------------

<div id="myDiv">
  <p>Dit is de originele inhoud.</p>
</div>

\--- /code ---

## --- code ---

language: js
filename: scripts.js
line_numbers:
--------------------------------------------------

// Update HTML element inhoud
document.querySelector(#myDiv).innerText = "Nieuwe tekst inhoud zonder HTML tags!";

\--- /code ---

### .textContent

`.textContent` verwijst alleen naar de tekstinhoud van een HTML-element.

## --- code ---

language: html
filename: index.html
line_numbers:
--------------------------------------------------

<div id="myDiv">
  <p>Dit is de originele inhoud.</p>
</div>

\--- /code ---

## --- code ---

language: js
filename: scripts.js
line_numbers:
--------------------------------------------------

// Update HTML element inhoud
document.querySelector(#myDiv).textContent = "Nieuwe tekst inhoud met HTML tags <strong>behouden</strong>!";

\--- /code ---
