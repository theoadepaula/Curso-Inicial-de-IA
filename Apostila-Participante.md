---
title: "IA na prática para a gestão e fiscalização de contratos públicos"
subtitle: "Apostila do participante"
---

# Sobre este material

Este guia acompanha o curso de introdução ao uso de inteligência artificial (IA) no trabalho
do servidor público, com foco na gestão e fiscalização de contratos. Serve para consulta e
prática depois do encontro. A ideia central percorre todo o material:

> **A IA é uma ferramenta de apoio. Ela não substitui o servidor.** Quem orienta a IA, revisa
> e assina é você. O dever de pensar não se delega.

---

# 1. O que é IA generativa (e o que não é)

A IA generativa (ChatGPT, Claude, Gemini e outras) funciona como um "autocompletar avançado":
prevê a próxima palavra com base em grande volume de textos. Por isso escreve bem — e por isso
também **inventa informação** com aparência de verdade. Esse erro é chamado de **alucinação**.

Consequência prática: tudo que for fato, número ou dispositivo de lei deve ser **conferido na
fonte oficial** antes de uso.

## Mitos comuns

| Mito | Realidade |
|---|---|
| "A IA pensa como gente" | Ela calcula a próxima palavra provável |
| "A IA é sempre certa" | Ela erra e inventa; confira sempre |
| "A IA vai me substituir" | Substitui tarefas, não quem pensa e decide |
| "Tudo que eu colo fica privado" | No plano grátis, pode treinar o modelo; configure |
| "Usar IA é trapaça" | É ferramenta de trabalho; o cuidado é revisar e assumir o resultado |

## RAG: quando a IA consulta documentos antes de responder

- **IA comum:** responde "de cabeça", pelo que aprendeu no treino — pode desatualizar e inventar.
- **RAG** (*Retrieval-Augmented Generation*): a IA **consulta uma base de documentos confiáveis
  antes de responder** e **cita a fonte**. Menos alucinação, mais atual e auditável.
- *Analogia:* prova de cabeça (IA comum) × prova com consulta ao material (RAG).
- **Quais usam RAG:** NotebookLM (seus documentos), Perplexity (a web com fontes),
  ChatGPT/Claude/Gemini quando você anexa um arquivo ou liga a busca, e assistentes do órgão
  (ex.: ChatTCU). No setor público, RAG é o caminho recomendado para documentos internos.

---

# 2. As ferramentas e qual usar para quê

Não existe "a melhor IA". Existe a melhor para cada tarefa.

| Quero… | Opção indicada |
|---|---|
| Analisar um contrato ou TR longo | Claude |
| Redigir ofício ou relatório formal | Claude ou ChatGPT |
| Trabalhar dentro do Google (Docs, Drive) | Gemini |
| Trabalhar dentro do Office (Word, Excel) | Microsoft Copilot |
| Pesquisar com fontes citadas | Perplexity |
| Estudar meus próprios documentos | NotebookLM |
| Transformar um normativo em vídeo ou áudio didático | NotebookLM |
| Editar uma imagem existente | Gemini |
| Criar uma imagem | ChatGPT ou Midjourney |

**Sobre as IAs estrangeiras sem controle (ex.: DeepSeek, Qwen, Kimi):** podem processar dados
fora do país, sob outra legislação. Use apenas para testes com conteúdo público; não envie
documentos de trabalho.

---

# 3. Segurança e LGPD: o que pode e o que não pode

**Regra de ouro:** trate a IA como um e-mail enviado para fora do órgão.

**Pode, em geral:** documentos públicos (editais e leis já publicados), textos sem dado
pessoal, conteúdo anonimizado.

**Não envie sem cuidado:** dados pessoais (CPF, nome, endereço), informações sigilosas,
minutas ainda não publicadas, senhas.

**Como reduzir o risco:**

1. Troque nomes por papéis ("a CONTRATADA", "o fiscal") e dados reais por marcadores (`[CPF]`, `[VALOR]`).
2. Em Configurações → Privacidade, desative o uso das conversas para treinamento.
3. Para documentos internos com segurança, use a versão corporativa contratada pelo órgão.
4. Pergunte-se: "se vazasse, causaria dano?"

A responsabilidade pelo ato administrativo é sempre do servidor, mesmo com apoio de IA.

---

# 4. Como pedir bem: a fórmula C-P-F-E

- **C**ontexto — qual a situação.
- **P**apel — "você é um fiscal de contratos experiente".
- **F**ormato — "responda em tabela".
- **E**specificidade — critérios, restrições, exemplos.

**Exemplo — pedido fraco:** "fala sobre fiscalização de contrato".

**Exemplo — pedido bom:** "Você é um fiscal técnico do SLU/DF. Liste em tabela os pontos de
atenção da fiscalização mensal de um contrato de limpeza urbana, separando obrigações da
contratada, documentos a exigir e penalidades."

Se a resposta não vier boa, ajuste em diálogo: "mais curto", "em tabela", "tom mais formal".

---

# 5. Uso responsável e sinais de alerta

Riscos do uso sem reflexão:

- **Viés de automação:** aceitar a resposta só porque "a máquina disse".
- **Atrofia do critério:** quem delega tudo perde a capacidade de analisar e decidir.
- **Alucinação:** a IA inventa fatos e leis. Em 2023, advogados foram multados por citar
  jurisprudência inexistente gerada por IA.

## Sinais de que a IA foi usada sem reflexão

| Sinal | O que se observa |
|---|---|
| Texto "perfeito" demais | Genérico, sem o caso concreto |
| Referência que ninguém acha | Lei ou processo que não se localiza |
| Resposta instantânea | Tarefa complexa sem rastro de análise |
| Não sabe explicar | A pessoa não justifica a própria conclusão |
| Termos estranhos | Fora do jargão da administração pública |

**Boas práticas (humano no circuito):** revisão obrigatória; verificação cruzada (citou um
artigo? confira no Planalto); anonimização; registro do uso; ferramentas homologadas para
dados sensíveis.

---

# 6. Prompts prontos para contratos

1. **Analisar cláusula:** "Você é especialista em contratos públicos. Analise o trecho abaixo e
   diga: o que obriga cada parte; riscos para o órgão; o que o fiscal deve verificar na prática."
2. **Checklist de fiscalização:** "Monte um checklist de fiscalização mensal em tabela: item a
   verificar | documento exigido | periodicidade | base contratual."
3. **Resumir processo:** "Resuma o documento em 5 linhas + decisões com prazos + pendências e
   responsáveis. Fiel ao texto; o que faltar, marque 'não consta'."
4. **Comparar propostas:** "Compare as opções em tabela (preço, prazo, conformidade, pontos de
   atenção). Não decida por mim."
5. **Minutar notificação:** "Redija uma minuta de notificação à contratada sobre [ocorrência],
   em tom formal e impessoal, com [colchetes] para eu preencher."

---

# 7. Glossário rápido

| Termo | Significado |
|---|---|
| Prompt | O comando ou pergunta dado à IA |
| Token | Pedaço de texto (≈ ¾ de palavra); mede tamanho e custo |
| Janela de contexto | Quanto a IA lê de uma vez; maior = documentos mais longos |
| Alucinação | Informação inventada com tom convincente |
| Multimodal | IA que entende texto, imagem, áudio e PDF |
| RAG | A IA consulta seus documentos antes de responder (reduz alucinação) |
| Enterprise | Versão corporativa que não treina com seus dados |

---

# 8. Primeiros passos (gratuito)

| Ferramenta | Endereço | Login |
|---|---|---|
| ChatGPT | chatgpt.com | Google, Microsoft, Apple ou e-mail |
| Claude | claude.ai | Google ou e-mail |
| Gemini | gemini.google.com | Conta Google |
| NotebookLM | notebooklm.google.com | Conta Google |

Ao criar a conta: desligue o uso das conversas para treinamento, instale o app no celular e
faça um teste simples. No celular, use o microfone — falar costuma ser mais rápido que digitar.

---

# 9. Plano dos primeiros 7 dias

| Dia | Tarefa |
|---|---|
| 1 | Criar conta, instalar o app e desligar o treinamento |
| 2 | Pedir o resumo de um documento público longo |
| 3 | Reescrever um e-mail ou ofício para ficar mais claro |
| 4 | Praticar a fórmula C-P-F-E em um pedido do seu trabalho |
| 5 | Subir um PDF público, fazer 3 perguntas e conferir as respostas |
| 6 | Criar um notebook no NotebookLM e gerar um resumo em áudio |
| 7 | Montar uma persona reutilizável e salvar 3 prompts favoritos |

---

# 10. Perguntas frequentes

**Todas as IAs são iguais?** Não. Cada uma tem pontos fortes; tenha duas ou três e escolha pela
tarefa.

**Posso subir documentos do trabalho?** Públicos, sim. Dados pessoais ou sigilosos, não, sem
anonimizar. Para documentos internos com segurança, use a versão corporativa do órgão.

**Como ser específico nos comandos?** Use C-P-F-E e ajuste em diálogo.

**Como usar a IA todo dia?** Comece pelas tarefas repetitivas (resumir o que chega, rascunhar o
que sai, conferir o que decide) e salve os prompts que funcionam.

---

# 11. Fontes oficiais (Governo Federal)

O **Núcleo de Inteligência Artificial (NIA)** da Secretaria de Governo Digital (SGD/MGI)
publicou materiais que respaldam este curso. Leitura recomendada (acesse pela página de
Inteligência Artificial do Governo Digital):

- **Guia de IA generativa no serviço público** — uso responsável.
- **Guia prático de prompt e pesquisa com IA** — reforça a fórmula C-P-F-E.
- **Guia de introdução ao RAG** — IA que consulta documentos confiáveis antes de responder
  (é o que o NotebookLM faz).
- **Glossário oficial de termos de IA**.
- **Portarias SGD/MGI nº 6.618/2024 e nº 473/2026** — diretrizes de IA no Executivo Federal.

> O que ensinamos aqui está **alinhado às diretrizes oficiais do Governo Federal**: a IA é
> apoio, exige verificação das fontes e a responsabilidade permanece com o servidor.

---

> **A IA não substitui o fiscal — ela amplia o bom fiscal.** Quem orienta é você.
> Ela faz a conta e o rascunho; o juízo e a assinatura são seus.
