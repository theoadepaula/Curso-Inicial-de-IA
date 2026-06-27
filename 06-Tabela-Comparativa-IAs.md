# Tabela Comparativa — Principais IAs (2026)

> Responde à pergunta: **"Todas as IAs têm as mesmas funcionalidades? Alguma é melhor
> para determinada tarefa?"** Resposta curta: **não são iguais** — cada uma tem forças.

## Visão geral

| Ferramenta | Empresa / País | Melhor para | Conta grátis? | Observações |
|---|---|---|---|---|
| **ChatGPT** | OpenAI (EUA) | Uso geral, criação de texto, imagens, voz | Sim | Mais popular; ecossistema grande; recursos avançados na versão paga (Plus) |
| **Claude** | Anthropic (EUA) | Textos longos, análise de documentos, redação cuidadosa, raciocínio | Sim | Forte em documentos extensos e tom profissional; bom para o setor público |
| **Gemini** | Google (EUA) | Integração com Google (Docs, Gmail, Drive), busca | Sim | Bem integrado ao Workspace; bom multimodal |
| **DeepSeek** | DeepSeek (China) | Raciocínio e código a baixo custo | Sim | Bom desempenho e gratuito; **dados podem ir a servidores na China — não subir docs de trabalho** |
| **Qwen** | Alibaba (China) | Multilíngue, código | Sim | Forte em vários idiomas; mesma ressalva de dados das chinesas |
| **Kimi** | Moonshot (China) | Documentos muito longos | Sim | Boa janela de contexto; mesma ressalva de dados |
| **NotebookLM** | Google (EUA) | Pesquisa sobre SUAS fontes, resumos, **áudio e vídeo** | Sim | Você sobe as fontes e ele responde com base nelas; gera podcast e vídeo |
| **Perplexity** | Perplexity (EUA) | Busca na web com fontes citadas | Sim | Ótimo para pesquisa com referências verificáveis |
| **Grok** | xAI (EUA) | Atualidades, integração com X/Twitter | Limitado | Acesso a conteúdo em tempo real do X |

## Qual usar para cada tarefa (guia rápido)

| Tarefa | Recomendação principal | Alternativas |
|---|---|---|
| Analisar um contrato longo / muitos documentos | **Claude** | ChatGPT, Kimi |
| Redigir ofício/relatório formal | **Claude** ou ChatGPT | Gemini |
| Pesquisar leis e normas com fontes | **Perplexity** | NotebookLM (sobre suas fontes) |
| Estudar um conjunto de normativos meus | **NotebookLM** | Claude |
| Gerar áudio (podcast) ou vídeo de um material | **NotebookLM** | — |
| Trabalhar dentro do Google (Docs/Gmail) | **Gemini** | — |
| Criar imagens | **ChatGPT** / Gemini | Grok |
| Testar IA sem custo, conteúdo público | DeepSeek / Qwen | — |

## Geração de vídeo por IA

> Mercado que muda muito rápido — trate as versões como exemplo. Para o servidor, o uso
> mais realista é **comunicação, treinamento e capacitação** (como os vídeos de IMR que já
> foram feitos no NotebookLM), não o trabalho-fim de fiscalização.

| Ferramenta | Empresa / País | Forte em | Observações |
|---|---|---|---|
| **Sora** | OpenAI (EUA) | Vídeo realista a partir de texto | Integrado ao ChatGPT; recursos avançados na versão paga |
| **Veo** | Google (EUA) | Vídeo de alta qualidade **com áudio**; integra ao Gemini | Bom para quem já usa Google |
| **Runway** (Gen-4) | Runway (EUA) | Edição e controle fino; usado por criadores | Ferramentas de edição de vídeo embutidas |
| **Kling / Hailuo** | Kuaishou / MiniMax (China) | Qualidade alta a baixo custo | ⚠️ mesma ressalva de dados das IAs chinesas |
| **NotebookLM (Video Overview)** | Google (EUA) | **Vídeo-resumo explicativo** a partir das SUAS fontes | Melhor opção para transformar normativo/manual em vídeo didático |

- **Para o setor público:** o caso de uso campeão é o **NotebookLM** — vira documento em vídeo
  didático sem precisar saber editar. Sora/Veo servem para peças de comunicação institucional.

## Geração e edição de imagens por IA

| Ferramenta | Forte em | Observações |
|---|---|---|
| **ChatGPT (imagem nativa)** | Seguir instruções, **texto dentro da imagem**, diagramas | Prático: gera e ajusta na própria conversa |
| **Gemini / "Nano Banana"** | **Edição conversacional** de imagens (mudar, remover, combinar) | Excelente para editar uma imagem existente em linguagem natural |
| **Midjourney** | Qualidade estética/artística | Foco em imagem bonita; menos em texto |
| **Adobe Firefly** | **Uso comercial seguro**; integrado ao Photoshop (preenchimento generativo) | Treinado com conteúdo licenciado — importa para direitos autorais |
| **Ideogram** | Imagens com **texto/letreiros** | Bom para banners, avisos |

- **Geração** = criar do zero a partir de texto. **Edição** = alterar uma imagem existente
  (trocar fundo, remover objeto, ampliar) — hoje o **Gemini** se destaca nisso.
- ⚠️ **Cuidado no serviço público:** imagens de IA podem ter **questões de direito autoral** e
  não servem como prova/registro oficial. Use para **comunicação e ilustração**, sinalizando
  que foi gerada por IA. Para uso comercial/institucional, **Firefly** é o mais seguro juridicamente.

## IAs corporativas (Enterprise) — o caminho seguro para o órgão

> Versões pensadas para empresas/governo: **não treinam com seus dados**, têm controle de
> administrador, registro de uso, login institucional (SSO) e garantias contratuais. É o que
> resolve, de verdade, a preocupação de segurança com documentos de trabalho.

| Ferramenta | Empresa | Diferencial corporativo |
|---|---|---|
| **ChatGPT Enterprise / Team** | OpenAI | Sem treino com dados; controles de admin; SSO |
| **Claude for Work (Team/Enterprise)** | Anthropic | Sem treino com dados; foco em segurança; bom p/ documentos longos |
| **Gemini for Workspace / Enterprise** | Google | Integra a Docs, Gmail, Drive do órgão; dados no ambiente Google |
| **Microsoft 365 Copilot** | Microsoft | Dentro de Word, Excel, Outlook, Teams; dados ficam no tenant do órgão |
| **Azure OpenAI / Amazon Bedrock** | Microsoft / AWS | Para **construir sistemas próprios** com governança e residência de dados |

- **Mensagem para a plateia:** se o órgão **contratar uma versão corporativa**, cai a maior
  barreira (privacidade) e o uso com documentos internos fica muito mais seguro. Vale levar
  essa demanda à área de TI/governança.

## Resumo — melhor uso de cada IA (visão de bolso)

| Quero… | Melhor opção | Alternativa |
|---|---|---|
| Analisar contrato/TR longo | **Claude** | ChatGPT, Gemini, Kimi |
| Redigir ofício/relatório formal | **Claude / ChatGPT** | Gemini |
| Trabalhar dentro do Google (Docs/Drive) | **Gemini** | — |
| Trabalhar dentro do Office (Word/Excel) | **Copilot** | — |
| Pesquisar com fontes citadas | **Perplexity** | NotebookLM |
| Estudar meus próprios documentos | **NotebookLM** | Claude |
| Vídeo didático de um normativo | **NotebookLM** | — |
| Vídeo de comunicação institucional | **Veo / Sora** | Runway |
| Criar uma imagem/ilustração | **ChatGPT / Midjourney** | Ideogram |
| Editar uma imagem existente | **Gemini ("Nano Banana")** | Photoshop/Firefly |
| Imagem para uso comercial seguro | **Adobe Firefly** | — |
| Segurança máxima com docs do órgão | **Versão corporativa** (Enterprise) | — |

## Mensagem-chave para o curso
- **Não existe "a melhor IA"** — existe a melhor para cada tarefa.
- Vale ter **2 ou 3 ferramentas** e saber quando usar cada uma.
- Para **documentos de trabalho**, prefira as ocidentais com privacidade configurada
  (ou conta institucional) e **evite as chinesas**.
- Todas **podem errar** — confira sempre.
