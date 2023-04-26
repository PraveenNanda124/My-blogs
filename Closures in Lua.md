 # Closures in Lua



In Lua, closures are functions that have access to variables outside of their local scope. Here's an example:





function counter()

  local count = 0

  return function()

    count = count + 1

    return count

  end

end



local c1 = counter()

print(c1()) -- prints 1

print(c1()) -- prints 2



local c2 = counter()

print(c2()) -- prints 1

print(c1()) -- prints 3

In this example, the counter function returns an anonymous function that increments a local variable count and returns its new value. Each time the anonymous function is called, it modifies its own count variable, which is unique to that instance of the function.
