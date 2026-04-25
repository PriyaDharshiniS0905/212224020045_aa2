## Write a C program to print the numbers from 1 to 100 but avoid printing multiples of 3 and number containing digit 5(5,15,25,35,..). Use continue in the program.
## Aim

To print numbers from 1 to 100 excluding multiples of 3 and numbers containing digit 5.

## Algorithm
1.Start

2.Loop from 1 to 100

3.If divisible by 3 → continue

4.If number contains digit 5 → continue

5.Print remaining numbers

6.Stop

 ## Program 
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
## Output
<img width="815" height="257" alt="image" src="https://github.com/user-attachments/assets/ecac3a3a-75ec-480d-8679-a5f68a161a4f" />

## Result
Thus the program has been executed successfully.
