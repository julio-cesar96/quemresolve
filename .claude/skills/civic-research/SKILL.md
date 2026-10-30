---
name: civic-research
description: Metodologia para pesquisar competências de cargos políticos, órgãos públicos, ouvidorias e legislação brasileira com fontes primárias. Use sempre que a tarefa envolver pesquisar quem é responsável por um serviço público, canais de reclamação/denúncia, ou normas (CF/88, leis, decretos, LGPD) para o projeto.
---

# Pesquisa cívica com fonte primária

## Ordem de trabalho

1. **Ler a referência certa antes de buscar**:
   - Competências e cargos → `references/competencias-ponto-de-partida.md`
   - Canais e ouvidorias → `references/fontes-oficiais.md`
   - Privacidade e denúncias → `references/lgpd-ponto-de-partida.md`
   Essas referências são **pistas para verificar**, não verdade final. Confirme cada item na fonte antes de usar.
2. **Buscar na fonte primária** (planalto.gov.br, gov.br, site do órgão). Use `fetch` para páginas estáticas; use o navegador (Playwright) só quando a página depende de JavaScript ou exige navegação.
3. **Registrar enquanto pesquisa**: para cada afirmação, guarde URL, data de acesso e o artigo/seção exato.
4. **Classificar confiança** de cada item: `✅` primária verificada, `🟡` secundária, `⚠️` não verificado.
5. **Escrever usando a skill `research-report`.**

## Armadilhas do domínio

- **Competência compartilhada é a regra, não a exceção.** Saúde (SUS), educação, assistência social e segurança envolvem mais de um nível. Descreva a divisão prática: quem financia, quem executa, quem fiscaliza.
  - Ex.: falta de remédio na UBS → execução municipal (atenção básica), com financiamento tripartite e listas de medicamentos definidas em âmbito federal/estadual. Verifique e explique.
- **Executivo executa; Legislativo legisla, fiscaliza e aprova orçamento.** Para cada problema, diga o que o parlamentar *pode* fazer (fiscalizar, requerimento de informação, emenda, convocar secretário) e o que *não pode* (executar a obra).
- **Órgãos que não são cargos eletivos também resolvem**: Tribunais de Contas, Ministério Público, Defensoria Pública, Procon, agências reguladoras (Anatel, ANEEL, ANS etc.), Controladorias. Inclua-os no roteamento.
- **Variação local**: cada município e estado tem sua ouvidoria, site e telefone próprios. Não generalize contatos de um lugar para todos. Documente o *padrão* (onde costuma ficar) e marque exemplos como exemplos.
- **Distrito Federal** acumula competências de estado e município. Trate como caso especial.
- **Serviço concedido** (ônibus, energia, água, telefonia) pode ter reclamação primeiro na empresa, depois na agência reguladora ou órgão municipal/estadual. Mapeie a escada de escalonamento.

## O que nunca fazer

- Inventar URL, telefone, número de artigo ou nome de sistema.
- Citar político, partido ou governo atual como exemplo.
- Afirmar que algo é "exclusivo" de um nível sem artigo de lei que sustente.
