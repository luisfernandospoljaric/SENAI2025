# Aula 07: Macros e funções 

## Objetivo da Aula: Macros
 
O que são Macros no Excel?
Macros no Excel são conjuntos de comandos que automatizam tarefas repetitivas. Elas podem ser criadas usando VBA (Visual Basic for Applications) ou recursos nativos do Excel, como o Power Query e Gravação de Macros.

---

## 🔹 Tipos de Macros no Excel
Macros com VBA (mais avançado)

Criadas usando código em VBA, permitindo personalização total.

Exemplo: Criar um botão para formatar células automaticamente.

Macros sem VBA (automatização sem programação)

Usam Power Query, Tabelas Dinâmicas, Formulários e Fórmulas para automatizar tarefas.

Exemplo: Criar uma automação para importar e organizar dados.

---

# 📊 Função CONT.VALORES no Excel

## 📌 O que é a função CONT.VALORES?

A função `CONT.VALORES` conta **o número de células não vazias** em um intervalo, independentemente do tipo de dado (texto, número, data, etc.).

---

## 📌 Sintaxe
```excel
CONT.VALORES(intervalo)
```


## 📝 Exemplo Prático

Imagine que você tem a seguinte tabela no Excel:

| A       | B        | C        |
|---------|---------|----------|
| João    | 5000    | 15/03/24 |
| Maria   |         | 20/03/24 |
| Carlos  | 6000    |          |
|         | 5500    | 25/03/24 |

Se usarmos a seguinte fórmula:

```excel
=CONT.VALORES(A1:C4)
```


-- O Excel retornará 8, pois há 8 células preenchidas (incluindo números, textos e datas), ignorando apenas as células vazias.