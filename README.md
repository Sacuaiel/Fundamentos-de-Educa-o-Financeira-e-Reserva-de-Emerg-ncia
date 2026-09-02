# 📘 Miniguia de Estudo — Fundamentos de Educação Financeira e Reserva de Emergência

Caderno temático criado no **NotebookLM**, reunindo fontes abertas sobre finanças pessoais introdutórias, com curadoria de fontes, engenharia de prompts e um miniguia final estruturado.

---

## 1. Contexto e Objetivos

**Tema escolhido:** Fundamentos de Educação Financeira e Reserva de Emergência.

Escolhi esse assunto por ser a base de qualquer decisão financeira mais avançada (investimentos, crédito, planejamento de longo prazo) e por existir farta documentação pública e confiável (bancos centrais, órgãos reguladores e instituições de pesquisa) que permite montar um caderno temático sólido no NotebookLM.

**Objetivos de estudo:**
- Entender os conceitos centrais de organização financeira pessoal (orçamento, reserva de emergência, endividamento).
- Compreender por que e como construir uma reserva de emergência (valor ideal, tipo de aplicação, liquidez).
- Criar um vocabulário técnico mínimo (glossário) para ler com autonomia outros materiais sobre finanças.
- Desenvolver prompts reutilizáveis que ajudem a revisar o tema no futuro ou aplicá-lo a outros assuntos financeiros.

---

## 2. Curadoria de Fontes

Fontes abertas (texto/PDF) selecionadas e carregadas no NotebookLM:

| # | Fonte | Tipo | Link |
|---|-------|------|------|
| 1 | Banco Central do Brasil — Caderno de Educação Financeira | PDF | https://www.bcb.gov.br/content/cidadaniafinanceira/documentos_cidadania/Cad_Cidadania_Financeira/caderno_cidadania_financeira.pdf |
| 2 | CVM — Portal do Investidor: Planejamento Financeiro | Página/PDF | https://www.investidor.gov.br/publicacao/Livro/planejamento_financeiro.html |
| 3 | Banco Central do Brasil — Série Cidadania Financeira (Estudos) | PDF | https://www.bcb.gov.br/acessoinformacao/cidadaniafinanceira |
| 4 | Serasa/SPC ou similar — Guia de Reserva de Emergência (artigo aberto) | Texto | *(inserir link do artigo escolhido)* |
| 5 | Fundação Getulio Vargas (FGV) — material aberto sobre finanças pessoais | PDF | *(inserir link do material escolhido)* |

> ⚠️ Ao montar o seu repositório de verdade, confirme os links (alguns portais reorganizam URLs periodicamente) e substitua os itens 4 e 5 pelas fontes que você efetivamente carregou no NotebookLM.

---

## 3. Engenharia de Prompts e "Cicatrizes"

Documentação do processo de perguntas e testes de prompt feitos dentro do NotebookLM.

### 3.1 Perguntas estratégicas elaboradas
1. "Quais são os elementos essenciais de um orçamento pessoal segundo as fontes carregadas?"
2. "Qual o valor recomendado de reserva de emergência e por quê varia entre os documentos?"
3. "Quais riscos as fontes apontam para quem não tem reserva de emergência?"
4. "Resuma, em linguagem simples, a diferença entre reserva de emergência e investimento de longo prazo."
5. "Gere um glossário com os 10 termos técnicos mais citados nas fontes."

### 3.2 Variações de prompt testadas

| Prompt testado | Resultado obtido | Referência (fonte) | Observações / troubleshooting |
|---|---|---|---|
| "Explique reserva de emergência." | Resposta genérica, sem citar fontes específicas | — | Prompt curto demais; a IA não ancorou a resposta nos documentos carregados. |
| "Com base apenas nas fontes carregadas, explique o que é reserva de emergência e cite a fonte de cada afirmação." | Resposta específica, com citações por documento | Fonte 1 e 2 | Pedir explicitamente "com base apenas nas fontes" e "cite a fonte" melhora muito a rastreabilidade. |
| "Crie um glossário de 10 termos financeiros presentes nos documentos, com definição de uma linha cada." | Glossário bem estruturado, mas com 2 termos repetidos | Fonte 1, 3 | Precisei pedir revisão para remover duplicatas — bom aprendizado sobre revisar saída antes de aceitar. |
| "Compare as recomendações de valor de reserva de emergência entre as fontes 1 e 2." | Resposta comparativa clara, apontando divergência de meses recomendados | Fonte 1 e 2 | Prompt comparativo funcionou melhor que perguntas isoladas para identificar divergências entre fontes. |

**Dificuldades encontradas (troubleshooting):**
- Perguntas muito abertas geravam respostas genéricas, sem referência às fontes carregadas — resolvido pedindo explicitamente citação de fonte.
- Respostas longas às vezes misturavam informação de fontes diferentes sem deixar claro qual vinha de onde — resolvido pedindo resposta em formato de tabela com coluna "fonte".
- Glossários gerados automaticamente às vezes traziam termos repetidos ou fora do escopo — resolvido com um prompt de revisão/filtragem após a primeira geração.

---

## 4. Miniguia de Estudo (Entrega Final)

### 4.1 Resumo estruturado

**O que é organização financeira pessoal**
Conjunto de práticas para planejar entradas e saídas de dinheiro, priorizando gastos essenciais, evitando endividamento não planejado e destinando parte da renda para reserva e investimentos.

**Reserva de emergência**
Valor guardado em aplicação de alta liquidez (fácil resgate), destinado a cobrir despesas em situações imprevistas (perda de renda, emergências médicas, reparos urgentes), evitando a necessidade de recorrer a dívidas caras.

**Por que ter uma reserva**
- Reduz a dependência de crédito emergencial (cartão, cheque especial), que costuma ter juros altos.
- Dá previsibilidade e segurança para decisões de médio/longo prazo (trocar de emprego, investir).
- Funciona como base antes de partir para investimentos de maior risco.

**Como dimensionar e onde guardar**
- O valor costuma ser calculado em meses de despesas essenciais (o número exato varia entre fontes, geralmente de 3 a 12 meses).
- Deve ficar em aplicações de alta liquidez e baixo risco (ex: fundos DI, Tesouro Selic, poupança), priorizando acesso rápido sobre rentabilidade.

### 4.2 Glossário de conceitos

| Termo | Definição |
|---|---|
| **Orçamento pessoal** | Planejamento das receitas e despesas de um indivíduo ou família em um período. |
| **Reserva de emergência** | Valor guardado com alta liquidez para cobrir imprevistos financeiros. |
| **Liquidez** | Facilidade e velocidade com que um ativo pode ser convertido em dinheiro sem perda relevante de valor. |
| **Endividamento** | Situação em que uma pessoa possui dívidas, especialmente quando comprometem parte relevante da renda. |
| **Juros compostos** | Juros calculados sobre o valor inicial mais os juros já acumulados em períodos anteriores. |
| **Renda fixa** | Categoria de investimento cuja remuneração segue regras definidas no momento da aplicação. |
| **Tesouro Selic** | Título público de renda fixa atrelado à taxa Selic, com alta liquidez. |
| **Educação financeira** | Processo de desenvolvimento de conhecimentos e atitudes para uma gestão financeira consciente. |
| **Planejamento financeiro** | Definição de metas financeiras de curto, médio e longo prazo e das estratégias para alcançá-las. |
| **Score de crédito** | Pontuação usada por instituições para avaliar o risco de conceder crédito a uma pessoa. |

### 4.3 Prompts reutilizáveis para futuras revisões

```
1. "Com base apenas nas fontes carregadas neste caderno, resuma o conceito de [TERMO], citando a fonte."

2. "Crie um glossário de 10 termos essenciais sobre [TEMA], com definição de uma linha cada, sem repetir conceitos."

3. "Compare as recomendações das fontes X e Y sobre [ASSUNTO] e destaque pontos de convergência e divergência."

4. "Gere 5 perguntas de revisão (estilo quiz) sobre os principais conceitos deste caderno, com gabarito comentado."

5. "Liste, em ordem de prioridade, os passos práticos recomendados pelas fontes para alguém iniciar [AÇÃO, ex: reserva de emergência / organização financeira]."
```

---

## 5. Como usar este repositório

1. Clone ou copie a estrutura deste README.
2. Substitua o tema, as fontes e as respostas pelos resultados reais do seu caderno no NotebookLM.
3. Use os prompts reutilizáveis da seção 4.3 como ponto de partida para revisões futuras ou para novos temas financeiros.

---

*Projeto desenvolvido como parte do desafio de projeto da DIO — Caderno Temático com NotebookLM.*
