# The ipairs Function in Lua

![l](https://user-images.githubusercontent.com/116082827/234736030-0b6f8999-0d56-4b35-bc96-c19443d868f9.jpeg)


The ipairs function is a built-in Lua function that returns an iterator for iterating over the elements of an array. Here's an example:





local my_array = {"apple", "banana", "cherry", "durian"}

for index, value in ipairs(my_array) do

  print(index, value)

end

In this example, my_array is an array of strings. The for index, value in ipairs(my_array) do line initializes the iterator and loops over each element of the array, returning both the index and the value of each element.
