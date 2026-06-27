# Casos Avançados — IA aplicada à fiscalização (além do básico)

> Usos mais potentes para o dia a dia do fiscal. Lembre: anonimizar dados sensíveis;
> conferir tudo na fonte oficial; a IA faz a conta e o rascunho, **você assina**.

---

## 1. Análise de PLANILHA com IA (o uso mais subutilizado)

A nova licitação é movida a **dado** (GPS, pesagem, IMR). A IA lê uma planilha e calcula
indicadores em segundos — ótimo para conferência do fechamento mensal.

> *(suba `exemplos-contrato-limpeza/planilha-exemplo-medicao-IMR.csv` — dados fictícios)*

### Prompt
```
Você é um fiscal técnico do SLU/DF. A planilha anexada traz, por serviço, os circuitos
planejados no mês e quantos ficaram abaixo da meta de execução. Para cada linha:
1) calcule X = [1 − (circuitos abaixo da meta ÷ planejados)] × 100;
2) diga em qual faixa do indicador (I03/I04/I05) o X se enquadra e qual o percentual de
   medição resultante para aquele serviço;
3) monte uma tabela final: Serviço | X calculado | Faixa | % de medição | Há desconto?
Use as faixas do IMR. Se eu não tiver informado alguma faixa, peça para eu confirmar no Anexo.
```

### 🟦 Resultado esperado (com os dados de exemplo)
| Serviço | X | Faixa | % medição | Desconto? |
|---|---|---|---|---|
| P1 (I03) | 91,0% | X ≥ 90% | 100% | Não |
| P2 (I04) | 92,5% | X ≥ 90% | 100% | Não |
| P5 (I05) | 96,25% | X ≥ 95% | 100% | Não |
| P6 (I05) | 91,67% | 90% ≤ X < 95% | **99%** | **Sim (−1% no P6)** |

> **Lição de ouro:** a IA é ótima para a **conta**, mas o fiscal confere a **faixa** contra o
> Anexo N e valida as exceções (feriado, falha de sistema do SLU). Excelente para Excel/Sheets:
> no plano pago, ChatGPT e Gemini fazem isso direto sobre a planilha.

---

## 2. Caso fim-a-fim: da vistoria ao documento assinado

Fluxo completo de um dia de fiscalização, mostrando a IA em **cada etapa**.

### Etapa 1 — anotação de campo vira relatório
```
Sou fiscal de contrato de limpeza urbana. A partir das minhas anotações de vistoria abaixo,
redija um relatório de fiscalização técnico e impessoal, com as seções: identificação,
data/local, constatações, conformidades, não conformidades e providências. Não invente nada
além das anotações; o que faltar, marque como "a verificar".

Anotações: "Vistoria RA Ceilândia, 10h. Dois contêineres semienterrados do P13A parados na
quadra X. Varrição P5 ok. Caminhão de coleta sem identificação visível. Papeleira quebrada
no ponto Y."
```

### Etapa 2 — gerar o checklist de providências
```
Com base no relatório acima, liste as providências que eu (fiscal) devo tomar, com prazo
sugerido e a base no IMR/contrato quando aplicável. Formato: Providência | Prazo | Indicador/cláusula.
```

### Etapa 3 — minutar a notificação
```
Redija a minuta de notificação à contratada sobre os contêineres semienterrados parados
(serviço P13A, indicador I06: 5 dias para regularizar após notificação), em tom formal,
exigindo comprovação por foto georreferenciada. Deixe [colchetes] para eu preencher.
```

> Mostre que **uma anotação rabiscada** vira, em minutos, **relatório + checklist + notificação**
> — mas cada peça passa pela revisão do fiscal antes de virar ato oficial.

---

## 3. Persona "Fiscal SLU" — prompt-base reutilizável

Cole este bloco **no início** de uma conversa (ou salve como instrução do projeto) para não
repetir o contexto toda vez:
```
A partir de agora, atue como um assistente de um FISCAL TÉCNICO de contratos de limpeza
urbana do SLU/DF. Contexto fixo:
- Contrato regido pela Lei 14.133/2021; nova licitação Pregão 90.005/2026 / TR 1/2026.
- Qualidade medida pelo IMR (17 indicadores), com faixas de desconto por serviço (P0–P20).
- O PDF do IMR em circulação é a versão 2022; sempre me lembre de confirmar faixas e códigos
  contra o Anexo N do TR 1/2026.
Regras de comportamento:
- Linguagem formal, impessoal e técnica da administração pública brasileira.
- Nunca afirme número, faixa ou artigo de lei sem me avisar para conferir na fonte.
- Quando faltar informação, escreva "a verificar" em vez de inventar.
Confirme que entendeu e aguarde minha tarefa.
```

---

## 4. Transcrição e resumo de reunião

A IA transforma o áudio de uma reunião de fiscalização em ata com pendências.
```
Vou colar a transcrição de uma reunião de acompanhamento do contrato. Gere:
1) resumo executivo em 5 linhas;
2) decisões tomadas (com responsável e prazo);
3) pendências em aberto;
4) próximos passos.
Mantenha-se fiel à transcrição; não acrescente o que não foi dito.

Transcrição: [cole aqui — gravada com app de transcrição ou pelo modo voz da IA]
```

> Dica: muitos celulares e o **modo voz** das IAs já transcrevem. Para dados sensíveis,
> prefira ferramenta homologada pelo órgão.
