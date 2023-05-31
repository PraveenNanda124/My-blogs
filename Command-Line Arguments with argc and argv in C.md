# Command-Line Arguments with argc and argv in C

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/6b1345b0-5ed4-44ca-932b-b5e52644e1db)


The argc and argv parameters of the main function allow you to handle command-line arguments passed to a C program. argc represents the number of arguments, and argv is an array of strings containing the actual arguments.



#include <stdio.h>



int main(int argc, char* argv[]) {

    printf("Number of arguments: %d\n", argc);



    printf("Arguments:\n");

    for (int i = 0; i < argc; i++) {

        printf("%d: %s\n", i, argv[i]);

    }



    return 0;

}

When running the program from the command line, you can pass arguments after the program name:



./program arg1 arg2 arg3

The program will print the number of arguments and list them with their respective indices.
