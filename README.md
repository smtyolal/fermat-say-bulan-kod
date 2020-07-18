# fermat-say-bulan-kod
#include <stdio.h>
#include <math.h>

/*
int exponent(int a, int b) {
        int result=a;
        for(int i=0;i<b-1;i++) {
                result *= a;
        }
        return result;
}
*/


int main () {




//Fermat sayı 2^2^n+1

long long int value;
printf("Fermat sayi kontrolu icin deger gir: ");
scanf("%lli",&value);

long long int solution=0,exp1=1;



   for (int i = 0; i <= value; i++)
   {
          
       solution = pow(2,pow(2,i)) + 1;

       if (value == solution)
       {
              break;
       }
       
   }


  if (value == solution)
  {
         printf("True");
  }

  if (value != solution)
  {
         printf("False");
  }
  
          




       return 0;
}
