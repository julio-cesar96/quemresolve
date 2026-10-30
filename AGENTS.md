# AGENTS.md

Fonte única da verdade para qualquer agente de IA trabalhando neste repositório (Claude Code, Antigravity, Codex, Cursor etc.). `CLAUDE.md` apenas importa este arquivo. Em caso de divergência entre documentos, **este arquivo prevalece**.

## O projeto

**Quem Resolve?** (nome provisório) — aplicativo de utilidade pública e educação cívica, distribuído como **PWA** (sem loja no MVP; empacotamento via Capacitor/TWA fica para depois, se fizer sentido).

Objetivos do produto:

1. Explicar ao cidadão, em linguagem simples, **o que é responsabilidade de cada cargo**: Prefeito, Governador, Presidente, Vereadores, Deputados Estaduais, Deputados Federais e Senadores.
2. **Rotear** o cidadão para o canal certo (ouvidoria, órgão de controle, Procon, MP etc.) quando um serviço público não funciona.

Fluxo central que todo o produto serve:

```
problema do dia a dia → quem é responsável (nível + cargo/órgão) → onde e como reclamar/denunciar
```

## Fase atual: PESQUISA

Estamos na **Fase 0 — Pesquisa e descoberta**. Nesta fase:

- **Não escrever código de aplicação.** Nada de `src/`, `package.json`, frameworks ou scaffolding de app.
- Toda saída vai para `docs/` em Markdown.
- Stack técnica **não está decidida**. Não presumir Next.js, React, Vite ou backend. Recomendações de stack só entram como opção em `docs/decisions/`, nunca como fato.

Fases previstas (não antecipar trabalho de fase posterior sem pedido explícito):

| Fase | Entrega | Pasta |
|---|---|---|
| 0 — Pesquisa | Mapeamento de competências, canais, LGPD, perguntas abertas | `docs/research/` |
| 1 — Decisões de produto | Respostas às perguntas abertas, escopo do MVP | `docs/decisions/` |
| 2 — Especificação técnica | Stack, modelo de dados, arquitetura do PWA | `docs/spec/` |
| 3+ — Implementação | Código | a definir |

## Regras de pesquisa (inegociáveis)

1. **Fonte primária sempre.** Prioridade: Constituição Federal (planalto.gov.br) > leis e decretos (planalto.gov.br, LexML) > portais oficiais (gov.br, sites de órgãos) > fontes secundárias confiáveis. Blogs, fóruns e conteúdo de IA não contam como fonte.
2. **Toda afirmação factual precisa de fonte** com URL e data de acesso. Artigos de lei citados pelo número (ex.: "CF/88, art. 30, V").
3. **Nunca inventar URL, telefone, e-mail ou número de artigo.** Se não encontrou ou não conseguiu abrir a página, escrever `⚠️ NÃO VERIFICADO` e seguir.
4. **Marcar confiança**: `✅ verificado na fonte primária`, `🟡 fonte secundária`, `⚠️ não verificado`.
5. **Competência comum e concorrente existe.** Saúde, educação, meio ambiente etc. são compartilhados entre níveis (CF/88, arts. 23 e 24). Não simplificar para "é só do prefeito" quando a resposta real é "depende"; explicar como a responsabilidade se divide na prática.
6. **Executivo ≠ Legislativo.** Vereadores e deputados não executam serviços (não tapam buraco nem compram remédio): legislam, fiscalizam, aprovam orçamento e propõem emendas. A pesquisa deve deixar isso explícito, porque é a confusão mais comum do público.
7. **Neutralidade.** Produto apartidário. Sem citar partidos, políticos atuais ou linguagem de campo político. Exemplos usam cargos, nunca pessoas.
8. **Copyright.** Parafrasear; citações literais só de texto legal (que é de domínio público) ou trechos curtos com aspas e fonte.

## Convenções de documentos

- Idioma: português do Brasil.
- Formato de relatório de pesquisa: usar a skill `research-report`.
- Metodologia de pesquisa cívica e lista de fontes oficiais: skill `civic-research`.
- Nomes de arquivo: `kebab-case.md`, sem acentos.
- Cada relatório termina com **Perguntas abertas** e **Fontes**.
- Decisões tomadas viram ADR curto em `docs/decisions/NNNN-titulo.md` (contexto, opções, decisão, consequências).

## Estrutura do repositório

```
AGENTS.md                 ← você está aqui (fonte da verdade; lido pelo Antigravity e outros)
CLAUDE.md                 ← importa AGENTS.md (Claude Code)
.claude/skills/           ← skills (originais), inclusive as de comando: pesquisa, verificar-fontes, fechar-fase
.claude/settings.json     ← permissões do Claude Code
.agents/skills/           ← symlinks para .claude/skills (Antigravity e outros)
.agent/workflows/         ← symlinks para os SKILL.md de comando (slash commands no Antigravity)
.mcp.json                 ← MCPs do projeto (Claude Code)
.agents/mcp_config.json   ← symlink para .mcp.json (Antigravity)
docs/
  prompts/                ← prompts versionados de cada etapa
  research/               ← Fase 0
  decisions/              ← Fase 1 (ADRs)
  spec/                   ← Fase 2
  progresso/              ← resumo ao fim de cada fase
```

## Ao final de cada fase

Registrar um resumo em `docs/progresso/fase-N-nome-curto.md` com: o que foi feito, o que foi decidido, desvios do plano, pendências para a próxima fase. Use o comando `/fechar-fase`.
