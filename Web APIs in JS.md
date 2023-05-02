# Web APIs in JS

![w](https://user-images.githubusercontent.com/116082827/235563565-33707152-9a04-432e-a018-4be86c4e8c60.png)


JavaScript is not just used for web development, but it is a crucial part of web development. It powers many of the Web APIs that enable modern web applications to access device features, interact with servers, and more.



Here is an example of using the fetch API to make a network request:





fetch('https://jsonplaceholder.typicode.com/posts')

  .then(response => response.json())

  .then(data => console.log(data))

  .catch(err => console.error(err));

In this example, we use the fetch API to make a GET request to the JSONPlaceholder API and retrieve a list of posts. We use the Promise syntax to handle the response and any errors.
