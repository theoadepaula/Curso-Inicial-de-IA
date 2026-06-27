# Demonstração ao vivo — Prompt RUIM vs BOM (nas 3 IAs)

> Roteiro de demonstração para o Bloco 4 (A arte do prompt) e o Bloco 5 (Casos).
> Usa os documentos reais da pasta [exemplos-contrato-limpeza/](exemplos-contrato-limpeza/).
>
> **Como conduzir:** abra Claude, ChatGPT e Gemini em abas. Rode primeiro o prompt RUIM,
> depois o BOM, na MESMA ferramenta — a plateia vê o salto de qualidade. Depois rode o
> prompt BOM nas três e compare. As **saídas do Claude abaixo são reais** (geradas agora);
> as colunas de ChatGPT/Gemini você preenche ao vivo.
>
> ⚠️ A IA pode errar faixas e números — confirme sempre no documento oficial.

---

## Antes de rodar: dá para anexar esses PDFs no plano gratuito?

**Sim — o problema não é o tamanho (os TRs têm < 1 MB), e sim o número de páginas** (TR 29 ≈ 78 pp; TR 1/2026 ≈ 93 pp) e as cotas do plano free.

| Ferramenta (grátis) | Comportamento esperado |
|---|---|
| **Gemini** | Melhor para os TRs grandes (contexto enorme); aguenta os dois juntos com mais folga |
| **Claude** | Aceita bem 1 documento; os **dois TRs juntos** podem estourar a cota da mensagem no free |
| **ChatGPT** | Aceita, mas em doc longo tende a ler **por partes**; tem limite diário de mensagens |

**Recomendações:** suba **um documento por vez**; para comparar TRs, cole só os **trechos
relevantes** em vez das 171 páginas; prefira o **IMR (26 pp)** para os demos; e **teste na
véspera** com a conta que usará. A **Matriz de Riscos (6,69 MB, escaneada)** é o upload mais
arriscado no free — exige OCR; teste antes.

---

## CASO 1 — Comparar o contrato emergencial (TR 29) com a nova licitação (TR 1/2026)

### ❌ Prompt RUIM
```
qual a diferença entre os dois contratos de limpeza?
```
**Por que é ruim:** sem documento anexado, sem papel, sem formato, sem foco. A IA
"chuta" com conhecimento genérico — fala de limpeza no geral, pode inventar dados e não
serve para o fiscal. *Saída típica:* um texto vago sobre "contratos emergenciais costumam
ser temporários e licitações são definitivas", sem os números do SLU.

### ✅ Prompt BOM
> *(anexe os dois PDFs: `SEI_183603394_Termo_de_Referencia_29.pdf` e `SEI_191536563_Termo_de_Referencia_1.pdf`)*
```
Você é um fiscal técnico de contratos de limpeza urbana do SLU/DF. Compare os dois Termos
de Referência anexados (TR 29/2025 = emergencial; TR 1/2026 = nova licitação) sob a ótica
de quem FISCALIZA. Responda em tabela com as colunas:
Aspecto | Emergencial (TR 29) | Nova licitação (TR 1/2026) | Impacto para o fiscal.
Cubra: número/organização dos serviços, como a qualidade é controlada e paga, base de
prova exigida, garantia e habilitação. Depois liste as 3 mudanças que mais exigem atenção
do fiscal. Use só os documentos; se algo não constar, escreva "não consta".
```

#### 🟦 Saída real do Claude (gerada agora, a partir do material de contexto)
| Aspecto | Emergencial (TR 29/2025) | Nova licitação (TR 1/2026) | Impacto para o fiscal |
|---|---|---|---|
| Natureza | Temporária/precária; acaba quando o regular é assinado | Definitiva, 60 meses, prorrogável | Muda o horizonte de planejamento da fiscalização |
| Serviços | 12 serviços agrupados (P1–P12) | 21 serviços desmembrados (P0–P20) | Mais frentes a acompanhar; serviços novos (P0, P12, P13, P18…) |
| Controle de qualidade | Fiscalização tradicional + glosa/multa pontual | **IMR – pagamento por resultado** (17 indicadores) + glosa/multa (coexistem) | A qualidade vira **número** (meta→faixa→desconto) |
| Base de prova | Relatório de fiscalização | **Sistemas** (GPS, pesagem), surveys, gravimetria, SEI | Fiscal valida o **dado** que alimenta o desconto |
| Garantia | 5% do valor **anual** | 5% do valor **total quinquenal** | Garantia muito maior; conferir vigência |
| Habilitação | Mais simples | Plano de Trabalho + atestados ≥50% por ≥12 meses; CREA | Exigências de qualificação mais rígidas |

**3 mudanças que mais exigem atenção do fiscal:**
1. **O IMR muda o jogo:** a qualidade passa a ser medida por 17 indicadores que reduzem o pagamento por faixas — o fiscal precisa dominar meta, fórmula e fonte de cada um.
2. **A prova vem de sistema:** GPS e pesagem alimentam a medição; o papel do fiscal é garantir que o dado é correto e rastreável (e tratar exceções legítimas).
3. **Mais serviços e novos serviços** (P0 Administração Local, P12, P13, P18-UTMB…): há frentes que não existiam no emergencial.

> *Observação do Claude: baseei-me no material; confirme os números (garantia, percentuais) direto no texto oficial dos TRs.*

#### 🟩 ChatGPT (preencher ao vivo) · 🟨 Gemini (preencher ao vivo)
| O que observar | ChatGPT | Gemini |
|---|---|---|
| Entendeu o PDF anexado? | | |
| Acertou os números (12 vs 21 serviços, garantia)? | | |
| Organização/clareza da tabela | | |
| Inventou algo (alucinação)? | | |

---

## CASO 2 — Calcular um desconto do IMR (indicador I03)

### ❌ Prompt RUIM
```
como funciona o desconto do IMR?
```
**Por que é ruim:** pergunta genérica, sem o anexo e sem o caso concreto. A IA explica
"em tese" e não calcula nada útil para o fechamento do mês.

### ✅ Prompt BOM
> *(anexe `Anexo___IMR.pdf`)*
```
Você é um fiscal técnico. Com base no IMR anexado, calcule o desconto deste caso e mostre
o passo a passo, citando a faixa aplicada:
Indicador I03 (Circuito de Coleta Convencional, serviço P1): foram planejados 200 circuitos
no mês e 18 ficaram abaixo de 90% de execução. Qual o percentual de medição do P1 segundo
as faixas do indicador? Mostre a conta. Depois me lembre do teto mensal de desconto do IMR
e diga se ele afeta este caso. Se alguma faixa estiver ambígua no documento, avise.
```

#### 🟦 Saída real do Claude (gerada agora)
**Passo a passo:**
1. Fórmula do I03: `X = [1 − (circuitos abaixo de 90% ÷ total planejado)] × 100`.
2. Substituindo: `X = [1 − (18 ÷ 200)] × 100 = [1 − 0,09] × 100 = 91%`.
3. Faixas do I03 (sobre o serviço P1): **X ≥ 90% → 100%** · 85% ≤ X < 90% → 99% · X < 85% → 98%.
4. Como **X = 91% ≥ 90%**, o resultado é **100% de medição do P1 — sem desconto neste indicador**.

**Teto mensal:** o IMR tem **teto de 20%** — a soma de todos os descontos de IMR no mês não
ultrapassa 20% do custo mensal total do contrato. Neste caso não há desconto pelo I03, então
o teto não é acionado por este indicador (mas outros indicadores do mês podem somar).

> *Observação do Claude: as faixas usadas vêm da versão 2022 do IMR; confirme contra o Anexo N do TR 1/2026 antes de aplicar no fechamento real.*

#### 🟩 ChatGPT · 🟨 Gemini (preencher ao vivo)
| O que observar | ChatGPT | Gemini |
|---|---|---|
| Achou a fórmula certa no anexo? | | |
| Fez a conta certa (91% → 100%)? | | |
| Lembrou do teto de 20%? | | |
| Avisou sobre confirmar a versão do anexo? | | |

---

## CASO 3 — De quem é o risco? (Matriz de Riscos)

### ❌ Prompt RUIM
```
quem paga quando o GPS para?
```

### ✅ Prompt BOM
> *(anexe `Matriz_de_Riscos___Anexo_Q.pdf`)*
```
Você é um fiscal de contrato. Com base na Matriz de Riscos anexada, diga em cada caso se o
risco é da CONTRATADA ou do CONTRATANTE (SLU/DF) e se o fiscal pode penalizar/glosar,
citando o item da matriz:
a) o GPS do caminhão da empresa parou por falha do equipamento dela;
b) o circuito não fechou porque o sistema do SLU (SIMLUR) caiu;
c) o diesel subiu 12%;
d) vandalismo atingiu 5% dos contêineres.
Se algo não estiver claro na matriz, escreva "não consta expressamente".
```

#### 🟦 Saída real do Claude (gerada agora)
| Caso | Risco de quem? | Fiscal pode penalizar? | Fundamento |
|---|---|---|---|
| a) GPS da empresa falhou | **Contratada** | Sim | Falha de GPS dos equipamentos da própria contratada é risco dela |
| b) Sistema do SLU (SIMLUR) caiu | **Contratante (SLU)** | **Não** | Falha dos sistemas do SLU é risco alocado ao contratante — circuitos afetados não contam |
| c) Diesel subiu 12% | **Contratada** | Não penaliza (é risco do negócio) | Variação de combustível **< 25%** é risco da contratada, sem reequilíbrio |
| d) Vandalismo em 5% dos contêineres | **Contratada** | Sim, dentro do limite | Vandalismo é risco da contratada **até 7,5%** da frota; 5% está dentro |

**Regra de ouro:** antes de glosar, pergunte *"de quem é este risco pela Matriz?"*. Se a
falha decorre de risco alocado ao SLU (ex.: caso b), **não se penaliza a contratada** — e
isso precisa estar documentado.

> *Observação do Claude: confirme os percentuais (25% combustível, 7,5% vandalismo) no texto oficial da Matriz.*

#### 🟩 ChatGPT · 🟨 Gemini (preencher ao vivo)
| O que observar | ChatGPT | Gemini |
|---|---|---|
| Classificou risco certo em cada caso? | | |
| Usou os limites (25%, 7,5%)? | | |
| Citou os itens da matriz? | | |

---

## CASO 4 — Alucinação: o erro que só o fiscal percebe

> **Objetivo da demo:** provar, na prática, que a IA não substitui o fiscal. Aqui a IA dá uma
> resposta **confiante, bem formatada e errada**. Quem não domina o IMR aceita; o bom fiscal pega.

### Pergunta feita à IA
```
No indicador I03 do IMR (Circuito de Coleta Convencional, serviço P1), o mês fechou com
X = 88% de conformidade. Qual o desconto, sobre o que ele incide, e qual a base legal?
```

### 🟥 Resposta ALUCINADA (exemplo realista — NÃO use como verdade)
> "Como X = 88% ficou **abaixo da meta de 90%**, aplica-se o **desconto de 10%**, de modo que
> a contratada recebe **90% do valor mensal do contrato** referente ao período. A glosa tem
> fundamento no **art. 47, §2º, da Lei nº 14.133/2021**, que disciplina a redução proporcional
> por descumprimento de níveis de serviço."

*Parece impecável: tom seguro, número redondo, cita lei. E está errado em 3 pontos.*

### 🟦 O que o fiscal que SABE a matéria percebe (4 erros)
| # | O que a IA disse | O que é correto (Anexo IMR) | Por que importa |
|---|---|---|---|
| 1 | Desconto de **10%** | Faixa **85% ≤ X < 90% → 99%** = desconto de **1%** | A IA inflou o desconto em 10×; geraria glosa indevida e litígio |
| 2 | Incide sobre **o contrato inteiro** | Incide **só sobre a medição do P1** | O IMR nunca desconta o contrato todo por um indicador |
| 3 | Esqueceu o **teto de 20%** mensal | A soma dos IMRs do mês não passa de 20% | Controle essencial no fechamento |
| 4 | "art. 47, §2º da Lei 14.133" | **Citação inventada** — a regra está no **próprio IMR (Anexo do TR)** | Alucinação clássica: lei que soa real, mas não diz isso |

### ✅ Resposta correta
> X = 88% cai na faixa **85% ≤ X < 90% → 99%**: a **medição do serviço P1** (e só dele) é paga
> a **99%** — desconto de **1%** sobre o P1. A regra é a do **Anexo IMR do TR 1/2026** (não de
> artigo da Lei 14.133). No fechamento, somar com outros IMRs do P1, respeitando o **teto de 20%**.

### 🎯 A lição (liga direto com a ênfase do curso)
- A alucinação **não vem com aviso** — vem bem escrita e confiante.
- **Só percebe quem conhece as faixas do IMR.** Um fiscal que "terceirizou o pensar" aplicaria
  um desconto 10× maior, com base legal falsa.
- **Por isso a IA não substitui o fiscal:** para checar a IA, é preciso já saber a resposta.
- Regra prática: **toda faixa, número e artigo de lei que a IA citar, confira na fonte oficial**
  (no IMR, contra o **Anexo N do TR 1/2026**).

> **Bônus (caso real para citar):** em 2023, advogados em Nova York foram **multados** por
> apresentar uma petição com **jurisprudência inventada pelo ChatGPT** — precedentes que não
> existiam (caso *Mata v. Avianca*). Houve outros casos parecidos depois. Mesmo erro, outro
> setor: confiaram sem conferir. *(Fontes no material `Briefing-Riscos-Uso-Indiscriminado-IA.md`.)*

---

## Como cada IA tende a se sair (minhas notas para o apresentador)
- **Claude:** forte em documentos longos, tabelas e tom formal; costuma sinalizar incertezas e pedir confirmação — bom para análise de TR/IMR.
- **ChatGPT:** muito versátil; lê PDFs bem na versão paga; ótimo para redigir minutas e variar formatos.
- **Gemini:** integra com Google (Docs/Drive); útil se os documentos já estão no Drive do órgão; bom multimodal.
- **Mensagem para a plateia:** as três acertam o essencial quando o **prompt é bom e o documento é anexado**. A diferença de qualidade vem **muito mais do prompt e do contexto** do que da escolha da ferramenta.

## Roteiro de 6 minutos para a demo ao vivo
1. (1 min) Rode o **prompt ruim** do Caso 1 no Claude. Mostre o resultado vago.
2. (2 min) Rode o **prompt bom** do Caso 1 no Claude. Compare na hora.
3. (2 min) Rode o **mesmo prompt bom** no ChatGPT e no Gemini. Preencha a tabela.
4. (1 min) Feche com a mensagem: "o segredo é o prompt + anexar o documento, não a marca da IA".
