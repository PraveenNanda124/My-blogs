# Promise.allSettled

![j](https://user-images.githubusercontent.com/116082827/236264966-e0e0d6c9-e369-450f-aded-853173e4bcee.png)


The Promise.allSettled method is a new addition to JavaScript's Promise API. It allows you to wait for all promises in an array to settle (i.e., either fulfill or reject), regardless of their outcome. Here's an example:



const promise1 = Promise.resolve('Success!');

const promise2 = Promise.reject('Error!');

const promise3 = Promise.resolve('Another success!');



Promise.allSettled([promise1, promise2, promise3])

  .then(results => console.log(results))

  .catch(error => console.error(error));



// Output:

// [

//   {status: "fulfilled", value: "Success!"},

//   {status: "rejected", reason: "Error!"},

//   {status: "fulfilled", value: "Another success!"}

// ]

In the code above, we create three promises (promise1, promise2, and promise3) with different outcomes. We then pass them to Promise.allSettled, which returns a new promise that resolves to an array of objects with a status property that indicates whether the promise was fulfilled or rejected, and a value or reason property that contains the fulfillment value or rejection reason, respectively.
