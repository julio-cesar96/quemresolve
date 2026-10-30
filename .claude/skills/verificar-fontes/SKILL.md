---
name: verificar-fontes
description: Revisa um relatório de docs/research/ como verificador independente, conferindo cada fonte e afirmação. Use quando o usuário pedir /verificar-fontes ou uma revisão de fontes de um relatório.
argument-hint: <caminho do relatório em docs/research/>
disable-model-invocation: true
---

# Verificar fontes

Relatório a revisar: $ARGUMENTS

(No Antigravity, o caminho é o texto digitado depois do comando.)

Trabalhe como se não tivesse escrito o relatório. De preferência, rode isto numa sessão nova.

1. Para cada item marcado ✅, abra a URL citada (MCP `fetch`) e confirme que ela sustenta a afirmação: artigo, nome do sistema, escopo.
2. Rebaixe para 🟡 ou ⚠️ o que não se confirmar e anote o motivo.
3. Procure URLs, telefones ou artigos que possam ter sido inventados.
4. Confira se há simplificações erradas de competência (ex.: tratar saúde como exclusiva do município).
5. Edite o arquivo com as correções e adicione no fim uma seção `## Revisão (AAAA-MM-DD)` listando o que mudou.
