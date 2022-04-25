#include <stdio.h>
#include "q02.h"
#include "q03.h"
#include "q04.h"
#include "q05.h"
#include "q07.h"

int main(void) {
  int select;
  
  printf("\nHello World! How are you doing today? There're some programs for you: \n");
  printf("\n1.Número em ordem inversa\n2.Média 4 notas\n3.Consoantes entre 10 caracteres\n4.Distinguir números pares e impares\n5.Soma e multiplicação de números\n");
  printf("\nEnter a number from 1 to 5: ");
  scanf("%i", &select);
  
    while (select>5 || select<1){
    printf("\nError. Number is not correct\nEnter a number from 1 to 5: ");
    scanf("%i", &select);
    }

  switch(select){
    case 1:
    printf("\nQuestão 2: Números reais em ordem inversa\n\n");
    q02();
    break;

    case 2:
    printf("\nQuestão 3: Média 4 notas\n\n");
    q03();
    break;

    case 3:
    printf("\nQuestão 4: Quantas consoantes há entre 10 letras\n\n");
    q04();
    break;

    case 4:
    printf("\nQuestão 5: Distinguir números pares e impares\n\n");
    q05();
    break;

    case 5:
    printf("\nQuestão 7: Soma e multiplicação de números\n\n");
    q07();
    break;
    
  }
  
  return 0;
}
