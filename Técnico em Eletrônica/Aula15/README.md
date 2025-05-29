# Aula 15 - Revisão para Prova.

# Indústria 4.0 – Resumo

A **Indústria 4.0** é considerada a **quarta revolução industrial**, caracterizada pela **automação inteligente** e pela **integração de tecnologias digitais** nos processos de produção. Ela conecta o mundo físico ao digital, tornando fábricas mais eficientes, conectadas e autônomas.

## 🔧 Principais Características

- **Internet das Coisas (IoT):** dispositivos e máquinas conectados trocando dados em tempo real.
- **Inteligência Artificial (IA) e Big Data:** análise avançada de dados para otimização e previsão de falhas.
- **Computação em Nuvem:** armazenamento e acesso remoto a sistemas e dados.
- **Robótica Avançada:** uso de robôs colaborativos (cobôs) que interagem com humanos.
- **Manufatura Aditiva (Impressão 3D):** criação de objetos a partir de modelos digitais.
- **Realidade Aumentada e Realidade Virtual:** apoio a manutenção, treinamento e desenvolvimento de produtos.

## ✅ Benefícios

- Aumento da **eficiência e produtividade**
- Redução de **erros e custos operacionais**
- Maior **flexibilidade** na produção
- Produtos mais **personalizados** e entregues rapidamente

## ⚠️ Desafios

- **Alto custo** de implementação inicial
- Necessidade de **profissionais qualificados**
- Riscos relacionados à **segurança cibernética**
- **Integração** com sistemas antigos (legados)

## 🌍 Impacto

A Indústria 4.0 vai além do chão de fábrica. Ela transforma toda a **cadeia de produção**, exigindo mudanças nos **modelos de gestão**, nos **perfis profissionais** e nos **modelos de negócio**. É uma revolução que busca **mais competitividade, inovação e sustentabilidade** no setor industrial.

---

# 🔐 Segurança Cibernética – Resumo

A **Segurança Cibernética** (ou **Cibersegurança**) é o conjunto de práticas, tecnologias e processos utilizados para **proteger sistemas, redes, programas e dados** contra ataques, danos ou acessos não autorizados. É essencial para garantir a **confidencialidade, integridade e disponibilidade** das informações no ambiente digital.

## 🛡️ Objetivos Principais

- **Confidencialidade:** garantir que apenas pessoas autorizadas tenham acesso às informações.
- **Integridade:** assegurar que os dados não sejam alterados de forma indevida.
- **Disponibilidade:** garantir que os sistemas e dados estejam acessíveis quando necessário.

## 🧰 Principais Ameaças

- **Malwares:** programas maliciosos como vírus, worms, trojans e ransomwares.
- **Phishing:** tentativas de enganar usuários para roubo de informações sensíveis.
- **Ataques DDoS:** sobrecarga de servidores para tirar sistemas do ar.
- **Engenharia Social:** manipulação psicológica para obter acesso ou informações.
- **Acessos não autorizados:** invasões a sistemas por hackers ou insiders mal-intencionados.

## 🔐 Boas Práticas de Segurança

- Utilizar **senhas fortes** e autenticação em dois fatores (2FA)
- Manter **softwares e sistemas atualizados**
- Utilizar **antivírus e firewalls**
- Fazer **backup** regular de dados
- Educar usuários sobre **ameaças digitais**
- Monitorar constantemente **acessos e atividades suspeitas**

## 🏛️ Áreas da Segurança Cibernética

- **Segurança de Rede:** proteção contra invasões e tráfego malicioso
- **Segurança da Informação:** políticas e controles para proteger dados
- **Segurança de Aplicações:** proteção contra vulnerabilidades em softwares
- **Resposta a Incidentes:** identificação, contenção e mitigação de ataques
- **Governança e Conformidade:** cumprimento de normas como LGPD, GDPR, ISO 27001

## 📈 Importância

Com o aumento da digitalização e do armazenamento de dados na nuvem, a segurança cibernética se tornou **fundamental para empresas, governos e indivíduos**. Proteger informações sensíveis é crucial para manter a **confiança, a reputação e a continuidade dos negócios**.

---

# 💻 Linguagem C – Resumo

A **linguagem C** é uma linguagem de programação de **baixo nível com recursos de alto nível**, muito utilizada em sistemas embarcados, sistemas operacionais e aplicações que exigem alto desempenho. É uma das linguagens mais antigas e influentes da computação moderna.

---

## 🧱 Estrutura Básica de um Programa em C

```c
#include <stdio.h>

int main() {
    // Código aqui
    return 0;
}
```
## ➕ Operadores em C

### 🔢 Operadores Aritméticos

| Operador | Descrição      | Exemplo   |
|----------|----------------|-----------|
| `+`      | Adição         | `a + b`   |
| `-`      | Subtração      | `a - b`   |
| `*`      | Multiplicação  | `a * b`   |
| `/`      | Divisão        | `a / b`   |
| `%`      | Módulo         | `a % b`   |

---

### 🔍 Operadores Relacionais

| Operador | Descrição           | Exemplo   |
|----------|---------------------|-----------|
| `==`     | Igual               | `a == b`  |
| `!=`     | Diferente           | `a != b`  |
| `>`      | Maior               | `a > b`   |
| `<`      | Menor               | `a < b`   |
| `>=`     | Maior ou igual      | `a >= b`  |
| `<=`     | Menor ou igual      | `a <= b`  |

---

### ⚙️ Operadores Lógicos

| Operador | Descrição       | Exemplo           |
|----------|-----------------|--------------------|
| `&&`     | E lógico        | `a > 0 && b < 10`  |
| `||`     | OU lógico       | `a == 1 || b == 2` |
| `!`      | NÃO lógico      | `!(a == b)`        |

---


## Exemplos em C

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

## 📚 Bibliotecas Mais Usadas na Linguagem C

Em C, as bibliotecas fornecem funções prontas que facilitam a manipulação de entrada/saída, cálculos matemáticos, manipulação de strings, controle de tempo e muito mais. Abaixo estão as bibliotecas padrão mais utilizadas:

---

### 📥 `#include <stdio.h>`

**Standard Input/Output**  
Contém funções para entrada e saída de dados, como:

- `printf()` – imprime dados no console
- `scanf()` – lê dados do usuário
- `fopen()`, `fclose()` – manipulação de arquivos

---

### 🧮 `#include <math.h>`

**Funções matemáticas**  
Permite usar funções como:

- `pow(x, y)` – exponenciação (x elevado a y)
- `sqrt(x)` – raiz quadrada
- `sin(x)`, `cos(x)`, `tan(x)` – funções trigonométricas
- `log(x)` – logaritmo natural

> ⚠️ Necessário compilar com `-lm` (ex: `gcc programa.c -lm`)

---

### 🧵 `#include <stdlib.h>`

**Utilitários gerais da linguagem**

- `malloc()`, `calloc()` – alocação dinâmica de memória
- `free()` – libera memória alocada
- `rand()` – gera número aleatório
- `exit()` – finaliza o programa

---

### 🧠 `#include <string.h>`

**Manipulação de strings (cadeias de caracteres)**

- `strlen()` – comprimento da string
- `strcpy()` – copia uma string
- `strcat()` – concatena strings
- `strcmp()` – compara strings

---

### ⏰ `#include <time.h>`

**Manipulação de data e hora**

- `time()` – retorna o tempo atual em segundos
- `clock()` – mede tempo de execução
- `localtime()` – converte para data/hora local
- `strftime()` – formata data/hora

---

### 👌 Outras Bibliotecas Comuns

| Biblioteca         | Descrição                                    |
|--------------------|----------------------------------------------|
| `<ctype.h>`        | Testes e conversões de caracteres (`toupper`, `isdigit`) |
| `<limits.h>`       | Constantes relacionadas a limites de tipos numéricos |
| `<float.h>`        | Limites de precisão para tipos `float` e `double` |
| `<stdbool.h>`      | Suporte ao tipo `bool` (verdadeiro/falso)    |
| `<assert.h>`       | Testes de afirmação durante a execução (`assert()`) |

---

### 🧠 Dica

Sempre verifique qual biblioteca possui as funções que você deseja usar. Consultar a [documentação oficial do C](https://en.cppreference.com/w/c/header) pode ajudar bastante!

---


