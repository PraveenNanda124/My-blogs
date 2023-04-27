# Metatables and Metamethods in Lua

![l](https://user-images.githubusercontent.com/116082827/234774869-5459e4e3-cf87-4577-9af1-7346257d44cd.jpeg)


Metatables and metamethods allow you to define custom behavior for tables in Lua. Here's an example:





local my_table = {1, 2, 3}



local my_metatable = {

  __add = function (table1, table2)

    local result = {}

    for i = 1, #table1 do

      result[i] = table1[i] + table2[i]

    end

    return result

  end

}



setmetatable(my_table, my_metatable)



local another_table = {4, 5, 6}

local sum_table = my_table + another_table



for i = 1, #sum_table do

  print(sum_table[i])

end

In this example, my_table is a table of integers. The __add metamethod is defined in my_metatable, which is then set as the metatable for my_table using the setmetatable function. When my_table is added to another_table, the __add metamethod is called and returns a new table with the sums of the corresponding elements in both tables.
