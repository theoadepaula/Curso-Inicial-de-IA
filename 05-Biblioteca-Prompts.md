# Biblioteca de Prompts — Gestão e Fiscalização de Contratos Públicos

> Prompts prontos para colar nas IAs (Claude, ChatGPT, Gemini). Ajuste o que está
> entre [colchetes]. **Lembre-se de anonimizar dados sigilosos antes de colar** (ver
> Guia de Segurança). A IA pode errar — confira sempre na fonte oficial.

## Como funciona um bom prompt (a fórmula C-P-F-E)
- **Contexto:** quem você é e qual a situação.
- **Papel:** que especialista a IA deve "encarnar".
- **Formato:** como você quer a resposta (tabela, lista, ofício, etc.).
- **Exemplos/Especificidade:** detalhes, critérios, restrições.

Exemplo da fórmula montada:
> "Você é um **fiscal de contratos** experiente da administração pública do DF (papel).
> Estou analisando um contrato de prestação de serviços continuados de limpeza (contexto).
> Liste em **tabela** os principais pontos de atenção para a fiscalização mensal (formato),
> separando obrigações da contratada, documentos a exigir e penalidades aplicáveis (especificidade)."

---

## 1. Análise de cláusulas contratuais
```
Você é um especialista em direito administrativo e contratos públicos.
Analise o trecho de contrato abaixo e me diga, em tópicos:
1) o que esta cláusula obriga cada parte a fazer;
2) riscos ou ambiguidades para o órgão público;
3) o que o fiscal deve verificar na prática para cumprir esta cláusula.
Use linguagem simples. Se algo depender de norma específica, diga qual verificar.

Trecho:
"""
[cole aqui o texto da cláusula — anonimizado]
"""
```

## 2. Checklist de fiscalização mensal
```
Você é um fiscal de contratos públicos. Com base no objeto descrito abaixo,
monte um checklist de fiscalização mensal em formato de tabela com as colunas:
Item a verificar | Documento/evidência exigida | Periodicidade | Base contratual.
Foque em itens objetivos e verificáveis.

Objeto do contrato: [ex.: serviços continuados de coleta de resíduos / limpeza urbana]
```

## 3. Resumo de processo longo
```
Resuma o documento abaixo para um gestor com pouco tempo. Entregue:
- 5 linhas de resumo executivo;
- principais decisões/prazos com datas;
- pendências e responsáveis;
- pontos que exigem atenção ou risco.
Mantenha-se fiel ao texto; se algo não estiver claro, sinalize "não consta".

Documento:
"""
[cole o texto — anonimizado]
"""
```

## 4. Comparação de propostas/itens
```
Compare as opções abaixo em uma tabela, com uma coluna por proposta e linhas para:
preço, prazo, garantias, conformidade com o edital e pontos de atenção.
Ao final, aponte objetivamente prós e contras de cada uma, sem decidir por mim.

Propostas:
[cole os dados — anonimizados]
```

## 5. Minuta de notificação à contratada
```
Você é um servidor público do DF redigindo uma notificação formal à empresa contratada.
Redija uma minuta de ofício de notificação por [descreva a ocorrência: ex. atraso na
execução / descumprimento de cláusula X], em tom formal, impessoal e técnico, conforme
padrão da administração pública. Inclua espaços [entre colchetes] para os dados que eu
devo preencher. Cite a base contratual de forma genérica para eu confirmar depois.
```

## 6. Tradução de "juridiquês" para a equipe
```
Explique a cláusula/norma abaixo em linguagem simples, como se fosse para um colega
que não é da área jurídica. Dê um exemplo prático de como isso aparece no dia a dia
da fiscalização.

Texto: [cole aqui]
```

## 7. Elaboração de relatório de fiscalização
```
Com base nas anotações abaixo, organize um relatório de fiscalização com as seções:
1) Identificação do contrato; 2) Período; 3) Atividades verificadas;
4) Conformidades; 5) Não conformidades e providências; 6) Conclusão.
Mantenha tom técnico e impessoal. Não invente fatos: use só o que está nas anotações.

Anotações:
"""
[cole suas anotações — anonimizadas]
"""
```

## 8. Estudo de norma / pesquisa
```
Explique o que diz a [Lei nº 14.133/2021 / Decreto X / IN Y] sobre [tema:
ex. sanções administrativas a contratadas]. Liste os artigos relevantes e o que cada um
determina, em linguagem simples. Importante: indique que devo confirmar o texto na fonte
oficial, pois você pode citar dispositivos de forma imprecisa.
```

## Dicas finais
- **Itere:** se a resposta não ficou boa, peça ajustes ("mais curto", "em tabela", "tom mais formal").
- **Dê exemplos** do que você considera uma boa resposta.
- **Peça as fontes** e confira-as — especialmente artigos de lei e números.
- **Nunca** peça à IA a decisão final do ato administrativo; use-a como apoio.
