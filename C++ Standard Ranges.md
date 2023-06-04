# C++ Standard Ranges

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/2fc4c354-b8a4-4fdf-b422-056315613daa)


C++20 introduced the Standard Ranges library, which provides a set of algorithms and range adaptors that operate on sequences of elements. It offers a more expressive and composable way to work with ranges, making code more readable and reducing boilerplate. Here's an example demonstrating the usage of Standard Ranges:



#include <iostream>

#include <vector>

#include <ranges>



int main() {

    std::vector<int> numbers = {1, 2, 3, 4, 5};



    // Filtering even numbers and mapping to squares

    auto result = numbers | std::views::filter([](int x) { return x % 2 == 0; })

                          | std::views::transform([](int x) { return x * x; });



    for (int num : result) {

        std::cout << num << " ";

    }

    std::cout << std::endl;



    return 0;

}

In the above code, we have a vector numbers containing a sequence of integers. We use the pipe operator | to compose a series of operations on the numbers range. We first filter the even numbers using the filter view and then transform each element by squaring it using the transform view.



The result is a range of filtered and transformed values. We iterate over this range using a range-based for loop and print each number.



The Standard Ranges library provides a rich set of algorithms and adaptors that can be combined and chained together to perform complex operations on ranges, simplifying code and making it more readable.
