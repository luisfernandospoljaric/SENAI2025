# Aula03

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



# EXERCICIOS
##	EXERCICIO 1
 Faça um Programa que leia três números e mostre-os em ordem decrescente.

##	EXERCICIO 2 
Faça um Programa que peça os 3 lados de um triângulo. O programa deverá informar se os valores podem ser um triângulo. Indique, caso os lados formem um triângulo, se o mesmo é: equilátero, isósceles ou escaleno.

Dicas: Três lados formam um triângulo quando a soma de quaisquer dois lados for maior que o terceiro; Triângulo Equilátero: três lados iguais; Triângulo Isósceles: quaisquer dois lados iguais; Triângulo Escaleno: três lados diferentes;

##	EXERCICIO 3
 Faça um Programa que peça um número inteiro e determine se ele é par ou impar. Dica: utilize o operador módulo (resto da divisão).

##	EXERCICIO 4 
Faça um Programa que leia 2 números e em seguida pergunte ao usuário qual operação ele deseja realizar.

O resultado da operação deve ser acompanhado de uma frase que diga se o número é: par ou ímpar; positivo ou negativo; inteiro ou decimal

## 	EXERCICIO 5
 Faça um programa que faça 5 perguntas para uma pessoa sobre um crime. As perguntas são: "Telefonou para a vítima?" "Esteve no local do crime?" "Mora perto da vítima?" "Devia para a vítima?" "Já trabalhou com a vítima?"

O programa deve no final emitir uma classificação sobre a participação da pessoa no crime.

Se a pessoa responder positivamente a 2 questões ela deve ser classificada como "Suspeita", entre 3 e 4 como "Cúmplice" e 5 como "Assassino". Caso contrário, ele será classificado como "Inocente". 

## 	EXERCICIO 6 
Faça um programa para a leitura de duas notas parciais de um aluno. O programa deve calcular a média alcançada por aluno e apresentar: A mensagem "Aprovado", se a média alcançada for maior ou igual a sete; A mensagem "Reprovado", se a média for menor do que sete; A mensagem "Aprovado com Distinção", se a média for igual a dez.

##	EXERCICIO 7 

Faça um Programa para um caixa eletrônico.

O programa deverá perguntar ao usuário a valor do saque e depois informar quantas notas de cada valor serão fornecidas.

As notas disponíveis serão as de 1, 5, 10, 50 e 100 reais. O valor mínimo é de 10 reais e o máximo de 600 reais.

O programa não deve se preocupar com a quantidade de notas existentes na máquina.

Exemplo 1: Para sacar a quantia de 256 reais, o programa fornece duas notas de 100, uma nota de 50, uma nota de 5 e uma nota de 1;

Exemplo 2: Para sacar a quantia de 399 reais, o programa fornece três notas de 100, uma nota de 50, quatro notas de 10, uma nota de 5 e quatro notas de 1.

##	EXERCICIO 8
Um posto está vendendo combustíveis com a seguinte tabela de descontos: Álcool: até 20 litros, desconto de 3% por litro acima de 20 litros, desconto de 5% por litro Gasolina: até 20 litros, desconto de 4% por litro acima de 20 litros, desconto de 6% por litro

Escreva um algoritmo que leia o número de litros vendidos, o tipo de combustível (codificado da seguinte forma: A-álcool, G-gasolina), calcule e imprima o valor a ser pago pelo cliente sabendo-se que o preço do litro da gasolina é R$ 2,50 o preço do litro do álcool é R$ 1,90.

# Fomulário para entrega + Desafio

https://forms.gle/bk5CeJSbCCFUqUDR9


-------------------------------------------------------------------------------------
## Resposta.1

Algoritmo "Ordena_Tres_Numeros"
Var
    numero1, numero2, numero3: Real
Inicio
    Escreva("Digite um numero: ")
    Leia(numero1)
    Escreva("Digite outro numero: ")
    Leia(numero2)
    Escreva("Digite mais um numero: ")
    Leia(numero3)

    Se (numero1 > numero2) e (numero2 > numero3) Entao
        Escreva(numero1, " ", numero2, " ", numero3)
    Senao
    Se (numero1 > numero3) e (numero3 > numero2) Entao
        Escreva(numero1, " ", numero3, " ", numero2)
    Senao
    Se (numero2 > numero1) e (numero1 > numero3) Entao
        Escreva(numero2, " ", numero1, " ", numero3)
    Senao
    Se (numero2 > numero3) e (numero3 > numero1) Entao
        Escreva(numero2, " ", numero3, " ", numero1)
    Senao
    Se (numero3 > numero1) e (numero1 > numero2) Entao
        Escreva(numero3, " ", numero1, " ", numero2)
    Senao
        Escreva(numero3, " ", numero2, " ", numero1)
    FimSe
    Fimse
    Fimse
    Fimse
    FimSe


## Resposta.2

Var
    lado1, lado2, lado3: Real
Inicio
    Escreva("Digite o primeiro lado do triângulo: ")
    Leia(lado1)
    Escreva("Digite o segundo lado do triângulo: ")
    Leia(lado2)
    Escreva("Digite o terceiro lado do triângulo: ")
    Leia(lado3)

Se (lado1 + lado2 > lado3) e (lado1 + lado3 > lado2) e (lado2 + lado3 > lado1) Entao
   Se (lado1 = lado2) e (lado2 = lado3) Entao
            Escreva("É um triângulo equilátero!")
   Senao
        Se (lado1 = lado2) ou (lado1 = lado3) ou (lado2 = lado3) Entao
            Escreva("É um triângulo isósceles!")
        Senao
            Escreva("É um triângulo escaleno!")
        FimSe
   fimse
Senao
        Escreva("Não é um triângulo!")
FimSe


## Resposta.3

Algoritmo "Par_ou_Impar"
Var
    numero: Inteiro
Inicio
    Escreva("Digite um número inteiro: ")
    Leia(numero)

    Se (numero Mod 2 = 0) Entao
        Escreva("Par")
    Senao
        Escreva("Ímpar")
    FimSe
Fimalgoritmo


## Resposta.4

Algoritmo "Calculadora_Paridade_Sinal_Tipo"
Var
    numero1, numero2, resultado: Real
    op: Caractere
Inicio
    Escreva("Digite um número: ")
    Leia(numero1)
    Escreva("Digite outro número: ")
    Leia(numero2)
    Escreva("Digite qual operação (+, -, * ou /) deseja realizar: ")
    Leia(op)

    Se (op = '+') Entao
        resultado <- numero1 + numero2
    Senao Se (op = '-') Entao
        resultado <- numero1 - numero2
    Senao Se (op = '*') Entao
        resultado <- numero1 * numero2
    Senao Se (op = '/') Entao
        Se numero2 <> 0 Entao
            resultado <- numero1 / numero2
        Senao
            Escreva("Erro: divisão por zero!")
            Pare
        FimSe
    Senao
        Escreva("Operação inválida!")
        Pare
    FimSe

    Escreva("O resultado é: ", resultado, "\n")

    Se (Resultado Mod 2 = 0) Entao
        Escreva("Par")
    Senao
        Escreva("Ímpar")
    FimSe

    Se (resultado >= 0) Entao
        Escreva("\nPositivo")
    Senao
        Escreva("\nNegativo")
    FimSe

    Se (resultado = Trunc(resultado)) Entao
        Escreva("\nInteiro")
    Senao
        Escreva("\nDecimal")
    FimSe

Fimalgoritmo


## Resposta.5

Algoritmo "Classificacao_Crime"
Var
    resposta: Caractere
    positivos: Inteiro
Inicio
    positivos <- 0

    Escreva("Telefonou para a vítima? (S ou N): ")
    Leia(resposta)
    Se (resposta = 'S') ou (resposta = 's') Entao
        positivos <- positivos + 1
    FimSe

    Escreva("Esteve no local do crime? (S ou N): ")
    Leia(resposta)
    Se (resposta = 'S') ou (resposta = 's') Entao
        positivos <- positivos + 1
    FimSe

    Escreva("Mora perto da vítima? (S ou N): ")
    Leia(resposta)
    Se (resposta = 'S') ou (resposta = 's') Entao
        positivos <- positivos + 1
    FimSe

    Escreva("Devia para a vítima? (S ou N): ")
    Leia(resposta)
    Se (resposta = 'S') ou (resposta = 's') Entao
        positivos <- positivos + 1
    FimSe

    Escreva("Já trabalhou com a vítima? (S ou N): ")
    Leia(resposta)
    Se (resposta = 'S') ou (resposta = 's') Entao
        positivos <- positivos + 1
    FimSe

    Se (positivos < 2) Entao
        Escreva("Inocente")
    Senao Se (positivos = 2) Entao
        Escreva("Suspeita")
    Senao Se (positivos < 5) Entao
        Escreva("Cúmplice")
    Senao
        Escreva("Assassino")
    FimSe
Fimalgoritmo


## Resposta.6

Algoritmo "Calcula_Media_Aprovacao"
Var
    nota1, nota2, media: Real
Inicio
    Escreva("Digite a primeira nota: ")
    Leia(nota1)
    Escreva("Digite a segunda nota: ")
    Leia(nota2)

    media <- (nota1 + nota2) / 2.0

    Se (media = 10) Entao
        Escreva("Aprovado com Distinção")
    Senao Se (media >= 7) Entao
        Escreva("Aprovado")
    Senao
        Escreva("Reprovado")
    FimSe
Fimalgoritmo

## Resposta.7

Algoritmo "Caixa_Eletronico"
Var
    valor, cem, cinquenta, dez, cinco, um: Inteiro
Inicio
    Escreva("Digite o valor a ser sacado (entre 10 e 600): ")
    Leia(valor)

    Se (valor < 10) ou (valor > 600) Entao
        Escreva("Valor inválido!")
    Senao
        cem <- valor Div 100
        valor <- valor - (cem * 100)

        cinquenta <- valor Div 50
        valor <- valor - (cinquenta * 50)

        dez <- valor Div 10
        valor <- valor - (dez * 10)

        cinco <- valor Div 5
        valor <- valor - (cinco * 5)

        um <- valor

        Se (cem > 0) Entao
            Escreva("\n", cem, " nota(s) de cem")
        FimSe
        Se (cinquenta > 0) Entao
            Escreva("\n", cinquenta, " nota(s) de cinquenta")
        FimSe
        Se (dez > 0) Entao
            Escreva("\n", dez, " nota(s) de dez")
        FimSe
        Se (cinco > 0) Entao
            Escreva("\n", cinco, " nota(s) de cinco")
        FimSe
        Se (um > 0) Entao
            Escreva("\n", um, " nota(s) de um")
        FimSe
    FimSe
Fimalgoritmo


## Resposta.08

Algoritmo "Calcula_Preco_Combustivel"
Var
    litros, preco: Real
    combustivel: Caractere
Inicio
    Escreva("Digite quantos litros você quer abastecer: ")
    Leia(litros)
    
    Escreva("Digite A para álcool ou G para gasolina: ")
    Leia(combustivel)

    Se (combustivel = 'A') ou (combustivel = 'a') Entao
        preco <- litros * 1.9
        Se (litros <= 20) Entao
            preco <- preco - (1.9 * litros * 3 / 100)
        Senao
            preco <- preco - (1.9 * litros * 5 / 100)
        FimSe
    Senao Se (combustivel = 'G') ou (combustivel = 'g') Entao
        preco <- litros * 2.5
        Se (litros <= 20) Entao
            preco <- preco - (2.5 * litros * 4 / 100)
        Senao
            preco <- preco - (2.5 * litros * 6 / 100)
        FimSe
    FimSe

    Escreva("O preço a pagar é R$", preco:2)
Fimalgoritmo
