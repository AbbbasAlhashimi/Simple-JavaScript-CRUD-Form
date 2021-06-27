# Simple-JavaScript-CRUD-Form
Simple JavaScript Form that allows the user to insert text values, display them into a table, then Modify or Delete Them.
The project consists of 3 files:<br>
<Ul>
  <li><b>index.html:</b> The file consists of two Tables: the <i>First Table:</i> that allows 4 inputs (Full Name, Employee Code, Salary, and City). And the <i>Second Table:</i> is linked to class [list] and display the inserted values. <br> Please note that the form has a call for default HTML5 functions [onsubmit="event.preventDefault();" autocomplete="off"]. The [event.preventDefault()] hides passed out parameters from the address bar. and the [autocomplete="off"] disables form auto-complete feature.</li>
  <li><b>stlyes.css:</b>The stylesheet file consists of fixed styles that includes body. table, cells, rows, and dynamic values like the <i>[label.validation-error]</i> which is a conditional case by which false entries or empty ones can trigger the [validation-error] class to show or hide the validation error message.</li>
  <li><b>script.js:</b> The File consists of a single constant values set to [null] and 8 Functions:
    <ul>
      <li><b>onFormSubmit()</b> The Function submits entries after the form is filled out. As you can see, the form cannot submit blank entries therefore emty strings are considered as invalid entries. However, once the form entries including <i>[Full Name]</i> are inserted, the function then saves entries.</li>
      <li><b>readFormData()</b> Entred Values are stored into the browser's public storage as an arry of content that remains visible until the session is over.</li>
      <li><b>insertNewRecord(data)</b> Once the form is submitted, the HTML5 Tag [tbody] which looks empty, will be used to display the content of the [employeeList] table. Each row cells whill be stored into the [newRow] array with maximum value of [table.length]. Each row consists of 4 Cells including the [Edit/Delete] clickable links that operate as an entry writter. Entries are filled into the DOM via the [newRow] Cells.</li>
      <li><b>resetForm()</b> The function calls out DOM entries by their ID values then set their values into an empty string.</li>
    <ul>
  
  </li>
</ul>
