# React Hooks

![r](https://user-images.githubusercontent.com/116082827/235344201-d3114d9a-5baf-4d8d-bdb3-0a3639060723.jpeg)


React Hooks are a way to add state and other React features to functional components. Before hooks, you had to use class components to use state, but now you can use hooks in functional components. Here's an example of using the useState hook to create a counter:





import React, { useState } from 'react';



function Counter() {

  const [count, setCount] = useState(0);



  return (

    <div>

      <p>You clicked {count} times</p>

      <button onClick={() => setCount(count + 1)}>

        Click me

      </button>

    </div>

  );

}

In this code, useState is a hook that takes an initial value (0 in this case) and returns an array with the current state value (count) and a function to update the state (setCount).
