## Write a C program for a number guessing game where the loop continues for wrong guesses, breaks on a correct guess, and exits the program using return if the user enters -1.
## Aim
To implement a guessing game using loop, break, and return.

## Algorithm

1.Start

2.Fix a number (e.g., 7)

3.Take user input

4.If input = -1 → exit (return)

5.If correct → break

6.Else continue loop

7.Stop

## Program
~~~
#include <stdio.h>

int main() {
    int guess, num = 7;

    while(1) {
        printf("Enter your guess (-1 to quit): ");
        scanf("%d", &guess);

        if(guess == -1)
            return 0;

        if(guess == num) {
            printf("Correct guess!\n");
            break;
        }
        else {
            printf("Wrong guess. Try again.\n");
        }
    }
~~~
## Output

## Result
Thus the program has been executed successfully.
    return 0;
}
