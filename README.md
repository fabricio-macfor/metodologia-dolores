# Metodologia Dolores

Skill de IA que audita relatórios de marketing com a Metodologia Dolores, apresentada no livro *O Abismo dos Dados*, de Fabricio Macias. Funciona no Claude Code e também como instrução no ChatGPT e no Gemini.

> "Os CMOs não devem se contentar com relatórios cheios de números, mas vazios de significado."
> *O Abismo dos Dados*, Parte VI

## O que é

O livro parte de um diagnóstico: o marketing digital mede quase tudo, mas costuma organizar os números por canal e celebrar métricas que impressionam sem mover o negócio. A Metodologia Dolores reorganiza as métricas por objetivo, em quatro pilares, e separa o que é relevante do que é vaidade.

Esta skill aplica o método ao material que você colar: um relatório, uma lista de KPIs ou o export de um painel.

## O que a skill entrega

1. Pergunta o objetivo de negócio, se ele não vier no pedido.
2. Classifica cada métrica em um dos quatro pilares ou, quando ela não pertence a nenhum, como métrica de negócio ou operacional.
3. Testa cada métrica com os três critérios de relevância do livro (entende o cliente? conecta ao negócio? é acionável?) e marca as de vaidade.
4. Mostra as lacunas de cada pilar.
5. Devolve uma tabela métrica, pilar, veredito e ação, com resumo e próximos passos.
6. A pedido, traz as rotinas diária, semanal, mensal e trimestral e a divisão de orçamento por pilar sugeridas no livro.

## Os quatro pilares

| Pilar | Pergunta-guia do livro |
|---|---|
| Proeminência | Como a marca é percebida e lembrada no ambiente digital? |
| Valorização | O público observa a marca como relevante e confiável? |
| Fidelidade | Estamos construindo relações duradouras com nossos clientes? |
| Advocacia | Nossos clientes estão promovendo a marca de forma ativa? |

## Instalação no Claude Code

A pasta da skill precisa ficar em `~/.claude/skills/metodologia-dolores/`, com o `SKILL.md` na raiz.

```bash
git clone https://github.com/fabricio-macfor/metodologia-dolores.git ~/.claude/skills/metodologia-dolores
```

Sem git, baixe o ZIP do repositório, extraia e renomeie a pasta para `metodologia-dolores` dentro de `~/.claude/skills/`. Para usar em um único projeto, coloque a pasta em `.claude/skills/metodologia-dolores/` na raiz do projeto.

Uso: cole o relatório e peça a análise. A skill entra sozinha quando o pedido envolve métricas de marketing. Para chamá-la diretamente, digite `/metodologia-dolores`.

## Uso no ChatGPT e no Gemini

- **ChatGPT:** crie um GPT personalizado. Cole o conteúdo de `SKILL.md` nas instruções e envie os três arquivos de `referencias/` como arquivos de conhecimento. Num Projeto, use as instruções e os arquivos do projeto da mesma forma.
- **Gemini:** crie um Gem. Cole o conteúdo de `SKILL.md` nas instruções e adicione os três arquivos de `referencias/` como conhecimento. Se a extensão `.md` não for aceita, salve os arquivos como `.txt`.
- **Em qualquer conversa:** cole `SKILL.md` e, em seguida, o conteúdo dos três arquivos de `referencias/`. Depois, envie o relatório.

O cabeçalho do `SKILL.md` (entre as linhas `---`) pode ser colado junto; ele não atrapalha.

## Exemplo

Trecho do [exemplo 1](exemplos/01-loja-online-cosmeticos.md), com dados fictícios. O usuário cola o relatório mensal de uma loja online, organizado por canal, e informa o objetivo quando a skill pergunta: aumentar a receita em 20% até março, principalmente com clientes que já compraram.

| Métrica | Pilar | C/N/A | Veredito | Ação |
|---|---|---|---|---|
| Impressões (3,4 mi) | Proeminência | ✗/✗/✗ | Vaidade: impressões isoladas | Retirar; o alcance já cobre a visibilidade |
| Tráfego direto (14.900) | Proeminência | ✓/✗/✓ | Relevante | Manter como apoio de Proeminência |
| Taxa de conversão do e-commerce (1,4%) | Valorização | ✓/✓/✓ | Relevante | Manter no painel principal; abrir por campanha e por cliente novo ou recorrente |
| Assinantes da newsletter (22.400) | Fidelidade | ✗/✗/✗ | Vaidade: base sem análise de engajamento | Substituir pela frequência de interação e de compra de quem recebe a newsletter |

C: entende o cliente. N: conecta ao objetivo. A: é acionável.

Na mesma saída, a skill aponta que Fidelidade, o pilar que sustenta a meta, não tem nenhuma métrica relevante e recomenda medir recompra, LTV e CAC. O [exemplo 2](exemplos/02-escola-de-idiomas-nova-cidade.md) traz uma escola de idiomas que abre unidades em uma cidade nova, com rotinas e divisão de orçamento.

## Estrutura

- `SKILL.md`: fluxo, formato de saída e travas.
- `referencias/pilares.md`: os quatro pilares, como medir cada um e os casos ambíguos.
- `referencias/criterios-e-vaidade.md`: critérios de relevância, lista de vaidade e mapa objetivo → métricas.
- `referencias/rotinas-e-orcamento.md`: rotinas de acompanhamento e divisão de orçamento.
- `exemplos/`: dois casos com entrada e saída.

## Fidelidade ao livro

O que a skill afirma sobre o método vem do livro, com parte, capítulo e página indicados nas referências. Onde o livro não trata de um ponto, a skill diz isso, e as métricas que o livro não cita aparecem marcadas com asterisco. As regras de aplicação que não são texto do livro estão identificadas como "Procedimento da skill". A skill aplica a metodologia; ela não é a ferramenta Dolores mencionada no livro.

## Crédito

A Metodologia Dolores é apresentada no livro *O Abismo dos Dados*, de Fabricio Macias.

- Livro na Amazon: https://www.amazon.com.br/dp/8587962361
- Autor: https://fabriciomacias.com.br

## Licença

Os arquivos deste repositório estão sob a licença [CC BY 4.0](LICENSE). É permitido copiar, adaptar e redistribuir, inclusive para uso comercial, desde que se dê crédito ao autor, com link para a licença, e se indiquem as alterações feitas. Os trechos do livro citados em `referencias/` continuam protegidos pelos direitos autorais da obra e aparecem aqui como citação, com indicação de autor e origem.

## English

**Metodologia Dolores** is an AI skill that audits marketing reports using the Dolores Methodology, presented in the Brazilian book *O Abismo dos Dados* by Fabricio Macias.

- **What it does:** asks for the business objective when it is missing; sorts each metric into four pillars (Proeminência, prominence; Valorização, perceived value; Fidelidade, loyalty; Advocacia, advocacy); tests relevance with the book's three questions (does it explain customer behavior, does it connect to the business objective, is it actionable); flags vanity metrics; shows gaps per pillar; and returns a table with an action for each metric, a summary and next steps. On request, it adds the review routines and the budget split per pillar suggested in the book.
- **Claude Code:** clone or copy this repository to `~/.claude/skills/metodologia-dolores/` and paste a report, or type `/metodologia-dolores`.
- **ChatGPT and Gemini:** paste `SKILL.md` into the instructions of a custom GPT or a Gem and upload the three files in `referencias/` as knowledge.
- **Language:** the skill answers in the user's language and keeps the pillar names in Portuguese, with an English gloss on first mention.
- **Credit:** book on Amazon, https://www.amazon.com.br/dp/8587962361; author, https://fabriciomacias.com.br.
- **License:** CC BY 4.0 for the files in this repository. Quotes from the book remain under the book's copyright.
