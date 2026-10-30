---
name: research-report
description: Formato padrão para relatórios de pesquisa em docs/research/. Use ao escrever ou revisar qualquer arquivo de pesquisa do projeto, para manter estrutura, níveis de confiança e lista de fontes consistentes.
---

# Formato de relatório de pesquisa

Salvar em `docs/research/<tema-em-kebab-case>.md`. Use `templates/relatorio.md` como esqueleto.

## Regras

- Abrir com **Resumo** de no máximo 5 linhas: o que foi pesquisado e as 3 conclusões principais.
- Preferir **tabelas** para mapeamentos (cargo × responsabilidade, problema × responsável × canal).
- Cada linha de tabela ou afirmação factual leva marca de confiança (`✅` / `🟡` / `⚠️`) e referência numérica à lista de Fontes, ex.: `[3]`.
- Linguagem simples, como se fosse explicar para um cidadão leigo. Termos jurídicos aparecem entre parênteses depois da explicação.
- Seção **Lacunas** lista o que não foi possível verificar e por quê.
- Seção **Perguntas abertas** lista decisões de produto que a pesquisa levantou (formato: pergunta, opções, impacto).
- Seção **Fontes** numerada: título, URL, data de acesso (AAAA-MM-DD).
- Não incluir código nem decisões de stack.

## Checklist antes de salvar

- [ ] Nenhum URL, telefone ou artigo sem verificação está marcado como ✅
- [ ] Toda linha de tabela tem fonte
- [ ] Executivo vs. Legislativo explícito onde importa
- [ ] Nenhum político ou partido citado
- [ ] Lacunas e Perguntas abertas preenchidas
