In JavaScript, you can view and change the inner text content of an HTML element using various DOM properties.

These include:
+ `.innerHTML` this property finds and returns the text content as well as the CSS styling, attributes and HTML tags of an element.

For example: 

--- code ---
---
language: html
filename: index.html
line_numbers: true
---

      <div id="myDiv">
        <p>This is the original content.</p>
      </div>
      
--- /code ---

--- code ---
---
language: js
filename: script.js
line_numbers: true
---
     
     // Update Copyright Year function 
     document.getElementById('myDiv').innerHTML = "<p>New content with <strong>HTML</strong> tags!</p>";
    
--- /code ---

+ `.innerText` this property finds and returns the text content as well as the CSS styling but not the tags and attributes of an element.

--- code ---
---
language: html
filename: index.html
line_numbers: true
---

    <div id="myDiv">
        <p>This is the original content.</p>
    </div>

--- /code ---

--- code ---
---
language: js
filename: script.js
line_numbers: true
---
     
     // Update Copyright Year function 
    document.getElementById('myDiv').innerText = "New text content without HTML tags!";
    
--- /code ---

+ `.textContent` this property returns only the text content of an HTML element.

--- code ---
---
language: html
filename: index.html
line_numbers: true
---

      <div id="myDiv">
        <p>This is the original content.</p>
    </div>

--- /code ---

--- code ---
---
language: js
filename: script.js
line_numbers: true
---
     
     // Update Copyright Year function 
    document.getElementById('myDiv').textContent = "New text content with HTML tags <strong>preserved</strong>!";
    
--- /code ---
