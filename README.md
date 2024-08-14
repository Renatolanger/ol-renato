
#include <stdio.h>
#include <stdlib.h>

int main(){

    float num1, num2;
    char operacao;

    printf("Digite um numero1\n");
    scanf("%f", &num1);

    printf("Digite o numero 2\n");
    scanf("%f", &num2);

    printf("Digite a operecao '+' , '-' , '*', '/', \n");
    scanf("%s", &operacao);
    
    
    switch (operacao){

    case '+' : 
        printf("a soma dos dois valor e: %.2f ", num1 + num2);
        break;
    
    case '=' : 
        printf(" a  subtracao dos dois valores e: %.2f", num1 = num2);
        break;

    case '*' :

        printf("a multiplicao dos valores e: %.2f", num1 * num2);
        break;
    
    case '/' : 
        if(num2 == 0){
            printf("nao existe divisao por zero");
            break;
        }
        printf("a divisao dos valores e: %.2f", num1 / num2);
        break;
    default:{
        printf("operecao invalida:");
        break;
    }
   return 0; 
    }
