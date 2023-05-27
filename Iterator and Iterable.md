# Iterator and Iterable

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/4c496f84-1dda-4e23-9727-b9052fe60389)


The iterator and iterable protocols provide a way to define and iterate over collections or sequences of data in JavaScript.





const myIterable = {

  [Symbol.iterator]() {

    let count = 0;

    return {

      next() {

        count++;

        if (count <= 5) {

          return { value: count, done: false };

        }

        return { done: true };

      }

    };

  }

};



for (const value of myIterable) {

  console.log(value);

}

// Output: 1, 2, 3, 4, 5

In the example above, the myIterable object implements the iterable protocol by defining a method with the key [Symbol.iterator]. The method returns an iterator object with the next method, which provides the next value in the sequence.
