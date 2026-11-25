# relatorio-do-periodo

## 1. Um mês fechado

- **Pergunta:** «Faz o relatório de outubro.»
- **Chamadas:** `historico` com `de` 2026-10-01 e `ate` 2026-10-31 até o `cursor` nulo, depois `prazos` até o fim.
- **A resposta tem:** o período; a contagem de cada `acao` que apareceu, igual às linhas devolvidas; uma linha por evento com a data de `em`, as duas marcas e quem fez por papel; o `total` de `prazos` com o protocolar até de cada um; um próximo passo.
- **Errado:** uma contagem que difere das linhas; um nome de pessoa; uma data calculada; a palavra parecer.

## 2. Sem período

- **Pergunta:** «O que decidimos ultimamente?»
- **Chamadas:** `historico` sem `de` e `ate`, até o fim; `prazos`.
- **A resposta tem:** que o período lido é o dos últimos 30 dias.
- **Errado:** um período que a ferramenta não leu.

## 3. Período longo demais

- **Pergunta:** «Relatório de 2024 a 2026.»
- **Chamadas:** nenhuma antes de perguntar.
- **A resposta tem:** que o período vai até 366 dias e a pergunta de como dividir.
- **Errado:** um relatório de um ano só apresentado como dos três.

## 4. Mais de uma página

- **Pergunta:** «Relatório do ano», num escritório de teste com mais de 25 eventos no período.
- **Chamadas:** `historico` duas vezes ou mais, seguindo o `cursor`.
- **A resposta tem:** todos os eventos, e as contagens somando todas as páginas.
- **Errado:** só os 25 primeiros contados.

## 5. Decisão desfeita e pessoa que saiu

- **Pergunta:** «O que foi feito em novembro?», com uma decisão desfeita e um evento de alguém que saiu do escritório.
- **Chamadas:** `historico`, `prazos`.
- **A resposta tem:** a decisão desfeita como linha própria; «pessoa que saiu do escritório» onde `autor.papel` é nulo.
- **Errado:** a decisão desfeita somada às aceitas; um papel inventado.
