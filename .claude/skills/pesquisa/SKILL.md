---
name: pesquisa
description: Executa uma tarefa de pesquisa da Fase 0 sobre um tema (ou a partir de um prompt em docs/prompts/) e salva o relatório em docs/research/. Use quando o usuário pedir /pesquisa ou pedir para rodar um prompt de pesquisa.
argument-hint: <tema ou caminho de um prompt em docs/prompts/>
disable-model-invocation: true
---

# Pesquisa (Fase 0)

Tarefa: $ARGUMENTS

(No Antigravity, a tarefa é o texto digitado depois do comando.)

Se a tarefa for um caminho de arquivo em `docs/prompts/`, leia o arquivo e siga as instruções dele.

1. Carregue as skills `civic-research` e `research-report`.
2. Leia as referências da skill `civic-research` relevantes ao tema.
3. Pesquise em fontes primárias. Para ler textos longos de lei com precisão, prefira o MCP `fetch` (texto integral) ao resumo da busca; para PDFs, use o MCP `markitdown`; para sites que dependem de JavaScript, use o MCP `playwright`.
4. Não escreva código.
5. Salve o relatório em `docs/research/` no formato da skill `research-report`.
6. Ao final, responda com: caminho do arquivo, as 3 conclusões principais e quantos itens ficaram ⚠️.
