# Prompt 01 — Pesquisa: competências e ouvidorias (v2)

> Rodar com: `/pesquisa docs/prompts/01-pesquisa-competencias-e-ouvidorias.md`
> Executar **uma parte por vez** (A, B, C). Ao terminar cada parte: parar, listar pendências (`⚠️ NÃO VERIFICADO`) e aguardar o "seguir".
> Papel, regras de fonte e formato: `AGENTS.md` e skills `civic-research` e `research-report`. Em divergência, `AGENTS.md` prevalece.
> A parte a executar vem depois do caminho (ex.: `... parte B`). Se nenhuma for indicada, executar **só a Parte A**.

Atue como Arquiteto de Software e Pesquisador de Produtos Cívicos. Estamos na Fase 0 (Pesquisa) do app descrito no `AGENTS.md`. Não implemente código.

## Antes de começar

1. Confirmar que existem e ler `competencias-ponto-de-partida.md`, `fontes-oficiais.md` e `lgpd-ponto-de-partida.md` (caminho: `.claude/skills/civic-research/references/`). Se algum faltar, **parar e avisar**. Não reconstruir de memória.
2. Registrar no topo de cada relatório a data real de acesso e o escopo coberto.

## Público e escopo

- Público: cidadão comum, sem conhecimento jurídico. Texto simples primeiro; base legal em bloco separado.
- Cargos: Prefeito, Governador, Presidente, Vereador, Deputado Estadual, Deputado Federal, Senador, **mais** nota sobre o Distrito Federal (Deputado Distrital, sem Vereador) e seção curta sobre quem **não** é cargo eletivo mas é confundido com eles (juiz, promotor, delegado, agências reguladoras).
- Profundidade dos canais: **federal** completo; **estadual** e **municipal** como padrão ("onde encontrar") + até 3 exemplos reais cada, de regiões diferentes, marcados como exemplo. Não tentar cobrir 27 UFs nem 5.570 municípios.
- Fora de escopo: nomes de pessoas e partidos, dados de candidatos, parecer jurídico, valores em R$ sem fonte

## Parte A — Competências → `docs/research/competencias.md`

**A1. Os 7 cargos.** Para cada um: o que faz no dia a dia, base legal (CF/88 ou lei, com artigo), Executivo ou Legislativo, e o que **pode** e **não pode** resolver.

**A2. Matriz problema → responsável.** Usar os problemas da referência e **garantir cobertura mínima** destas áreas (acrescentar o que faltar, marcando como "adição"): saúde; educação; segurança pública; trânsito e transporte coletivo; vias e obras (buraco, calçada, iluminação, drenagem); saneamento, lixo e limpeza urbana; energia, telefonia e internet; meio ambiente e poluição sonora; assistência social e benefícios (CadÚnico, Bolsa Família, INSS); moradia; consumo (banco, plano de saúde, operadora, compras); trabalho; direitos (violência doméstica, criança e adolescente, idoso, discriminação); mau uso de dinheiro público e conduta de servidor; acesso à informação pública; propaganda eleitoral irregular e compra de voto; demora e acesso à Justiça.

- Colunas: ID (P01…) · problema · quem executa · quem financia/regula (se diferente) · papel do Legislativo · confiança · fonte (número `[n]`).
- Competência compartilhada: não escolher um nível. Explicar a divisão em bloco abaixo da tabela.
- Incluir explicitamente os casos de fronteira: **quem administra a via** (federal/estadual/municipal), **serviço concedido** e **público vs. privado**.

**A3. O que vereador e deputado podem fazer pelo cidadão** (pedido de providência, indicação, requerimento de informação, fiscalização, emenda), sem prometer resolução. Regimentos variam: marcar o que não for verificado.

**A4. FAQ do cidadão** (respostas de até 3 frases, com fonte): quem cuida da minha rua? · vereador/deputado pode resolver meu problema? · já reclamei e nada aconteceu, e agora? · qual a diferença entre ouvidoria, Procon, MP, Defensoria e Tribunal de Contas? · posso denunciar sem me identificar? · qual o prazo de resposta e como acompanho o protocolo? · é caso de polícia ou de ouvidoria? · o que é emenda parlamentar e quem decide onde vai? · quem fiscaliza prefeito, governador e presidente? · preciso de advogado? · moro no DF: quem é quem?

**A5. Promessa × competência do cargo.** Para cada um dos 7 cargos (e o DF), liste em linguagem simples exemplos de promessas que **cabem** ao cargo, que **não cabem** e que **dependem de outro nível ou poder** (lei, orçamento, parceria), com base legal. Incluir um checklist de 5 a 8 perguntas que o eleitor pode fazer a qualquer candidato ("isso é atribuição do cargo?", "precisa de lei? quem aprova?", "de onde vem o dinheiro?"). Só competência e viabilidade formal: nunca avaliar se a promessa é boa nem se será cumprida. Sem partidos nem pessoas (regra 7, ADR 0001).

## Parte B — Canais → `docs/research/ouvidorias.md`

**B1. Canais oficiais.** Incluir órgãos que não são cargos eletivos: Ministérios Públicos, Tribunais de Contas, Defensorias, Controladorias, ouvidorias das polícias, Procon, agências reguladoras (ANS, Anatel, ANEEL, ANAC e as de saneamento e transporte aplicáveis), Banco Central, consumidor.gov.br, Fala.BR, Conselho Tutelar, Justiça Eleitoral. Por canal: o que aceita · esfera · aceita anônimo (com fonte) · URL oficial · confiança.

**B2. Padrão estadual e municipal.** Onde encontrar, com até 3 exemplos reais cada, marcados como exemplo.

**B3. Escadas de escalonamento** (com prazos legais de resposta quando houver fonte): serviço concedido (empresa → agência/órgão → MP/Procon); serviço público direto; conduta policial; consumo privado.

**B4. Emergência vs. ouvidoria.** Telefones de emergência e proteção (polícia, SAMU, bombeiros, violência contra a mulher, crianças), confirmados em fonte oficial, e o aviso de que ouvidoria não substitui emergência.

## Parte C — LGPD e perguntas abertas → `docs/research/lgpd.md` + índice

**C1. LGPD.** Responder às perguntas da referência, comparando "app só redireciona" e "app recebe e encaminha a denúncia", e diferenciando denúncia anônima de identificada com sigilo. Separar em três blocos: (i) o que a lei diz (com artigo), (ii) interpretação, (iii) recomendação de produto. Não é parecer jurídico: indicar o que exigiria advogado ou DPO. Normas candidatas, a **confirmar no texto vigente**: Lei 13.709/2018, Lei 12.527/2011, Lei 13.460/2017, Lei 13.608/2018.

**C2. Perguntas abertas.** 3 a 5 decisões estratégicas de produto para a Fase 1 (escopo regional inicial, busca por CEP/geolocalização, offline, redirecionar vs. receber denúncias, manutenção dos contatos municipais). Para cada uma: opções, prós e contras, impacto em custo **qualitativo** (baixo/médio/alto) com a premissa. Não decidir: decisão é da Fase 1.

## Regras anti-erro

- `✅` só se a página foi aberta nesta sessão e o dado foi lido nela. Página bloqueada ou que não abriu: `⚠️ NÃO VERIFICADO`. Não substituir por memória nem por fonte secundária sem rotular `🟡`.
- URL, telefone e e-mail: copiar da página oficial. Nunca deduzir padrão de domínio.
- Exemplos de estado e município: só os que foram efetivamente acessados.
- Artigos de lei: conferir o texto vigente (alterações posteriores).
- Não afirmar "aceita anônimo" nem prazos sem fonte por canal.
- Na dúvida entre "um nível" e "compartilhado": registrar "depende" e explicar.

## Formato e critério de pronto

- Fonte nas tabelas por número `[n]`; lista de Fontes no fim com URL, data de acesso e confiança.
- Seguir o template da skill `research-report`: Resumo (até 5 linhas), tabelas, **Lacunas**, **Perguntas abertas** e **Fontes**, nesta ordem.
- `docs/research/competencias-e-ouvidorias.md` fica como **índice**: resumo de cada parte, perguntas abertas consolidadas e lista de todos os `⚠️` pendentes.
- Pronto quando: os 7 cargos e o DF estão cobertos; toda área da cobertura mínima tem linha na matriz; todo canal tem URL `✅` ou `⚠️`; nenhuma afirmação factual está sem fonte; a lista de pendências está no índice.