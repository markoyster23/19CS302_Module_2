# EX 9 C program to find the sum of odd digits using do while loop.
## DATE:
## AIM:
To write a program to print the string "KEYBOARD" n number of times.
## Algorithm
1. To understand how to extract individual digits of a number.
2. To learn how to identify odd digits using conditional statements.
3. To implement the do-while loop in C.
4. To perform cumulative addition based on a condition.
5. To develop logical thinking for solving digit-based problems.
6. END
## Program:
```
#include <stdio.h>

int main() {
    int number, digit, sum = 0;

    // Input from user
    printf("Enter a positive integer: ");
    scanf("%d", &number);

    int temp = number; // Store original number for display

    if (number == 0) {
        sum = 0;
    } else {
        // Loop to extract and check each digit
        do {
            digit = number % 10;      
            if (digit % 2 != 0) {    
                sum += digit;         
            }
            number /= 10;            
        } while (number > 0);
    }
    printf("Sum of odd digits in %d = %d\n", temp, sum);

    return 0;
}

```

## Output:
Enter a positive integer: 52693
Sum of odd digits in 52693 = 17


## Result:
Thus the program was executed and the output was verified successfully.
