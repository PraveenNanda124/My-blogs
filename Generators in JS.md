# Generators in JS

![g](https://user-images.githubusercontent.com/116082827/235502178-edd6f928-f59a-4e19-8b24-a49fe66765fa.png)


Generators are functions that can pause and resume their execution, allowing for more flexible control flow in JavaScript. They are created using the function* syntax and the yield keyword.



Here is an example of using a generator to generate a sequence of Fibonacci numbers:



function* fibonacci() {

  let [prev, curr] = [0, 1];

  while (true) {

    [prev, curr] = [curr, prev + curr];

    yield curr;

  }

}



const fib = fibonacci();



console.log(fib.next().value); // 1

console.log(fib.next().value); // 2

console.log(fib.next().value); // 3

console.log(fib.next().value); // 5

In this example, we create a generator function fibonacci that generates an infinite sequence of Fibonacci numbers using the yield keyword. We then create a generator object fib from this function and use the .next() method to retrieve each successive value.
