# IC — MOOC de Introdução à Programação Competitiva em Python

Plano de trabalho e proposta para avaliação do orientador • versão 0.2 • 08/10/2026

## 1. Definições confirmadas

Fonte: conversa de Thomas com o Prof. Nunes, em 08/10/2026.

- Curso voltado aos alunos, no formato MOOC.
- Vídeos curtos para explicar conceitos, resolver problemas e apresentar estratégias e algoritmos.
- Python como linguagem de ensino.
- Introdução à linguagem em paralelo ao avanço do curso.
- Primeiro MOOC de introdução à programação competitiva, incluindo entrada/saída, validação de casos de teste, `if`, `for` e arrays.

Neste documento, “arrays” será tratado inicialmente como **listas de Python**, a confirmar com o professor. Listas atendem às atividades propostas; não são tecnicamente idênticas a arrays de tamanho fixo de outras linguagens.

A informação anterior de que os alunos já conhecem programação básica continua como expectativa do público, mas Python completo não será exigido de entrada: os recursos usados serão introduzidos ou retomados no momento necessário. O nível mínimo de autonomia com computador e execução de código ainda precisa ser confirmado.

**Mudanças em relação à versão 0.1:** o produto principal passa de uma sequência de encontros presenciais e guias docentes para um curso assíncrono. Guias para professores tornam-se complementares. A trilha avançada e a duração de 90 minutos por encontro deixam de orientar a primeira entrega.

## 2. Proposta resumida para o orientador

**Título proposto:** Introdução à Programação Competitiva com Python.

**Objetivo:** ao final, o aluno deverá interpretar problemas simples, ler e produzir dados no formato pedido, utilizar condições, repetições e listas, criar casos de teste e resolver problemas introdutórios de forma independente.

**Público proposto:** estudantes com contato inicial com programação, sem experiência competitiva. Introdução contextualizada a Python, sem exigir C++.

**Formato proposto:** cinco módulos, aproximadamente 18 vídeos de 4–8 minutos, pequenas atividades entre vídeos e quatro problemas finais. Faixa estimada de vídeo total: 72–144 minutos. O tempo completo de estudo será maior, sobretudo pela prática, e deverá ser estimado no piloto. Quantidade, duração e módulos ainda não foram aprovados pelo professor.

**Produto mínimo para avaliação inicial:** mapa do curso, roteiro de um vídeo, um problema resolvido e um exercício de transferência com gabarito e testes. Após a aprovação do padrão, produzir o restante.

**Não incluído neste primeiro MOOC:** C++, estruturas avançadas, grafos, programação dinâmica, busca binária e técnicas de otimização como eixo principal. A ideia intuitiva de eficiência pode aparecer, mas análise assintótica formal fica para uma continuidade a discutir.

## 3. Estrutura proposta do primeiro MOOC

| Módulo | Vídeos propostos | Objetivo prático |
|---|---|---|
| 1 — Conhecer o problema e o ambiente | 1. O que é programação competitiva; 2. Como ler um enunciado; 3. Executar um programa Python | Identificar tarefa, dados e resultado; executar código |
| 2 — Entrada, saída e testes | 4. `input`, `int` e variáveis; 5. `print` e formato de saída; 6. Testar além dos exemplos; 7. Resolução comentada | Transformar a especificação em um programa testável |
| 3 — Decisões | 8. Comparações e `if/else`; 9. Condições de fronteira; 10. Resolução comentada | Escolher a resposta correta, inclusive no limite |
| 4 — Repetições | 11. `for` e `range`; 12. Acumuladores e contadores; 13. Resolução comentada | Processar várias entradas sem repetir código |
| 5 — Listas e integração | 14. Criar listas e acessar índices; 15. Ler vários valores; 16. Percorrer listas; 17. Resolução integrada; 18. Preparação para o desafio final | Armazenar e processar sequências com os recursos aprendidos |

Atividade breve depois de cada vídeo conceitual: prever saída, escolher um teste, encontrar um erro ou completar poucas linhas. Problema independente depois de cada resolução, com mudança de contexto e pistas graduais.

“Vídeo curto” será uma diretriz, não uma obrigação de cortar uma explicação importante no meio. Separar leitura, estratégia e implementação em vídeos distintos apenas quando cada parte fizer sentido por si mesma.

## 4. Sequência de introdução a Python

| Recurso | Momento de introdução | Cuidado |
|---|---|---|
| Variáveis, inteiros e operações | Entrada/saída | `input()` retorna texto; explicitar conversão |
| `print()` | Primeiras soluções | Não inserir mensagens extras em saída de juiz |
| Comparações e indentação | Decisões | Diferenciar `=` de `==` e explicar blocos |
| `for` e `range` | Repetições | Mostrar que o limite final de `range` não é incluído |
| Acumuladores e contadores | Repetições | Inicialização e atualização são partes da estratégia |
| Listas e índices | Sequências | Índices começam em zero; acesso deve respeitar tamanho |
| `split()` | Vários valores na mesma linha | Mostrar a lista de textos antes da conversão |
| `append()` e conversão item a item | Leitura de listas | Começar com laço explícito |

Não usar compreensões de lista, `map`, funções próprias ou leitura com `sys.stdin` antes de explicar o recurso, se vierem a ser necessários. Preferir código compreensível na introdução; atalhos podem ficar como notas posteriores.

Nem todo problema com vários números precisa armazená-los: mostrar quando um contador ou acumulador basta e quando guardar a sequência é útil.

## 5. O que significa validar casos de teste

Há duas interpretações possíveis na fala do professor: ensinar o aluno a testar a própria solução e preparar testes para corrigir os exercícios. A proposta contempla ambas, mas a prioridade deve ser confirmada.

### Para o aluno

- Calcular a resposta esperada antes de executar.
- Comparar saída real e esperada.
- Testar exemplos, entradas mínimas e valores exatamente na fronteira de uma condição.
- Quando permitido pelo enunciado, testar zeros, negativos, empates, repetições e listas com um elemento.
- Explicar que passar nos exemplos não garante correção geral.

O programa pode assumir entradas válidas se o enunciado garantir isso. Não confundir testes da solução com criar mensagens de validação para dados inválidos.

### Para a equipe produtora

Cada problema terá uma solução de referência, casos documentados e restrições consistentes. A política de comparação de saída deve ser definida pela plataforma: texto, espaços, linhas e respostas numéricas precisam de regras explícitas.

Termos como Accepted e Wrong Answer serão introduzidos com significado. Erros de execução e de sintaxe serão diferenciados. Demonstrações de uma plataforma específica só serão produzidas depois de ela ser escolhida.

## 6. Padrão de produção de cada vídeo

**Identificação:** código, título, objetivo, pré-requisitos e duração estimada.

**Roteiro:** situação-problema → ideia → exemplo visual ou código → teste → síntese → tarefa.

**Entregáveis:** roteiro de narração, notas de tela, código quando houver, atividade, gabarito, testes e legenda/transcrição revisada.

**Critérios de revisão:** um objetivo central; nenhum recurso de Python não explicado; exemplos corretos; código legível; áudio compreensível; atividade alinhada ao objetivo; acessibilidade básica com transcrição e sem depender apenas de cores.

**Fluxo:** rascunho → revisão técnica → revisão pelo orientador → gravação piloto → revisão de áudio/tela/legenda → versão para publicação.

É mais barato corrigir o roteiro antes de gravar. Não gravar o curso inteiro antes da avaliação do primeiro vídeo.

## 7. Primeiro roteiro para avaliação

### Vídeo 1 — O que é programação competitiva?

**Duração proposta:** 4–6 minutos. **Objetivo:** reconhecer o ciclo enunciado → estratégia → programa → teste. **Não exige código.** Roteiro abaixo é um rascunho de produção, ainda sem gravação.

| Trecho | Narração sugerida | Tela |
|---|---|---|
| Abertura | “Você recebe uma descrição de um problema. Precisa descobrir como resolvê-lo e escrever um programa que funcione para as entradas permitidas. Esse é o tipo de tarefa que vamos praticar neste curso.” | Título e uma situação simples |
| Problema | “Uma equipe marcou pontos em duas rodadas. Dados os pontos de cada rodada, queremos o total. Se marcou 3 e depois 5, a resposta é 8. Mas o programa precisa funcionar também para outros valores.” | Dados: 3 e 5; resultado: 8 |
| Estratégia | “Antes de escrever código, vamos dizer o que precisa acontecer: ler dois números, somá-los e apresentar o resultado.” | Três passos destacados |
| Especificação | “O enunciado informa o que entra, o que deve sair e quais valores são permitidos. Esses detalhes fazem parte do problema. Se a saída pede apenas um número, adicionar uma frase pode causar rejeição pelo avaliador.” | Entrada, saída e restrições |
| Testes | “Depois de implementar, comparamos o resultado com o que esperávamos. Um exemplo correto ajuda, mas não é prova suficiente. Precisamos pensar em outros casos, como duas rodadas com zero ponto.” | Casos 3/5 e 0/0 |
| Estratégias | “Nos próximos vídeos, vamos aprender recursos de Python quando precisarmos deles para resolver os problemas: condições, repetições e listas. Também vamos discutir por que a estratégia funciona.” | Mapa simplificado do curso |
| Fechamento | “Antes do próximo vídeo, tente responder: quais dados precisamos receber nesse problema e qual resultado precisamos produzir?” | Pergunta de pausa |

Nota de produção: em fala natural, conferir se o roteiro cabe no tempo sem acelerar artificialmente; expandir o exemplo com participação do aluno se necessário. Não preencher tempo repetindo definições.

## 8. Primeiro problema e atividade de transferência

Esses itens são especificações iniciais para revisão; código de referência e testes executáveis ainda não foram produzidos.

### PC-01 — Pontos em duas rodadas

**Objetivo:** leitura de inteiros, soma e saída. **Uso:** resolução comentada após os vídeos de entrada/saída.

Uma equipe participou de duas rodadas. Dados os pontos obtidos em cada rodada, determine a soma dos pontos.

**Entrada:** duas linhas; a primeira contém o inteiro A e a segunda contém o inteiro B. **Restrições:** 0 ≤ A, B ≤ 1000.

**Saída:** uma linha com o inteiro A + B, sem mensagem adicional.

**Exemplo:** entrada `3` na primeira linha e `5` na segunda; saída `8`.

**Estratégia de referência:** ler e converter os dois valores, somar, imprimir. Tempo e memória auxiliares constantes dentro das restrições definidas.

| A | B | Saída esperada | Finalidade |
|---:|---:|---:|---|
| 3 | 5 | 8 | Exemplo |
| 0 | 0 | 0 | Mínimos |
| 0 | 1000 | 1000 | Um valor zero |
| 1000 | 1000 | 2000 | Máximos |
| 12 | 7 | 19 | Detectar concatenação de textos |

**Erro a demonstrar:** somar textos lidos diretamente pode concatená-los. Mostrar a diferença entre `"3" + "5"` e `3 + 5` depois de explicar a conversão.

### PC-02 — Estoque após reposição

**Objetivo:** aplicar a mesma estrutura de entrada/saída em uma expressão diferente. **Uso:** tentativa independente antes do gabarito.

Uma loja tinha E unidades, recebeu R unidades e vendeu V unidades. Determine o estoque final.

**Entrada:** três linhas com os inteiros E, R e V, nessa ordem. **Restrições:** 0 ≤ E, R ≤ 1000; 0 ≤ V ≤ E + R.

**Saída:** uma linha com o estoque final.

**Exemplo:** E = 10, R = 4, V = 6; saída `8`.

**Pistas:** quais operações aumentam o estoque? Qual operação diminui? O estoque inicial sozinho é suficiente para limitar as vendas?

**Gabarito reservado:** E + R − V. A condição V ≤ E + R garante resultado não negativo.

| E | R | V | Saída esperada |
|---:|---:|---:|---:|
| 10 | 4 | 6 | 8 |
| 0 | 0 | 0 | 0 |
| 2 | 5 | 7 | 0 |
| 1000 | 1000 | 0 | 2000 |

Na versão entregue aos alunos, separar o gabarito e os testes reservados do enunciado.

## 9. Avaliação e dimensão científica

**Para o curso:** atividades de compreensão; problemas independentes por módulo; desafio final com entrada/saída, condição, repetição e listas. Critério inicial sugerido: resolver os problemas obrigatórios e explicar pelo menos uma estratégia; a regra de conclusão depende da plataforma e do professor.

**Para a IC:** objetivo, método e relatório devem seguir o projeto aprovado. Esta conversa define o produto educacional, mas não define uma pesquisa experimental. Não será exigida uma nova pergunta de pesquisa como condição para começar os materiais.

Se o orientador desejar avaliar o curso, uma pergunta candidata é: “Quais dificuldades surgem no uso de um MOOC que introduz Python em paralelo à resolução de problemas competitivos?” Dados possíveis: testes de compreensão, problemas resolvidos, dúvidas e feedback. Visualização de vídeo ou conclusão do curso, isoladamente, não demonstram aprendizagem.

Coleta de dados de participantes para pesquisa depende de alinhamento institucional. Resultados, referências e participação não serão presumidos. Antes/depois sem comparação adequada não permite atribuir todo ganho ao curso.

## 10. Organização e próximos passos

Estrutura proposta: projeto; curso/modulo-01; roteiros; codigos; exercicios; testes; gravacoes; transcricoes; relatorios. As pastas, vídeos e plataforma ainda não foram criados; este documento reúne o planejamento e a amostra inicial.

| Prioridade | Ação | Estado |
|---|---|---|
| 1 | Confirmar Python, MOOC e escopo introdutório | Confirmado pelo professor |
| 2 | Revisar mapa e roteiro apresentados neste documento | Pronto para avaliação inicial |
| 3 | Confirmar plataforma, prazo e carga horária | Pendente |
| 4 | Produzir soluções executáveis e validar exercícios iniciais | Pendente |
| 5 | Gravar um vídeo piloto | Após revisão do roteiro |
| 6 | Revisar padrão e produzir módulo 1 completo | Pendente |
| 7 | Produzir módulos seguintes | Depois de validar o padrão |

### Pontos para o orientador avaliar

1. O recorte e a sequência dos cinco módulos representam o primeiro MOOC esperado?
2. Qual conhecimento mínimo será exigido de entrada?
3. Em “validação dos casos de teste”, qual dimensão deve receber mais atenção?
4. Qual plataforma hospedará vídeos e exercícios? Haverá juiz automático?
5. Qual a vigência da IC, disponibilidade semanal e exigências de relatório?
6. Qual duração e número de vídeos são viáveis?

### Registro de decisões

08/10/2026: Python confirmado; público aluno; formato MOOC; linguagem introduzida em paralelo; primeiro curso limitado aos fundamentos. Estrutura de cinco módulos, 18 vídeos, exercícios e roteiro são propostas da versão 0.2, aguardando avaliação do Prof. Nunes.
