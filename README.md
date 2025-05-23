# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```
#include <stdio.h>

int main() {
    int M, N, i;
    printf("Enter the starting value (M): ");
    scanf("%d", &M);
    printf("Enter the ending value (N): ");
    scanf("%d", &N);
    printf("Even numbers from %d to %d are:\n", M, N);
    for (i = M; i <= N; i++) {
        // Check if the number is even
        if (i % 2 == 0) {
            printf("%d ", i);
        }
    }

    printf("\n");

    return 0;
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/f46a9a74-9b97-4a70-806d-a25a1f1e72fc)









## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```
#include <stdio.h>

int main() {
   
    int rows;
    printf("Enter the number of rows: ");
    scanf("%d", &rows);
    for (int i = 1; i <= rows; i++) {
        for (int j = 1; j <= i; j++) {
            printf("* ");
        }
        printf("\n"); 
    }

    return 0;
}
```


## OUTPUT:
![image](https://github.com/user-attachments/assets/81ff6743-9275-4526-870c-847762847314)




## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```
#include <stdio.h>
void add(int a, int b);
void subtract(int a, int b);

int main() {
    
    int num1, num2;
    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);
    add(num1, num2);
    subtract(num1, num2);

    return 0;
}

void add(int a, int b) {
    int sum = a + b;
    printf("Addition of %d and %d is: %d\n", a, b, sum);
}
void subtract(int a, int b) {
    int diff = a - b;
    printf("Subtraction of %d and %d is: %d\n", a, b, diff);
}

```


## OUTPUT:
![image](https://github.com/user-attachments/assets/74a835ca-f499-477d-8642-4ad1151d3fee)


## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include <stdio.h>

int main() {

    int num, digit, sum = 0;
    printf("Enter a number: ");
    scanf("%d", &num);
    for (int temp = num; temp > 0; temp /= 10) {
        digit = temp % 10;  
        if (digit % 2 != 0) {  
            sum += digit;      
        }
    }

    printf("Sum of odd digits = %d\n", sum);

    return 0;
}
```


## OUTPUT:
![image](https://github.com/user-attachments/assets/7fe16c95-5248-47af-b1eb-bfd214a37243)




## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include <stdio.h>

void fact();

int main() {

    fact();
    return 0;
}

void fact() {
    int i, N;
    long long factorial = 1;  

    printf("Enter a positive integer: ");
    scanf("%d", &N);


    if (N < 0) {
        printf("Factorial is not defined for negative numbers.\n");
        return;
    }
    for (i = 1; i <= N; i++) {
        factorial *= i;
    }

    printf("Factorial of %d is: %lld\n", N, factorial);
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/5e24443f-0dd4-4222-88c9-659200017e02)


## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
