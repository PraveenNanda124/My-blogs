# Tables as Arrays in Lua

![l](https://user-images.githubusercontent.com/116082827/234663956-e2335f0a-e477-4685-8e23-25e41aac62dd.png)


Lua's tables can be used to represent arrays, with integer keys and consecutive indices starting at 1. Here's an example:





local my_array = {"apple", "banana", "cherry", "durian"}

for i = 1, #my_array do

  print(my_array[i])

end

In this example, my_array is an array of strings. The for i = 1, #my_array do line loops over each element of the array using its index.
