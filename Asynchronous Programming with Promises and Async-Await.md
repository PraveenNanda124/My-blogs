# Asynchronous Programming with Promises and Async/Await

![a](https://user-images.githubusercontent.com/116082827/235464842-056b9ecb-03ac-4b3f-a42e-2ebbc14a1332.png)


Asynchronous programming allows your code to execute non-blocking I/O operations, which can improve the performance of your applications. JavaScript supports asynchronous programming through callbacks, but Promises and Async/Await provide more convenient and readable syntax.



Here is an example of using Promises:





function getUser(id) {

  return new Promise((resolve, reject) => {

    setTimeout(() => {

      resolve({ id: id, username: 'johnDoe' });

    }, 2000);

  });

}



getUser(1)

  .then(user => console.log(user))

  .catch(err => console.error(err));

In this example, the getUser function returns a Promise that resolves with a user object after 2 seconds. We use the .then() method to handle the resolved value and the .catch() method to handle any errors.



Here is the same example using Async/Await:





async function displayUser() {

  try {

    const user = await getUser(1);

    console.log(user);

  } catch (err) {

    console.error(err);

  }

}



displayUser();

In this example, the displayUser function is declared as async, which allows us to use the await keyword to wait for the Promise to resolve before continuing. We use a try/catch block to handle any errors.
