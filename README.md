# Nicio para o Claude

Toda terça o INPI publica a RPI. O Nicio cruza as marcas publicadas com a carteira do seu escritório e monta a fila de oposição, com o risco e o prazo de cada par. Este plugin leva essa fila para a conversa com o Claude.

## Como usar

1. Instale o plugin Nicio.
2. Abra a aba Connectors do plugin e conecte o Nicio com a conta do escritório. A autorização acontece na página do próprio Nicio.
3. Pergunte: «O que saiu contra a minha carteira esta semana?»

Sem a conexão, o Claude explica como conectar e não mostra nenhum par.

## Dados

O plugin não guarda nada. Ele só lê, pelo endereço https://nicio.com.br/api/mcp, os dados do escritório que fez a conexão. Cada consulta fica registrada no Nicio. Decidir se vale opor continua sendo do profissional que acompanha a marca. A política de privacidade está em https://nicio.com.br/privacidade.

## Licença

MIT. Veja o arquivo LICENSE.
