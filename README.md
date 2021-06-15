# Armstrong-Number in c.
#include <stdio.h>

int main()
{   int n,count=0,abtakkaprod,abtakkasum,i,a,b,digit;
   
    printf("Enter the number\n");
    scanf("%d",&n);
     b=a=n;
    while(n>0)
   { 
       n=n/10;
       count++;
   }
   abtakkasum=0;
   while(a>0)
   {    
       digit=a%10;
       a=a/10;
       abtakkaprod=1;
       for(i=1; i<=count; i++)
       abtakkaprod=abtakkaprod*digit;
       abtakkasum=abtakkasum+abtakkaprod;
   }
   if (abtakkasum==b)
   {
       printf(" %d is armstrong:",b);
   }
   else
   {
       printf("the number %d is is not armstrong:",b);
       return 0;
   }
}
