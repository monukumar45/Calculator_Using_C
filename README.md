# Calculator_Using_C
#include<stdio.h>
int main()  
{  
    char opt;  
    int num1, num2;   
    float res;  
    printf (" Choose an operator(+, -, *, /) to perform the operation in C Calculator \n ");  
    scanf ("%c", &opt); 
    if (opt == '/' )  
    {  
        printf (" You have selected: Division");  
    }  
    else if (opt == '*')  
    {  
        printf (" You have selected: Multiplication");  
     }  
       
    else if (opt == '-')  
    {  
        printf (" You have selected: Subtraction");  
     }  
        else if (opt == '+')  
    {  
        printf (" You have selected: Addition");  
     }     
    printf (" \n Enter the first number: ");  
    scanf(" %d", &num1);
    printf (" Enter the second number: ");  
    scanf (" %d", &num2);
      
    switch(opt)  
    {  
        case '+':  
            res = num1 + num2;
            printf (" Addition of %d and %d is: %.2f", num1, num2, res);  
            break;  
          
        case '-':  
            res = num1 - num2;
            printf (" Subtraction of %d and %d is: %.2f", num1, num2, res);  
            break;  
              
        case '*':  
            res = num1 * num2;
            printf (" Multiplication of %d and %d is: %.2f", num1, num2, res); 
            break;            
          
        case '/':  
            if (num2 == 0) 
            {  
                printf (" \n Divisor cannot be zero. Please enter another value ");  
                scanf ("%d", &num2);        
                }  
            res = num1 / num2; 
            printf (" Division of %d and %d is: %.2f", num1, num2, res);  
            break;  
        default:
            printf (" Something is wrong!! Please check the options ");        
    }  
    return 0;  
}
