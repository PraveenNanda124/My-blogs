# Template Literals

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/d177d713-c31a-4abb-b6ee-99ec21cb1fea)


Template literals provide an improved way to work with strings in JavaScript. They allow you to embed expressions and multiline strings easily.



const name = 'John';

const age = 30;



console.log(`My name is ${name} and I am ${age} years old.`);

// Output: My name is John and I am 30 years old.



const multilineString = `

This is a multiline string.

It can span across multiple lines.

`;

console.log(multilineString);

/* Output:

This is a multiline string.

It can span across multiple lines.

*/

In the example above, the ${} syntax is used within the template literal to embed expressions (variables, calculations, etc.) within the string. Additionally, template literals can span multiple lines without needing to concatenate strings.
