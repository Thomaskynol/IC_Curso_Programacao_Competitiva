# Task Plan: IC — Mapa de 8 módulos + aulas dos 3 primeiros + wiki

## Goal

Entregar o mapa dos 8 módulos do curso básico (descrições breves), o mapa de aulas dos 3 primeiros módulos (título + duração + resumo) e uma wiki nova da IC, tudo fundamentado em estudo pedagógico.

## Next Step

Criar a wiki nova da IC (Phase 3) após aprovação do mapa de aulas.

## Current Phase

Phase 2 — Estudo pedagógico

## Phases

### Phase 1: Entrevista / Requisitos (brainstorming)

- [x] Perguntar o que está implícito/faltando (público, escopo, limites básico vs avançado, formato, avaliação, wiki)
- [x] Registrar respostas em findings.md
- [x] Fechar escopo antes de qualquer produção
- **Status:** complete

### Phase 2: Estudo pedagógico

- [x] Estudar fundamentação (ordem de ensino de programação competitiva para iniciantes, MOOC/microlearning, OBI/InterIF como referência)
- [x] Registrar síntese + justificativa da sequência em findings.md (com fontes quando houver)
- [x] Definir critérios de ordenação dos 8 módulos
- **Status:** complete

### Phase 3: Wiki nova da IC (llm-wiki)

- [ ] Criar estrutura em /opt/data/wikis/ic-programacao-competitiva (SCHEMA.md, index.md, log.md) SEM alterar WIKI_PATH global
- [ ] Ingerir conteúdo do Git + instruções da entrevista como raw/
- [ ] Criar/atualizar páginas, index e log
- **Status:** pending (depois da aprovação dos módulos — a wiki registra decisões aprovadas)

### Phase 4: Mapa dos 8 módulos

- [x] Propor 8 módulos (1–3 preservados/revisados + 5 novos) com descrição breve cada
- [x] Justificar sequência a partir do estudo da Fase 2
- [ ] Entregar como proposta em chat + arquivo para revisão (sem commit sem pedido, cf. AGENTS.md)
- **Status:** in_progress (proposta pronta, aguardando aprovação do usuário)

### Phase 5: Mapa de aulas dos 3 primeiros módulos

- [x] Para cada aula: título, duração estimada, resumo breve
- [x] Respeitar formato microaula 1–3 min, pré-requisitos explícitos
- [ ] Entregar para revisão
- **Status:** in_progress (proposta salva em docs/producao/mapa-aulas-m01-m03.md, aguardando aprovação)

### Phase 6: Entrega e revisão

- [ ] Revisar coerência módulos ↔ aulas ↔ pendências da reunião 07/11
- [ ] Listar decisões/pendências para o orientador
- [ ] Aguardar aprovação antes da aula aprofundada do M01-A01 (fora deste escopo)
- **Status:** pending

### Phase 7: Roteiro da M01-A01 (novo pedido do usuário, 09/11)

- [x] Escrever script completo (fala, cenas, tempos, apoio visual, áudio/edição)
- [x] Seguir ficha do modelo-microaula.md
- [x] Entregar para revisão (sem gravar nada, só roteiro)
- **Status:** complete (aprovado pelo usuário; commit + push autorizados)

## Key Questions

1. Quem é o aluno do curso básico? (idade, vínculo IFSP, experiência prévia com programação?)
2. O que delimita básico vs avançado? (até onde vai o básico — ex: quais estruturas/algoritmos ficam de fora?)
3. Os 3 primeiros módulos estão trancados ou podem ser revisados pelo estudo pedagógico?
4. Formato das microaulas vale para os 8 módulos? (1–3 min, 1 objetivo por vídeo, pré-requisitos)
5. Como o aluno será avaliado? (só exercícios OBI/InterIF, quizzes, projeto?)
6. Wiki nova: onde mora, em que língua, só você + orientador ou pública?
7. Há prazo ou ordem de entrega? (os 8 módulos de uma vez ou por partes?)

## Decisions Made

| Decision | Rationale |
|----------|-----------|
| Planejamento em arquivos na raiz do repo clonado (/opt/data/IC_Curso_Programacao_Competitiva) | Trabalho multi-fase, precisa sobreviver entre sessões |
| Wiki nova em /opt/data/wikis/ic-programacao-competitiva, sem tocar no WIKI_PATH global | WIKI_PATH é global/snapshotted; outra sessão pode estar viva |
| Pesquisa do estudo pedagógico SOMENTE via web_extract (nada de agent-reach, deep research ou similares) | Determinação do usuário em 09/11/2026 |
| Nada de commit/push sem pedido | Regra do AGENTS.md do repo |

## Errors Encountered

| Error | Attempt | Resolution |
|-------|---------|------------|
|       |         |            |

## Notes

- Using superpowers:brainstorming para a entrevista; superpowers:writing-plans antes do plano de execução detalhado, se virar projeto com design escrito.
- Aula aprofundada do M01-A01 fica para depois, fora deste escopo.
