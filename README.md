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
# include <math.h>
void calculate_emi(float p,float r,float t)
{
    
    r=r/(12*100);
    t=t*12;
   float  emi=(p*r*pow(1+r,t))/(pow(1+r,t)-1);
    printf("Monthly EMI is= %.3f",emi);
}



int main()
{
     
    float p,r,t;
    scanf("%f%f%f",&p,&r,&t);
    calculate_emi(p,r,t);
    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/c6998e0c-1a74-4dd7-a27e-50d02736600b)


## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

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
# include <stdio.h>
int main()
{
    int num;
    scanf("%d",&num);
    int a=0;
    int b=1;
    printf("%d %d ",a,b);
    for(int i=3;i<=num;i++)
    {
        int c=a+b;
        printf("%d ",c);
        a=b;
        b=c;
    }
    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/fe8b46e9-7b74-4cbe-8a2b-3a460effa95a)


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

int main() {
    int n;
    scanf("%d", &n);
    int arr[n];
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    
    printf("%d\n", arr[n - 1]);

    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/5fc0040c-bef3-4db0-abfe-350c0b1070bd)


## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM

```
#include<stdio.h>
int main(){
    int n,count=0;
    scanf("%d",&n);
    int a[n];
    for(int i=0;i<n;i++){
        scanf("%d",&a[i]);
    }
    for(int i=0;i<n;i++){
        if(a[i]>0){
            count++;
        }
    }
    printf("count  of positive numbers  in array: %d",count);
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/ad4d3763-f126-49c8-ab6b-f811e0e2e41c)


## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:

```
#include<stdio.h>
int main(){
    int n,i;
    scanf("%d",&n);
    int arr[n];
    for(int i=0;i<n;i++){
        scanf("%d",&arr[i]);
    }
    for(i=0;i<n;i++){
        if(arr[i]%2==0){
            printf("E ");
        }
        else{
            printf("%d ",arr[i]);
        }
    }
}
```

## Output:
 
![image](https://github.com/user-attachments/assets/a6b60e04-633e-480b-a3b1-ba1f885dc240)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



