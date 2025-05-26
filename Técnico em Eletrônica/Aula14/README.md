# Aula 14

## Estruturas de Decisão: `if`, `else if` e `else` em C

As estruturas de decisão permitem que um programa tome decisões com base em condições. Em C, usamos principalmente as palavras-chave `if`, `else if` e `else` para esse fim.

## 🔹 Sintaxe Básica

```c
if (condição) {
    // Bloco de código se a condição for verdadeira
} else if (outra_condição) {
    // Bloco de código se a outra_condição for verdadeira
} else {
    // Bloco de código se nenhuma condição anterior for verdadeira
}
```

## Exemplo: Verificação de número positivo, negativo ou zero

```c
#include <stdio.h>

int main() {
    int numero;

    printf("Digite um número: ");
    scanf("%d", &numero);

    if (numero > 0) {
        printf("O número é positivo.\n");
    } else if (numero < 0) {
        printf("O número é negativo.\n");
    } else {
        printf("O número é zero.\n");
    }

    return 0;
}
```

## Regras Importantes
- Os parênteses () ao redor da condição são obrigatórios.

- As chaves {} delimitam os blocos de código a serem executados.

- O else if é opcional e pode ser usado múltiplas vezes.

- O else é opcional e aparece por último, tratando o caso em que nenhuma condição anterior foi satisfeita.

## Exemplo 2: Verificação de nota.

```c
#include <stdio.h>

int main() {
    float nota;

    printf("Digite a nota do aluno: ");
    scanf("%f", &nota);

    if (nota >= 7.0) {
        printf("Aprovado!\n");
    } else if (nota >= 5.0) {
        printf("Recuperação.\n");
    } else {
        printf("Reprovado.\n");
    }

    return 0;
}
```

## Dicas
✅ Sempre verifique se a lógica das condições está correta.
✅ Utilize indentação para facilitar a leitura do código.
✅ Você pode aninhar estruturas if dentro de outras, se necessário.

# Operadores Aritméticos e Lógicos em C

## ✅ Operadores Aritméticos

| Operador | Descrição           | Exemplo        | Resultado      |
|----------|---------------------|----------------|----------------|
| `+`      | Adição              | `5 + 3`        | `8`            |
| `-`      | Subtração           | `10 - 4`       | `6`            |
| `*`      | Multiplicação       | `2 * 6`        | `12`           |
| `/`      | Divisão             | `8 / 2`        | `4`            |
| `%`      | Módulo (resto)      | `10 % 3`       | `1`            |

## ✅ Operadores Lógicos

| Operador | Nome                | Descrição                                   | Exemplo               | Resultado      |
|----------|---------------------|---------------------------------------------|------------------------|----------------|
| `&&`     | E lógico (AND)      | Verdadeiro se ambos os operandos forem verdadeiros | `(5 > 2 && 4 > 1)` | `true (1)`     |
| ||     | OU lógico (OR)      | Verdadeiro se pelo menos um operando for verdadeiro | `(5 < 2 || 4 > 1)` | `true (1)`     |
| `!`      | NÃO lógico (NOT)    | Inverte o valor lógico                      | `!(5 > 2)`            | `false (0)`    |


# Exercicios:

## Fáceis
1. Verificar se um número é par ou ímpar

2. Verificar se a pessoa é maior de idade

3. Verificar se um número é positivo, negativo ou zero

## Médio
4. Calcular conceito de uma nota.
9 ou mais, "Parabéns, aprovado com mérito!!"
7 ou mais, "Parabéns, aprovado"
5 ou mais, "Parabéns"
menos, "Reprovado"

5. Verificar se três lados formam um triângulo

6. Verificar se um ano é bissexto

## Dificéis
7. Classificar triângulo (equilátero, isósceles ou escaleno)

8. Calculadora simples (operações básicas +, - , / e *)

9. Sistema de login simples, Validar usuário e senha.

## Desafio
10. Verificar se três valores podem ser lados de um triângulo e classificá-lo

## Formulário de Envio:

https://forms.gle/369Jh3XRF1zsxnHF8