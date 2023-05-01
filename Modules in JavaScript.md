# Modules in JavaScript

![m](https://user-images.githubusercontent.com/116082827/235474342-9fcf37ac-04cc-4764-b4ed-69e45e27d251.jpeg)


JavaScript modules allow you to organize your code into separate files and export/import functionality between them.



Here is an example of exporting a function from a module:





// math.js

export function square(x) {

  return x * x;

}



// app.js

import { square } from './math.js';



console.log(square(5)); // 25

In this example, we export a square function from a math.js module and import it into an app.js module using the import statement.



These are just a few examples of new and important JavaScript topics. I hope this gives you an idea of some areas to explore further!
