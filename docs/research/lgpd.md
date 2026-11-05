# LGPD, denúncias e perguntas abertas

> Fase 0 — Pesquisa · Parte C do prompt 01 · Atualizado em 2026-11-04 · Data de acesso a todas as fontes: 2026-11-04
> Escopo: o que a LGPD e as leis de ouvidoria/denúncia dizem sobre um app que **só redireciona** ou **recebe e encaminha** reclamações; anonimato × sigilo; 5 decisões estratégicas para a Fase 1.
> **Não é parecer jurídico.** Onde a resposta exigiria advogado ou encarregado (DPO), está indicado.
> Legenda: ✅ verificado na fonte primária (página aberta e lida nesta sessão) · 🟡 fonte secundária ou interpretação minha · ⚠️ não verificado
> Referências `[C n]`: lista de Fontes de [competencias.md](competencias.md); `[B n]`: lista de Fontes de [ouvidorias.md](ouvidorias.md).

## Resumo

Li o texto vigente da Lei 13.709 (LGPD), da Lei 13.608 (denúncia e proteção do informante) e o art. 31 da LAI; os demais (Lei 13.460) vieram da Parte A. Conclusões: (1) a LGPD vale também para o setor privado e para meios digitais, então **qualquer app que trate dado de pessoa identificável está sob ela**; o que muda é o tamanho da carga; (2) **anônimo e sigiloso são coisas diferentes**: anônima não identifica ninguém (e pode ser arquivada por falta de elementos), sigilosa identifica mas protege a identidade (Lei 13.608, arts. 3º e 4º-B); (3) o modelo "só redireciona" reduz muito o risco, mas **CEP/localização, estatísticas de uso e qualquer dado digitado** continuam sendo tratamento. Há **12 pendências ⚠️**.

---

## 1. LGPD (C1)

### 1.1 Normas lidas

| Norma | Artigos lidos | Conf. | Fonte |
|---|---|---|---|
| Lei 13.709/2018 (LGPD) | 1º, 3º, 4º (caput e começo), 5º (I, II, III, VI, VII, VIII), 6º (I–III), 7º (I–IX), 8º (caput), 11 (caput e I), 14 (caput), 15, 18 (I–V), 23, 37, 39, 41, 42, 46, 48 | ✅ (parcial; ver Lacunas) | [1] |
| Lei 13.608/2018 (Disque-Denúncia e informante) | 1º–6º, incluindo 4º-A, 4º-B, 4º-C (incluídos pela Lei 13.964/2019) | ✅ | [2] |
| Lei 12.527/2011 (LAI) | art. 31 (informações pessoais) e arts. 10–11, 15 (Parte A) | ✅ | [3][C5] |
| Lei 13.460/2017 | arts. 10, 13, 16 (Parte A) | ✅ | [C4] |

### 1.2 Pergunta 1: o app só redireciona ou recebe e encaminha?

**(i) O que a lei diz**

- A LGPD aplica-se a "qualquer operação de tratamento" por pessoa natural ou jurídica, de direito público ou privado, "independentemente do meio", e dado pessoal é qualquer informação "relacionada a pessoa natural identificada ou identificável" (arts. 1º, 3º e 5º, I) ✅ [1].
- **Controlador** decide sobre o tratamento; **operador** trata em nome do controlador e deve seguir as instruções dele (art. 5º, VI–VII; art. 39) ✅ [1].
- Controlador deve indicar **encarregado**, com identidade e contato divulgados publicamente (art. 41 e §1º) ✅ [1]. Registro das operações (art. 37), medidas de segurança (art. 46) e comunicação de incidente à ANPD e ao titular (art. 48) ✅ [1]. Responsabilidade por danos (art. 42) ✅ [1].
- Órgãos públicos tratam dados para sua finalidade pública (art. 23) ✅ [1].

**(ii) Interpretação** 🟡

| Aspecto | **A. "Só redireciona"** (app abre o site/telefone do canal oficial) | **B. "Recebe e encaminha"** (usuário digita a denúncia no app) |
|---|---|---|
| Dados da denúncia | O app não os vê. O relato é digitado no site do órgão, que é o controlador | O app passa a ter nome, relato, fotos etc. Dado pessoal tratado pelo app |
| Papel do app | Não trata a denúncia. Pode tratar dados de uso (analytics, CEP, localização) se eles identificarem a pessoa | Provavelmente **controlador** (decide a finalidade) ou **operador**, dependendo de acordo com o órgão: ⚠️ exige advogado/DPO |
| Dados sensíveis | Em regra não | Possível: o relato pode revelar saúde, origem racial, opinião política (art. 5º, II); exige base específica (art. 11: ex.: consentimento específico e destacado) ✅ lei, 🟡 aplicação |
| Obrigações | Política de privacidade e minimização do que for coletado | Todas as acima: encarregado, registro, segurança, incidente, direitos do titular (art. 18), prazo de guarda e exclusão (art. 15) |
| Segurança | Menor | Alta: um vazamento expõe denunciantes (sigilo é a promessa do canal) |
| Dependência do órgão | Só de links e telefones corretos | Precisa de integração/aceite de cada órgão: ⚠️ não pesquisado |

**(iii) Recomendação de produto** (para discutir na Fase 1, não é decisão)

- Partir do modelo **A** ("roteador, não receptor") como padrão, pois menor risco e custo. Isso é coerente com a recomendação de partida da referência [B-ref]. A opção B só se houver um motivo claro e assessoria jurídica.
- Mesmo em A: o aviso ao usuário ("você será levado ao site do órgão") deve ficar claro, e o app não deve guardar o que o usuário digitar.

### 1.3 Pergunta 2: anônima × identificada com sigilo

**(i) O que a lei e os canais dizem**

- **Informante identificado:** "terá assegurado, pelo órgão que receber a denúncia, o sigilo dos seus dados" (Lei 13.608, art. 3º) ✅ [2]. A identidade só é revelada por "relevante interesse público ou interesse concreto para a apuração", com comunicação prévia e concordância formal do informante (art. 4º-B e parágrafo único) ✅ [2].
- **Proteção contra retaliação** e isenção de responsabilidade civil ou penal pelo relato, exceto se o informante apresentou **consciente** informações ou provas falsas (art. 4º-A, parágrafo único; art. 4º-C) ✅ [2].
- **Ouvidoria pública (Lei 13.460):** a manifestação "conterá a identificação do requerente", sem exigências que inviabilizem; a identificação é "informação pessoal protegida com restrição de acesso" (art. 10, caput, §1º e §7º) ✅ [C4].
- **LAI, art. 31:** informações pessoais ligadas a intimidade, vida privada, honra e imagem têm acesso restrito a agentes autorizados e ao titular, por até 100 anos ✅ [3].
- Telefone "Disque-Denúncia" em transporte concedido deve exibir **garantia de anonimato**, na forma do regulamento (art. 1º, II) ✅ [2].

**(ii) Como cada tipo funciona na prática** (exemplos lidos na Parte B)

| | **Anônima** | **Identificada com sigilo** |
|---|---|---|
| O que é | Ninguém sabe quem enviou | O órgão sabe quem é, mas protege a identidade (Lei 13.608, art. 3º e 4º-B) ✅ |
| Permite pedir complemento? | Não: o MPSP diz que, sem elementos suficientes, a anônima é arquivada "porque não possibilita entrarmos em contato" ✅ [B20] | Sim, o órgão pode entrar em contato |
| Gera protocolo / acompanhamento? | ⚠️ varia por canal (não verificado para anônimas) | Normalmente sim; MPF tem "Acompanhamento da denúncia" ✅ existência [B3] |
| Exemplos | MPF: anônima só por correio ✅ [B4]. TCU Ouvidoria: "Manifestações anônimas" ✅ [B6]. MPSP: pode ser anônima ✅ [B20]. **Disque 100:** "as denúncias podem ser anônimas" ✅ [B31]. **Fala.BR:** opção de manifestação anônima, segundo a Ouvidoria da PF ✅ [B30] | MPF: dados do denunciante em sigilo ✅ [B4]. TCU denúncia: sigilo se solicitado ✅ [B7]. MPSP: opção sigilosa ✅ [B20]. **Pardal (Justiça Eleitoral):** exige identificação (e-Título/gov.br), com identidade protegida por sigilo ✅ [B35]. Disque 100: sigilo da fonte quando solicitado ✅ [B31] |
| Canais que **exigem** identificação | Consumidor.gov.br ✅ [B2]; ouvidoria da Lei 13.460 (identificação é elemento) ✅ [C4] | — |

**(iii) Recomendação** 🟡: o app não deve usar "denúncia anônima" como termo genérico. Para cada canal, mostrar o que a página oficial **afirma** (aceita anônimo / exige identificação / sigilo) e, quando não houver informação (⚠️), dizer "confirme no canal". Evitar prometer anonimato que o app não controla.

### 1.4 Pergunta 3: dados que uma denúncia costuma conter

| Dado | Pode ser sensível? | Observação | Conf. | Fonte |
|---|---|---|---|---|
| Nome, CPF, e-mail, telefone | Não sensível, mas pessoal | Identifica o denunciante | ✅ (definição) | [1] art. 5º, I |
| Endereço do fato / local | Pessoal se ligado a alguém | Localização do problema vs. residência da pessoa | 🟡 | [1] art. 5º, I |
| Relato livre | **Sim, potencialmente** | Pode citar saúde, raça, religião, opinião política, vida sexual de qualquer pessoa | ✅ (lista do art. 5º, II) | [1] |
| Fotos e vídeos | Sim, se houver pessoa identificável | Imagem de pessoa identificável é dado pessoal 🟡; biometria é sensível só "quando vinculada" (art. 5º, II) | 🟡 | [1] |
| Dados de terceiros (denunciado, vítima, testemunha, crianças) | Sim | Crianças: tratamento "em seu melhor interesse" (art. 14) ✅ | ✅ | [1] |

### 1.5 Pergunta 4: base legal

**(i) Lei:** hipóteses do art. 7º incluem consentimento (I), cumprimento de obrigação legal (II), execução de políticas públicas pela administração pública (III), exercício regular de direitos (VI), legítimo interesse do controlador ou de terceiro, exceto se prevalecerem direitos do titular (IX). Dados sensíveis: art. 11 (ex.: consentimento "específico e destacado" para finalidades específicas) ✅ [1]. O consentimento deve ser dado por escrito ou meio que demonstre a vontade (art. 8º) ✅ [1].

**(ii) Interpretação** 🟡
- *Se o app não guarda nada* (modelo A, processamento só no aparelho), pode não haver tratamento por parte do app a justificar base legal; **mas** isso depende de como o dado é processado: ⚠️ assessoria.
- *CEP/geolocalização:* a LGPD não cria categoria própria no texto lido; localização de pessoa identificável é dado pessoal (art. 5º, I). Como classificar CEP isolado ou localização aproximada: ⚠️ (depende de poder ou não identificar a pessoa; ver guias da ANPD).
- *Base mais adequada para guardar algo* (preferências, histórico): consentimento (art. 7º, I) ou legítimo interesse (art. 7º, IX). Qual escolher e como documentar: **exige advogado/DPO** ⚠️.

**(iii) Recomendação** 🟡: evitar precisar escolher base legal, **não guardando** dados identificáveis (Fase 1).

### 1.6 Pergunta 5: requisitos mínimos se o app guardar dados

| Requisito | O que a lei diz | Conf. | Fonte |
|---|---|---|---|
| Finalidade, adequação e necessidade (coletar o mínimo) | Art. 6º, I–III | ✅ | [1] |
| Política de privacidade / informar o titular | Princípios do art. 6º e direitos do art. 18 (o texto lido não traz o formato da política) | ✅ (princípios) · ⚠️ (formato) | [1] |
| Encarregado (DPO) com contato público | Art. 41 e §1º. Eventual dispensa/flexibilização para agentes de pequeno porte: ⚠️ não verificada | ✅ · ⚠️ | [1] |
| Direitos do titular: confirmação, acesso, correção, anonimização/bloqueio/eliminação, portabilidade | Art. 18, I–V (incisos seguintes truncados) | ✅ · ⚠️ | [1] |
| Término do tratamento e eliminação | Art. 15 (finalidade alcançada, fim do período, pedido do titular, ordem da ANPD) | ✅ | [1] |
| Segurança e incidente | Arts. 46 e 48 | ✅ | [1] |
| Registro das operações | Art. 37 | ✅ | [1] |
| Prazo de guarda de logs de acesso (Marco Civil) | Lei 12.965/2014 não aberta | ⚠️ | — |

### 1.7 Pergunta 6: denúncia falsa e exposição de terceiros

**(i) Lei:** a proteção do informante não vale se ele apresentou, **de modo consciente**, informações ou provas falsas (Lei 13.608, art. 4º-A, parágrafo único) ✅ [2]. Crime de denunciação caluniosa e outros tipos penais: ⚠️ (Código Penal não lido). Uso indevido de informações pessoais obtidas: o responsável responde (LAI, art. 31, §2º) ✅ [3].

**(ii) Interpretação** 🟡: se o app **receber** conteúdo (modelo B), pode ficar exposto a responsabilidade por dano a terceiros (LGPD, art. 42 ✅ [1]) — ver advogado. No modelo A, o risco é menor porque o conteúdo vai direto ao órgão.

**(iii) Recomendação** 🟡: aviso no app antes de abrir o canal: "não coloque dados de terceiros que não sejam necessários; não envie fotos de pessoas"; não hospedar relatos nem fotos.

### 1.8 O que exigiria advogado ou encarregado (DPO)

1. Classificar o app como controlador ou operador (e, se encaminhar a órgãos, o que isso implica).
2. Escolher e documentar a base legal para qualquer dado guardado.
3. Decidir se há dispensa ou simplificação para o porte do projeto (regulamento da ANPD ⚠️).
4. Hospedagem fora do país (transferência internacional, LGPD a partir do art. 33: ⚠️ não lido) e compartilhamento com órgãos públicos (arts. 26–27: ⚠️ não lidos).
5. Qualquer funcionalidade com **crianças e adolescentes**, incluindo o "ECA Digital" citado no site da ANPD ⚠️ (não lido).
6. Retenção e logs (Marco Civil ⚠️).
7. Termos de uso e responsabilidade por conteúdo de terceiros.

---

## 2. Perguntas abertas para a Fase 1 (C2)

Não decido nada aqui; cada opção traz prós, contras e **custo qualitativo** com a premissa. As premissas são minhas e podem estar erradas.

### Q1. Escopo regional inicial

| Opção | Prós | Contras | Custo (premissa) |
|---|---|---|---|
| **Nacional, só federal + padrão ("procure a ouvidoria do seu município/estado")** | Cobre todo mundo; contatos federais são poucos e estáveis | Genérico para o local, que é onde está a maioria dos problemas (Parte A) | **Baixo** (premissa: ~20 canais federais, revisão periódica) |
| **Um estado ou região piloto, com contatos estaduais e das principais cidades** | Respostas concretas para quem está na região | Quem está fora recebe só o padrão; curadoria manual | **Médio** (premissa: dezenas de contatos por estado) |
| **Nacional com diretório completo de municípios** | Máxima utilidade | Inviável manualmente (5.570 municípios); contatos mudam (Parte B) | **Alto** (premissa: sem automação ou parceria) |

Evidência: nos 3 exemplos municipais e 8 estaduais da Parte B, cada local tinha estrutura e nomes diferentes ([ouvidorias.md](ouvidorias.md), seção 2).

### Q2. Busca por CEP / geolocalização

| Opção | Prós | Contras | Custo (premissa) |
|---|---|---|---|
| **Usuário escolhe estado/município numa lista** | Sem coleta de localização; simples e privado | Um passo a mais para o usuário | **Baixo** |
| **CEP digitado, resolvido para município** | Rápido; mais familiar | Exige base/serviço de CEP e IBGE (existência registrada em [fontes-oficiais.md](../../.claude/skills/civic-research/references/fontes-oficiais.md)); CEP pode ser dado pessoal se vinculado à pessoa (ver 1.5: ⚠️) | **Médio** (premissa: serviço externo ou base própria) |
| **Geolocalização automática** | Mais conveniente em campo | Pede permissão; é a opção de maior sensibilidade de privacidade; imprecisão perto de divisa de município | **Médio/alto** (premissa: política de privacidade e minimização) |

### Q3. Funcionamento offline

| Opção | Prós | Contras | Custo (premissa) |
|---|---|---|---|
| **Conteúdo educativo offline; canais e contatos online** | Educação cívica sempre disponível; contatos não ficam desatualizados | Quem está sem rede não vê telefone | **Baixo/médio** |
| **Tudo offline (inclui contatos)** | Útil sem internet (ex.: telefones) | Risco de mostrar telefone desatualizado; precisa de aviso de data | **Médio** (premissa: versionar e datar contatos) |
| **Só online** | Sempre atualizado | Inútil sem rede; menos adequado para quem tem dados limitados | **Baixo** |

*Observação:* emergências (SAMU 192, PM 190, Bombeiros 193, Defesa Civil 199, PRF 191, Ligue 180 e Disque 100 ✅, todos verificados em páginas oficiais na Parte B, rodada de 2026-11-04) são os contatos mais críticos para offline. Se forem guardados offline, mostrar a data da verificação.

### Q4. Redirecionar vs. receber denúncias

| Opção | Prós | Contras | Custo (premissa) |
|---|---|---|---|
| **Só redirecionar (modelo A)** | Menor carga de LGPD; sem custódia de relatos; sem integração | Não "resolve" no próprio app; o usuário digita de novo no site do órgão | **Baixo** |
| **Receber e encaminhar (modelo B)** | Experiência única; possíveis dados agregados | Carga de LGPD alta (1.2); exige aceite dos órgãos ⚠️; risco de vazamento de denunciantes; exige advogado/DPO | **Alto** (premissa: equipe de segurança e jurídico) |
| **Redirecionar com ajuda para preparar o texto, sem enviar** | Melhora a qualidade da reclamação | Se o texto passar pelo servidor, volta ao modelo B; pode ser só no aparelho | **Médio** (premissa: processamento local) |

### Q5. Manutenção dos contatos

| Opção | Prós | Contras | Custo (premissa) |
|---|---|---|---|
| **Curadoria manual com data de verificação visível** | Qualidade controlada | Não escala; contatos mudam | **Médio** → alto com o crescimento |
| **Verificação automática de links + revisão humana por exceção** | Escala melhor; detecta links quebrados | Não detecta telefone errado nem mudança de regra | **Médio** |
| **Apontar sempre para páginas-índice oficiais (sem copiar telefone)** | Quase sem manutenção | Menos útil; depende de a página existir (vimos páginas que retornam "não encontrada") | **Baixo** |

Evidência: nesta pesquisa algumas páginas oficiais deram "não encontrada" ou falharam (ver Lacunas de [ouvidorias.md](ouvidorias.md)).

---

## Lacunas

12 pendências ⚠️:

1. LGPD: arts. 4º, III (alíneas), 6º IV–X, 18 VI–IX, 41 §§2º–3º, 26–27 (compartilhamento com poder público) e 33 e seguintes (transferência internacional) não lidos ou truncados.
2. Regulamento da ANPD sobre agentes de pequeno porte e eventual dispensa de encarregado.
3. Guias da ANPD sobre agentes de tratamento, legítimo interesse e anonimização: só links localizados no site; **conteúdo não lido**. O site da ANPD aparece nesta data como "Agência Nacional de Proteção de Dados".
4. "ECA Digital" (citado no site da ANPD): não lido; relevante se houver público infantojuvenil.
5. Marco Civil da Internet (Lei 12.965/2014) e guarda de registros.
6. Código Penal (denunciação caluniosa e correlatos).
7. Decreto(s) federal(is) sobre ouvidoria e proteção do denunciante: não localizados; não citei de memória.
8. Lei 9.807/1999 (proteção a testemunhas), citada na Lei 13.608, art. 4º-C.
9. Se denúncias **anônimas** geram protocolo e podem ser acompanhadas: o MPSP (não permite contato) foi lido; o Pardal gera protocolo, mas **não** é anônimo ✅; MPF, TCU, Fala.BR e Disque 100 (para anônimas): ⚠️.
10. Como a ANPD trata **CEP/localização** aproximada.
11. Enquadramento do app como controlador ou operador no modelo B.
12. Aceite/integração dos órgãos para receber denúncias vindas de um terceiro (modelo B).

## Perguntas abertas

As 5 decisões estratégicas estão na seção 2 (Q1–Q5). Perguntas jurídicas que dependem de advogado/DPO: ver 1.8.

## Fontes

1. Lei 13.709/2018 (LGPD) — https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm — acesso em 2026-11-04 — 🟡 (leitura de 2026-11-04 não reconfirmada na revisão de 2026-11-05: planalto.gov.br inacessível)
2. Lei 13.608/2018 (Disque-Denúncia; informante, com alterações da Lei 13.964/2019) — https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13608.htm — acesso em 2026-11-04 — 🟡 (leitura de 2026-11-04 não reconfirmada na revisão de 2026-11-05: planalto.gov.br inacessível)
3. Lei 12.527/2011 (LAI), art. 31 — https://www.planalto.gov.br/ccivil_03/_ato2011-2014/2011/lei/l12527.htm — acesso em 2026-11-04 — 🟡 (leitura de 2026-11-04 não reconfirmada na revisão de 2026-11-05: planalto.gov.br inacessível)
4. ANPD, página inicial — https://www.gov.br/anpd/pt-br — acesso em 2026-11-04 (reaberta em 2026-11-05) — ✅ (só existência de guias e canais; conteúdo não lido)

`[C n]` = [competencias.md](competencias.md) (acesso em 2026-11-03). `[B n]` = [ouvidorias.md](ouvidorias.md) (acesso em 2026-11-04). `[B-ref]` = referência interna `lgpd-ponto-de-partida.md`, que é pista, não fonte.

## Revisão (2026-11-05)

Revisão independente via `/verificar-fontes`. **Limitação:** `planalto.gov.br` não respondeu nesta sessão (curl e MCP `fetch` falharam na conexão; o Playwright MCP estava ocupado), então **não foi possível reabrir as Fontes 1–3**.

**O que mudou**
- Fontes 1, 2 e 3 (Leis 13.709, 13.608 e 12.527): ✅ → 🟡 na lista de Fontes, com o motivo. Os ✅ de artigos no corpo do texto dependem dessas fontes e ficam **pendentes de reconferência** (não foram contraditos, apenas não reconfirmados). Reabrir quando o site estiver acessível.
- Fonte 4 (ANPD): reaberta e confirmada (`gov.br/anpd/pt-br`, HTTP 200). A página cita "Agência Nacional de Proteção de Dados" e também "Autoridade Nacional de Proteção de Dados", e menciona "ECA Digital". Mantém ✅ (só existência), como o relatório já dizia.

**Conferido sem alteração**
- Não encontrei URL, telefone ou artigo claramente inventado. Os links internos (`competencias.md`, `ouvidorias.md`, `fontes-oficiais.md`, `lgpd-ponto-de-partida.md`) existem.
- Citações de artigos consistentes com o que se conhece das leis (conferência de memória, não é verificação): LGPD arts. 5º, 7º, 11, 18, 41; Lei 13.608 arts. 3º, 4º-A a 4º-C; LAI art. 31; Lei 13.460 art. 10.
- Competência: o relatório não faz simplificações de competência; o tema aqui é LGPD/denúncia.
- Contagem de pendências (12) bate com a lista em Lacunas. Os ✅ de `[B n]` e `[C n]` (telefones de emergência, Disque 100 etc.) pertencem a outros relatórios e **não foram revisados aqui**.
