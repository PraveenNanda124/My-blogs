# Optional catch binding

![j](https://user-images.githubusercontent.com/116082827/236297290-4817a509-ac0a-4293-a800-0fbf88436b4b.png)


The optional catch binding is a new feature in JavaScript that allows you to omit the catch parameter if you don't need it. Here's an example:



try {

  // some code that might throw an error

} catch {

  // handle the error without a catch parameter

}

In the code above, we're using a try-catch block to handle errors that might occur in some code. Since we don't need to access the error object in the catch block, we can omit the catch parameter altogether.
