# 📊 Exercício de Excel – Funções de Contagem

## Situação
Você é responsável por organizar uma planilha com os **dados de uma turma de alunos**.  
Na tabela abaixo, estão as **notas** e algumas informações preenchidas e outras em branco.

| Aluno   | Nota | Situação   |
|---------|------|------------|
| Ana     | 8    | Aprovado   |
| Bruno   | 7    | Aprovado   |
| Carla   |      |            |
| Diego   | 5    | Reprovado  |
| Elisa   | 9    | Aprovado   |
| Felipe  |      |            |
| Giovana | 6    | Reprovado  |
| Hugo    | 10   | Aprovado   |
| Isabela |      |            |

---

## 📌 Tarefas

### 1. CONT.NÚM  
Conte quantos alunos **têm notas lançadas** (não estão em branco).  

```excel
=CONT.NÚM(B2:B10)
```

### 2. CONT.VALORES

Conte quantos alunos já possuem alguma **situação preenchida** (Aprovado ou Reprovado).
```excel
=CONT.VALORES(C2:C10)
```

### 3. CONT.SE

Conte quantos alunos estão **Aprovados**:
```excel
=CONT.SE(C2:C10;"Aprovado")
```
Conte quantos alunos estão **Reprovados**:
```excel
=CONT.SE(C2:C10;"Reprovado")
```

## Desafio Extra:
Use o CONT.SE para descobrir quantos alunos tiraram nota maior ou igual a 7.

```excel
=CONT.SE(B2:B10;">=7")
```

### Objetivo:
Este exercício ajuda a praticar as funções:

- CONT.NÚM

- CONT.VALORES 

- CONT.SE

Essas funções são fundamentais para **análise de dados em Excel.**