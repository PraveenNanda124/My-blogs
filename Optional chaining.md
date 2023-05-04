 # Optional chaining

![j](https://user-images.githubusercontent.com/116082827/236224176-77c6209d-c40f-4492-9f8e-eea7a21993df.png)


Optional chaining is a new feature in JavaScript that allows you to safely access nested properties or methods of an object, without worrying about whether intermediate properties or methods exist or not. Here's an example:



const person = {

  name: 'John Doe',

  address: {

    street: '123 Main St',

    city: 'New York',

    state: 'NY'

  }

};



console.log(person.address?.zipCode); // Output: undefined

In the code above, the person object has a nested address object. The optional chaining operator (?.) is used to safely access the zipCode property of the address object. If the address property does not exist, undefined will be returned.
