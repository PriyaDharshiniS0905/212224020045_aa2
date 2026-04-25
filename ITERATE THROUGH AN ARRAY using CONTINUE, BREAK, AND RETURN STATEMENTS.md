## Write a C program that iterates through an array and, within a loop, uses continue  to skip negative elements, break when a zero is encountered, and return to exit the program if an element greater than 100 is found, then print the resulting behavior for the array {10, -5, 20, 0, 150, 30}.

## Aim
To ITERATE THROUGH AN ARRAY using CONTINUE, BREAK, AND RETURN STATEMENTS.

## Algorithm
1.START

2.INITIALIZE array {10, -5, 20, 0, 150, 30}

3.TRAVERSE the array using loop

4.If element is NEGATIVE → CONTINUE

5.If element is ZERO → BREAK

6.If element is GREATER THAN 100 → RETURN

7.PRINT valid elements

8.STOP

## Program
~~~
#include <stdio.h>

int main() {
    int a[] = {10, -5, 20, 0, 150, 30};
    int i;

    for(i = 0; i < 6; i++) {

        if(a[i] < 0)
            continue;

        if(a[i] == 0)
            break;

        if(a[i] > 100)
            return 0;

        printf("%d ", a[i]);
      }
      return 0;
}
~~~

## Output 
<img width="803" height="233" alt="image" src="https://github.com/user-attachments/assets/951525f4-a7e2-4d34-beef-3a99d7237693" />

## Result 
Thus, the code executed successfully
