----
# **PROGRAMMING FOR PROBLEM SOLVING ESC-18105**
----
----
---
## **NAME** - ***MD AQUIB HASSAN***
## **ROLL NO.** - *1914071*
## **BRANCH** - *CIVIL ENGINEERING*
'''
---
----

#         PROGRAMS

----

## 1. ADD TWO NUMBERS
```C
#include<stdio.h>
void main()
{
        int a,b;
        printf("Enter the two number to be added\n");
        scanf("%d%d",&a,&b);
        printf("Sum  : %d + %d = %d \n",a,b,a+b);

}
```

----
## 2. AVG.OF N NUMBER
```C
#include<stdio.h>
void main()     
{
        int n;
        float sum=0;
        printf("Enter number of elements \n");

        scanf("%d",&n);
        int a[n];
        printf(" now enter %d elements\n",n);
        for(int i=1;i<=n;i++)
        {       
                scanf("%d",&a[i]);
                sum+=a[i];
        }
        float avg;
        avg = sum/n;
        printf("Average of %d elements is %0.2f \n",n,avg);
}       
```

----
## 3. WEEKDAYS BY USING SWITCH STATEMENT
```C
#include<stdio.h>
void main()
{
        int a;
        printf("Enter any integer between 1 to 7\n");
        scanf("%d",&a);
        switch(a)
        {
                case 1:
                        printf("MONDAY\n");
                        break;
                case 2:
                        printf("TUESDAY\n");
                        break;
                case 3:
                        printf("WEDNESDAY\n");
                        break;
                case 4:
                        printf("THRUSDAY\n");
                        break;
                case 5:
                        printf("FRIDAY\n");
                        break;
                case 6:
                        printf("SATURDAY\n");
                        break;
                case 7:
                        printf("SUNDAY\n");
                        break;
                default :
                        printf("Enter number between 1 to 7\n");
                        break;
        }
}  
```

----
## 4. NUMBER IS EVEN OR ODD
```C
#include<stdio.h>
void main()
{
        int a;
        printf("enter the number\n");
        scanf("%d",&a);
        if(a%2==0)
                printf("EVEN\n");
        else
                printf("ODD\n");
}
```

----
## 5. TABLE OF ANY NUMBER
```C
#include<stdio.h>
int main()
{
        int n,i;
        printf("enter the number \n");
        scanf("%d",&n);
        printf("\t\t\tTABLE OF %d\n",n);
        printf("\t\t\t==========\n");
        for(i=1;i<11;i++)
        {
                printf("%d * %d = %d\n",n,i,n*i);
        }               
        return 0;       
}
```

----
## 6. ARMSTRONG NUMBER
```C
#include<stdio.h>
int main()
{
        int sum=0,digit;
        int n, temp;
        printf("enter any positive integer number");
        scanf("%d",&n);
        temp=n;
        while(temp>0)
        {
                digit=temp%10;
                temp/=10;
                sum=sum+digit*digit*digit;
        }
        if(n==sum)
                printf("\n %d is a armstrong number\n",n);
        else
                printf("\n %d is not a armstrong number\n",n);
}
```

----
## 7. CALCULATOR
```C
#include<stdio.h>


void main()
{
        
        puts(" _______________ ");
        puts("|_______________|");
        puts("| 1 | 2 | 3 |   |");
        puts("|___|___|___|   |");
        puts("| 4 | 5 | 6 | + |");
        puts("|___|___|___|___|");
        puts("| 7 | 8 | 9 | - |");
        puts("|___|___|___|___|");
        puts("|     0     | * |");
        puts("|___________|___|");

}
```
----
## 8. BUBBLE SORT
```C
#include<stdio.h>
int main()
{
        int i,n,k,temp;
        printf("\n enter the array size\n");
        scanf("%d",&n);
        int a[n];
        printf("enter %d elements of array\n",n);
        for(i=0;i<n;i++)
                scanf("%d",&a[i]);
        for(k=0;k<n-1;k++)
        {
                for(i=0;i<n-k-1;i++)
                {
                        if(a[i]>a[i+1])
                        {
                                temp=a[i];
                              
