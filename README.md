# IC de Programação Competitiva

![Status](https://img.shields.io/badge/status-em_desenvolvimento-yellow)
![Python](https://img.shields.io/badge/python-3-blue)
![Formato](https://img.shields.io/badge/formato-MOOC_microaulas-green)

Projeto de iniciação científica no **IFSP — Campus Araraquara**, com orientação do **Prof. Nunes**.
O objetivo é produzir um **curso básico introdutório de programação competitiva em Python**,
tendo a **OBI** e o **InterIF** como referências de exercícios e avaliação.

O curso segue o formato **MOOC** e é organizado em **módulos de microaulas**:
cada vídeo trata de **um único objetivo** e dura em média **1 a 3 minutos**
(uma resolução mais longa pode extrapolar). Cada microaula declara seus
**pré-requisitos**, de modo que quem já sabe um tópico pode saltá-lo.

## O curso em 8 módulos

| # | Módulo | Resumo | Estado |
|---|---|---|---|
| M01 | Introdução à programação competitiva | O que é, benefícios, OBI/InterIF, linguagens, eficiência, leitura de enunciados e avaliação — tudo sem código | Roteiros em produção |
| M02 | Entrada, saída e problemas de cálculo | Formato de E/S, restrições, Python mínimo e o Teleférico resolvido no papel e no código | Roteiros em produção |
| M03 | Python e condicionais | Primeiro programa, variáveis, comparações, booleanos, if/else/elif e um problema de decisão completo | Roteiros em produção |
| M04 | Laços e repetição | `while`/`for`, acumulação e contagem em problemas OBI | Mapa pronto |
| M05 | Strings | Texto como sequência, busca e contagem em problemas OBI | Mapa pronto |
| M06 | Vetores (listas) | Coleções, índices, frequência e extremos em problemas OBI | Mapa pronto |
| M07 | Matrizes (listas de listas) | Linhas, colunas e laços aninhados em problemas OBI em grade | Mapa pronto |
| M08 | Funções e consolidação | Funções com parâmetros e um problema OBI resolvido de ponta a ponta como capstone | Mapa pronto |

O mapa completo está em [curso/README.md](curso/README.md), com o detalhamento
das 22 aulas dos três primeiros módulos.

## Onde encontrar cada coisa

| Material | Onde está |
|---|---|
| Mapa dos módulos e aulas | [curso/README.md](curso/README.md) |
| Exercício do módulo 2 | [Teleférico adaptado](curso/modulo-02-entrada-e-saida/teleferico.md) |
| Modelo para preparar uma aula | [Ficha de microaula](docs/modelo-microaula.md) |
| Mapa de aulas M01–M03 (título, duração, resumo) | [docs/producao/mapa-aulas-m01-m03.md](docs/producao/mapa-aulas-m01-m03.md) |
| Roteiro da aula M01-A01 | [docs/producao/roteiro-m01-a01.md](docs/producao/roteiro-m01-a01.md) |
| Storyboard do Teleférico | [docs/producao/animacao-teleferico.md](docs/producao/animacao-teleferico.md) |
| Decisões da reunião de 07/11/2026 | [docs/reunioes/2026-11-07.md](docs/reunioes/2026-11-07.md) |
| Estudo pedagógico e decisões | [findings.md](findings.md) |
| Andamento do trabalho | [progress.md](progress.md) · [task_plan.md](task_plan.md) |
| Materiais anteriores (histórico) | [docs/historico/](docs/historico/README.md) |

## Estrutura do repositório

```text
├── curso/                  # conteúdo do curso (mapa + exercícios por módulo)
├── docs/
│   ├── modelo-microaula.md # ficha padrão para preparar uma aula
│   ├── producao/           # mapas de aulas, roteiros e storyboards
│   ├── reunioes/           # registros de reunião e decisões
│   └── historico/          # materiais anteriores, preservados como referência
├── AGENTS.md               # orientações para quem trabalha neste repo
├── findings.md             # estudo pedagógico, entrevistas e decisões
├── progress.md             # diário de andamento
└── task_plan.md            # plano de trabalho por fases
```

## Contribuindo

Leia o [AGENTS.md](AGENTS.md) antes de alterar a estrutura do curso, e o registro
de reunião mais recente mais o [mapa do curso](curso/README.md) antes de mexer
nos módulos. Mudanças em remoto, commits e publicação dependem do pedido do
responsável pela tarefa. Materiais históricos são preservados; adaptações de
exercícios identificam a fonte original.
