 # File I/O in Lua

![l](https://user-images.githubusercontent.com/116082827/234808026-b4eeb72b-f12d-4ecd-8dfa-915c6b64ee21.jpeg)


Lua supports file I/O operations for reading and writing files. Here's an example:



local file = io.open("myfile.txt", "w")

file:write("Hello, world!\n")

file:close()



file = io.open("myfile.txt", "r")

local contents = file:read("*all")

file:close()



print(contents)

In this example, a file named "myfile.txt" is opened for writing using the io.open function, and a string is written to the file using the file:write method. The file is then closed using the file:close method. Next, the file is opened again for reading, and its contents are read into a string using the file:read method with the "*all" pattern. Finally, the file is closed again and the contents are printed to the console.







