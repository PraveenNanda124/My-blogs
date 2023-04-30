# TypeScript

![t](https://user-images.githubusercontent.com/116082827/235348219-d613072b-f104-48a4-a743-bf4e5ddb4094.png)


TypeScript is a superset of JavaScript that adds static typing and other features to help catch errors at compile time instead of runtime. Here's an example of using TypeScript to create a function that takes two numbers and returns their sum:





function addNumbers(a: number, b: number): number {

  return a + b;

}

In this code, we're using the : number syntax to specify that the function should return a number. We're also using the : number syntax to specify that both a and b should be numbers. If we try to pass a non-number to this function, TypeScript will give us an error at compile time instead of letting the error happen at runtime.
