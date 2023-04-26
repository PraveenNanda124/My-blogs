# Error Handling in Lua



In Lua, you can handle errors using the pcall function. Here's an example:





function divide(x, y)

  if y == 0 then

    error("cannot divide by zero")

  else

    return x / y

  end

end



local status, result = pcall(divide, 10, 0)



if status then

  print("result:", result)

else

  print("error:", result)

end

In this example, the divide function checks for a division by zero error and raises an error using the error function if necessary. The pcall function calls divide with arguments 10 and 0, and captures any errors that occur. If the call was successful, status will be true and result will contain the return value of divide. If an error occurred, status will be false and `
