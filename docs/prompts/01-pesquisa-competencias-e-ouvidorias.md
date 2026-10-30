# Prompt 01 — Pesquisa: competências e ouvidorias

> Rodar com: `/pesquisa docs/prompts/01-pesquisa-competencias-e-ouvidorias.md`
> Papel, regras de fonte e formato já estão em `AGENTS.md` e nas skills `civic-research` e `research-report`.

Atue como Arquiteto de Software e Pesquisador de Produtos Cívicos. Estamos na Fase 0 (Pesquisa) do app descrito no `AGENTS.md`. Não implemente código.

## Tarefas

### 1. Mapeamento de competências

Para cada cargo (Prefeito, Governador, Presidente, Vereador, Deputado Estadual, Deputado Federal, Senador), descreva em linguagem simples:

- o que faz no dia a dia, com base legal (artigo da CF/88 ou lei);
- se é Executivo ou Legislativo, e o que isso significa na prática para o cidadão (o que o cargo **pode** e **não pode** resolver).

Em seguida, monte a **matriz problema → responsável** usando os problemas-exemplo da referência `competencias-ponto-de-partida.md`. Colunas: problema · nível responsável pela execução · quem financia/regula (se diferente) · papel do Legislativo · confiança · fonte. Quando a competência for compartilhada, explique a divisão em vez de escolher um único nível.

### 2. Canais e ouvidorias

Mapeie os canais oficiais de reclamação e denúncia, incluindo órgãos que não são cargos eletivos (Ministérios Públicos, Tribunais de Contas, Defensorias, Controladorias, ouvidorias das polícias, Procon, agências reguladoras, consumidor.gov.br, Fala.BR). Para cada canal: o que aceita, esfera, se aceita anônimo, URL oficial verificada.

Para canais que variam por município ou estado, documente o **padrão** de onde encontrá-los, com 2 ou 3 exemplos reais marcados como exemplo. Inclua a **escada de escalonamento** para serviços concedidos (empresa → agência/órgão → MP/Procon).

### 3. Privacidade e LGPD

Responda às perguntas da referência `lgpd-ponto-de-partida.md`, comparando os modelos "app só redireciona" e "app recebe e encaminha a denúncia", e diferenciando denúncia anônima de identificada com sigilo.

### 4. Perguntas abertas

Liste de 3 a 5 decisões estratégicas de produto a tomar antes da especificação técnica (ex.: escopo regional inicial, busca por CEP/geolocalização, suporte offline, redirecionar vs. receber denúncias, manutenção dos dados de contato municipais). Para cada uma: opções, prós e contras, impacto em custo.

## Saída

Salvar em `docs/research/competencias-e-ouvidorias.md`, no formato da skill `research-report`. Se o arquivo passar de ~600 linhas, dividir em `competencias.md`, `ouvidorias.md` e `lgpd.md` e deixar `competencias-e-ouvidorias.md` como índice.
