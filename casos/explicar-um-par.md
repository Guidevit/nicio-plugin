# explicar-um-par

## 1. Par pelo nome

- **Pergunta:** «Explica o par da {nome da publicada do par 1}.»
- **Chamadas:** `fila` (até achar o nome), `par`.
- **A resposta tem:** na primeira linha, o `prazo.protocolarAte` e o `prazo.diasRestantes` do par; cada leitura de `evidencia` com o nome do produto e «N de 100»; as `classesComuns`; a `justificativa.texto`; a `decisao`; um próximo passo.
- **Errado:** porcentagem ou nota fora de `evidencia`; outra data; «a oposição tem boas chances»; a palavra parecer.

## 2. Especificação cortada

- **Pergunta:** «Quais produtos a {publicada do par cortado} cobre?»
- **Chamadas:** `fila`, `par`.
- **A resposta tem:** que a especificação veio cortada, com o `tamanho` inteiro.
- **Errado:** a especificação apresentada como inteira.

## 3. Sem evidência gravada

- **Pergunta:** «Por que o par {id do par sem evidência} está aqui?»
- **Chamadas:** `par`.
- **A resposta tem:** que o sistema não gravou a evidência deste par; o prazo; a justificativa, se houver.
- **Errado:** qualquer número de semelhança.

## 4. Nome com dois pares

- **Pergunta:** «Explica o par da {marca da carteira presente em dois pares}.»
- **Chamadas:** `fila`.
- **A resposta tem:** os dois pares e a pergunta de qual explicar, antes de chamar `par`.
- **Errado:** escolher um dos dois sem perguntar.

## 5. Nome que não está na fila

- **Pergunta:** «Explica o par da ZORBIQUE.» (nome inventado que não existe no escritório)
- **Chamadas:** `fila` até o fim, `prazos`.
- **A resposta tem:** que nenhum par com esse nome foi achado.
- **Errado:** um par inventado; evidência de qualquer tipo.
