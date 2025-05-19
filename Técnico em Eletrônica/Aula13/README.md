# Aula 13

## Linguagem C
- Aló mundo.
```c
#include <stdio.h>
int main(){
	printf("Alô mundo!");
	return 0;
}
```
- Algoritmo que lê duas variáveis a e b e imprime a soma de a e b.
```c
#include <stdio.h>
int main(){
    //Definição de variáveis
    int a, b, c;
    
    printf("Digite dois números inteiros:\n");
    //Entrada
    scanf("%d %d", &a, &b);

    //Processamento
    c = a + b;
    printf("A soma de a + b = %d", c);
    return 0;
}
```
## Exercicios: 

1- Faça um Programa que peça um número e então mostre a mensagem O número informado foi [número].

2- Faça um Programa que converta metros para centímetros.

3- Faça um Programa que calcule a área de um quadrado, em seguida mostre o dobro desta área para o usuário.

4- Faça um Programa que pergunte quanto você ganha por hora e o número de horas trabalhadas no mês. Calcule e mostre o total do seu salário no referido mês.

5- Tendo como dados de entrada a altura de uma pessoa, construa um algoritmo que calcule seu peso ideal, usando a seguinte fórmula: (72.7*altura) - 58

6- Faça um Programa que peça o raio de um círculo, calcule e mostre sua área.

7 - Faça um Programa que pergunte quanto você ganha por hora e o número de horas trabalhadas no mês. Calcule e mostre o total do seu salário no referido mês.
