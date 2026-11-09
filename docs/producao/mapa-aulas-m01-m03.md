# Mapa de aulas — M01, M02, M03 (proposta para revisão)

> Status: proposta de 09/11/2026, revisada com feedback do usuário, a partir do estudo pedagógico em `findings.md`.
> Não commitar sem pedido (AGENTS.md). M01–M03 e a ordem entre eles estão trancados;
> as aulas dentro deles foram reorganizadas. Duração de 1–3 min é média;
> exercício pode extrapolar (Q5). Um conteúdo por aula.

## Módulo 1 — Introdução à programação competitiva (sem código, 8 aulas)

| ID | Título | Duração | Resumo | Pré-requisitos |
|---|---|---|---|---|
| M01-A01 | O que é programação competitiva? | 2 min | Apresenta o formato: resolver problemas com código e submeter a um avaliador. | Nenhum |
| M01-A02 | Por que participar? Benefícios e portas (NOVA) | 3 min | O que a prática desenvolve e abre: entrevistas técnicas, raciocínio e função cognitiva, olimpíadas e universidade. | M01-A01 |
| M01-A03 | OBI e InterIF | 2 min | Situa as duas competições que orientam o curso: quem participa, como são as provas, por que os exercícios vêm delas. | M01-A02 |
| M01-A04 | Linguagens: Python aqui, C++ lá fora (NOVA) | 3 min | O curso usa Python; C++ é a linguagem mais comum nas competições (C e Java também aparecem). Ideia central: a linguagem é a ferramenta, os problemas são os mesmos. | M01-A03 |
| M01-A05 | Tipos de problema: certo não basta, tem que ser eficiente (NOVA) | 3 min | Muitos problemas são fáceis de resolver e difíceis de resolver bem: introduz limite de tempo e a ideia de solução otimizada, sem formalizar complexidade. | M01-A04 |
| M01-A06 | Como ler um enunciado | 3 min | Ensina a localizar num enunciado real o que é pedido, os dados fornecidos e as regras; o aluno sai sabendo separar pergunta de contexto. | M01-A05 |
| M01-A07 | Como uma solução é avaliada | 3 min | Mostra conceitualmente que o avaliador roda a solução com vários casos de teste escondidos e compara saídas; introduz a ideia de caso de teste. | M01-A06 |
| M01-A08 | Atividade no papel: destrinchando um enunciado | 4 min | O aluno recebe um enunciado curto e marca dados, pergunta e regras, sem resolver nem codar; fecha o módulo com verificação ativa. | M01-A07 |

## Módulo 2 — Entrada, saída e problemas de cálculo (Python mínimo, 6 aulas)

| ID | Título | Duração | Resumo | Pré-requisitos |
|---|---|---|---|---|
| M02-A01 | Como ler o formato da entrada | 2 min | Identifica valores, ordem e divisão em linhas usando o Teleférico (C na 1ª linha, A na 2ª); o aluno sai lendo qualquer bloco "Entrada". | M01-A06 |
| M02-A02 | Como escrever a saída esperada | 2 min | Identifica o resultado pedido e o formato exato da linha de saída; confere com os exemplos do Teleférico. | M02-A01 |
| M02-A03 | O que as restrições garantem | 3 min | Usa os limites do enunciado (2 ≤ C ≤ 100, 1 ≤ A ≤ 1.000) para reconhecer entradas válidas e o tamanho do problema. | M02-A02 |
| M02-A04 | Variáveis, contas e print em Python (NOVA) | 3 min | Python mínimo: criar variáveis, fazer contas (+, -, *, /) e mostrar o resultado com print. Sem condicionais, sem laços. | M02-A03 |
| M02-A05 | Resolvendo o Teleférico no papel e no código | 5 min | Primeiro o raciocínio manual (C = 10, A = 23 → 10 + 10 + 3); depois a tradução para poucas linhas de Python. A última viagem conta mesmo com lugares vazios. | M02-A04 |
| M02-A06 | Casos de teste e casos de borda | 4 min | Confere o raciocínio com C = 10 e A = 20, 21 e 3, e nomeia o conceito: caso de borda é a entrada no limite (divisão exata, sobra de um, mínimo e máximo das restrições). | M02-A05 |

## Módulo 3 — Python e condicionais (8 aulas)

| ID | Título | Duração | Resumo | Pré-requisitos |
|---|---|---|---|---|
| M03-A01 | Executando um primeiro programa em Python | 3 min | Mostra como rodar um programa curto que lê dois números e imprime um resultado; amarra o M02 (E/S) ao código. | M02-A04 |
| M03-A02 | Variáveis e valores em Python | 2 min | Retoma variáveis com mais calma: nomes, reutilização e tipos pelo uso, sem teoria. | M03-A01 |
| M03-A03 | Comparações em Python | 2 min | Avalia expressões com `==`, `!=`, `<`, `>`, `<=`, `>=` e lê o resultado; base das decisões. | M03-A02 |
| M03-A04 | Booleanos e operadores lógicos (NOVA) | 3 min | Valores `True`/`False` e como combinar condições com `e` (`and`), `ou` (`or`) e `não` (`not`). | M03-A03 |
| M03-A05 | Como usar if | 2 min | Executa um trecho só quando a condição é verdadeira; um conceito, um exemplo. | M03-A04 |
| M03-A06 | Como usar else | 2 min | Trata o caminho em que a condição não vale; contrasta com a aula anterior. | M03-A05 |
| M03-A07 | Como usar elif | 3 min | Organiza decisões com mais de duas possibilidades em cadeia; mostra a ordem de avaliação. | M03-A06 |
| M03-A08 | Resolvendo um problema de decisão | 5 min | Traduz uma regra de enunciado OBI em if/elif/else e confere a resposta nos limites; capstone que fecha o ciclo ler → codar → conferir. | M03-A07 |

## O que mudou nesta revisão (feedback do usuário, 09/11)

- M01: +3 aulas (A02 benefícios, A04 linguagens, A05 tipos de problema/eficiência); resto renumerado.
- M02: passa a incluir Python mínimo (A04 nova) e resolve o Teleférico também em código (A05); A06 passa a nomear casos de borda explicitamente. Revisa R1: condicionais continuam só no M03.
- M03: +1 aula (A04 booleanos e operadores lógicos) entre comparações e if; resto renumerado.
- `match/case` segue fora do básico (R3); nada muda por causa disso.
