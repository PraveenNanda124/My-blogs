# Web Storage

![w](https://user-images.githubusercontent.com/116082827/235746148-59def617-4a82-4e21-b670-ce8309a34dec.jpeg)


Web storage is a way to store data in a user's browser using the localStorage and sessionStorage APIs. This can be useful for saving user preferences, caching data, and reducing server requests.

Here's an example of how to use localStorage to store and retrieve data:





<!DOCTYPE html>

<html>

  <head>

    <title>Web Storage Example</title>

    <script>

      function saveData() {

        var name = document.getElementById("name").value;

        localStorage.setItem("username", name);

      }

      function loadData() {

        var name = localStorage.getItem("username");

        document.getElementById("display-name").innerHTML = name;

      }

    </script>

  </head>

  <body onload="loadData()">

    <h1>Welcome</h1>

    <p>Enter your name:</p>

    <input type="text" id="name">

    <button onclick="saveData()">Save</button>

    <p>Your name is: <span id="display-name"></span></p>

  </body>

</html>
