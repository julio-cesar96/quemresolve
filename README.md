# Quem Resolve? (nome provisório)

App cívico (PWA) que explica o que é responsabilidade de cada cargo político e encaminha o cidadão para o canal certo de reclamação ou denúncia.

**Fase atual:** 0 — Pesquisa. Ainda não há código.

## Pré-requisitos (macOS)

```bash
brew install node uv   # npx para o Playwright MCP, uvx para fetch e markitdown
```

## Para agentes de IA

Leia `AGENTS.md`. Ele vale para Claude Code, Antigravity e outros.

| | Claude Code | Antigravity |
|---|---|---|
| Regras | `CLAUDE.md` → importa `AGENTS.md` | `AGENTS.md` (nativo) |
| Skills | `.claude/skills/` | `.agents/skills/` (symlinks) |
| Comandos | `/pesquisa` etc. (skills) | `.agent/workflows/` (symlinks) |
| MCPs | `.mcp.json` | `.agents/mcp_config.json` (symlink) |

Edite sempre os arquivos originais em `.claude/` e `.mcp.json`; os symlinks acompanham.

## Rodando a primeira pesquisa

```
/pesquisa docs/prompts/01-pesquisa-competencias-e-ouvidorias.md
/verificar-fontes docs/research/competencias-e-ouvidorias.md
/fechar-fase 0 pesquisa
```
