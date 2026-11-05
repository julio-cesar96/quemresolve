# Competências e ouvidorias: índice da pesquisa (prompt 01)

> Fase 0 — Pesquisa · Atualizado em 2026-11-04
> Este arquivo é só o **índice**: resumo de cada parte, perguntas abertas consolidadas e lista de pendências ⚠️. O conteúdo está nos três relatórios.
> Legenda: ✅ verificado na fonte primária · 🟡 fonte secundária ou interpretação · ⚠️ não verificado

## Relatórios

| Parte | Arquivo | Acesso às fontes | Resumo |
|---|---|---|---|
| A — Competências | [competencias.md](competencias.md) | 2026-11-03 | 7 cargos + DF, 42 problemas na matriz, vereador/deputado, FAQ, promessa × competência. Quem executa × quem legisla. Muitos casos "dependem de quem administra o serviço ou a via". |
| B — Canais | [ouvidorias.md](ouvidorias.md) | 2026-11-04 | Canais federais (Fala.BR, MPF, TCU, agências, Banco Central, consumidor.gov.br), exemplos estaduais e municipais, escadas de escalonamento, emergência. Anonimato varia por canal. |
| C — LGPD e decisões | [lgpd.md](lgpd.md) | 2026-11-04 | LGPD, anônimo × sigiloso, modelo "só redireciona" × "recebe e encaminha", 5 decisões para a Fase 1. |

Fontes primárias: texto vigente da CF/88 e de 12 leis no Planalto (8.080, 9.503, 13.460, 12.527, 9.394, 8.078, 9.504, 8.069, 11.340, 11.445, 13.709, 13.608), mais páginas oficiais de ~25 órgãos. Detalhes em cada relatório.

## Perguntas abertas consolidadas

Decisões para a **Fase 1** (nenhuma foi tomada na pesquisa).

| # | Tema | Pergunta | Onde |
|---|---|---|---|
| 1 | Escopo regional | Nacional (só federal + padrão), piloto regional ou diretório completo? | [lgpd.md](lgpd.md) Q1 |
| 2 | Localização | Lista de municípios, CEP ou geolocalização? | [lgpd.md](lgpd.md) Q2 |
| 3 | Offline | Quanto do conteúdo e dos contatos funciona sem rede? | [lgpd.md](lgpd.md) Q3 |
| 4 | Papel do app | Só redirecionar, ajudar a redigir sem enviar, ou receber denúncias? | [lgpd.md](lgpd.md) Q4 |
| 5 | Manutenção | Como manter telefones e URLs atualizados? | [lgpd.md](lgpd.md) Q5; [ouvidorias.md](ouvidorias.md) #1–2 |
| 6 | Roteamento | Como descobrir de quem é a via/serviço (municipal, estadual, federal)? | [competencias.md](competencias.md) #1 |
| 7 | Lacunas de conteúdo | Ocultar ou mostrar com aviso as áreas ainda ⚠️ (idoso, discriminação, assistência social)? | [competencias.md](competencias.md) #4 |
| 8 | Variação local | Texto genérico com aviso ou curadoria por município (Lei Orgânica, regimentos)? | [competencias.md](competencias.md) #5 |
| 9 | Anonimato | Como mostrar o que cada canal afirma sobre anonimato, quando é incerto? | [ouvidorias.md](ouvidorias.md) #3 |
| 10 | Emergência | Exibir 190/193 só depois de verificar em fonte oficial? | [ouvidorias.md](ouvidorias.md) #4 |
| 11 | Conteúdo opcional | Seção "promessa × competência" no MVP (ADR 0001)? Registro local de protocolos? | [competencias.md](competencias.md) #3; [ouvidorias.md](ouvidorias.md) #5 |
| 12 | Jurídico | Itens para advogado/DPO: controlador × operador, base legal, dispensa de encarregado, transferência internacional, crianças (ECA Digital) | [lgpd.md](lgpd.md) 1.8 |

## Pendências ⚠️ (todas)

Total: **61** (A: 23 · B: 26 · C: 12; alguns itens aparecem em mais de um relatório, então a soma pode contar a mesma pendência duas vezes). Eram 73 antes da rodada de resolução de 2026-11-04 (A: 27 · B: 34 · C: 12). A lista completa e numerada está na seção **Lacunas** de cada relatório (itens resolvidos aparecem riscados); abaixo, o resumo por tema.

### Alta prioridade (afetam segurança ou o fluxo central)

- **Emergência:** ~~190, 193, Disque 100 e Ligue 180~~ ✅ resolvidos em 2026-11-04 (190, 192, 193, 199, 191, 180 e 100 verificados). Restam o anonimato do Ligue 180 e o atendimento da DPU. ([ouvidorias.md](ouvidorias.md))
- **Justiça Eleitoral:** ~~canal local~~ ✅ resolvido (Pardal, Eleições 2026, exige e-Título/gov.br, com sigilo). Novo ⚠️: se o Pardal segue ativo fora do período eleitoral.
- **Ouvidorias de polícia e controle:** ~~controle externo pelo MP (CF art. 129, VII)~~ ✅; PF e PRF ✅. Seguem ⚠️: ouvidorias/corregedorias das polícias estaduais e controladorias. (B-7)
- **De quem é a via/serviço:** como identificar a circunscrição (A-11); agências de saneamento e de transporte local (B-9, A-12).
- **Anonimato:** Fala.BR ✅ (opção anônima, segundo a PF) e Disque 100 ✅. Seguem ⚠️: ANEEL, Anatel, ANS, ANAC, ANTT, Banco Central, DPU, Procon, Conselho Tutelar, Ligue 180, CGU. (B-2)

### Média prioridade (conteúdo)

- Competências por nível: ~~CF art. 204, art. 61 §2º, IPVA/IR~~ ✅ resolvidos em 2026-11-04. Seguem ⚠️: Lei 8.742 (LOAS), art. 21, XIV (redação completa, polícias do DF), financiamento e listas do SUS, Lei 8.080 art. 16, Lei 11.445 art. 3º, percentual das emendas (art. 166 §9º). (A-4, A-5, A-7 a A-10)
- Leis específicas não abertas: Estatuto da Pessoa Idosa, Lei 7.716, Lei 8.213, Bolsa Família/CadÚnico, Lei 9.099, Estatuto da Cidade, Judiciário (arts. 92–126). (A-15, A-16, A-18, A-19, A-23)
- Regras locais: Lei Orgânica, Constituições estaduais, regimentos das Casas, regras de calçada e poluição sonora. (A-1 a A-3, A-21, A-22)
- Contatos: ~~telefone da ANTT~~ ✅ (166, 2026-11-05); telefone da DPU, contatos de Procon-PE, TCE-PE e DPE-PE, Conselho Tutelar por município, adesão ao Fala.BR, exemplos de Sul/Norte/Centro-Oeste. (B-3, B-10 a B-15)
- Anonimato e protocolo de denúncias anônimas fora do MPSP. (C-9)

### Jurídico / LGPD (depende de advogado ou DPO)

- LGPD: artigos truncados ou não lidos (4º III, 6º IV–X, 18 VI–IX, 26–27, 33+), regulamento da ANPD (pequeno porte), guias da ANPD (só links), ECA Digital, Marco Civil, Código Penal, Lei 9.807, decretos federais de ouvidoria; classificação de CEP/localização; papel do app como controlador/operador; aceite dos órgãos para receber denúncias. (C-1 a C-8, C-10 a C-12)

## Nota de processo

- Pesquisa feita em três rodadas (A: 2026-11-03; B e C: 2026-11-04), com parada e "seguir" a cada parte, como pede o prompt.
- Textos legais foram lidos no Planalto pelo navegador (Playwright), pois `fetch` e `curl` falharam por falta de rede. A página da CF mostra texto antigo e vigente lado a lado; só citei o vigente.
- Decisões de produto e de stack **não** foram tomadas. Ver `docs/decisions/` na Fase 1.

- **Rodada de resolução (2026-11-04):** resolvidos 190, 193 (e 199, 191), Disque 100, Ligue 180 (horário e canais), anonimato do Fala.BR, Pardal (Justiça Eleitoral), controle externo da polícia (CF art. 129, VII) e CF arts. 61 §2º, 153 III, 155 III e 204. **Não resolvidos** por falta de página oficial acessível: telefone da ANTT, atendimento da DPU (404), polícias estaduais, Sul/Norte/Centro-Oeste, e itens jurídicos de LGPD.
