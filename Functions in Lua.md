 Functions in Lua



Functions in Lua are defined using the function keyword. Here's an example:





function add(x, y)

  return x + y

end



local result = add(10, 20)

print(result)

Lua functions can also return multiple values. Here's an example:





function square_and_cube(x)

  return x^2, x^3

end



local square, cube = square_and_cube(3)

print(square, cube)![l](https://user-images.githubusercontent.com/116082827/234358699-ed7d214e-7fdb-4a70-8b22-c29bc2041768.jpeg)
