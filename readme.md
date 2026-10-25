# Segundo Cérebro: Formação de Preço e Pricing Intelligence

Notebook especialista em formação de preço e inteligência de mercado, montado no Gemini Notebook (antigo NotebookLM) a partir de fontes que eu mesmo selecionei e conferi. As respostas abaixo foram geradas pelo notebook, com citações das fontes (prints na pasta `prints/`).

## 1. Tema e objetivo

> **Objetivo:** Ter um especialista que me explique como se forma o preço de venda, do custo e do ponto de equilíbrio até o markup, a concorrência e a precificação com dados, para aplicar em vagas e projetos de Market Intelligence e Pricing.

**O que o segundo cérebro precisa saber:**
- Diferença entre custos e despesas e como chegar ao custo unitário
- Ponto de equilíbrio e margem de contribuição
- Como o regime tributário entra no preço (Simples Nacional e Lucro Presumido)
- Markup e margem: as fórmulas e a diferença entre os dois
- Os cinco modelos de precificação e quando usar cada um
- Como dados e IA mudam a precificação, e como é a carreira na área

## 2. Fontes que entraram

Foram 5 fontes, em 3 formatos (PDF, artigos e vídeos). Print do painel de fontes: `prints/fontes.png`.

| # | Formato | Fonte | Por que confio | Ressalvas |
|---|---------|-------|----------------|-----------|
| 1 | PDF | **Guia Prático de Precificação para os Pequenos Negócios**, Sebrae Bahia / Sebrae Energia, 2020 (27 páginas, conteudista Luiz Marques de Andrade Filho) | Instituição de apoio a micro e pequenas empresas, autor identificado, referências bibliográficas (Assef, 2008; Bruni e Fama, 2014) e exemplos com contas que dá para refazer | Publicado em 2020, então regras e limites tributários precisam ser conferidos; foco em pequenos negócios |
| 2 | Artigo | [Modelos de precificação: 5 métodos para definir preço no varejo](https://www.infoprice.co/blog/modelos-de-precificacao/), InfoPrice, 07/10/2026 | Empresa especializada em pricing, conteúdo recente, fórmulas com exemplos numéricos e referência a estudo externo (Global Pricing Study 2025, Simon-Kucher) | A empresa vende ferramentas de pricing (viés comercial) e o artigo não traz autor individual |
| 3 | Artigo | [Precificação Inteligente: como o Big Data ajuda neste processo?](https://blog.neoway.com.br/precificacao-inteligente/), Neoway, 08/12/2021 (atualizado em 2023) | Empresa de Big Data e Analytics, e cita pesquisa da McKinsey | Mais antigo, viés comercial e autoria institucional |
| 4 | Vídeo | PricingCast, "Inteligência de Mercado e Pricing com Camila Pimentel..." (https://www.youtube.com/watch?v=1SIZ7qRWnXI) | _preencher: título completo, canal e por que confio (quem fala, experiência na área)_ | _preencher_ |
| 5 | Vídeo | PricingCast, "O Futuro da Inteligência de Mercado e do Pricing" (https://www.youtube.com/watch?v=FmtAz30I1uY), com Alex Leate, da Live University | _preencher: título completo, canal e por que confio_ | _preencher_ |

**Critérios que usei para aceitar uma fonte:**
- Autor ou instituição identificáveis e com experiência na área
- Exemplos numéricos que eu consigo refazer
- Conteúdo com data e, de preferência, recente
- Formatos variados (PDF, artigo, vídeo)
- Declarar o viés quando a fonte é de empresa que vende ferramenta

**Fontes que descartei:** posts de Instagram e conteúdos que apareceram em resumos de IA mas que eu não abri nem conferi.

## 3. Diretriz de comportamento do notebook

```
Comporte-se como um especialista sênior em formação de preço e inteligência de
mercado. Responda sempre em português do Brasil, de forma clara e direta, usando
apenas as fontes do notebook. Indique de qual fonte vem cada informação. Quando
houver cálculo, mostre a fórmula e a conta passo a passo. Quando as fontes
divergirem em algum conceito, aponte a divergência em vez de escolher uma. Se a
resposta não estiver nas fontes, diga que não encontrou em vez de inventar.
```

## 4. Perguntas, respostas e fontes

Os textos abaixo são resumos das respostas do notebook. Para as perguntas com print, a imagem mostra a resposta com uma citação aberta, apontando o trecho da fonte.

### Teste inicial: o notebook leu as tabelas do PDF?
**Pergunta:** Qual é o custo unitário de produção do sabão middle class e como ele é composto?

**Resposta do notebook:** R$ 2,11 por unidade, somando R$ 1,45 de material direto (matéria-prima R$ 0,85 mais embalagem R$ 0,60), R$ 0,45 de mão de obra direta e R$ 0,21 de custos indiretos de fabricação rateados. Ele refez todas as contas passo a passo, incluindo a fórmula do uso bruto da matéria-prima (uso líquido ÷ (1 − % de perda)). O resultado bate com o exemplo do guia do Sebrae.

**Fontes citadas:** 19655.pdf (Guia do Sebrae)

**Print:** `prints/chat-00-teste-pdf.png`

### Pergunta 1
**Qual a diferença entre custos e despesas, e por que isso importa para formar o preço?**

**Resposta do notebook:** Custos são os gastos ligados à produção do bem ou serviço (matéria-prima, embalagem, mão de obra direta e custos indiretos de fabricação); despesas são os gastos de gestão e vendas. Pelo custeio por absorção, só os custos entram no custo unitário (CMV/CSP). As despesas entram no preço de outra forma: a média delas sobre o faturamento compõe o mark-up. O notebook também mostrou como o piso de preço depende dos custos e despesas variáveis, com o exemplo da margem de contribuição-alvo (custo variável de R$ 10,00 resulta em preço de R$ 18,18).

**Fontes citadas:** 19655.pdf e "Modelos de precificação: 5 métodos para varejo e indústria" (InfoPrice)
### Pergunta 2
**Como se calcula o ponto de equilíbrio e como reduzi-lo?**

**Resposta do notebook:** O ponto de equilíbrio contábil é gastos fixos ÷ (preço − gasto variável unitário). O financeiro tira a depreciação, por ser gasto não desembolsável. No exemplo do guia (empresa de instalação de energia solar): gastos fixos de R$ 25.000, ticket médio de R$ 780,42 e margem de contribuição unitária de R$ 525,92, o que dá 47,54 clientes, arredondado para 48. Para reduzir: cortar gastos fixos ou aumentar a margem de contribuição, subindo o preço/ticket ou reduzindo o gasto variável unitário.

**Fontes citadas:** 19655.pdf

**Print:** `prints/chat-02.png`

### Pergunta 3
**Qual a diferença entre markup e margem, e por que um markup de 30% não dá 30% de margem?**

**Resposta do notebook:** Markup é o percentual aplicado sobre o custo; margem é o lucro sobre o preço de venda. Com markup multiplicador de 30% sobre um custo de R$ 10,00, o preço é R$ 13,00, o lucro é R$ 3,00 e a margem real é 23,1%. Para garantir a margem desejada usa-se o markup divisor, 1 ÷ (1 − soma dos % sobre a venda); para 30% de margem, o preço seria R$ 14,29. As duas fontes concordam nesse ponto e se complementam.

**Fontes citadas:** "Modelos de precificação" (InfoPrice) e 19655.pdf

**Print:** `prints/chat-03.png`

### Pergunta 4
**Quais são os cinco modelos de precificação e como combiná-los pelo papel de cada categoria?**

**Resposta do notebook:** Custo + markup, margem de contribuição-alvo, concorrência, valor e dinâmico. Os dois primeiros partem de dentro da empresa; os outros três, do mercado. Combinação por papel de categoria: tráfego usa concorrência, com margem de contribuição como piso; margem usa dinâmico; destino usa valor; conveniência usa dinâmico para itens menos elásticos. A regra de ouro é manter um piso de margem em todos os modelos.

**Fontes citadas:** "Modelos de precificação" (InfoPrice), com a divergência sobre precificação dinâmica apontada em relação ao artigo da Neoway
### Pergunta 5
**Qual a diferença entre precificação dinâmica e precificação inteligente, e qual o papel dos dados?**

**Resposta do notebook:** Segundo a Neoway, a dinâmica é um estágio anterior e mais simples, baseado em reagir aos preços da concorrência, enquanto a inteligente usa Big Data e algoritmos estatísticos para atingir objetivos próprios. Já a InfoPrice trata a dinâmica como um dos cinco modelos, com ajustes contínuos por demanda, estoque e concorrência. O notebook apontou essa divergência. Sobre dados: escala (milhares de SKUs sem gargalo humano), granularidade (por cidade ou bairro), elasticidade e previsão de demanda, e automação com IA.

**Fontes citadas:** "Precificação Inteligente" (Neoway), "Modelos de precificação" (InfoPrice) e os episódios do PricingCast
### Pergunta 6
**Onde as fontes se complementam e onde elas divergem?**

**Resposta do notebook:** Complementam: o guia do Sebrae dá a base interna (custos, ponto de equilíbrio, tributos, markup), a InfoPrice dá os modelos e os papéis por categoria, e a Neoway e os vídeos tratam de dados, IA e da relação entre inteligência de mercado e pricing. Divergem: no conceito de precificação dinâmica (Neoway x InfoPrice) e na estrutura das áreas (unificar IM e Pricing, no episódio #19, ou migrar equipes de IM para Pricing, no #43).

**Fontes citadas:** as cinco fontes do notebook

**Print:** `prints/chat-06.png`

### Pergunta 7
**O que os vídeos dizem sobre a carreira e a evolução da área de inteligência de mercado e pricing?**

**Resposta do notebook:** O pricing começou como tabela de preços operacional e virou área estratégica. A inteligência de mercado cresceu primeiro, mas teve dificuldade de provar ROI, e o pricing, que usa o mesmo ciclo analítico e mede impacto em margem e faturamento, ganhou espaço. Sobre carreira: "ninguém nasce pricer" (as pessoas vêm de vendas, finanças, tecnologia e trade), a pergunta certa vale mais que volume de dados e é preciso ter um patrocinador executivo. Sobre IA: o profissional não será substituído pela tecnologia, e sim por quem a usa, e ganha valor em raciocínio lógico, interpretação de contexto e relacionamento. O notebook também apontou uma lacuna entre a formação acadêmica tradicional e a prática da área.

**Fontes citadas:** PricingCast #19 e #43

**Print:** `prints/chat-07.png`

## 5. Observações sobre a qualidade das respostas

Conferi as respostas contra as fontes, e estes foram os pontos de atenção:
- **Acertos verificados:** o custo de R$ 2,11 do sabão, o ponto de equilíbrio de 48 clientes (R$ 525,92 de margem de contribuição) e a conta do markup (R$ 10,00 resulta em R$ 13,00 e margem de 23,1%) batem com o guia do Sebrae e com o artigo da InfoPrice.
- **Extrapolação:** na pergunta 2, o notebook ligou o ponto de equilíbrio ao artigo da Neoway, mas esse artigo usa "ponto de equilíbrio" num sentido amplo (equilíbrio entre margem e conversão), e não no sentido contábil do Sebrae.
- **Inconsistência:** na pergunta 6, o notebook listou o markup como divergência entre as fontes, mas na pergunta 3 ele já tinha dito que as fontes concordam. As duas fontes recomendam o markup divisor.
- **Datas:** o guia do Sebrae é de 2020 e o artigo da Neoway é de 2021, então números e regras tributárias precisam ser conferidos antes de uso real.
- **Slides, slide "Escada de Maturidade":** o quadro verde no canto inferior direito saiu com texto embaralhado.
- **Slides, slide "Estratégia Híbrida":** diz que itens de conveniência usam "Custo + Markup ou Valor", mas o artigo da InfoPrice indica precificação dinâmica para itens menos elásticos, com margem de contribuição de apoio. A classificação por "Curva A" e "Curva C" também não aparece no artigo.

## 6. Materiais gerados

- Mapa mental: `materiais/mapa-mental.png`
- Slides (12 slides): `materiais/slides.pdf`

## 7. Link do notebook

[Abrir o notebook](https://notebook.google.com/notebook/e1b05762-104a-44b8-8ea5-75541f55e7fd)

## 8. O que aprendi

Antes eu via precificação como custo mais uma margem. Com o notebook entendi que o resultado depende de separar custos e despesas, de calcular o ponto de equilíbrio e de usar o markup do jeito certo: um markup de 30% sobre o custo entrega só 23,1% de margem, e o markup divisor resolve isso.

O notebook acertou as contas do guia do Sebrae (R$ 2,11 de custo unitário e 48 clientes no ponto de equilíbrio), respondeu citando as fontes e apontou sozinho a divergência entre precificação dinâmica e inteligente.

Precisou de correção em alguns pontos: ele forçou uma ligação entre o ponto de equilíbrio e o artigo da Neoway, listou o markup como divergência depois de ter dito que as fontes concordavam, e os slides saíram com um quadro de texto embaralhado e uma classificação que não está no artigo.

Na escolha das fontes, eu faria diferente: dois dos três textos vêm de empresas que vendem soluções de pricing e o guia do Sebrae é de 2020. Incluiria uma fonte independente e mais recente, e vídeos mais focados em formação de preço, já que os dois que usei falam mais de carreira e da evolução da área.
