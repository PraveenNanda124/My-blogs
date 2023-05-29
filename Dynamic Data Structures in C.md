# Dynamic Data Structures

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/129d6d6a-68f8-4789-b0ad-5707a817fb8d)


In addition to arrays, C allows you to create dynamic data structures such as linked lists, stacks, queues, and trees. Implementing these data structures enhances your ability to manage complex data efficiently.





#include <stdio.h>

#include <stdlib.h>



struct Node {

    int data;

    struct Node* next;

};



struct Stack {

    struct Node* top;

};



void push(struct Stack* stack, int data) {

    struct Node* newNode = (struct Node*)malloc(sizeof(struct Node));

    newNode->data = data;

    newNode->next = stack->top;

    stack->top = newNode;

}



int pop(struct Stack* stack) {

    if (stack->top == NULL) {

        printf("Stack underflow\n");

        return -1;

    }



    struct Node* temp = stack->top;

    int data = temp->data;

    stack->top = stack->top->next;

    free(temp);



    return data;

}



int main() {

    struct Stack stack;

    stack.top = NULL;



    push(&stack, 3);

    push(&stack, 2);

    push(&stack, 1);



    printf("Popped element: %d\n", pop(&stack));

    printf("Popped element: %d\n", pop(&stack));

    printf("Popped element: %d\n", pop(&stack));

    printf("Popped element: %d\n", pop(&stack));



    return 0;

}
