# Optional Chaining Operator

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/e9e49878-5f1d-480b-bdcb-294999dd103c)


The optional chaining operator (?.) allows you to access nested properties of an object without worrying about potential null or undefined values.



const person = {

  name: 'John',

  address: {

    street: '123 Main St',

    city: 'New York'

  }

};



const street = person.address?.street;

console.log(street);

// Output: 123 Main St



const zipCode = person.address?.zipCode;

console.log(zipCode);

// Output: undefined

In the example above, the optional chaining operator is used to access the street property of the address object. If any intermediate property in the chain is null or undefined, the result will be undefined.
