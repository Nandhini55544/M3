# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <math.h>
void emi(float p,float ar,float y)
{
    float mr=ar/(12*100);
    float m=y*12;
    float r=(p*mr*pow(1+mr,m)/(pow(1+mr,m)-1));
    printf("Monthly EMI is= %.3f\n",r);
}
int main()
{
    float p,r,t;
    scanf("%f %f %f",&p,&r,&t);
    emi(p,r,t);
    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/0057a5d5-16aa-455c-8345-b4d7b9243d52)

## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 8.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() {
    int a = 0, b = 1, nextTerm;
    int count = 1, n = 8;  
    do {
        printf("%d ", a);
        nextTerm = a + b;
        a = b;
        b = nextTerm;
        count++;
    } while (count <= n);
    printf("\n");
    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/8c5deb92-e434-462d-bd53-884fa74cce37)


## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main()
{
    int n;
    scanf("%d",&n);
    int a[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
}
        printf("%d ",a[n-1]);

    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/1963699e-3cd3-4b1d-a164-01b0f914ef05)

## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
Write a C Program to Print the Number of  Odd Numbers in an Array

## ALGORITHM
1. Start  
2. Declare an integer array `arr` and an integer variable `n` to store the size of the array  
3. Read the value of `n` (the size of the array) from the user  
4. Read `n` elements into the array `arr`  
5. Initialize a counter variable `count` to 0  
6. Use a loop to iterate through each element of the array  
   - For each element, check if it is odd (i.e., `arr[i] % 2 != 0`)  
   - If the element is odd, increment the `count`  
7. After the loop, print the value of `count` (the number of odd numbers in the array)  
8. End

## PROGRAM
```
#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    int a[n];
    for(i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    printf("Odd numbers in the array are - ");
    for(i=0; i<n;i++)
    {
        if (a[i]%2!=0)
        {
            printf("%d ",a[i]);
        }
    }
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/8d289c25-bbbd-4a56-bc54-d47e814afadd)

## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.

# EX -15 - Replace All Even Elements With '0' and odd elements with '1'

## Aim:
write a C program to replace all even elements by 0 and odd by 1 in one dimensional array

## Algorithm:
1. Start  
2. Declare an integer array `arr` and an integer variable `n` to store the size of the array  
3. Read the value of `n` (size of the array) from the user  
4. Read `n` elements into the array `arr`  
5. Use a loop to iterate through each element of the array  
   - For each element, check if it is even (i.e., `arr[i] % 2 == 0`)  
     - If it is even, replace the element with `0`  
   - If the element is odd (i.e., `arr[i] % 2 != 0`), replace the element with `1`  
6. After processing all elements, print the modified array  
7. End

## Program:
```
#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    int a[n];
    for(i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    for(i=0;i<n;i++)
    {
        if(a[i]%2==0)
        {
            a[i]=0;
        }
    }
    for(i=0;i<n;i++)
    {
        if(a[i]%2!=0)
        {
            a[i]=1;
        }
    }
    for(i=0;i<n;i++)
    {
        printf("%d ",a[i]);
    }
}
```
## Output:
![image](https://github.com/user-attachments/assets/d5d3eed8-880c-495c-a867-b7051c12b088)
 
## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



