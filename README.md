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

#include<stdio.h>

int main()

{

    int a, b, sum, subtraction, multiplication;
    float division;

    printf("Enter two numbers:");
    scanf("%d %d",&a,&b);

    sum = a + b;

    subtraction = a - b;

    multiplication = a * b;

    division = a / b;

    printf("Addition = %d,\nSubtraction = %d,\nMultiplication %d,\nDivision %.3f.\n",sum,subtraction,multiplication,division);

    return 0;
    
}


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

#include<stdio.h>
int main()
{

    int i,n;
    scanf("%d",&n);
    int fact =1;
    for(i=1;i<=n;i=i+1)
    {
        fact = fact*i;
    }
    printf("%d",fact);
    
}


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
Ans:-

#include<stdio.h>
int main()
{

    printf("Enter the two integer numbers : ");
    int i1 = 0, i2 = 0;
    scanf("%d %d",&i1, &i2);

    int GCD = 0;
    int max = (i1 > i2) ? i1 : i2;
    for(int i = 1; i<= max/2;i++)
    {
        if(i1%i==0 && i2%i==0)
            GCD = i;
    }
    int LCM = max;
    for(; LCM <= i1*i2 ; LCM++)
    {
        if(LCM%i1 == 0 && LCM%i2 == 0)
        break;
    }
    printf("GCD=%d , LCD=%d",GCD, LCM);

    return 0;
    
}

16. Write a C program to find the number of integers divisible by 5 between the given range num1 and num2, where num1 < num2. Also find the sum of all these integer numbers, which are divisible by 5 and display the total.
Ans :-

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
Ans :-

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
           printf("");
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
Ans :-
কোনো একটি সংখ্যা যেমন 121 কে উল্টা করে লিখলেও 121 হয়, এই ধরণের সংখ্যাকে প্যালিন্ডোম (Palindrome) সংখ্যা বলে।
আবার, কোনো শব্দকে উল্টা ভাবে লিখলে যদি একই রকম হয় তবে সেটি একটা প্যালিন্ডোম।

#include<stdio.h>
int main()
{

    int num, n, reminder, rev = 0;
    
    printf("Enter a number : ");
    scanf("%d",&num);
    
    n = num;
    while (num > 0)
    {
        reminder = num % 10;
        rev = rev * 10 + reminder;
        num = num / 10;
    }
    if (n == rev)
    {
        printf("This is a palindrome number.\n");
    }
    else
    {
        printf("This is not a palindrome number.\n");
    }
    return 0;
    
}


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

#include <stdio.h>
int main()
{
    
    int num1, num2, flag_var, i, j;
   
    printf("Enter two range(input integer numbers only):");
    scanf("%d %d", &num1, &num2);
    printf("Prime numbers from %d and %d are:\n", num1, num2);
   
    for(i=num1+1; i<num2; ++i)
    {
      flag_var = 0; // use of this statement, it's just like a trap.
      for(j=2; j<=i/2; ++j)
      {
         if(i%j == 0)
         {
            flag_var = 1;
            break;
         }
      }
      if(flag_var == 0)
      {
         printf("%d\n",i);
      }
    }
    return 0;
  
}

28. Write a C program to find the fibonacci series in c programming: c program for Fibonacci series without and with recursion.                                      Ans :-  

উল্লেখ্য যে, পর পর দুটি সংখ্যা যোগ করলে ফিবন্যাসি সিরিজের তৃতীয় সংখ্যাটি পাওয়া যায়।

#include<stdio.h>
main()
{

    int i, Max;
    scanf("%d",&Max); // Taking the number for consecutive fibonacci. Just like, 10, 20 or ..........
    int fibo [Max];
    fibo [0] = 1;
    fibo [1] = 1;
    printf("\nFirst %d consecutive fibonacci numbers are :\n",Max);
    for(i=2;i<=Max;i++)
    {
        fibo [i] = fibo [i-2] + fibo [i-1];
    }
    for(i=0;i<Max;i++)
    {
        printf("%5d",fibo [i]);
    }
    return 0;
    
}



29. Write a C program to find the maximum or highest element in array.
Ans:-

#include<stdio.h>
int main()
{

    int size;
    printf("Enter the number of elements in array:\n");
    scanf("%d", &size);

    int array[size], maximum, a, location = 1;

    printf("Enter %d integers:\n", size);

    for (a = 0 ; a < size ; a++)
    {
        scanf("%d", &array[a]);

        maximum = array[0];
    }
    for (a = 1 ; a < size ; a++)
    {
        if (array[a] > maximum)
        {
                maximum  = array[a];
                location = a+1;
        }
    }

    printf("Maximum element is present at location %d and it's value is %d.\n", location, maximum);
    
}


30. Write a C program to find the minimum or smallest element in array.
Ans:-

#include<stdio.h>
int main()
{

    int size;

    printf("Enter the number of elements in array\n");
    scanf("%d", &size);

    int array[size], minimum, i, location = 1;

    printf("Enter %d integers\n", size);

    for (i = 0; i < size; i++)
        scanf("%d", &array[i]);

    minimum = array[0];

    for (i = 1; i < size; i++)
    {
        if (array[i] < minimum)
        {
                minimum  = array[i];
                location = i+1;
        }
    }

    printf("Minimum element is present at location %d and it's value is %d.\n", location, minimum);
    
}

31. Write a C program to find an item from an array by Linear search.
Ans:-

#include<stdio.h>
int main()
{

    int arr[100], n, search, i;
    printf("How many elements in array : ");
    scanf("%d",&n);
    for(i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
    }
    printf("Enter your search number : ");
    scanf("%d", &search);
    for(i=0;i<n;i++)
    {
        if(arr[i] == search)
        {
            printf("%d find successfully find the location is %d\n", search, i+1);
            break;
        }
    }
    if(i == n)
    {
        printf("Unsuccessfully\n");
    }
    return 0;
    
}


32. Write a C program to find an item from an array by binary search.
Ans:-

33. Write a C program to reverse an array.
Ans:-

#include<stdio.h>
int main()
{

    int i, j, num;
    printf("How many number you will take = ")
    scanf("%d",&num);
    printf("Give me the number = \n")
    int a[num], b[num];
    for(i=0;i<num;i++)
    {
        scanf("%d",&a[i]);
    }
    for(i = num - 1, j = 0; i >= 0;i--,j++)
    {
        b[j] = a[i];
    }
    printf("Reverse the number : \n");
    for (i = 0; i < num; i++)
        printf("%d\n", b[i]);
        
    return 0;
        
}


34. Write a C program to insert an element into an array.
Ans:-

35. Write a C program to delete an element from an array.
Ans:-

36. Write a C program to add two matrices.
Ans:-

#include<stdio.h>
int main()
{

    int i, j, m, n;
    printf("How many row and column you will take for two Matrix :");
    scanf("%d %d",&m,&n);
    int a[m][n], b[m][n], sum[m][n];
    printf("Enter First Matrix:\n");
    for(i = 0;i<m;i++)
    {
        for(j = 0;j<n;j++)
        {
            scanf("%d",&a[i][j]);
        }
    }
    printf("Enter Second Matrix:\n");
    for(i = 0;i<m;i++)
    {
        for(j = 0;j<n;j++)
        {
            scanf("%d",&b[i][j]);
        }
    }
    printf("Sum of two Matrix:\n");
    for(i = 0;i<m;i++)
    {
        for(j = 0;j<n;j++)
        {
            sum[i][j] = a[i][j] + b[i][j];
            printf("%d\t",sum[i][j]);
        }
        printf("\n");
    }
    printf("\n");

    return 0;

}


37. Write a C program to Subtract matrices.
Ans:-

#include<stdio.h>
int main()
{

    int i, j, m, n;
    printf("How many row and column you will take for two Matrix :");
    scanf("%d %d",&m,&n);
    int a[m][n], b[m][n], subtract[m][n];
    printf("Enter First Matrix:\n");
    for(i = 0;i<m;i++)
    {
        for(j = 0;j<n;j++)
        {
            scanf("%d",&a[i][j]);
        }
    }
    printf("Enter Second Matrix:\n");
    for(i = 0;i<m;i++)
    {
        for(j = 0;j<n;j++)
        {
            scanf("%d",&b[i][j]);
        }
    }
    printf("Subtract of two Matrix:\n");
    for(i = 0;i<m;i++)
    {
        for(j = 0;j<n;j++)
        {
            subtract[i][j] = a[i][j] - b[i][j];
            printf("%d\t",subtract[i][j]);
        }
        printf("\n");
    }
    printf("\n");

    return 0;

}


38. Write a C program to transpose a matrix.
Ans:-

#include<stdio.h>
int main()
{

    int i, j, m, n;
    printf("");
    scanf("%d %d",&m,&n);
    int Matrix[m][n], Transpose[m][n];
    printf("Input a Matrix:");
    for(i = 0;i<m;i++)
    {
        for(j = 0;j<n;j++)
        {
            scanf("%d",&Matrix[i][j]);
        }
    }
    for(i = 0;i<m;i++)
    {
        for(j = 0;j<n;j++)
        {
            Transpose[j][i] = Matrix[i][j];
        }
    }
    printf("The Transpose of Matrix:");
    for(i = 0;i<n;i++)
    {
        for(j = 0;j<m;j++)
        {
            printf("%d ",Transpose[i][j]);
        }
        printf("\n");
    }

    return 0;

}

39. Write a C program to multiply two matrices.
Ans:-

#include<stdio.h>
int main()
{

    int first [10][10],second[10][10],result[10][10],r1,r2,c1,c2,i,j,k,sum=0;

    printf("Enter rows and column for 1st matrix: ");
    scanf("%d  %d", &r1, &c1);
    printf("Enter rows and column for 2nd matrix: ");
    scanf("%d  %d", &r2, &c2);

    while(c1!=r2)
    {
        printf ("Error!! Column of 1st matrix not equal to row of 2nd");

        printf("Enter rows and column for 1st matrix: ");
        scanf("%d  %d", &r1, &c1);
        printf("Enter rows and column for 2nd matrix: ");
        scanf("%d  %d", &r2, &c2);
    }

    printf("\nEnter elements for 1st Matrix\n");
    for(i=0;i<r1;i++)
    {
        for(j=0;j<c1;j++)
        {
            printf("first [%d][%d]= ",i,j);
            scanf("%d", &first[i][j]);
        }
    }
    printf("\nEnter elements for 2nd Matrix\n");
    for(i=0;i<r2;i++)
    {
        for(j=0;j<c2;j++)
        {
            printf("second [%d][%d]= ",i,j);
            scanf("%d", &second[i][j]);
        }
    }
        for(i=0;i<r1;i++)
    {
         for(j=0;j<c2;j++)
    {
         for(k=0;k<c1;k++)
         {
           sum = sum + first[i][k]*second[k][j];
         }


       result[i][j] = sum;
        sum = 0;
      }
    }


    printf("\n\nFirst Matrix\n");
    for(i=0;i<r1;i++)
    {
        printf(" ");
        for(j=0;j<c1;j++)
        {
            printf("%d ", first[i][j]);
        }
        printf("\n");
    }

       printf("\n\nSecond Matrix\n");
    for(i=0;i<r2;i++)
    {
        printf("\t");
        for(j=0;j<c2;j++){
            printf("%d ", second[i][j]);}
        printf("\n");
    }

     printf("\n\nResult Matrix\n");
    for(i=0;i<r1;i++)
    {
        printf("\t");
        for(j=0;j<c2;j++){
            printf("%d ", result[i][j]);}
        printf("\n");
    }

    return 0;
}

40. Write a C program to print a string.
Ans:-

#include<stdio.h>
int main()
{

    int i;
    char university_name[20]="East West University";
    for(i=0;i<20;i++)
    {
        printf("%c",university_name[i]);
    }
    
    return 0;
}

41. Write a C program to print length of string.
Ans:-

#include<stdio.h>
#include<string.h>
int main()
{

    char a[100];
    int length;

    printf("Enter a string,to calculate it's length\n");
    gets(a);

    length = strlen(a);

    printf("Length of entered string is %d\n",length);

    return 0;
    
}

42. Write a C program to compare two strings.
Ans:-

#include<stdio.h>
#include<string.h>
int main()
{

    char a[100], b[100];
    printf("Enter the first string\n");
    gets(a);
    printf("Enter the second string\n");
    gets(b);
    if(strcmp(a,b) == 0)
    {
        printf("Entered strings are equal.\n");
    }
    else
    {
        printf("Entered strings are not equal.\n");
    }

    return 0;
    
}

43. Write a C program to copy two strings.
Ans:-

#include<stdio.h>
#include<string.h>
int main()
{

    char source[1000], destination[1000];
    printf("Input a string\n");
    gets(source);
    strcpy(destination,source);
    printf("Source string:      \"%s\"\n",source);
    printf("Destination string: \"%s\"\n",destination);

    return 0;
    
}

44. Write a C program to concatenate two strings.
Ans:-

#include<stdio.h>
#include<strings.h>
int main()
{

    char a[1000], b[1000];
    printf("Enter the first strings\n");
    gets(a);
    printf("Enter the second strings\n");
    gets(b);
    strcat(a,b);
    printf("Strings obtained on concatenation is %s\n",a);

    return 0;
    
}


45. Write a C program to reverse a string.
Ans:-

#include<stdio.h>
int main()
{

    int i, j, num;
    printf("How many number you will take for sentence = ");
    scanf("%d",&num);
    printf("Give me the sentence = \n");
    char a[num], b[num];
    for(i=0;i<num;i++)
        {
            scanf("%c",&a[i]);
        }
    for(i = num - 1, j = 0; i >= 0;i--,j++)
        {
            b[j] = a[i];
        }
    printf("Reverse the sentence : \n");
    for (i = 0; i < num; i++)
    {
        printf("%c", b[i]);
    }
    
    return 0;
        
}

46. Write a C program to delete vowels from a string.

47. Write a C program to check subsequence.

48. Write a C program to remove spaces, blanks from a string.

49. Write a C program to change the case of a string.

50. Write a C program to swap two strings.

51. Write C program to find frequency of characters in a string.

52. Write C program to find the anagrams. Two words are said to be anagrams of each other
if the letters from one word can be rearranged to form the other word.

53. Write a program to copy one string to another using pointer.

54. Write a program to concatenate two strings using pointers.

55. Write a program to find the sum of all the elements of an array using pointers.

56. Write a program to search an element in array using pointers.

57. Write a C program to read a file.

58. Write a C program to copy a file.

59. Write a C program to merge two files.

60. Write a C program to a delete a file.

61. Write a C program to generate random numbers.

62. Write a C program to add two complex numbers.

63. Write a C program to accept two integers for a coordinate point and determine its
quadrant.

64. Students need to do a project based on C language.

