# Modules in Lua



Modules in Lua allow you to organize code into reusable units. Here's an example:





-- mymodule.lua

local M = {}



function M.foo()

  print("hello from mymodule")

end



return M

In this example, mymodule.lua defines a module that contains a single function foo. The return statement at the end of the module makes the M table available to other code that requires the module. Here's an example of using the mymodule module:





local mymodule = require("mymodule")



mymodule.foo() -- prints "hello from mymodule"

In this example, require("mymodule") loads the mymodule module and returns its exported table (M in the previous example). The mymodule.foo() line calls the foo function defined in the module.
