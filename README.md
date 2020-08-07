# arkadas-sayilari-bulan-kod-parcasi

#include <stdio.h>
#include <math.h>


int are_friends(int number1, int number2){      
       int collect1=0, collect2=0;

       for(register unsigned int i = 1; i < number1; i++){

              if(number1 % i == 0)
                     collect1 += i;
              if (collect1 == number2)
              {
                     break;
              }
              
       }

       for (register unsigned int j = 1; j < number2; j++)
       {
              
              if(number2 % j == 0)
                     collect2 += j;
              if (collect2 == number1)
              {
                     break;
              }
       }
       
       if (collect1 == number2 && collect2 == number1)
       {
              printf("Arkadas sayidir.");
       }
       else
       {
              printf("Arkadas sayi degildir.");
       }
       
