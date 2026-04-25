# #  Write a C program to traverse a 2D matrix and print the values until a negative number is found. Use break statement.

## AIM 
To traverse a 2D matrix element-by-element and terminate all processing immediately upon encountering a negative value using the break statement.

## ALGORITHM 

1.Initialize a 2x2 matrix and a "stop" flag to 0.

2. Start the outer loop to iterate through each row.
  
3. Start the inner loop to iterate through each column.

4. Check if the current element is negative.
   
5. Break the inner loop and set the flag to 1 if a negative is found.

6. Check the flag in the outer loop and break immediately if it is 1.

7. Print the current element if no negative has been encountered yet.

## PROGRAM
~~~
#include <stdio.h>

int main() {
    int matrix[2][2] = {
        {1, 2},
        {-3, 4}
    };

    int foundNegative = 0;

    printf("Scanning 2x2 Matrix:\n");

    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 2; j++) {
            if (matrix[i][j] < 0) {
                foundNegative = 1;
                break; // Breaks the column loop
            }
            printf("Value at [%d][%d]: %d\n", i, j, matrix[i][j]);
        }

        if (foundNegative) {
            printf("Negative value found! Stopping traversal.\n");
            break; // Breaks the row loop
        }
    }

    return 0;
}
~~~

## OUTPUT
<img width="809" height="271" alt="image" src="https://github.com/user-attachments/assets/a56dffdf-5f06-44e9-a667-7ffc9908bf13" />

## RESULT
Thus the program has been executed successfully.

