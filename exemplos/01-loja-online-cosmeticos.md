# Exemplo 1: loja online de cosméticos

Dados fictícios. O exemplo mostra a pergunta do objetivo, quando ele falta, e um relatório organizado por canal, com muitas métricas de vaidade.

## Entrada

**Usuário:**

Segue o relatório de outubro da nossa loja online de cosméticos. Pode avaliar?

```text
Redes sociais
- Seguidores no Instagram: 48.300 (+2.100 no mês)
- Curtidas: 96.500
- Comentários: 3.140
- Compartilhamentos: 1.870
- Visualizações de Reels: 1,2 milhão

Mídia paga
- Impressões: 3,4 milhões
- Alcance: 920 mil
- Cliques: 41.200
- CTR: 1,2%
- CPC: R$ 0,85
- ROAS: 3,1

Site
- Sessões: 186.000
- Tráfego direto: 14.900 sessões
- Tempo médio na página: 1min42s
- Taxa de conversão do e-commerce: 1,4%
- Pedidos: 2.604
- Receita: R$ 312.480

E-mail
- Assinantes da newsletter: 22.400

Avaliações
- Nota média no site: 4,6 de 5 (212 avaliações no mês)
```

## Pergunta da skill

Antes de classificar, preciso do objetivo de negócio que este relatório deveria mover. A Metodologia Dolores julga cada métrica pela ligação com esse objetivo. Qual é o principal agora: aumentar a receita, aumentar a recompra, atrair novos clientes ou outro? Se houver meta e prazo, informe também.

## Resposta do usuário

Aumentar a receita do e-commerce em 20% até março de 2027, principalmente com clientes que já compraram.

## Saída da skill

---

## Diagnóstico Dolores

**Objetivo de negócio:** aumentar a receita do e-commerce em 20% até março de 2027, principalmente com clientes que já compraram.
**Material analisado:** relatório de outubro (redes sociais, mídia paga, site, e-mail e avaliações), 19 métricas.

### Resumo

Das 19 métricas, 10 são relevantes e 9 são vaidade. O relatório está organizado por canal, o formato que o livro chama de falácia dos silos, e por isso soma alcance, cliques e curtidas sem mostrar o que move a receita. Valorização é o pilar mais bem medido, com taxa de conversão e CTR; Fidelidade, que sustenta a meta de vender mais para quem já comprou, tem só uma métrica, e ela é de vaidade. Sem recompra, retenção, LTV e CAC, não há como saber se a receita de clientes recorrentes está crescendo.

### Métricas por pilar

| Métrica | Pilar | C/N/A | Veredito | Ação |
|---|---|---|---|---|
| Seguidores no Instagram (48.300) | Proeminência* | ✗/✗/✗ | Vaidade: número bruto | Retirar do painel principal |
| Visualizações de Reels (1,2 mi) | Proeminência | ✗/✗/✗ | Vaidade: visualizações sem engajamento qualitativo | Retirar do painel principal |
| Impressões (3,4 mi) | Proeminência | ✗/✗/✗ | Vaidade: impressões isoladas | Retirar; o alcance já cobre a visibilidade |
| Alcance (920 mil) | Proeminência | ✗/✗/✓ | Relevante | Manter como apoio de Proeminência |
| Sessões (186.000) | Proeminência | ✗/✗/✗ | Vaidade: total sem origem | Contextualizar: abrir por origem e ler junto com a conversão |
| Tráfego direto (14.900) | Proeminência | ✓/✗/✓ | Relevante | Manter como apoio de Proeminência |
| Curtidas (96.500) | Valorização | ✗/✗/✗ | Vaidade: curtidas isoladas | Retirar; verificar se quem interage tem o perfil de quem compra |
| Comentários (3.140) | Valorização | ✗/✗/✗ | Vaidade: contagem sem leitura do conteúdo | Contextualizar: classificar o conteúdo (dúvidas, intenção de compra, reclamações) |
| Cliques (41.200) | Valorização | ✗/✗/✗ | Vaidade: cliques sem ligação com conversão | Substituir pela taxa de conversão das campanhas |
| CTR (1,2%) | Valorização | ✓/✗/✓ | Relevante | Manter como apoio, sempre lido junto com a conversão |
| Tempo médio na página (1min42s) | Valorização | ✓/✗/✗ | Relevante | Manter como apoio, fora do painel principal |
| Taxa de conversão do e-commerce (1,4%) | Valorização | ✓/✓/✓ | Relevante | Manter no painel principal; abrir por campanha e por cliente novo ou recorrente |
| Assinantes da newsletter (22.400) | Fidelidade | ✗/✗/✗ | Vaidade: base sem análise de engajamento | Substituir pela frequência de interação e de compra de quem recebe a newsletter |
| Compartilhamentos (1.870) | Advocacia | ✗/✗/✗ | Vaidade: número bruto, sem contexto | Contextualizar: taxa de compartilhamento e o que é compartilhado |
| Nota média no site (4,6; 212 avaliações) | Advocacia | ✓/✗/✓ | Relevante | Manter como apoio; responder às avaliações e ler as negativas como pontos de frustração |
| ROAS (3,1) | Negócio* | ✗/✓/✓ | Relevante | Manter no painel principal e complementar com CAC e LTV |
| Pedidos (2.604) | Negócio | ✓/✓/✓ | Relevante | Manter no painel principal; separar clientes novos e recorrentes |
| Receita (R$ 312.480) | Negócio | ✗/✓/✓ | Relevante | Manter no painel principal; separar a receita de clientes recorrentes |
| CPC (R$ 0,85) | Operacional | ✗/✗/✓ | Relevante | Manter na revisão semanal, fora do painel principal |

C: entende o cliente. N: conecta ao objetivo. A: é acionável. `*`: métrica que o livro não cita; pilar inferido pela pergunta-guia.

### Lacunas por pilar

| Pilar | Situação | O que falta (sugestão do livro) | Ligação com o objetivo |
|---|---|---|---|
| Proeminência | Coberto: tráfego direto e alcance | Share of voice | Indireta |
| Valorização | Coberto: taxa de conversão e CTR | Engajamento qualitativo; taxa de conversão por campanha | Direta: a conversão gera os pedidos |
| Fidelidade | Parcial: só uma métrica, de vaidade | Taxa de recompra, frequência de compra, taxa de retenção, LTV e NPS | Direta: a meta depende de quem já comprou |
| Advocacia | Coberto: avaliações | Menções orgânicas, taxa de compartilhamento e vendas por indicação | Indireta |

Fora dos pilares, falta o CAC, que o livro associa ao aumento de receita junto com o LTV (Parte V, Cap. 1).

### Próximos passos

1. Reorganizar o relatório por pilar, não por canal, com um painel principal de até 10 métricas-chave ligadas ao objetivo: receita e pedidos, separados entre clientes novos e recorrentes, taxa de conversão, ROAS, taxa de recompra, frequência de compra, taxa de retenção, LTV e CAC. Tráfego direto, alcance, CTR e avaliações ficam como apoio no relatório mensal.
2. Passar a medir Fidelidade: ligar cada pedido ao histórico do cliente para obter recompra, frequência de compra e LTV. O livro pede unificar dados de vendas, marketing e CRM em um único sistema (Parte I, Cap. 4).
3. Medir o CAC e lê-lo junto com o LTV, o par que o livro associa ao aumento de receita (Parte V, Cap. 1).
4. Aplicar aos clientes atuais o plano de Fidelidade do livro: comunicação pós-compra, programa que recompense compras recorrentes e monitoramento de sinais de desengajamento, como a falta de compras recentes (Parte IV, Cap. 3).
5. Tirar as nove métricas de vaidade do painel principal ou dar a elas o contexto que falta: conteúdo dos comentários, taxa de compartilhamento e comparação entre o perfil de quem interage e o de quem compra (Parte II, Cap. 3).

Base: *O Abismo dos Dados*, de Fabricio Macias.
