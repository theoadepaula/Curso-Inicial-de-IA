# Prompts de Exemplo — baseados nos documentos reais da Nova Licitação (SLU/DF)

> Prompts prontos construídos sobre os documentos da pasta
> [exemplos-contrato-limpeza/](exemplos-contrato-limpeza/). São **casos reais** de
> fiscalização do contrato de limpeza urbana — ótimos para a demonstração ao vivo.
>
> **Por que estes documentos são seguros para o curso:** edital, Termo de Referência e
> anexos (IMR, Matriz de Riscos) são **públicos** depois de publicados. Use-os à vontade.
> Ainda assim, ao subir documentos no dia a dia, remova dados pessoais (CPF, e-mails) —
> ver [Guia de Segurança](04-Guia-Seguranca-LGPD.md).

## Documentos de referência (na pasta de exemplos)
| Arquivo | O que é |
|---|---|
| `SEI_183603394_Termo_de_Referencia_29.pdf` | **TR 29/2025** — contrato emergencial vigente (P1–P12) |
| `SEI_191536563_Termo_de_Referencia_1.pdf` | **TR 1/2026** — nova licitação (21 serviços P0–P20) |
| `Anexo___IMR.pdf` | **IMR** — Instrumento de Medição de Resultado (17 indicadores) |
| `Matriz_de_Riscos___Anexo_Q.pdf` | **Matriz de Riscos** — quem responde por cada evento |
| `SEI_201119023_Edital_Pregao_Presencial_90005_2026.pdf` | **Edital** do Pregão 90.005/2026 |

> **Como usar:** na maioria das IAs (Claude, ChatGPT, Gemini), clique no clipe/anexo,
> suba o PDF indicado e cole o prompt. No NotebookLM, adicione o PDF como *fonte* e
> pergunte. Sempre **confira o resultado contra o documento oficial** — a IA pode errar.

---

## A. Entender e resumir um documento

### A1. Resumo executivo do TR da nova licitação
> *(suba `SEI_191536563_Termo_de_Referencia_1.pdf`)*
```
Você é um analista de contratos públicos. Resuma este Termo de Referência para um
fiscal técnico que tem 5 minutos. Entregue:
1) objeto e abrangência em 3 linhas;
2) quantos serviços existem e como estão divididos em lotes;
3) prazo de vigência e valor estimado;
4) as 5 obrigações da contratada mais relevantes para a fiscalização;
5) o que mudou em relação a um contrato anterior, se o documento mencionar.
Não invente números: se algo não constar, escreva "não consta no documento".
```

### A2. Glossário do contrato para a equipe
> *(suba o TR 1/2026)*
```
Liste e explique, em linguagem simples, os 15 termos técnicos mais importantes deste
Termo de Referência (ex.: IMR, glosa, UTMB, transbordo, dedicação exclusiva de mão de
obra). Para cada um: definição em 1 frase + por que importa para o fiscal. Formato: tabela.
```

---

## B. Comparar o emergencial (TR 29) com a nova licitação (TR 1/2026)

### B1. O que muda para o fiscal
> *(suba os dois TRs: `...Referencia_29.pdf` e `...Referencia_1.pdf`)*
```
Compare os dois Termos de Referência anexados (TR 29/2025, emergencial, e TR 1/2026, nova
licitação) sob a ótica de quem FISCALIZA. Monte uma tabela com as colunas:
Aspecto | Contrato emergencial (TR 29) | Nova licitação (TR 1/2026) | Impacto para o fiscal.
Cubra ao menos: nº e organização dos serviços, como a qualidade é controlada e paga,
base de prova exigida, garantia contratual e habilitação. Ao final, liste em tópicos
as 3 mudanças que mais exigem atenção do fiscal. Baseie-se só nos documentos.
```

### B2. Serviços novos que passam a ser fiscalizados
> *(suba o TR 1/2026)*
```
Com base neste Termo de Referência, liste os serviços que existem na nova licitação e
explique, para cada serviço que pareça novo ou desmembrado, o que o fiscal passará a
acompanhar na prática. Tabela: Código do serviço | Nome | O que o fiscal verifica.
Se o documento não deixar claro que é "novo", apenas descreva o serviço.
```

---

## C. IMR — pagamento por resultado (o coração da nova fiscalização)

### C1. Explicar um indicador e como aplicá-lo
> *(suba `Anexo___IMR.pdf`)*
```
Você é um fiscal técnico experiente. Explique o indicador I06 (Operação e Manutenção de
Contêineres Semienterrados) deste IMR para um colega que vai aplicá-lo pela primeira vez.
Detalhe: (1) a meta; (2) como contar os dias / a fórmula; (3) qual a fonte da prova;
(4) as faixas de desconto e sobre qual serviço o desconto incide. Termine com um alerta
de 1 linha sobre o que confirmar na versão oficial do anexo antes de aplicar desconto.
```

### C2. Simular o cálculo de desconto de um mês
> *(suba o IMR — útil para treinar a equipe)*
```
Vou te dar uma situação hipotética de fechamento mensal. Com base nas regras do IMR
anexado, calcule o desconto e mostre o passo a passo, citando a faixa aplicada:

Situação: no indicador I03 (Circuito de Coleta Convencional, serviço P1), foram planejados
200 circuitos no mês e 18 ficaram abaixo de 90% de execução. Qual o percentual de medição
do P1 segundo as faixas do indicador? Mostre a conta. Depois lembre-me do teto mensal de
desconto previsto no IMR e diga se ele afeta este caso.
IMPORTANTE: confirmarei as faixas no anexo oficial; aponte se alguma premissa ficou incerta.
```

### C3. Checklist de fechamento mensal do IMR
> *(suba o IMR)*
```
Monte um checklist operacional para o fiscal fechar o mês do IMR, em tabela com:
Indicador | Fonte do dado / com quem confirmar | O que o fiscal precisa ter em mãos | Risco se faltar.
Cubra todos os indicadores do anexo. Ao final, acrescente um lembrete sobre acúmulo de
descontos no mesmo serviço e sobre o teto mensal.
```

---

## D. Matriz de Riscos — o que pode (e o que não pode) cobrar

### D1. De quem é o risco?
> *(suba `Matriz_de_Riscos___Anexo_Q.pdf`)*
```
Você é um fiscal de contrato. Com base na Matriz de Riscos anexada, responda: em cada
situação abaixo, o risco é da CONTRATADA ou do CONTRATANTE (SLU/DF), e o fiscal pode ou
não penalizar/glosar? Justifique citando o item da matriz.
a) O GPS de um caminhão da empresa parou de transmitir por falha do equipamento dela.
b) O circuito não fechou porque o sistema do SLU (SIMLUR) ficou fora do ar.
c) O preço do diesel subiu 12% no período.
d) Contêineres foram vandalizados, atingindo 5% da frota.
Se algum caso não estiver claramente coberto, diga "a matriz não trata expressamente".
```

### D2. Guia de bolso da Matriz de Riscos
> *(suba a Matriz de Riscos)*
```
Resuma a Matriz de Riscos anexada em um "guia de bolso" do fiscal: duas listas curtas —
"Risco da CONTRATADA (posso cobrar)" e "Risco do SLU (não penalizar a contratada)" —
com os eventos mais frequentes na fiscalização. Mantenha-se fiel ao documento.
```

---

## E. Produzir documentos a partir dos casos

### E1. Minuta de notificação (indicador I06/I07)
```
Você é um fiscal do SLU/DF redigindo uma notificação formal à empresa contratada.
Contexto: um contêiner semienterrado (serviço P13A) está fora de operação e, pelo IMR
(indicador I06), a empresa tem 5 dias para regularizar após a notificação. Redija a minuta
da notificação em tom formal e impessoal, conforme padrão da administração pública,
incluindo: identificação do equipamento e local [entre colchetes], descrição da
irregularidade, prazo de regularização, exigência de comprovação por foto georreferenciada
e advertência sobre o desconto do IMR caso não cumpra. Deixe [colchetes] para eu preencher.
```

### E2. Esqueleto de relatório mensal de fiscalização
```
Monte a estrutura de um relatório mensal de fiscalização do contrato de limpeza urbana,
com as seções e o que entra em cada uma, considerando que a medição depende do IMR
(indicadores), de demandas de Ouvidoria e de dados de sistema (GPS, pesagem). Tom técnico
e impessoal. Não preencha com dados — só a estrutura e instruções do que coletar em cada parte.
```

---

## F. Fluxo com NotebookLM (pesquisa, áudio e vídeo)

Você já fez isso na pasta `Material_Fiscais` — vale mostrar no curso como replicar:
```
1. No NotebookLM, crie um notebook "Nova Licitação 90.005/2026".
2. Adicione como fontes: o Edital, o TR 1/2026, o Anexo IMR e a Matriz de Riscos.
3. Pergunte (com fontes citadas): "Liste os 17 indicadores do IMR e, para cada um,
   a meta e a faixa de desconto, citando a página."
4. Gere um Audio Overview (podcast) para a equipe ouvir, e um Video Overview por tema
   (ex.: um vídeo só sobre o IMR, outro sobre a Matriz de Riscos).
```

---

## Lembrete final (repetir para a equipe)
- Estes PDFs são **públicos** — por isso servem de exemplo. Documentos sigilosos: anonimizar.
- A IA **erra** faixas, números e citações de artigos. **Confirme sempre** no documento oficial
  (no caso do IMR, contra o **Anexo N do TR 1/2026**, pois o PDF disponível é a versão de 2022).
- A IA faz o rascunho e a conta; **quem assina e responde é o fiscal**.
