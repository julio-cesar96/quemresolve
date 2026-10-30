# CLAUDE.md

Instruções do projeto ficam em `AGENTS.md` (compartilhado com Antigravity e outros agentes). Não duplicar regras aqui.

@AGENTS.md

## Específico do Claude Code

- Skills do projeto: `.claude/skills/` (`civic-research`, `research-report`).
- Comandos (também são skills): `/pesquisa <tema>`, `/verificar-fontes <arquivo>`, `/fechar-fase <N> <nome>`.
- MCPs: `.mcp.json` na raiz (`fetch`, `markitdown`, `playwright`). Aprovar na primeira execução.
- Permissões: `.claude/settings.json`. Ajustes pessoais vão em `.claude/settings.local.json` (fora do git).
