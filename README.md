exercici8

# Lista-P1



#include <stdio.h>

int main(void) {

//declaração de variaveis
float e_resistor_1;
float e_resistor_2;
float e_resistor_3;
float e_resistor_4;
float resistencia_total;
float req_1;
float req_2;


//entrada com valor das resistencias
printf("Resistor 1[r]:\n");
scanf("%f",&e_resistor_1);

printf("Resistor 2[r]:\n");
scanf("%f",&e_resistor_2);


printf("Resistor 3[r]:\n");
scanf("%f",&e_resistor_3);


printf("Resistor 4[r]:\n");
scanf("%f",&e_resistor_4);

//conversão das resistencias em paralelo

printf("inicio: Calculo\n");
req_1= (e_resistor_1 * e_resistor_2) / (e_resistor_1 + e_resistor_2);


printf("inicio: Calculo\n");
req_2= ( req_1 * e_resistor_3) / (req_1 + e_resistor_3);


printf("inicio: Calculo\n");
resistencia_total = ( req_2 * e_resistor_3) / (req_2 + e_resistor_3);


//saida da resistencia total
printf("o valor total da resistencia:%f", resistencia_total);


  
  return 0;
}
