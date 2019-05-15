# frontend-development-basics

frontend development is divided into two category and the first is an input to the next. As both requires different experties there will always be 2 teams.

* User Experience
* User Interface

### User Experience (UX)
The input for the user experience team is the business requirement and output is the screens with styleguides. The member of this team has the experience of improving usability, ease of use etc. 

### User Interface (UI)
The team gets the UX (Design and Style guide) and develops the Interface and the behaviour. 

As an UI developer you need to know
* html - provides you the components/elements to create the screen elements
* stylesheet (css) - provides you with the style elements match the design requirement of the screen
* javascript (js) - provides you with components to ecrich the behaviour

#### html
- The file name should be saved with extention wither .htm or .html
- Though not mandatory but the page contant should be placed inside <body></body> element.````
```
<html>
  <head>
    <title>My Website</title>
  </head>
  <body>
    The page contents which includes plain text, formatted text, html elements etc goes here.
  </body>
</html>
```

Javascripts can be used in html in 3 ways 
* inline 
* in header as functions 
* as an external file

The external file has the advantage of separating the concerns into different files, making the code modular and easy for extentios and reuse.

Lets say you want to alert the text inouted upon clicking on OK button

via inline
```
<html>
  <input type="text" id="employeeName" name="employeeName"/>
  <input type="submit" value="ok" onClick="alert(document.getElementById('employeeName').value)"/>
</html>
```

via function in header
```
<html>
  <head>
    <script>
      function showName(){
        alert(document.getElementById('employeeName').value);
      }
    </script>
  </head>
  <body>
    <input type="text" id="employeeName" name="employeeName"/>
    <input type="submit" value="ok" onClick="showName()"/>
  </body>
</html>
```

via function in separate file
myscripts.js
```
  function showName(){
      function showName(){
        alert(document.getElementById('employeeName').value);
  }
```
myhtmlfile.html

```
<html>
  <head>
    <script src=myscript.js></script>
  </head>
  <body>
    <input type="text" id="employeeName" name="employeeName"/>
    <input type="submit" value="ok" onClick="showName()"/>
  </body>
</html>
```




