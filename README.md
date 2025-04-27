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

    #include<stdio.h>
    int main()
    {
	int i,m,n;
	printf("ENTER TWO NUMBERS:\n");
	scanf("%d%d",&m,&n);
	for(i=m;i<=n;i++)
	{
		if(i%2==0)
		{
			printf("%d ",i);
		}
	}
    }


## OUTPUT:

![Screenshot 2025-04-27 090425](https://github.com/user-attachments/assets/19729b9c-5f93-4dde-98c1-459c3a1228eb)

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
    #include<stdio.h>
    int main()
    {
	int row,i,j;
	printf("ENTER NO. OF ROWS:\n");
	scanf("%d",&row);
	for(i=1;i<=row;i++)
	{
		for(j=1;j<=i;j++)
		{
			printf("*");
		}
		printf("\n");
	}
    }

## OUTPUT:

![Screenshot 2025-04-27 090844](https://github.com/user-attachments/assets/40bf1901-4b2c-4df5-875b-c37fa4b74804)

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

    #include<stdio.h>
    void addition(int a,int b)
    {
    int sum;
    sum=a+b;
    printf("ADDITION: %d\n",sum);	
    }
    void sub(int a,int b)
    {
	int diff;
	diff=a-b;
	printf("SUBTRACTION: %d\n",diff);
    }
    int main()
    {
	int num1,num2;
	printf("ENTER TWO NUMBERS:\n");
	scanf("%d%d",&num1,&num2);
	addition(num1,num2);
	sub(num1,num2);
    }

## OUTPUT:

![Screenshot 2025-04-27 091435](https://github.com/user-attachments/assets/62be34e6-f93d-4015-acef-7b6a3a47fea2)

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
    #include<stdio.h>
    int main()
    {
	int i,k,sum=0;
	printf("ENTER ANY DIGIT:\n");
	scanf("%d",&i);
	for(;i!=0;i/=10)
	{
		k=i%10;
		if(k%2!=0)
		{
			sum+=k;
		}
	}
	printf("SUM OF ODD DIGITS = %d",sum);
	
    }

## OUTPUT:

![Screenshot 2025-04-27 092126](https://github.com/user-attachments/assets/3d7ab419-52eb-4b26-bbb8-30095b07f98e)

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
    #include<stdio.h>
    void fact();
    int main()
    {
    fact();
    return 0;
    }
    void fact() 
    {
    int i,n;
    long long int factorial = 1;
    printf("ENTER A NUMBER:\n");
    scanf("%d",&n);
    for(i=1;i<=n;i++) 
	{
        factorial*=i;
    }
    printf("Factorial of %d is %d\n",n,factorial);
    }

## OUTPUT:

![Screenshot 2025-04-27 092456](https://github.com/user-attachments/assets/e5dd8102-5a6e-496c-b817-110247868252)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
