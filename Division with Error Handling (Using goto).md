## Write a C program that performs division of two user inputs and uses goto  to handle errors like division by zero or invalid input by redirecting control for re-entry.

## Aim
To perform division and handle division by zero using goto.
## Algorithm
1.Start
2.Input two numbers
3.If denominator = 0 → go to error
4.Perform division
5.Display result
6.Error label → ask re-entry
7.Stop
## Program
~~~
#include <stdio.h>

int main() {
    float a, b;

start:
    printf("Enter two numbers: ");
    scanf("%f %f", &a, &b);

    if(b == 0) {
        printf("Error! Division by zero.\n");
        goto start;
    }

    printf("Result = %.2f\n", a / b);

    return 0;
}


~~~
## OUTPUT

## RESULT 
Thus, the program has been executed successfully .
