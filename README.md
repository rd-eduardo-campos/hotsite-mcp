---
name: hotsite-mcp-readme
description: Índice e plano do hotsite proposto para comunicação de IA e MCP da RD Station. Lista as 9 páginas, define escopo, status, dependências e ciclo de validação por área. Use este documento quando o usuário pedir contexto sobre o projeto do hotsite, quando precisar saber em que estágio uma página está ou ao planejar a publicação no repositório público.
metadata:
  author: Eduardo Campos
  author-email: eduardo.campos@rdstation.com
  created-at: 2026-05-26T00:00:00-03:00
  updated-at: 2026-05-26T00:00:00-03:00
  updated-by: Eduardo Campos
  updated-by-email: eduardo.campos@rdstation.com
  version: 1.0.0
  status: draft
  approval-status: aguardando-validacao
  destino-final: repositorio-publico-github-rd
---

# Hotsite MCP — RD Station

Hotsite proposto para a comunicação institucional do MCP (Model Context Protocol) e da estratégia de IA da RD Station para o mercado brasileiro.

> **Status:** primeira versão em construção. Conteúdo pronto para revisão das áreas (Marketing, Produto, Conteúdo, Comercial). Quando aprovado, será publicado em repositório público no GitHub para consulta interna e externa.

---

## O que é este hotsite

Um conjunto de 9 páginas estáticas + 1 categoria de blog que organiza a oferta de IA e MCP da RD Station em uma narrativa única e navegável.

A ideia é dupla:

1. **Curto prazo — alinhamento interno.** Servir como base de discussão entre Marketing, Produto, Conteúdo e Comercial sobre como a RD comunica IA e MCP daqui para frente.

2. **Médio prazo — material público.** Quando aprovado e revisado, ser publicado como hotsite oficial. As páginas de recurso de produto (CRM, Marketing, Conversas) podem ser incorporadas como seções dentro de `rdstation.com/produtos/`.

---

## Conteúdo do hotsite

### Estrutura de arquivos

```
disciplinas/hotsite-mcp/
├── README.md                      # Este arquivo — índice e plano
├── _styles.css                    # CSS único compartilhado por todas as páginas (Tangram tokens)
├── index.html                     # Home — organiza todas as páginas
├── o-que-e-mcp.html               # Educativo: MCP para leigos, sem tecniquês
├── glossario.html                 # Glossário de MCP, IA e termos RD Station
├── mcp-crm.html                   # Recurso: MCP do RD Station CRM (55 ferramentas)
├── mcp-marketing.html             # Recurso: MCP do RD Station Marketing (27 ferramentas)
├── mcp-conversas.html             # Recurso: MCP do RD Station Conversas (12 ferramentas)
├── mcp-multiproduto.html          # Estratégia: IA Multiproduto — MCP em cadeia
├── skills-mcp.html                # Prompts prontos por papel, produto e momento
├── ia-mercado-vs-rd.html          # Análise: como o mercado fala de IA vs RD
└── categoria-blog-ia.md           # Nova categoria de blog "Inteligência Artificial" (em PT-BR)
```

### Função de cada página

| Página | O que entrega | Quem revisa |
|---|---|---|
| [`index.html`](index.html) | Hero + cards organizando todas as páginas + tabela comparativa | Marketing + Conteúdo |
| [`o-que-e-mcp.html`](o-que-e-mcp.html) | Explicação simples do MCP, com analogias, casos antes/depois e passo a passo de ativação | Conteúdo + Produto |
| [`glossario.html`](glossario.html) | Definições curtas de MCP, IA, agente, tool, cliente, server e mais | Produto |
| [`mcp-crm.html`](mcp-crm.html) | Página de recurso do MCP do CRM — 55 ferramentas, prompts e casos de uso | Produto + Comercial |
| [`mcp-marketing.html`](mcp-marketing.html) | Página de recurso do MCP do Marketing — 27 ferramentas, prompts e casos de uso | Produto + Comercial |
| [`mcp-conversas.html`](mcp-conversas.html) | Página de recurso do MCP do Conversas — 12 ferramentas, prompts e casos de uso | Produto + Comercial |
| [`mcp-multiproduto.html`](mcp-multiproduto.html) | Fluxos cross-produto: como a IA orquestra Marketing → CRM → Conversas | Produto + Marketing |
| [`skills-mcp.html`](skills-mcp.html) | Coletânea de prompts prontos por papel (vendedor, gestor, analista) | Comercial + Marketing |
| [`ia-mercado-vs-rd.html`](ia-mercado-vs-rd.html) | Análise estratégica: o que o mercado diz, onde estamos à frente, onde temos lacuna | Marketing + Estratégia |
| [`categoria-blog-ia.md`](categoria-blog-ia.md) | Proposta de nova categoria no Blog RD Station: linha editorial, palavras-chave, conteúdos por funil | Conteúdo + SEO |

---

## Como navegar o hotsite

Todas as páginas têm:

- **Header sticky** com navegação para as principais seções
- **Breadcrumb** logo abaixo do header indicando a hierarquia
- **Footer unificado** com links agrupados por finalidade (começando · por produto · estratégia)

Link inicial: abrir `index.html` no navegador. A partir dali, todas as outras páginas são acessíveis em 1 clique.

---

## Design system

- Tokens visuais do **Tangram Design System** da RD Station — exatamente os mesmos usados nas páginas oficiais
- **Cores primárias:** cyan #00DBFF, navy #002233, branco
- **Tipografia:** DM Sans (400, 500, 700, 800)
- **Estrutura responsiva** (mobile, tablet, desktop)
- **CSS único** em `_styles.css` para facilitar manutenção

Quando o hotsite for publicado no GitHub, basta servir os arquivos estáticos. Não há dependência de framework.

---

## Relação com a pasta `hot-site-do-mcp`

Esta pasta (`hotsite-mcp`) **complementa**, não substitui, a pasta `disciplinas/hot-site-do-mcp/`.

| Pasta | Função |
|---|---|
| `disciplinas/hot-site-do-mcp/` | Materiais de **pesquisa e planejamento**: catálogo das 94 ferramentas, anatomia das páginas RD, design system, posicionamento estratégico |
| `disciplinas/hotsite-mcp/` | **Implementação visual** do hotsite — as páginas em HTML, prontas para revisão e publicação |

A pasta de pesquisa permanece como referência para evoluções futuras. A pasta `hotsite-mcp` é o artefato visual.

---

## Ciclo de validação por área

Cada página tem revisores naturais. Sugestão de fluxo de aprovação:

### Etapa 1 — Validação interna (próximas 2 semanas)

| Quem | O que valida |
|---|---|
| Marketing | Mensagens-chave, posicionamento, tom de voz, alinhamento com narrativa "Brasilidades" |
| Produto | Precisão técnica sobre o MCP, número de ferramentas, status de releases |
| Conteúdo | Tom, padrão de escrita, alinhamento com tom-de-voz documentado |
| Comercial | Argumentos de vendas, exemplos de prompt aplicáveis, casos de uso reais |
| Estratégia | Comparativo de mercado, leitura competitiva |

### Etapa 2 — Ajustes editoriais

Após retorno das áreas, consolidação de revisão em uma única passada por página.

### Etapa 3 — Publicação no GitHub

- Criar repositório público (sugestão de nome: `rd-station-mcp-hotsite`)
- Configurar GitHub Pages
- Subir os arquivos
- Configurar domínio público se aprovado pelo time de Marketing

### Etapa 4 — Incorporação nas páginas oficiais

As 3 páginas de recurso (CRM, Marketing, Conversas) podem ser adaptadas como seções dentro de `rdstation.com/produtos/`. O blog category vira parte de `marketing/blog/categorias/`.

---

## O que ainda precisa ser produzido (próximos passos)

### Conteúdo

- [ ] **Vídeos de tutorial** para a página `o-que-e-mcp.html` (Claude Desktop, ChatGPT, n8n, Make)
- [ ] **Cases atribuídos à IA** — pelo menos 3 clientes reescritos com foco em LYNN, Rê e Agentes (ver guia em `docs/varredura-ia/cases-ia-narrativa.html`)
- [ ] **Proof point de produtividade** — coletar dado quantitativo de tempo economizado com MCP/IA
- [ ] **Calculadora de ROI** — interativa, na página de Agentes de IA
- [ ] **Página dedicada do Radar GEO** com bridge para produtos
- [ ] **Posts pilares do blog** (5 primeiros da categoria Inteligência Artificial)

### Visual

- [ ] **Diagramas SVG** para a página `mcp-multiproduto.html` (fluxos visuais)
- [ ] **Screenshots de produto** — Claude Desktop conectado ao MCP, exemplos reais de conversa
- [ ] **Ícones próprios** para LYNN, Rê e Agentes (avatares)
- [ ] **OG images** para compartilhamento social de cada página

### Produto / Dev

- [ ] Validar URLs públicas do MCP (`mcp.rdstationmentor.com/crm`, etc) e estabilidade
- [ ] Confirmar que o número de 94 ferramentas está correto e atualizado
- [ ] Sincronizar com release notes para que o hotsite reflita estado atual do produto

---

## Checklist de aprovação por página

Antes de publicar, cada página precisa do "ok" em cada item abaixo.

| Página | Marketing | Produto | Conteúdo | Comercial |
|---|---|---|---|---|
| `index.html` | ☐ | ☐ | ☐ | – |
| `o-que-e-mcp.html` | ☐ | ☐ | ☐ | – |
| `glossario.html` | – | ☐ | ☐ | – |
| `mcp-crm.html` | ☐ | ☐ | ☐ | ☐ |
| `mcp-marketing.html` | ☐ | ☐ | ☐ | ☐ |
| `mcp-conversas.html` | ☐ | ☐ | ☐ | ☐ |
| `mcp-multiproduto.html` | ☐ | ☐ | – | ☐ |
| `skills-mcp.html` | ☐ | – | ☐ | ☐ |
| `ia-mercado-vs-rd.html` | ☐ | – | ☐ | – |
| `categoria-blog-ia.md` | ☐ | – | ☐ | – |

---

## Premissas e dados usados

Conteúdo construído com base nos seguintes documentos do vault:

- **Catálogo de ferramentas:** `disciplinas/hot-site-do-mcp/catalogo-mcp-rd-station.md` — fonte das 94 ferramentas em 3 servidores
- **Anatomia das páginas RD:** `disciplinas/hot-site-do-mcp/anatomia-das-paginas-rd.md` — padrões estruturais do site
- **Design system:** `disciplinas/hot-site-do-mcp/design-system-rd.md` + `docs/_template/tangram.css` — tokens e classes
- **Posicionamento vs mercado:** `disciplinas/hot-site-do-mcp/posicionamento-mcp-vs-mercado.md` — análise competitiva
- **Tom de voz:** `marketing/tom-de-voz/tom-de-voz.md` — manual da RD baseado em 41 posts do blog
- **Benchmark de IA:** `docs/varredura-ia/concorrentes-ia-benchmark.html` — varredura de 25/05/2026
- **Briefing IA:** `docs/varredura-ia/briefing-ia-paginas-produto.html` — auditoria das páginas atuais
- **Cases de IA:** `docs/varredura-ia/cases-ia-narrativa.html` — framework de cases atribuídos à IA

---

## Convenções deste hotsite

- **Sem citar concorrentes pelo nome.** As referências de mercado são genéricas ("padrão do mercado", "players globais") — alinhado com prática RD de comunicação institucional
- **"Você" como sujeito** em todas as páginas — segunda pessoa, tom educativo com calor humano
- **MCP sempre traduzido** quando aparece pela primeira vez em uma página
- **Cores de produto:** roxo para CRM, ciano para Marketing, verde para Conversas — usado em badges e bordas
- **CTAs sempre em ação direta:** "Conectar agora", "Ver casos de uso", "Ativar MCP do CRM"

---

## Como rodar localmente

Não precisa de build. É HTML estático:

```bash
cd disciplinas/hotsite-mcp
python3 -m http.server 8080
# abrir http://localhost:8080
```

Ou abrir `index.html` diretamente no navegador.

---

## Versão e histórico

- **v1.0.0 (26/05/2026):** primeira versão do hotsite com 9 páginas HTML + 1 categoria de blog. Pronto para revisão das áreas.

---

## Contato

Owner do projeto: Eduardo Campos (eduardo.campos@rdstation.com)

Para sugestões, abrir issue no repositório quando publicado, ou alinhar diretamente pelos canais internos da RD Station.
