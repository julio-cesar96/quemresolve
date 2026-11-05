# Fase 0 — Pesquisa e descoberta: resumo de fechamento

> Fechada em 2026-11-05. Prompt executado: [01-pesquisa-competencias-e-ouvidorias.md](../prompts/01-pesquisa-competencias-e-ouvidorias.md)

## O que foi feito

| Arquivo | Conteúdo |
|---|---|
| [competencias.md](../research/competencias.md) | 7 cargos + DF, órgãos não eletivos, matriz de 42 problemas × responsável, o que vereador e deputado podem e não podem fazer, FAQ, "promessa × competência" |
| [ouvidorias.md](../research/ouvidorias.md) | Canais federais, exemplos estaduais e municipais, escadas de escalonamento, emergência |
| [lgpd.md](../research/lgpd.md) | LGPD aplicada ao produto, anônimo × sigiloso, modelo "só redireciona" × "recebe e encaminha", 5 decisões para a Fase 1 |
| [competencias-e-ouvidorias.md](../research/competencias-e-ouvidorias.md) | Índice, perguntas abertas consolidadas e pendências por prioridade |

Método: CF/88 e 13 leis lidas no texto vigente do Planalto, mais páginas oficiais de cerca de 25 órgãos, via navegador (Playwright), porque `fetch` e `curl` falharam por falta de rede. Pesquisa em três partes (A, B, C), mais uma rodada de resolução de pendências (2026-11-04 e 05) e uma conferência final de consistência.

Conclusões principais:

1. Quem executa o serviço depende de quem administra o serviço ou a via. Vereador e deputado legislam e fiscalizam, não executam.
2. Não existe "porta única" de reclamação. O Fala.BR cobre órgãos federais; consumo, telecom, energia e saúde suplementar têm canal próprio.
3. O anonimato varia por canal (Fala.BR e Disque 100 admitem; Pardal e consumidor.gov.br exigem identificação). Isso pesa na decisão de o app só redirecionar ou também receber denúncias.

## O que foi decidido

Nenhuma decisão nova. Vale a ADR existente: [0001](../decisions/0001-foco-em-quem-resolve-sem-recomendar-candidatos.md). As decisões de produto estão listadas abaixo como perguntas abertas.

## Desvios do plano

- Nenhum código nem stack foi escrito ou escolhido.
- `fetch` e `curl` não funcionaram; usei o Playwright para todas as leituras.
- A rodada de resolução de pendências não estava no plano original, foi pedida durante a fase.
- A página da CF no Planalto mistura texto antigo e vigente; só o vigente foi citado.
- A contagem de pendências foi corrigida mais de uma vez. O total de **61** é aproximado, porque algumas pendências aparecem em mais de um relatório.

## Pendências para a Fase 1

### Perguntas abertas (decisões de produto)

| # | Tema | Pergunta | Onde |
|---|---|---|---|
| 1 | Escopo regional | Nacional (só federal + padrão), piloto regional ou diretório completo? | [lgpd.md](../research/lgpd.md) Q1 |
| 2 | Localização | Lista de municípios, CEP ou geolocalização? | lgpd.md Q2 |
| 3 | Offline | Quanto do conteúdo e dos contatos funciona sem rede? | lgpd.md Q3 |
| 4 | Papel do app | Só redirecionar, ajudar a redigir sem enviar, ou receber denúncias? | lgpd.md Q4 |
| 5 | Manutenção | Como manter telefones e URLs atualizados? | lgpd.md Q5 |
| 6 | Roteamento | Como descobrir de quem é a via ou o serviço? | [competencias.md](../research/competencias.md) #1 |
| 7 | Lacunas de conteúdo | Ocultar ou mostrar com aviso as áreas ainda ⚠️? | competencias.md #4 |
| 8 | Variação local | Texto genérico com aviso ou curadoria por município? | competencias.md #5 |
| 9 | Anonimato | Como mostrar o que cada canal afirma, quando é incerto? | [ouvidorias.md](../research/ouvidorias.md) #3 |
| 10 | Emergência | Quais números exibir? (agora há fonte oficial para 190, 192, 193, 199, 191, 180, 100) | ouvidorias.md #4 |
| 11 | Conteúdo opcional | "Promessa × competência" no MVP? Registro local de protocolos? | competencias.md #3; ouvidorias.md #5 |
| 12 | Jurídico | Itens para advogado ou DPO (controlador × operador, base legal, encarregado, crianças) | lgpd.md 1.8 |

### Itens ⚠️ ainda não verificados (cerca de 61)

- **Parte B (26), alta prioridade:**
  - Anonimato de ANEEL, Anatel, ANS, ANAC, ANTT, Banco Central, DPU, Procon, Conselho Tutelar, Ligue 180 e CGU.
  - Ouvidorias e corregedorias das polícias estaduais e controladorias.
  - Atendimento da DPU (o site gov.br/dpu deu 404).
  - Se o Pardal segue ativo fora do período eleitoral.
  - Exemplos do Sul, Norte e Centro-Oeste.
  - Agências de saneamento e de transporte local.
- **Parte A (23):**
  - Lei Orgânica, Constituições estaduais e regimentos.
  - Leis específicas não abertas: Estatuto da Pessoa Idosa, Lei 7.716, Lei 8.213, Bolsa Família, Lei 9.099, Estatuto da Cidade.
  - Judiciário (arts. 92–126).
  - LOAS lida só em parte (arts. 1º, 2º, 6º, 13 e 15).
  - Financiamento do SUS e listas de medicamentos.
  - Percentual das emendas (art. 166, §9º).
- **Parte C (12):** itens que dependem de advogado ou DPO, mais LGPD, ECA Digital, Marco Civil e guias da ANPD não lidos por inteiro.

A lista numerada está na seção **Lacunas** de cada relatório.
