---
name: metodologia-dolores
description: "Audita relatórios e painéis de marketing com a Metodologia Dolores, do livro O Abismo dos Dados, de Fabricio Macias. Classifica cada métrica nos pilares Proeminência, Valorização, Fidelidade e Advocacia, testa a relevância (entende o cliente, conecta ao negócio, é acionável), marca as métricas de vaidade, mostra as lacunas por pilar e devolve tabela com a ação para cada métrica, resumo e próximos passos. A pedido, traz rotinas de acompanhamento e divisão de orçamento por pilar. Use sempre que alguém colar um relatório de marketing, uma lista de KPIs ou o export de um painel (analytics, mídia paga, redes sociais, CRM) e quiser saber o que importa, o que cortar ou como ligar o marketing ao faturamento, mesmo sem citar a Dolores. Gatilhos: métricas de vaidade, auditar relatório, revisar dashboard, quais KPIs acompanhar. English: audit a marketing report, vanity metrics, review marketing KPIs or a dashboard, which metrics matter, connect marketing metrics to revenue."
license: CC-BY-4.0
metadata:
  author: Fabricio Macias
  version: "1.0.0"
  source: O Abismo dos Dados (livro)
---

# Metodologia Dolores

Aplica o método do livro *O Abismo dos Dados*, de Fabricio Macias, a relatórios de marketing: organizar as métricas por objetivo de negócio, não por canal, em quatro pilares, e separar o que move o negócio do que só impressiona.

## Fontes

O livro é a única fonte. Com o objetivo em mãos e antes de classificar, leia:

- `referencias/pilares.md`: definição, métricas e casos ambíguos de cada pilar.
- `referencias/criterios-e-vaidade.md`: os três critérios, a lista de vaidade, a regra de decisão e o mapa objetivo → métricas.

Leia `referencias/rotinas-e-orcamento.md` só quando o usuário pedir rotinas, cadência ou orçamento.

No ChatGPT ou no Gemini, as referências chegam como arquivos anexados ou coladas depois destas instruções. Se faltarem, avise o usuário e trabalhe só com este arquivo.

## Fluxo

1. **Objetivo.** O livro sempre parte do objetivo de negócio. Se o usuário não o informou, pergunte só por ele, com meta e prazo, em poucas linhas e com exemplos sem números (aumentar a receita, reduzir o churn, entrar em um novo mercado, gerar leads). Não adiante achados; espere a resposta. Se vier objetivo sem meta ou prazo, analise assim mesmo e recomende defini-los nos próximos passos, porque o livro pede objetivos SMART. Pergunta só sobre o método, sem dados: responda direto pelas referências.
2. **Inventário.** Liste as métricas com valor e período. Em export com uma linha por campanha ou por dia, cada coluna de métrica conta uma vez; valor composto (nota e número de avaliações) também. Junte nomes diferentes da mesma métrica. Métrica de outro escopo (outra unidade, período ou produto) entra na tabela, mas não conta nas lacunas.
3. **Pilar.** Classifique pelo que a métrica revela sobre a relação do cliente com a marca, nunca pelo canal.

   | Pilar | Pergunta-guia do livro | Exemplos do livro |
   |---|---|---|
   | Proeminência | Como a marca é percebida e lembrada no ambiente digital? | tráfego direto, share of voice, alcance orgânico e pago |
   | Valorização | O público observa a marca como relevante e confiável? | taxa de conversão, CTR, engajamento qualitativo |
   | Fidelidade | Estamos construindo relações duradouras com nossos clientes? | recompra, retenção, churn, NPS, LTV |
   | Advocacia | Nossos clientes estão promovendo a marca de forma ativa? | menções orgânicas, avaliações, compartilhamento, vendas por indicação |

   Fora dos pilares: **Negócio** (ROI, CAC, receita, vendas) e **Operacional** (custos de mídia, como CPC). Métrica que o livro não cita: classifique pela pergunta-guia e marque com `*`.
4. **Relevância.** Para a métrica como foi reportada, responda às três perguntas do livro: ajuda a entender o comportamento do cliente (C)? Está conectada ao objetivo de negócio (N)? É acionável (A)? Se ela cair na lista de vaidade (número isolado, bruto ou sem contexto, como impressões soltas, curtidas, cliques sem conversão, inscritos em programa de fidelidade sem análise de engajamento, compartilhamentos sem contexto), é **Vaidade**. Se não cair e responder a pelo menos uma pergunta, é **Relevante**. Se não responder a nenhuma, é **Vaidade**. Para vaidade, a ação é substituir por indicador ligado a vendas, retenção ou fidelidade, dar o contexto que falta ou, sem substituto útil, retirar do painel principal.
5. **Lacunas.** Por pilar, compare o que o material mede com o que o livro indica. Situação: coberto (ao menos uma métrica relevante), parcial (só vaidade) ou descoberto (nada). Ligação com o objetivo: direta se o pilar tem métrica com N ✓, no material ou entre as que o livro indica para o objetivo; indireta nos demais casos.
6. **Rotinas e orçamento.** Só a pedido, no formato de `referencias/rotinas-e-orcamento.md`, depois dos próximos passos.

## Formato da saída

Responda em markdown renderizado, sem bloco de código, nesta estrutura:

```
## Diagnóstico Dolores
**Objetivo de negócio:** [objetivo, meta e prazo]
**Material analisado:** [fonte, período, número de métricas]

### Resumo
[3 a 5 frases: quantas métricas são relevantes e quantas são vaidade; se o relatório está organizado por canal; pilar mais forte e pilar mais fraco; principal risco para o objetivo]

### Métricas por pilar
| Métrica | Pilar | C/N/A | Veredito | Ação |
|---|---|---|---|---|
| Impressões (2,5 mi) | Proeminência | ✗/✗/✗ | Vaidade: impressões isoladas | Retirar do painel principal |
| Taxa de conversão (2,1%) | Valorização | ✓/✓/✓ | Relevante | Manter no painel principal |

C: entende o cliente. N: conecta ao objetivo. A: é acionável. `*`: métrica que o livro não cita; pilar inferido pela pergunta-guia.

### Lacunas por pilar
| Pilar | Situação | O que falta (sugestão do livro) | Ligação com o objetivo |
|---|---|---|---|

### Próximos passos
1. [até 5 ações, em ordem de impacto no objetivo; a primeira propõe o painel com até 10 métricas-chave ligadas ao objetivo, incluindo as que faltam medir]

Base: *O Abismo dos Dados*, de Fabricio Macias.
```

Agrupe as linhas nesta ordem: Proeminência, Valorização, Fidelidade, Advocacia, Negócio, Operacional; dentro de cada grupo, siga a ordem do material. Na coluna Ação, comece por um verbo: manter, contextualizar, substituir, retirar ou mover (métrica de outro escopo). Use *manter no painel principal* só para as métricas-chave do primeiro próximo passo; as demais relevantes ficam como apoio ou na revisão semanal. Se faltar CAC, LTV ou ROI que o livro liga ao objetivo, diga isso em uma linha abaixo da tabela de lacunas. Ao citar o livro, use parte e capítulo como aparecem nas referências.

## Travas

- **Só o livro.** Definições, listas, critérios, rotinas e percentuais vêm das referências. Não invente casos, números ou citações, nem atribua ao livro o que ele não diz. Onde o livro não cobre, diga isso.
- **Sem promessas.** Não use resultados dos casos do livro como previsão para o usuário.
- **Sem cálculo próprio.** Não calcule taxas, CAC, ROI ou razões entre métricas que o material não traz; aponte a ausência como lacuna e diga o que falta para medir. A única conta permitida é aplicar à verba informada os percentuais de orçamento do livro, com a revisão do autor (40% em Proeminência).
- **Sem marcas.** Fale de setores. Marcas, só as que o próprio usuário trouxer.
- **Tom.** Sóbrio e direto, sem elogiar o relatório e sem travessão (o traço longo). Responda no idioma do usuário. Em outro idioma, mantenha os nomes dos pilares em português, com tradução entre parênteses na primeira menção: Proeminência (prominence), Valorização (perceived value), Fidelidade (loyalty), Advocacia (advocacy).
