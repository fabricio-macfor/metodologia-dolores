# Exemplo 2: escola de idiomas em uma cidade nova

Dados fictícios. O objetivo já vem na mensagem, o material é um export de painel e o usuário pede também rotinas e divisão de orçamento.

## Entrada

**Usuário:**

Somos uma escola de idiomas com unidades em três cidades e abrimos duas unidades em uma cidade nova em agosto. Objetivo: chegar a 600 alunos matriculados nas unidades novas até junho de 2027; hoje são 140. Abaixo, o export do painel das unidades novas no trimestre de julho a setembro. Quero o diagnóstico, as rotinas de acompanhamento e a divisão do orçamento. A verba de marketing das unidades novas para o próximo trimestre é de R$ 180.000.

```text
metrica;valor
impressoes_anuncios;2.300.000
alcance_regiao;410.000
visualizacoes_video;380.000
seguidores_perfil_cidade;5.200
curtidas;18.900
sessoes_site_cidade;36.500
trafego_direto_cidade;2.100
share_of_voice_local;6%
tempo_medio_pagina;0:58
leads_aula_experimental;1.240
taxa_conversao_site;3,4%
custo_por_lead;R$ 38
comparecimento_aula_experimental;42%
matriculas;140
cac;R$ 610
avaliacoes_google;4,8 (96 avaliações)
matriculas_por_indicacao;12
rematricula_unidades_antigas;81%
```

## Saída da skill

---

## Diagnóstico Dolores

**Objetivo de negócio:** chegar a 600 alunos matriculados nas duas unidades novas até junho de 2027 (hoje, 140).
**Material analisado:** export do painel das unidades novas, julho a setembro, 18 métricas.

### Resumo

Das 18 métricas, 13 são relevantes e 5 são vaidade. O painel não está organizado por canal: mede a presença na cidade (tráfego direto, share of voice local) e o caminho até a matrícula (leads, comparecimento, matrículas). Proeminência e Valorização são os pilares mais fortes. O mais fraco é Fidelidade: a meta é de alunos matriculados, então cada cancelamento sai da conta, e o painel não mede retenção nas unidades novas; a única métrica do pilar é das unidades antigas. Faltam também a conversão de aula experimental em matrícula e o LTV para ler o CAC.

### Métricas por pilar

| Métrica | Pilar | C/N/A | Veredito | Ação |
|---|---|---|---|---|
| Impressões de anúncios (2,3 mi) | Proeminência | ✗/✗/✗ | Vaidade: impressões isoladas | Retirar; o alcance na região já cobre a visibilidade |
| Visualizações de vídeo (380 mil) | Proeminência | ✗/✗/✗ | Vaidade: visualizações sem engajamento qualitativo | Retirar do painel principal |
| Seguidores do perfil da cidade (5.200) | Proeminência* | ✗/✗/✗ | Vaidade: número bruto | Retirar do painel principal |
| Alcance na região (410 mil) | Proeminência | ✗/✓/✓ | Relevante | Manter como apoio de Proeminência |
| Sessões do site na cidade (36.500) | Proeminência | ✗/✗/✗ | Vaidade: total sem origem | Contextualizar: abrir por origem e ler junto com a taxa de conversão |
| Tráfego direto na cidade (2.100) | Proeminência | ✓/✓/✓ | Relevante | Manter no painel principal |
| Share of voice local (6%) | Proeminência | ✗/✓/✓ | Relevante | Manter no painel principal |
| Curtidas (18.900) | Valorização | ✗/✗/✗ | Vaidade: curtidas isoladas | Retirar; verificar se quem interage tem o perfil de quem se matricula |
| Tempo médio na página (0:58) | Valorização | ✓/✗/✗ | Relevante | Manter como apoio, fora do painel principal |
| Leads para aula experimental (1.240) | Valorização* | ✓/✓/✓ | Relevante | Manter no painel principal |
| Taxa de conversão do site (3,4%) | Valorização | ✓/✓/✓ | Relevante | Manter no painel principal |
| Comparecimento à aula experimental (42%) | Valorização* | ✓/✓/✓ | Relevante | Manter no painel principal |
| Rematrícula das unidades antigas (81%) | Fidelidade* | ✓/✗/✗ | Relevante | Mover para o painel das unidades antigas; está fora do escopo deste objetivo |
| Avaliações no Google (4,8; 96 avaliações) | Advocacia | ✓/✗/✓ | Relevante | Manter como apoio; facilitar e responder avaliações |
| Matrículas por indicação (12) | Advocacia | ✓/✓/✓ | Relevante | Manter no painel principal |
| Matrículas (140) | Negócio | ✓/✓/✓ | Relevante | Manter no painel principal; é a métrica do objetivo |
| CAC (R$ 610) | Negócio | ✗/✓/✓ | Relevante | Manter no painel principal e ler junto com o LTV, que falta |
| Custo por lead (R$ 38) | Operacional* | ✗/✗/✓ | Relevante | Manter na revisão semanal |

C: entende o cliente. N: conecta ao objetivo. A: é acionável. `*`: métrica que o livro não cita; pilar inferido pela pergunta-guia.

### Lacunas por pilar

| Pilar | Situação | O que falta (sugestão do livro) | Ligação com o objetivo |
|---|---|---|---|
| Proeminência | Coberto: tráfego direto, share of voice local e alcance | Engajamento orgânico | Direta: o livro liga mercado novo a tráfego direto e share of voice em canais locais |
| Valorização | Coberto: taxa de conversão, leads e comparecimento | Engajamento qualitativo; conversão de aula experimental em matrícula | Direta: é o caminho até a matrícula |
| Fidelidade | Descoberto: a única métrica do pilar é das unidades antigas | Taxa de retenção, tempo de retenção, NPS e LTV | Direta: a meta é de alunos matriculados, e quem cancela sai da conta |
| Advocacia | Coberto: avaliações e matrículas por indicação | Menções orgânicas | Direta: as matrículas por indicação somam à meta |

### Próximos passos

1. Montar o painel principal com até 10 métricas-chave: matrículas, taxa de retenção das unidades novas, tráfego direto na cidade, share of voice local, leads para aula experimental, comparecimento, conversão de aula experimental em matrícula, taxa de conversão do site, matrículas por indicação e CAC.
2. Medir a retenção desde já: cancelamentos e tempo de retenção dos alunos das unidades novas, mais NPS das primeiras turmas. O livro liga a redução do churn à taxa de retenção (Parte V, Cap. 1).
3. Medir a conversão de aula experimental em matrícula, para saber onde o caminho entre o comparecimento e a matrícula perde alunos.
4. Calcular o LTV com o financeiro e lê-lo junto com o CAC; o livro trata os dois como a medida da sustentabilidade financeira da estratégia (Parte II, Cap. 3).
5. Seguir o plano de Proeminência para mercados-alvo, com conteúdos de topo de funil que educam ou inspiram e parcerias com influenciadores alinhados aos valores da escola (Parte IV, Cap. 3), e tirar do painel principal as cinco métricas de vaidade, abrindo as sessões por origem.

### Rotinas de acompanhamento

Base: Parte IV, Cap. 4.

| Frequência | O que o livro manda olhar | Métricas deste painel |
|---|---|---|
| Diária | Métricas em tempo real: desempenho de campanhas pagas, tráfego ao site e interações em redes sociais | Alcance na região e custo por lead; sessões do site na cidade só como monitoramento de campanha |
| Semanal | Métricas intermediárias, como taxas de conversão, CTR e CAC; padrões e tendências para ajustes táticos | Taxa de conversão do site, leads, comparecimento, CAC |
| Mensal | Dados de todos os pilares em relatório completo, apresentado em reunião interdepartamental | Painel principal completo, com retenção (a criar), avaliações e matrículas por indicação, revisto com a equipe comercial e a coordenação das unidades |
| Trimestral | Revisão estratégica que conecta métricas ao impacto no negócio e redefine prioridades | Matrículas frente à meta de 600, share of voice local e divisão do orçamento |

A Parte II, Cap. 3 sugere outra cadência para algumas métricas: taxa de conversão e CTR diárias; CAC e tráfego qualificado semanais; retenção, LTV e ROI mensais. Em cada revisão, o livro pede três passos: identificar padrões, explorar causas e definir ações prioritárias (Parte V, Cap. 4).

### Divisão de orçamento

Base: Parte IV, Cap. 3, com a revisão do autor. Verba informada: R$ 180.000 no trimestre.

| Pilar | Parcela | Foco | Valor |
|---|---|---|---|
| Proeminência | 40% | campanhas de alcance | R$ 72.000 |
| Valorização | 25% | anúncios e conteúdos para engajamento | R$ 45.000 |
| Fidelidade | 20% | programas de retenção e relacionamento | R$ 36.000 |
| Advocacia | 15% | programas de embaixadores e engajamento | R$ 27.000 |

Para mercado novo, o livro orienta a definir os mercados prioritários onde a Proeminência é baixa (Parte IV, Cap. 3) e, quando falta visibilidade em mercados emergentes, a direcionar mais orçamento para campanhas regionais (Parte IV, Cap. 4), sem trazer outra tabela de percentuais.

Base: *O Abismo dos Dados*, de Fabricio Macias.
