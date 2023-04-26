 # Bitwise Operators in Lua
![l](https://user-images.githubusercontent.com/116082827/234656248-292d6162-96c6-4829-919c-cb1489d3f930.jpeg)



Lua supports bitwise operators that operate on integers at the bit level. Here's an example:





local x = 0x0F

local y = 0x10



print(bit.band(x, y)) -- bitwise AND

print(bit.bor(x, y)) -- bitwise OR

print(bit.bxor(x, y)) -- bitwise XOR

print(bit.bnot(x)) -- bitwise NOT

print(bit.lshift(x, 2)) -- bitwise left shift

print(bit.rshift(x, 2)) -- bitwise right shift

In this example, x and y are hexadecimal values that are used to demonstrate the various bitwise operators available in Lua.
