# 0001 — Foco em "quem resolve meu problema"; sem ranquear nem recomendar candidatos

- **Status:** Aceita
- **Data:** 2026-11-03
- **Fase:** 1 (Decisões de produto)

## Contexto

O produto foi definido no `AGENTS.md` como educação cívica e roteamento de reclamações, com neutralidade como regra inegociável (regra 7: sem partidos, sem políticos atuais, exemplos usando cargos e nunca pessoas).

Durante a revisão do prompt 01, surgiu a ideia de o site também ajudar na escolha de candidatos: avaliar se promessas fazem sentido e explicar legendas e coligações ("um candidato apoia o outro"). Isso levantou o conflito entre ajudar a decidir o voto e manter o produto apartidário.

## Opções consideradas

1. **Manter o foco em "quem resolve meu problema"**, com apoio eleitoral apenas educativo e sem dados de candidatos.
   - Prós: coerente com a regra 7; baixo risco jurídico e reputacional; sem manutenção de dados a cada eleição; valor contínuo entre eleições.
   - Contras: não responde "em quem votar" (intencional).
2. **Incluir informações de candidatos e partidos** (perfis, histórico, comparação), sem recomendar.
   - Prós: maior atratividade em período eleitoral.
   - Contras: exige citar pessoas e partidos atuais (viola a regra 7), manutenção contínua, risco de viés percebido e de dados desatualizados, exposição à legislação eleitoral.
3. **Ranquear ou recomendar candidatos.**
   - Descartada: contradiz o caráter apartidário do produto.

## Decisão

Adotamos a **opção 1**.

- O valor central do produto é o fluxo **problema → quem é responsável → onde reclamar**.
- O app **não ranqueia, não recomenda e não compara** candidatos ou partidos, e não exibe dados de candidatos. Quando houver necessidade, apenas aponta para fontes oficiais (ex.: portais do TSE), sem reproduzir os dados.
- Conteúdo de apoio ao eleitor é permitido, desde que **educativo e neutro**, e secundário ao fluxo central:
  - **"Essa promessa cabe a esse cargo?":** uso da matriz de competências para indicar se um tipo de promessa é atribuição do cargo (ex.: construir hospital estadual, legislar sobre tributo federal). Responde apenas sobre competência, nunca se a promessa é boa ou será cumprida.
  - **Mecanismo de legendas, coligações e federações:** explicação de como funcionam, sem citar partidos ou políticos. As regras vigentes devem ser verificadas no TSE e na legislação antes de entrar no conteúdo (`⚠️ A VERIFICAR`).
- A regra 7 do `AGENTS.md` permanece como está.

## Consequências

- **Prompt 01:** a versão revisada passa a incluir, na Parte A, uma seção curta sobre tipos de promessa e competência do cargo. Pesquisa sobre sistema eleitoral e partidos fica como prompt separado e de menor prioridade (um eventual Prompt 02), a rodar depois do prompt 01.
- **Produto:** sem módulo de candidatos, não há manutenção de dados por eleição e o uso não depende do calendário eleitoral.
- **Posicionamento:** o app é comunicado como ferramenta de utilidade pública e educação cívica, não como guia de voto.
- **Reabertura:** incluir dados de candidatos ou partidos no futuro exige novo ADR que substitua este e revisão da regra 7.
- **Pendências:** confirmar no TSE as regras atuais de coligação e federação e o calendário eleitoral antes de qualquer conteúdo sobre o tema.