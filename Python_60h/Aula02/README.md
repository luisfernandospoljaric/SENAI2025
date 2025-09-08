# Aula02

# Algoritmos

Conjunto de passos lógicos e iterativos para resolução de um problema.

## Problema
Algo que possua uma solução porém não trivial.

## Exemplo de problema
- Escovar os dentes - Não é um problema (Possui solução trivial)
- Tocar a superfície do Sol - Não é um problema (Não possui solução)
- Trocar uma lâmpada - É um problema (Possui solução porém não trivial)

## Exemplo de algoritmo
### Problema: Trocar uma lâmpada (Portugol)
```portugol
0 - Início
1 - Pegar a escada e uma lâmpada nova
2 - Posicionar a escada
3 - Subir na escada
4 - Ajustar a lâmpada e fazer um teste, se acender ir para o passo 6, senão ir para o passo 5
5 - Trocar a lâmpada e ir para o passo 4.
6 - Descer da escada
7 - Guardar a escada e a lampada nova ou descartar a lâmpada queimada
8 - Fim
```

### Desafio: Pérolas e balança
Um joalheiro possui 9 pérolas e uma balançã do tipo prato de dois pratos. Todas as pérolas possuem o mesmo peso, exceto uma que é mais leve. Utilizando a balança, escreva um algoritmo que descura quantas pesagens no mínimo são necessárias para descobrir qual é a pérola mais leve?

## Conhecimentos:
- 1 Lógica e algoritmos
	- 1.1. Definição
	- 1.2. Estruturas
		- 1.2.1.Sequência
		- 1.2.2.Seleção
		- 1.2.3.Repetição

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
## Missão
- Assistir o vídeo: [Hello World Como Você Nunca Viu! | Entendendo C](https://www.youtube.com/watch?v=Gp2m8ZuXoPg) de Fábio Akita.

# EXERCICIOS

1 - Faça um Programa que peça um número e então mostre a mensagem O número informado foi [número].

2 - Faça um Programa que converta metros para centímetros.

3 - Faça um Programa que peça o raio de um círculo, calcule e mostre sua área.

4 - Faça um Programa que calcule a área de um quadrado, em seguida mostre o dobro desta área para o usuário.

5 - Faça um Programa que peça a temperatura em graus Celsius, transforme e mostre em graus Farenheit.


## Exercicios parte 2:

1 - Faça um Programa que pergunte quanto você ganha por hora e o número de horas trabalhadas no mês. Calcule e mostre o total do seu salário no referido mês.

2 - Tendo como dado de entrada a altura (h) de uma pessoa, construa um algoritmo que calcule seu peso ideal, utilizando as seguintes fórmulas: Para homens: (72.7h) - 58 Para mulheres: (62.1h) - 44.7

3 - João Papo-de-Pescador, homem de bem, comprou um microcomputador para controlar o rendimento diário de seu trabalho.

Toda vez que ele traz um peso de peixes maior que o estabelecido pelo regulamento de pesca do estado de São Paulo (50 quilos) deve pagar uma multa de R$ 4,00 por quilo excedente.

João precisa que você faça um programa que leia a variável peso (peso de peixes) e calcule o excesso.

Gravar na variável excesso a quantidade de quilos além do limite e na variável multa o valor da multa que João deverá pagar. Imprima os dados do programa com as mensagens adequadas.

4 - Faça um Programa que pergunte quanto você ganha por hora e o número de horas
trabalhadas no mês.

Calcule e mostre o total do seu salário no referido mês,
sabendo-se que são descontados 11% para o Imposto de Renda,
8% para o INSS e 5% para o sindicato, faça um programa que nos dê:
    salário bruto.
    quanto pagou ao INSS.
    quanto pagou ao sindicato.
    o salário líquido.
calcule os descontos e o salário líquido, conforme a tabela abaixo:

    + Salário Bruto : R$
    - IR (11%) : R$
    - INSS (8%) : R$
    - Sindicato ( 5%) : R$
    = Salário Liquido : R$

Obs.: Salário Bruto - Descontos = Salário Líquido.


# Formulário para envio:

https://docs.google.com/forms/d/e/1FAIpQLSfXGs6RJcuXzpQfne8b1zB885zh8Fkc-_JzRIID7EgZiXe7xQ/viewform?usp=sf_link

