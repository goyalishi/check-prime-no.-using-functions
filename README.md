#include <stdio.h>
//WAP to find whether a number is prime or not using functions
int prime(int);
int main()
{
    int num,res;
    printf("enter the number to check:\n");
    scanf("%d",&num);
    res=prime(num);
    if(res>1)
    printf("no. is not prime.");
    else
    printf("no. is prime.");
   
    return 0;
}

// function definition
int prime(int n)
{
    int i,fact=0;
    for(i=2;i<=n;i++)
    {
        if(n%i==0)
        fact++;
        
    }
    return(fact);
}

