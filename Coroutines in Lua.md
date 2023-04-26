# Coroutines in Lua



Coroutines in Lua allow you to suspend and resume the execution of a function. Here's an example:





function coroutine_func()

  for i = 1, 5 do

    print("coroutine_func", i)

    coroutine.yield()

  end

end



co = coroutine.create(coroutine_func)



for i = 1, 10 do

  print("main", i)

  coroutine.resume(co)

end

In this example, the coroutine_func function prints a message and then yields execution. The coroutine.create function creates a new coroutine object based on the coroutine_func. The coroutine.resume function starts or resumes the execution of the coroutine. The output of this code will alternate between messages from the main function and messages from the coroutine function.
