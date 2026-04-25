# #  Write a C program to traverse a 2D matrix and print the values until a negative number is found. Use break statement.

## AIM 

To print numbers from 1 to 100 excluding multiples of 3 and numbers containing digit 5.

## ALGORITHM 

1.Start

2.Loop from 1 to 100

3.If divisible by 3 → continue

4.If number contains digit 5 → continue

5.Print remaining numbers

6.Stop

## PROGRAM
~~~
#include <stdio.h>

int main() {
    int i, temp;

    for(i = 1; i <= 100; i++) {
        if(i % 3 == 0)
            continue;

        temp = i;
        while(temp > 0) {
            if(temp % 10 == 5)
                break;
            temp /= 10;
        }
        if(temp > 0)
            continue;

        printf("%d ", i);
    }

    return 0;
}
~~~

## OUTPUT
<img width="808" height="252" alt="image" src="https://github.com/user-attachments/assets/d3c4b713-45e8-43ca-93c1-739d946b5580" />

## RESULT
Thus the program has been executed successfully.

