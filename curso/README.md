# Mapa do curso

Sequência dos 8 módulos do curso básico, a partir da [reunião de 07/11/2026](../docs/reunioes/2026-11-07.md),
do estudo pedagógico em [`findings.md`](../findings.md) e das decisões registradas com o responsável.
A unidade de produção é uma microaula com um objetivo (média de 1 a 3 minutos, um conteúdo por aula),
com pré-requisitos explícitos para permitir entrada lateral na trilha (MOOC).

## Módulo 1 — Introdução à programação competitiva (sem código)

Apresentação sem código. O aluno conhece o formato dos desafios, por que participar,
as linguagens do meio e a diferença entre resolver e resolver com eficiência,
antes de aprender a ler enunciados e entender a avaliação.

| ID | Microaula | Objetivo |
|---|---|---|
| M01-A01 | O que é programação competitiva? | Explicar o tipo de desafio que o curso ensina a resolver. |
| M01-A02 | Por que participar? Benefícios e portas | Mostrar o que a prática desenvolve e abre (entrevistas, raciocínio, olimpíadas). |
| M01-A03 | OBI e InterIF | Situar as duas competições que orientam a escolha dos exercícios. |
| M01-A04 | Linguagens: Python aqui, C++ lá fora | Apresentar as linguagens da modalidade; o curso usa Python. |
| M01-A05 | Tipos de problema: certo não basta | Introduzir limite de tempo e a ideia de solução otimizada. |
| M01-A06 | Como ler um enunciado | Localizar o que o problema pede, as informações fornecidas e as regras. |
| M01-A07 | Como uma solução é avaliada | Mostrar conceitualmente que um avaliador roda a solução com diferentes casos. |
| M01-A08 | Atividade no papel: destrinchando um enunciado | Marcar dados, pergunta e regras num enunciado real, sem resolver. |

Roteiro pronto: [M01-A01](../docs/producao/roteiro-m01-a01.md).

## Módulo 2 — Entrada, saída e problemas de cálculo (Python mínimo)

O aluno lê entradas, determina saídas e confere casos no papel; depois usa o
mínimo de Python (variáveis, contas, `print`) para calcular a resposta e testar
casos de borda. Sem condicionais e sem laços.

| ID | Microaula | Objetivo |
|---|---|---|
| M02-A01 | Como ler o formato da entrada | Identificar os valores, sua ordem e a divisão em linhas. |
| M02-A02 | Como escrever a saída esperada | Identificar o resultado e apresentá-lo no formato pedido. |
| M02-A03 | O que as restrições garantem | Usar os limites do enunciado para reconhecer entradas válidas. |
| M02-A04 | Variáveis, contas e print em Python | Criar variáveis, fazer contas e mostrar o resultado. |
| M02-A05 | Resolvendo o Teleférico no papel e no código | Justificar as viagens manualmente e traduzir para Python. |
| M02-A06 | Casos de teste e casos de borda | Conferir o raciocínio nos limites, nomeando o conceito de caso de borda. |

Exercício da sequência: [Teleférico adaptado](modulo-02-entrada-e-saida/teleferico.md).

## Módulo 3 — Python e condicionais

Primeiro contato sistemático com código: executar, guardar valores, comparar,
combinar condições com booleanos e decidir com if/else/elif, fechando com um
problema de decisão resolvido de ponta a ponta.

| ID | Microaula | Objetivo |
|---|---|---|
| M03-A01 | Executando um primeiro programa em Python | Mostrar como executar um exemplo curto com entrada e saída. |
| M03-A02 | Variáveis e valores em Python | Guardar um valor e usá-lo em um exemplo curto. |
| M03-A03 | Comparações em Python | Avaliar uma condição como verdadeira ou falsa. |
| M03-A04 | Booleanos e operadores lógicos | Combinar condições com `and`, `or` e `not`. |
| M03-A05 | Como usar if | Executar um trecho quando a condição é verdadeira. |
| M03-A06 | Como usar else | Tratar o caso em que a condição não vale. |
| M03-A07 | Como usar elif | Organizar decisões com mais de duas possibilidades. |
| M03-A08 | Resolvendo um problema de decisão | Traduzir uma regra do enunciado em condições e conferir a resposta nos limites. |

Decisão registrada: `match/case` fica fora do básico (vai para o avançado).

## Módulo 4 — Laços e repetição (mapa pronto)

`while` e `for`, repetição condicionada versus contada, percorrer sequências e
problemas de acumulação e contagem em exercícios OBI de repetição simples.

## Módulo 5 — Strings (mapa pronto)

Texto como sequência: acesso, fatiamento, busca e contagem de caracteres em
problemas OBI de manipulação de texto. Vem antes de vetores porque, em Python,
a string é o caso simples e imutável de sequência.

## Módulo 6 — Vetores / listas (mapa pronto)

Guardar coleções em listas: índices, percurso com laços, frequência, máximo e
mínimo em problemas OBI de lista.

## Módulo 7 — Matrizes / listas de listas (mapa pronto)

Tabela como vetor de vetores: linhas, colunas e laços aninhados em problemas
OBI em grade.

## Módulo 8 — Funções e consolidação (mapa pronto)

Dividir o programa em funções com parâmetros e, como capstone do básico, um
problema OBI resolvido de ponta a ponta: ler, resolver, codar e testar.

---

Detalhamento das aulas de M01–M03 (título, duração, resumo e pré-requisitos):
[docs/producao/mapa-aulas-m01-m03.md](../docs/producao/mapa-aulas-m01-m03.md).
