# Teleférico — adaptação didática

A turma do colégio vai fazer uma excursão na serra e os alunos vão tomar um teleférico para subir até o pico de uma montanha. A cabine pode transportar, no máximo, **C alunos por viagem**.

Se a cabine comporta 10 alunos e a turma tem 20, é possível transportar todos em duas viagens, levando 10 em cada uma. A cabine pode viajar com lugares vazios. Todos os alunos devem ser transportados.

Dados a capacidade **C** e o número de alunos **A**, determine o menor número de viagens necessário para transportar a turma.

## Entrada

A primeira linha contém o inteiro **C**, a capacidade da cabine. A segunda linha contém o inteiro **A**, a quantidade de alunos.

## Saída

Uma linha com um inteiro que indica o menor número de viagens.

## Restrições

- 2 ≤ C ≤ 100.
- 1 ≤ A ≤ 1.000.

## Exemplos

| Exemplo | Primeira linha da entrada | Segunda linha da entrada | Linha da saída |
|---|---:|---:|---:|
| 1 | 10 | 20 | 2 |
| 2 | 12 | 55 | 5 |
| 3 | 100 | 87 | 1 |

## Uso na aula

Para a explicação na lousa, use C = 10 e A = 23. Duas viagens levam, no máximo, 20 alunos. Uma terceira acomoda os três restantes. Esse exemplo permite mostrar por que a última viagem conta mesmo quando sobram lugares.

Na atividade, peça que o aluno calcule a saída para C = 10 com 20, 21 e 3 alunos. Os resultados são 2, 3 e 1, respectivamente. Discuta o caso de divisão exata, a necessidade de mais uma viagem quando sobra um aluno e o caso em que uma viagem basta.

Esta adaptação remove a exigência de um monitor na cabine. A fonte é o [Teleférico da OBI 2017, Fase 1, Programação Nível 1](https://olimpiada.ic.unicamp.br/pratique/p1/2017/f1/teleferico/).
