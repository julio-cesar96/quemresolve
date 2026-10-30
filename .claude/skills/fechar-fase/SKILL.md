---
name: fechar-fase
description: Registra o resumo de uma fase concluída em docs/progresso/. Use quando o usuário pedir /fechar-fase ou disser que uma fase terminou.
argument-hint: <número da fase> <nome-curto>
disable-model-invocation: true
---

# Fechar fase

Fase: $ARGUMENTS

(No Antigravity, número e nome são o texto digitado depois do comando.)

Crie `docs/progresso/fase-<N>-<nome-curto>.md` com:

- **O que foi feito** (arquivos gerados em `docs/`)
- **O que foi decidido** (link para ADRs em `docs/decisions/`, se houver)
- **Desvios do plano** em relação ao `AGENTS.md`
- **Pendências** para a próxima fase (inclua todos os ⚠️ e perguntas abertas ainda sem resposta)

Depois, se a próxima fase mudar regras de trabalho, proponha a edição necessária no `AGENTS.md` (seção "Fase atual"), sem aplicar sem confirmação.
