# Iterators in Lua

![l](https://user-images.githubusercontent.com/116082827/234601751-20f25544-bc67-4ff5-b6f7-57960d86b26f.jpeg)


In Lua, iterators allow you to loop over a collection of data. Here's an example:





function my_iterator(data)

  local index = 0

  local max_index = #data

  return function()

    index = index + 1

    if index <= max_index then

      return data[index]

    else

      return nil

    end

  end

end



local my_data = {1, 2, 3, 4, 5}

for value in my_iterator(my_data) do

  print(value)

end

In this example, the my_iterator function returns an anonymous function that can be used to iterate over a given data array. The for value in my_iterator(my_data) do line initializes the iterator and loops over each value in my_data.
