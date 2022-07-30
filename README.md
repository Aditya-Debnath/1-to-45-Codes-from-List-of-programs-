# 1-to-45-Codes-from-List-of-programs
1 to 45 codes from the "List of programs" of CSE 103

1. Write a C program to get an input from keyboard and print it.
Ans :-

#include<stdio.h>

int main()

    {

    // If you want to take Character.
    char c;
    scanf("%c",&c);
    printf("%c",c);

    // If you want to take Integer number.
    int a;
    scanf("%d",&a);
    printf("%d",a);

    // If you want to take float/double number.
    double b;
    scanf("%lf",&b);
    printf("%lf",b);
    
    return 0;
    }

2. Write a C program to get two numbers from keyboard and add them.
Ans :-

#include<stdio.h>

int main()

{

    int A,B,sum;
    
    printf("Enter the value of 1st number =");
    scanf("%d",&A);
    printf("Enter the value of 2ed number =");
    scanf("%d",&B);
    
    sum=A+B;
    
    printf("The sum of two number = %d\n", sum);
    return 0;

}

3. Write a C program to check an integer whether odd or even.
Ans :-

#include <stdio.h>

int main()

{

    int a;
    
    printf("Give me number=");
    scanf("%d",&a);
    
    if (a%2!=0)
    printf("The number is odd\n");
    else
    printf("The number is even\n");

}

4. Write a C program C program to perform addition, subtraction, multiplication and division.
Ans :-

5. Write a C program to swap two numbers.
Ans :-

#include<stdio.h>

int main()

{

    int a, b, temp;
    
    printf("Enter two number\n");
    scanf("%d %d", &a,&b);
    printf("Before Swap: a=%d, b=%d\n", a, b);
    
    temp = a;
    a = b;
    b = temp;
    
    printf("After Swap: a=%d, b=%d", a, b);

    return 0;

}

6. Write a C program to check whether a given integer is positive.
Ans :-

#include<stdio.h>

int main()

{

    int Number;
    
    printf("Input a number :");
    scanf("%d", &Number);
    
    if (Number >= 0)
        printf("%d is a positive number\n", Number);
    else
        printf("%d is a negative number\n", Number);
    return 0;

}

7. Write a c program C program to check whether input alphabet is a vowel or not.
Ans :-

By using ""if else condition"" >>

include<stdio.h>

int main()

{

    char Input_a_alphabet;
    int isLowercaseVowel, isUppercaseVowel;

    printf("Enter an alphabet =");
    scanf("%c",&Input_a_alphabet);

    // evaluates to 1 (true) if Input a number is a lowercase vowel
    isLowercaseVowel = (Input_a_alphabet == 'a' || Input_a_alphabet == 'e' || Input_a_alphabet == 'i' || Input_a_alphabet == 'o' || Input_a_alphabet == 'u');
    // evaluates to 1 (true) if Input a number is a uppercase vowel
    isUppercaseVowel = (Input_a_alphabet == 'A' || Input_a_alphabet == 'E' || Input_a_alphabet == 'I' || Input_a_alphabet == 'O' || Input_a_alphabet == 'U');

    // evaluates to 1 (ture) if either isLowercaseVowel or isUppercaseVowel is true
    if (isLowercaseVowel || isUppercaseVowel)
        printf("%c is a vowel", Input_a_alphabet);
    else
        printf("%c is not a vowel", Input_a_alphabet);
    return 0;

}

By using ""Switch"" >> ( Don't use untill I remove this sentence. :D )

#include<stdio.h>
#include<conio.h>

main()

{
    char Input_a_alphabet;
    printf("Enter the alphabet =");
    Input_a_alphabet=getche();
    switch(Input_a_alphabet)
    {
       case 'a':
       case 'e':
       case 'i':
       case 'o':
       case 'u':
       printf(" is a vowel\n");
       break;
       default:
       printf(" is not a vowel");
    }
    getch();
}

8. Write a C program to check leap year.
Ans :-

#include<stdio.h>

main()

{

    int Year;
    printf("Enter the year");
    scanf("%d", &Year);
    if (Year%400==0 || (Year%100!=0 && Year%4==0))
        printf("%d is a leap year",Year);
    else
        printf("%d is not a leap year",Year);
    return 0;

}

9. Write a C program to find the largest of 3 numbers.
Ans :-

#include<stdio.h>
int main()
{

    int Number1,Number2,Number3;
    printf("The three numbers =\n");
    scanf("%d %d %d",&Number1,&Number2,&Number3);

    if ((Number1>Number2)&&(Number1>Number3))
                            {
        printf("\n %d is the largest number.",Number1);
                            }
    else if ((Number2>Number1)&&(Number2>Number3))
        {
        printf("\n %d is the largest number.",Number2);
        }
    else{
        printf("\n %d is the largest number.",Number3);
        }
    return 0;

}

10. Write a C program to solve the quadratic equation.

11. Write a C program to display the consecutive digits 0, 1, 2, . . . ,9.
Ans :-

******* You can use any loop. Just like >> while loop, for loop, do while loop.

#include<stdio.h>
int main()

{

    int i;

    for(i=0;i<9;i++)
    {
        printf("%d,",i);
    }

    if(i<10)
        {
            printf("%d.",i);
        }

    return 0;

}

12. Write a C program to find the sum of odd and even numbers from 1 to N.
Ans :-

#include<stdio.h>
int main()

{

    int N, i, Even_Sum = 0, Odd_Sum = 0;

    scanf("%d",&N);

    for(i=1 ; i<=N ; i++)
    {
        if(i%2==0)
        {
            Even_Sum = Even_Sum + i;
        }
        else
        {
            Odd_Sum = Odd_Sum + i;
        }
    }

    printf("Even sum is %d\n",Even_Sum);
    printf("Odd sum is %d\n",Odd_Sum);

}

13. Write a C program to calculate factorial of a number.
Ans :-

14. Write a C program to find the average of a list of numbers.
Ans :-

#include<stdio.h>
int main()

{

    int N, i, sum = 0,a;
    float average;

    scanf("%d",&N);

    for(i = 0 ; i < N ; i++)
    {
        scanf("%d",&a);
        sum = sum + a;
    }

    average = sum/N;
    printf("%f",average);

    return 0;

}

15. Write a C program to find the greatest common divisor (GCD) and least common
multiple (LCM) of two numbers.

16. Write a C program to find the number of integers divisible by 5 between the given range num1 and num2, where num1 < num2. Also find the sum of all these integer numbers, which are divisible by 5 and display the total.
Ans:-

#include<stdio.h>
int main()
{

   int i, Num1, Num2, count, sum = 0;

   printf("Enter the value of Num1 and Num2\n");
   scanf("%d %d",&Num1,&Num2);
   printf("Integers divisible by 5 are\n");

   for (i=Num1;i<Num2;i++)
   {
      if (i%5==0)
      {
         printf("%d,",i);
         count++;
         sum = sum + i;
      }
   }

  printf("\nNumber of integers divisible by 5 between %d and %d = %d\n",Num1,Num2,count);
  printf("Sum of all integers that are divisible by 5 = %d\n",sum);

  return 0;
  
}


17. Write a C program to convert a line of lowercase text to uppercase.

18. Write a program that asks user an arithmetic operator('+','-','*' or '/') and two operands and perform the corresponding calculation on the operands.

19. Write a C program to find the average of maximum of N positive numbers entered by user. But if the input is negative, display the average (excluding the average 
of negative input) and end the program.

20. Write a C program to find the average of a list of positive numbers only. If user enters negative number skip it.
Ans :-

#include<stdio.h>

int main()

{

    int a, i, N, sum = 0, count;
    
    float Average;
    scanf("%d",&N);
    
    for(i = 0 ; i < N ; i++)
    {
        scanf("%d",&a);
        if(a>0)
        {
        sum = sum + a;
        count++;
        }
        else
        {
           printf("SKIP\n");
        }
    }
    Average = sum/count;
    printf("%f",Average);
    
    return 0;

}


21. Write a C program to find the product of N integers entered by user. If user enters 0 skip it.

22. C program to find nCr and nPr: This code calculate nCr which is n!/(r!*(n-r)!) and nPr = n!/(n-r)!

23. Write C Program to reverse a number.

24. Write a C program to check Palindrome number: A palindrome number is a number such that if we reverse it, it will not change.

25. Write a C program to print patterns of numbers and stars.
         *
        ***
       *****
      *******
     *********
     
26. Write a C program to print the diamond patterns of stars.
         *
        ***
       *****
        ***
         *
         
27. Write a C program to find a list of prime numbers.
Ans :-

28. Write a C program to find the fibonacci series in c programming: c program for Fibonacci series without and with recursion.

29. Write a C program to find the maximum or highest element in array.
Ans:-

30. Write a C program to find the minimum or smallest element in array.
Ans:-

31. Write a C program to find an item from an array by Linear search.

32. Write a C program to find an item from an array by binary search.

33. Write a C program to reverse an array.

34. Write a C program to insert an element into an array.

35. Write a C program to delete an element from an array.

36. Write a C program to add two matrices.

37. Write a C program to Subtract matrices

38. Write a C program to transpose a matrix.

39. Write a C program to multiply two matrices.

40. Write a C program to print a string.
Ans:-

41. Write a C program to print length of string.

42. Write a C program to compare two strings.

43. Write a C program to compare two strings.

44. Write a C program to copy a string.
Ans:-

45. Write a C program to concatenate two strings.

46. Write a C program to reverse a string.


