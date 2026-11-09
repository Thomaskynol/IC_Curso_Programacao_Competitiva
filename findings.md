# Findings — IC Curso Programação Competitiva

## Fontes lidas (repo, 09/11/2026)

- `curso/README.md`: M01 sem código; M02 leitura de entrada/saída + Teleférico no papel (decisão Python-ali-ou-não em aberto); M03 Python mínimo + if/else/elif. match/case opcional.
- `docs/reunioes/2026-11-07.md`: MOOC, microaulas 1–3 min, 1 assunto = 1 ponto de entrada; trilhas recombináveis via pré-requisitos; Teleférico como exemplo do M02; pendências: M02 papel-vs-código, atividade no papel no M01, match/case, fechar títulos+pré-requisitos.
- `curso/modulo-02-entrada-e-saida/teleferico.md`: adaptação sem monitor; C 2..100, A 1..1000; exemplos (10,20)->2; (12,55)->5; (100,87)->1; lousa C=10,A=23; atividade C=10 com 20/21/3.
- `docs/modelo-microaula.md`: ficha com ID, objetivo em 1 frase, pré-requisitos, duração, estado, roteiro 3 passos, apoio visual com valores exatos.
- Pedido novo (transcrição do usuário): 2 cursos (básico primeiro); 8 módulos do básico (3 existentes contam); descrições breves por módulo; para os 3 primeiros: título + duração + resumo breve por aula; M01-A01 aprofundada fica para depois; exige estudo pedagógico prévio justificando sequência; criar wiki nova da IC a partir do Git + instruções; entrevista antes para extrair o implícito.

## Entrevista (em andamento)

- 2026-11-09, público-alvo (Q1): entrada quase-zero — aluno pode chegar só tendo "ouvido falar de Python", sem saber programar; haverá também gente com bom nível. Formato MOOC serve justamente para isso: quem sabe pula, quem não sabe tem tudo disponível. Decisão derivada: M01–M02 não podem pressupor código; trilha precisa ser autocontida desde o zero com pré-requisitos explícitos por microaula. (Resposta do usuário: público "muito variado", não dá para afirmar perfil único.)
- 2026-11-09, saída do básico / limite básico-vs-avançado (Q2, CORRIGIDO): os itens citados (o que é PC, portas/benefícios, E/S no código com saída formatada, condicionais, laços, básico de vetores/matrizes/strings) são EXEMPLOS do nível esperado, NÃO a lista fechada de módulos — os 8 módulos serão criados pelo estudo pedagógico. Nível-alvo do básico: ciclo completo de problema simples de juiz. Avançado = além do fundamental.
- 2026-11-09, travamento dos 3 primeiros (Q3): MÓDULOS e ORDEM dos 3 primeiros trancados (M01 intro → M02 E/S → M03 condicionais); AULAS dentro deles podem mudar/reorganizar pelo estudo. Os 5 novos (M04–M08) nascem do estudo pedagógico.
- 2026-11-09, avaliação (Q4): FORA deste escopo — alguma verificação entre módulos (prova ou similar) será discutida depois; não desenhar avaliação agora.
- 2026-11-09, formato das aulas (Q5): 1–3 min é MÉDIA, não teto — aula de exercício difícil/tópico longo pode extrapolar; regra dura é a MODULARIDADE: nunca mais de um conteúdo por aula. Vale para os 8 módulos.
- 2026-11-09, wiki (Q6): público = AGENTES DE IA que ajudam na IC — função é contexto/memória para respostas melhores em trabalho futuro da IC. Implicação: wiki em pt-BR, densa em decisões/pendências/premissas, entity/concept pages sobre curso, decisões da reunião, estudo pedagógico e transcrições do usuário como raw.
- 2026-11-09, pendências da reunião (Q7): SIM — o estudo pedagógico deve recomendar posição nas pendências abertas com o orientador (M02 papel-vs-código, atividade no papel no M01, match/case, títulos+pré-requisitos).

## Estudo pedagógico (concluído 09/11/2026 — só web_extract, cf. decisão em task_plan.md)

### Fontes extraídas
1. OBI Pratique — modalidades Iniciação (IJ/I1/I2) e Programação (PJ/P1/P2/PU); tarefas separadas por nível/ano. https://olimpiada.ic.unicamp.br/pratique/
2. Teleférico original OBI 2017 P1 F1 — COM monitor (C inclui monitor; ex. (10,20)->3). Confirma que a adaptação do repo removeu o monitor e recalculou os exemplos (10,20)->2. https://olimpiada.ic.unicamp.br/pratique/p1/2017/f1/teleferico/
3. Ementa oficial OBI Modalidade Programação (baseada na IOI syllabus). Ordem literal da seção Programação [PM]: criar/compilar/executar → sintaxe → variáveis/expressões → tipos primitivos → operadores aritméticos → leitura E/S → condicionais → repetição → operadores lógicos → strings → vetores (incl. multidimensionais) → funções → recursão. https://olimpiada.ic.unicamp.br/prepare/ementas/ementa_prog
4. OBI "Estude" — Modalidade Iniciação PROPOSITALMENTE sem ementa (só detecção de talento em lógica); recomendação oficial: investir em ensino de programação básica (Saci, gratuito, sem instalar nada). https://olimpiada.ic.unicamp.br/prepare/estude/
5. USACO Guide — roadmap organizado por tópico: recursos curados + problemsets por nível + progresso. Modelo de trilha para o MOOC. https://usaco.guide/
6. Microlearning (Wikipedia) — módulos compactos, 1 objetivo por módulo, vídeos curtos (2–10 min), avaliação após cada segmento, espaçamento no tempo, redução de carga cognitiva. https://en.wikipedia.org/wiki/Microlearning
7. Neps Academy — trilha Competitive Programmer (indicada pelo usuário; a OBI a recomenda na página "Estude"). Curso "Introduction to Programming": hardware/software → linguagens → primeiro programa + submissão → variáveis → leitura → aritmética → decisão (3 aulas separadas: if-else, if-else-if, switch) → while/for/doWhile → ... → vetores → matrizes → caracteres → strings. Curso "Introduction to Competitive Programming": introdução às competições → OBI vs ICPC → entender problemas → estratégias de prova → simulados. https://neps.academy/track/competitive-programmer

### Síntese (o que a evidência diz)
- Ler enunciado antes de codar é etapa própria (M01 papel) — a OBI Iniciação avalia exatamente isso sem exigir código.
- E/S vem ANTES de condicionais na ementa e no M02 do repo — fundação correta; resolver no papel antes do código reduz carga cognitiva (worked-example effect).
- Ordem canônica pós-condicionais: repetição → strings → vetores → multidimensionais → funções. É a ordem de dependência: laços permitem percorrer strings; strings motivam vetores; vetores generalizam para matrizes; funções organizam tudo.
- Microaula = 1 objetivo + verificação curta. Regra "1 conteúdo por aula" do usuário = princípio central do microlearning.
- MOOC com saltos exige pré-requisitos explícitos por aula (USACO Guide usa o mesmo mecanismo com trilhas).
- Neps confirma a espinha dorsal (decisões separadas em 3 aulas → laços → coleções) e valida o M03 atual do repo, que já separa if/else/elif. Divergência honesta: Neps (em C) põe matrizes ANTES de strings e inclui switch no introdutório — em Python, strings antes de listas é mais natural (ambas são sequências; string é o caso simples e imutável), e a posição sobre match/case segue abaixo.

### Critérios de ordenação dos 8 módulos (aplicados)
C1 Dependência: nenhum módulo usa conceito de módulo posterior. C2 Concreto→abstrato (papel→código→estrutura). C3 Ordem da ementa OBI [PM]. C4 Cada módulo fecha um ciclo "ler→resolver→codar→conferir" num problema OBI real. C5 Entrada lateral: aluno experiente entra em qualquer módulo pelos pré-requisitos.

### Recomendações nas pendências da reunião 07/11 (Q7)
R1 M02 fica SEM código (só papel): primeiro contato com Python acontece no M03-A01, que já lê entrada e escreve saída (amarra M02→M03). Motivo: público quase-zero + Iniciação sem código + carga cognitiva.
- REVISÃO de R1 em 09/11/2026 (decisão do usuário, prevalece): M02 passa a incluir Python MÍNIMO (variáveis, contas, print) suficiente para calcular o Teleférico; condicionais continuam só no M03. Motivo do usuário: resolver o exercício em código já no M02 aumenta o ganho sem custo alto, pois o raciocínio manual já foi feito no papel.
- 2026-11-09, casos de borda (decisão): NÃO é cedo — a dificuldade central do Teleférico (sobra de alunos) já É um caso de borda; M02-A05/A06 passam a nomear o conceito explicitamente e testar nos limites das restrições (C=2, C=100, A=1, A=1000). Hábito de verificação desde o início.
- 2026-11-09, expansão do M01 (pedido do usuário): +3 aulas (benefícios/portas, linguagens, tipos de problema). M01 vai a 8 aulas, todas sem código.
- 2026-11-09, booleanos no M03 (pedido do usuário + Neps tem "Logical Operators" antes do if): nova aula M03-A04 (True/False, e/ou/não) entre comparações e if. M03 vai a 8 aulas.
R2 Atividade no papel no M01: SIM, uma microaula de encerramento (localizar dados/pergunta/regras num enunciado real, sem resolver). Mantém M01 sem código e dá fechamento ativo.
R3 match/case: FORA do básico (vai para o avançado). Motivo: não consta da ementa [PM]; if/elif cobre as Fases 1 P1; básico deve ficar mínimo. Contraponto registrado: o Neps inclui switch no introdutório (em C) — se o orientador quiser simetria com C, cabe como aula opcional curta no M03, sem virar pré-requisito de nada.
R4 Recursão: FORA do básico (avançado), mesmo constando como [PM] — custo cognitivo alto; básico fecha em funções + capstone.
R5 Títulos + pré-requisitos: fechados no mapa de aulas (próxima fase) para M01–M03.

### Proposta dos 8 módulos (descrições breves)
- M01 Introdução à programação competitiva (TRANCADO): o que é, OBI/InterIF, como ler enunciado, como a solução é avaliada; tudo sem código, fecha com atividade no papel.
- M02 Entrada, saída e problemas de cálculo (TRANCADO, sem código): formato de entrada/saída, restrições, resolução manual (Teleférico adaptado) e criação de casos de teste no papel.
- M03 Python e condicionais (TRANCADO): primeiro programa (com E/S, amarrando o M02), variáveis, comparações, if/else/elif, um problema de decisão de ponta a ponta.
- M04 Laços e repetição: while e for, repetição condicionada vs contada, percorrer sequências, problemas de acumulação/contagem (ex. OBI F1 de repetição simples).
- M05 Strings: texto como sequência, acesso/fatiamento, busca e contagem de caracteres, problemas OBI de manipulação de texto.
- M06 Vetores (listas): guardar coleções, índices, percorrer com laços, frequência/máximo/mínimo, problemas OBI de lista.
- M07 Matrizes (listas de listas): tabela como vetor de vetores, linhas×colunas, percorrer com laços aninhados, problemas OBI em grade.
- M08 Funções e consolidação: dividir o programa em funções com parâmetros, um problema OBI P1 F1 resolvido de ponta a ponta (ler→resolver→codar→testar) como capstone do básico.
