# Private class fields

![j](https://user-images.githubusercontent.com/116082827/236367264-94b6e5d9-1a5d-47a9-9dad-81703c99ddb5.png)


Private class fields are a new feature in JavaScript that allow you to define private properties and methods in a class. Private fields are only accessible from within the class, and cannot be accessed or modified from outside the class. Here's an example:



class Person {

  #name;



  constructor(name) {

    this.#name = name;

  }



  greet() {

    console.log(`Hello, my name is ${this.#name}`);

  }

}



const john = new Person('John');

john.greet(); // Output: 'Hello, my name is John'



console.log(john.#name); // Output: Uncaught SyntaxError: Private field '#name' must be declared in an enclosing class

In the code above, we're defining a private field #name in the Person class, and a greet method that accesses the private field. We can create instances of the class (john), and call the greet method on them, but we cannot access the private field directly from outside the class.
