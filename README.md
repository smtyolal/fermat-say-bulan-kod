# fermat-say-bulan-kod

#include <stdio.h>
#include <math.h>

int main () {

//Fermat sayı 2^2^n+1

int value;
printf("Fermat sayi kontrolu icin deger gir: ");
scanf("%d",&value);

int solution=0,exp1=1;

const int exp2=2;

   for (int i = 0; i < value; i++)
   {
          
       solution = pow(2,pow(2,i)) + 1;

       if (value == solution)
       {
              break;
       }
       
   }
           
printf("%d",solution);



       return 0;
}
