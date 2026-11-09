# Roteiro da aula de dez minutos — exemplo das vans

Versão histórica do roteiro preparado antes da adoção do Teleférico. Para a sequência atual, consulte o [mapa do curso](../../curso/README.md).

## 0:00–1:00 — Abertura: o que é programação competitiva?

[NA TELA: título da aula. Depois, destacar três palavras: **interpretar → planejar → programar**.]

“Olá! Nesta primeira aula, vamos entender o que é programação competitiva e como começar a resolver um problema.

Na programação competitiva, recebemos desafios que precisam ser resolvidos por um programa. Cada problema apresenta uma situação, informa quais dados serão fornecidos e explica qual resposta precisamos produzir.

Nosso trabalho é interpretar essa descrição, pensar em uma estratégia e transformar essa estratégia em código. Depois, precisamos verificar se o programa funciona em diferentes situações.

Neste curso, vamos usar Python e trabalhar os fundamentos para resolver problemas de competições como a OBI e o InterIF.

Hoje, vamos começar pela interpretação. Ao final da aula, você deverá conseguir olhar para um enunciado e identificar três coisas: quais dados recebe, o que precisa descobrir e quais regras deve respeitar.”

## 1:00–2:30 — Apresentação do problema

[NA TELA: apresentar este **exemplo criado para a aula**, com uma ilustração simples de alunos e vans.]

> Uma escola precisa transportar seus alunos para um evento. Cada van pode levar, no máximo, uma determinada quantidade de alunos. Todos devem ser transportados em uma única viagem.
>
> Conhecendo a quantidade de alunos e a capacidade de cada van, determine o menor número de vans necessário.

“Vamos usar esse problema como exemplo.

Uma escola precisa levar seus alunos para um evento. Nós sabemos quantos alunos vão participar e quantos cabem em cada van. Precisamos descobrir a menor quantidade de vans suficiente para transportar todo mundo.

Imagine que sejam 23 alunos e que cada van comporte até 10 alunos.”

[LOUSA: escrever **23 alunos**, **10 alunos por van**. Desenhar três retângulos, representando as vans.]

“Na primeira van, podemos colocar 10 alunos. Na segunda, mais 10.

Já transportamos 20, mas ainda faltam três. Por isso, precisamos de uma terceira van, mesmo que ela não fique cheia.

Então, para esses dados, a resposta é três.

Perceba que já conseguimos resolver um caso sem escrever código. Esse é um bom começo: entender a situação e explicar o raciocínio com as nossas próprias palavras.

Depois, o programa deverá fazer isso para diferentes quantidades de alunos e capacidades.”

## 2:30–4:30 — Como ler um enunciado: entrada e saída

[NA TELA: destacar no enunciado, com cores diferentes, **dados fornecidos** e **resultado pedido**.]

“Podemos organizar a leitura de um problema em algumas perguntas.

A primeira é: quais informações eu recebo?

No nosso exemplo, recebemos dois números: a quantidade de alunos e a capacidade de cada van. Esses são os dados de entrada.

A segunda pergunta é: o que eu preciso descobrir?

Precisamos encontrar a menor quantidade de vans necessária. Esse será o resultado, ou seja, a saída.

A terceira pergunta é: quais regras essa resposta precisa respeitar?

Todo aluno precisa ser transportado. Nenhuma van pode ultrapassar sua capacidade. E precisamos usar a menor quantidade possível de vans.

Por exemplo, quatro vans conseguiriam transportar os 23 alunos. Mas a resposta pedida continua sendo três, porque três já são suficientes.”

[LOUSA: organizar uma versão curta.]

- **Entrada:** quantidade de alunos e capacidade.
- **Saída:** menor quantidade de vans.
- **Regras:** transportar todos, respeitar a capacidade e usar o mínimo necessário.

“Em problemas de programação, normalmente encontramos seções específicas explicando a entrada e a saída.

Para este exercício, vamos definir que a entrada contém dois números na mesma linha: primeiro a quantidade de alunos, depois a capacidade de cada van.”

[NA TELA: dois quadros lado a lado.]

| Entrada | Saída |
|---|---|
| `23 10` | `3` |

“O programa recebe 23 e 10 e deve produzir 3.

Essa ordem importa. Precisamos ler a especificação para saber o significado de cada valor e como apresentar a resposta.

Também precisamos seguir o formato solicitado. Se o problema pede somente um número, nossa saída deve apresentar esse número, sem acrescentar uma mensagem como ‘A resposta é três vans’.”

## 4:30–5:30 — Restrições: quais valores podem aparecer?

[NA TELA: acrescentar uma seção intitulada **Restrições deste exercício**.]

- Quantidade de alunos: de **1 a 1.000**.
- Capacidade de cada van: de **1 a 50** alunos.

“Além da entrada e da saída, precisamos observar as restrições.

Elas indicam quais valores podem aparecer nos testes. Para este exercício, vamos considerar entre um e mil alunos e uma capacidade entre um e cinquenta alunos por van.

Isso nos ajuda a entender quais situações o programa precisa tratar. Aqui, por exemplo, a capacidade sempre será positiva.

As restrições também ajudam a escolher uma estratégia que consiga terminar dentro dos limites de execução. Conforme avançarmos no curso, vamos estudar essa relação entre o tamanho da entrada e o trabalho realizado pelo programa.

Por enquanto, guarde esta ideia: as restrições fazem parte do problema e precisam entrar na nossa leitura.”

## 5:30–7:00 — Como o programa é avaliado?

[NA TELA: esquema simples: **entrada do teste → seu programa → resultado produzido**. Abaixo: **comparação com o resultado esperado**.]

“Depois de implementar uma solução, podemos enviá-la para um sistema de avaliação automática.

Esse sistema executa nosso programa com diferentes entradas e verifica os resultados produzidos. Ele também pode verificar condições como o tempo e a memória utilizados.

No nosso exemplo, um teste poderia fornecer 23 alunos e capacidade 10. O resultado esperado seria três.

Outro teste poderia fornecer 20 alunos e capacidade 10. Nesse caso, o resultado esperado seria dois.

Por isso, o programa precisa resolver a regra geral. Se ele simplesmente mostrar o número três em toda execução, vai acertar o primeiro exemplo e errar várias outras situações.

Os exemplos do enunciado ajudam a entender o funcionamento esperado, mas representam apenas alguns casos. O avaliador pode utilizar outros testes que você não vê antes da submissão.

Então, antes de enviar, precisamos testar nossa solução por conta própria: escolher entradas, calcular a resposta esperada e comparar com aquilo que o programa produz.

Esse hábito começa agora, mesmo antes de escrevermos o código.”

## 7:00–9:15 — Atividade: pensar em outros casos

[NA TELA: mostrar a tabela com as respostas das duas últimas linhas inicialmente escondidas.]

| Quantidade de alunos | Capacidade da van | Menor quantidade de vans |
|---:|---:|---:|
| 23 | 10 | 3 |
| 20 | 10 | ? |
| 3 | 10 | ? |

“Vamos verificar se entendemos a regra.

Já resolvemos o primeiro caso: 23 alunos, capacidade 10, três vans.

Agora pense no segundo: são 20 alunos, e cada van comporta até 10. Quantas vans precisamos?

E no terceiro: são apenas três alunos, com a mesma capacidade de 10. Qual seria a resposta?

Pause o vídeo e tente justificar as duas respostas. Você pode desenhar as vans ou distribuir os alunos em grupos.”

[FAZER UMA PAUSA BREVE. Depois, revelar as respostas enquanto explica.]

“Para 20 alunos, precisamos de duas vans. São 10 na primeira e 10 na segunda. Todos foram transportados, então podemos parar.

Para três alunos, precisamos de uma van. Ela ficará com lugares vazios, mas todos cabem nela.

Esses casos ajudam a perceber detalhes importantes da regra.

Quando os alunos preenchem exatamente as vans, como no caso de 20 alunos, não precisamos acrescentar outra.

Quando a quantidade de alunos é menor que a capacidade, como no caso de três alunos, ainda precisamos de uma van.

E quando sobra alguém depois de preencher algumas vans, como no caso de 23 alunos, precisamos de mais uma para transportar quem ficou.”

[LOUSA: apontar os três casos e escrever ao lado: **sobra**, **encaixe exato**, **uma van basta**.]

“Agora conseguimos descrever uma estratégia: organizar os alunos em grupos que respeitem a capacidade, contando quantas vans são necessárias até acomodar todos.

Essa descrição de passos já é um começo de algoritmo.

Mais adiante, vamos traduzir esse raciocínio para Python e discutir como calcular a resposta. Antes disso, precisamos ter certeza de que compreendemos a regra que o código deverá executar.”

## 9:15–10:00 — Encerramento

[NA TELA: checklist final.]

- O que recebo?
- O que preciso produzir?
- Quais regras e restrições existem?
- Que casos posso testar?

“Hoje, vimos que resolver um problema começa pela leitura.

Identificamos os dados de entrada, o resultado esperado, as regras e as restrições. Também usamos exemplos diferentes para conferir nosso raciocínio e entendemos como uma solução pode ser avaliada automaticamente.

Nos próximos problemas, use estas quatro perguntas como ponto de partida: o que recebo, o que preciso produzir, quais regras existem e quais casos posso testar?

Na próxima aula, vamos revisar os recursos de Python que usaremos para transformar esse planejamento em programas.”
