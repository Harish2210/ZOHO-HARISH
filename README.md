# ZOHO-HARISH
#include <stdio.h>
#include stdlib.h>
    int num,i,j;
    scanf("%d",&num);
    if(num<0)
    {
        printf("Invalid nuumber");
        return;
    }
    while(1)
    {
        num++;
        if(isReverse(num)==num)
        {
            printf("%d",num);
            return;
        }
    }
}
int isReverse(int number)
{
    int builtNumber=0,r;
    while(number>0)
    {
        r=number%10;
        builtNumber=(builtNumber*10)+r;
        number=number/10;
    }
    return builtNumber;
}

