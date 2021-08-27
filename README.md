#include <stdio.h>
#include <stdlib.h>

void desconto(float p)
{
float novovalor;
novovalor=p/1.10;

 printf("============================================================\n\n");
printf(" \n\n\t\t PRECO ATUALIZADO DENTRO DA FUNCAO\n");
printf("============================================================\n\n");

 printf(" \n R$%.2f\n",novovalor);

}

float aumento(float p)
{
float novovalor;
novovalor=p*1.10;

 printf("============================================================\n\n");
printf(" \n\n\t\t PRECO ATUALIZADO DENTRO DA FUNCAO\n");
printf("============================================================\n\n");
printf(" \n R$%.2f\n",novovalor);

 return novovalor;

}

int main()
{
float pr1,valoraumento,valordesconto;
char nome1[10];

printf("============================================================\n\n");
printf(" \n\n\t\t CADASTRO DE PRODUTOS\n");
printf("============================================================\n\n");

 printf("\n\nInforme o nome do primeiro produto\n");
gets (nome1);

 printf("\nInforme o preco do primeiro produto\n");
scanf("%f",&pr1);

 if(pr1>50)
{

 desconto(pr1);

 printf("============================================================\n\n");
printf(" \n\n\t\t PRECO ORIGINAL (PR1)-sem alteracao\n");
printf("============================================================\n\n");
printf(" \n R$%.2f\n",pr1);

}
if(pr1<50)
{
pr1=aumento(pr1);

 printf("============================================================\n\n");
printf(" \n\n\t\t PRECO ORIGINAL (PR1) - com alteracao\n");
printf("============================================================\n\n");
printf(" \n R$%.2f\n",pr1);
}

return 0;
}
