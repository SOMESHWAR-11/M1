# NAME: SOMESHWAR S
# REG NO: 212224040322
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
```
#include <stdio.h>

int main(){

char ch1, ch2, ch3;
scanf(" %c", &ch1);
scanf(" %c", &ch2);
scanf(" %c", &ch3);
printf("The reverse of %c%c%c is %c%c%c\n", ch1, ch2, ch3, ch3, ch2, ch1);
}
```

## OUTPUT:

![437965683-4e4e7e1f-5e98-49c4-bb63-c88cf183b691](https://github.com/user-attachments/assets/fda74988-7e76-45fe-a6a4-31013d4cc094)

## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:
```
#include <stdio.h>

int main()
{
    int A;
    scanf("%d", &A);
    if (A > 0)
    {
        printf("number is positive");
    }
    else if (A == 0)
    {
        printf("number is 0");
    }
    else
    {
        printf("number is negative");
    }
    return 0;
}
```
# OUTPUT:

![437965792-bb12f798-1e58-4182-9538-ecdddc5ed28b](https://github.com/user-attachments/assets/d886a8af-645b-43fd-a687-76a4d2b04f8e)

# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
```
#include <stdio.h>

int main() {
    int num1, den1, num2, den2;
    float frac1, frac2, min;

    printf("Enter numerator and denominator of first fraction: ");
    scanf("%d%d", &num1, &den1);

    printf("Enter numerator and denominator of second fraction: ");
    scanf("%d%d", &num2, &den2);

    frac1 = (float)num1 / den1;
    frac2 = (float)num2 / den2;

    min = (frac1 < frac2) ? frac1 : frac2;

    printf("The minimum of the two fractions is: %.2f\n", min);

    return 0;
}
```

## OUTPUT:

![437966158-fe488f5c-bade-41be-a478-c3b633f74cd6](https://github.com/user-attachments/assets/90ca2340-0566-4842-8b0b-b42eee6d1bfd)

## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.


# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:
```
#include <stdio.h>

int main() {
    int a;
    scanf("%d", &a);

    if (a == 1) {
        printf("The input value is equal to 1.\n");
    }

    if (a != 1) {
        printf("The input value is not equal to 1.\n");
    }

    return 0;
}
```

## OUTPUT:
![437966218-f6d9c64c-5f7a-4543-bd35-1d7e42fda214](https://github.com/user-attachments/assets/f71e22fe-a2cf-46dd-b020-f5b1a6deeaf5)

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:
```
#include <stdio.h>

int main() {
    int m1, m2, m3;
    float tot, per;

    printf("Enter marks for three subjects: ");
    scanf("%d%d%d", &m1, &m2, &m3);

    tot = m1 + m2 + m3;
    per = tot / 3;

    printf("Total Marks = %.2f\n", tot);
    printf("Percentage = %.2f%%\n", per);

    if (m1 >= 40 && m2 >= 40 && m3 >= 40 && per >= 60) {
        printf("Division = First\n");
    } else if (per >= 48) {
        printf("Division = Second\n");
    } else if (per >= 36) {
        printf("Division = Pass\n");
    } else {
        printf("Division = Fail\n");
    }

    return 0;
}
```

## OUTPUT:

![437966288-7a683cc1-a3a8-4ad9-b104-1650367c851b](https://github.com/user-attachments/assets/5d2e6185-6078-4cee-8473-78d35ac3663a)

## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

