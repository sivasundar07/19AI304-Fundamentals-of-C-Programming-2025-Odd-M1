# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
#include <stdio.h>
int main()
{
    int integer=10;
    float decimal=3.14;
    char character='A';
    char character1[]="Hello C";
    printf("INTEGER LITERAL : %d , SIZE OF INTEGER LITERAL IS : %ld bytes\n", integer, sizeof(integer) );
    printf("FLOAT LITERAL : %f , SIZE OF FLOAT LITERAL IS : %ld bytes\n", decimal, sizeof(decimal) );
    printf("CHARACTER LITERAL : %c , SIZE OF CHARACTER LITERAL IS : %ld bytes\n", character, sizeof (character));
    printf("STRING LITERAL : %s , SIZE OF STRING LITERAL IS : %ld bytes\n", character1, sizeof(character1) );
    return 0;
}
# Output:
<img width="1920" height="1080" alt="c1" src="https://github.com/user-attachments/assets/73fa1d6b-41ed-4e33-9271-c7007a5f683b" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
#include <stdio.h>
#define PI 3.14159
int main()
{
    const int DAYS = 7; 
    printf("Value of macro constant PI = %.5f\n", PI);
    printf("Value of constant variable DAYS = %d\n", DAYS);
    return 0;
}
# Output:
<img width="1920" height="1080" alt="C2" src="https://github.com/user-attachments/assets/148b0131-0def-456b-a958-ba0e95cdcdca" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
#include <stdio.h>
int main()
{
    int num;
    float dec;
    double dec2;
    char charac;
    printf("ENTER INTEGER:");
    scanf("%d", &num);
    printf("\nENTER DECIAML:");
    scanf("%f", &dec);
    printf("\nENTER DOUBLE:");
    scanf("%lf", &dec2);
    printf("\nENTER CHARACTER:");
    scanf(" %c", &charac);
    printf("\nOUTPUT:\n\n");
    printf("INTERGER :%d\n\n", num);
    printf("FLOAT :%f\n\n", dec);
    printf("DOUBLE :%lf\n\n", dec2);
    printf("CHARACTER :%c\n\n", charac);
    
}
# Output:
<img width="1920" height="1080" alt="c3" src="https://github.com/user-attachments/assets/03188f0a-ac6d-44db-ab8d-0defe955b24a" />

# Result: 

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
#include <stdio.h>
int main()
{
    int a, b;
    printf("ENTER NUMBER 1:");
    scanf("%d", &a);
    printf("ENTER NUMBER 2:");
    scanf("%d", &b);
    printf("ARITHMATIC OPERATIONS :\n");
    printf("ADDITION : %d\n", a+b);
    printf("SUBRACTION : %d\n", a-b);
    printf("MULTIPLICATION : %d\n", a*b);
    printf("DIVISION : %d\n", a/b);
    printf("REMAINDER : %d\n", a%b);
    printf("BITWISE OPERATIONS :\n");
    printf("AND : %d\n", a&b);
    printf("OR : %d\n", a|b);
    printf("XOR : %d\n", a^b);
    printf("LEFT SHIFT : %d\n", a<<b);
    printf("RIGHT SHIFT : %d\n", a>>b);
    printf("NOT a: %d\n", ~a);
    printf("NOT b: %d\n", ~b);
    return 0;
}
# Output:
<img width="1920" height="1080" alt="c4" src="https://github.com/user-attachments/assets/576b2f9a-9f21-4f30-bf47-8df52fdf4349" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
#include <stdio.h>
int main() 
{
    char value;
    printf("ENTER CHARACTER :"); 
    scanf("%c", &value); 
    ( value >= '0' && value <='9') ? printf("Digit") : 
    ((value >='a' && value <='z') || (value >='A' && value <='Z')) ?
     ((value == 'a' || value == 'e' || value == 'i' || value == 'o' || value=='u') || (value == 'A' || value == 'E' || value == 'I' || value == 'O' || value=='U') ) ?
      printf("Vowel") : printf("Consonant"): printf("Special character");
    return 0; 
}
# Output:
<img width="1920" height="1080" alt="C5" src="https://github.com/user-attachments/assets/b9fbb8e7-b29d-4077-a207-d96ffdca8758" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


