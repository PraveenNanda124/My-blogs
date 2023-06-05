# C++20 Contracts

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/bda3cf04-a92a-44d6-b3b6-8504da10ae96)


C++20 introduced the concept of contracts, which allow programmers to define preconditions, postconditions, and assertions within their code. Contracts provide a way to specify expectations and requirements at various points in a program, improving code clarity, robustness, and maintainability. Here's an example demonstrating the usage of contracts:



#include <iostream>

#include <cassert>



int divide(int a, int b) noexcept

    requires(b != 0)

{

    return a / b;

}



int main() {

    int a = 10;

    int b = 0;



    int result = divide(a, b);



    std::cout << "Result: " << result << std::endl;



    return 0;

}

In the above code, we define a divide function that performs integer division. We use the requires clause to specify a contract that states the function is only applicable when the second argument (b) is not equal to zero. This serves as a precondition for the function.



Within the function, we use the assert macro to validate the contract. If the contract is violated, the assert macro will trigger an assertion failure.



In the main() function, we call the divide function with an a value of 10 and a b value of 0. Since the precondition is not satisfied, the program will terminate with an assertion failure.



Contracts provide a formal and explicit way to express expectations and requirements in code, helping catch errors and prevent invalid behavior. They enhance code clarity, maintainability, and robustness.



It's important to note that the contract support in C++20 is still experimental, and the exact syntax and semantics may evolve in future revisions of the C++ standard.
