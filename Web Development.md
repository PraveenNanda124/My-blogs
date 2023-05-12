# Web Development

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/47955b38-0138-412a-8949-b2983345b51e)


Web development involves creating web applications that run in a web browser. It typically involves using web technologies such as HTML, CSS, and JavaScript to create the user interface, and a back-end programming language to handle server-side logic.

Example of a simple web application using HTML, CSS, and JavaScript:





<!DOCTYPE html>

<html>

  <head>

    <title>My Web App</title>

    <style>

      body {

        font-family: Arial, sans-serif;

      }

      h1 {

        color: #007bff;

      }

    </style>

  </head>

  <body>

    <h1>Welcome to my web app</h1>

    <p>Enter your name:</p>

    <input type="text" id="name">

    <button onclick="greet()">Greet</button>

    <p id="greeting"></p>

    <script>

      function greet() {

        var name = document.getElementById("name").value;

        document.getElementById("greeting").innerHTML = "Hello, " + name + "!";

      }

    </script>

  </body>

</html>
