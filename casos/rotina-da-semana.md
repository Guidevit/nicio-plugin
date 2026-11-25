# rotina-da-semana

## 1. A terça

- **Pergunta:** «Como está minha semana?»
- **Chamadas:** `resumo_da_fila`, `prazos`, `fila`.
- **A resposta tem:** na linha 1 a edição de `cobertura.ultimaEdicao`; nas três primeiras linhas o prazo mais curto entre o primeiro de `prazos` e o primeiro de `fila`; o `total` de `prazos`; os pares novos da edição; os números `urgente`, `ate30` e `mais30`; os lembretes por e-mail do Nicio; um próximo passo.
- **Errado:** um prazo calculado pelo modelo; o prazo mais próximo depois da terceira linha; conselho sobre opor.

## 2. Análise em andamento

- **Pergunta:** «O que saiu nesta terça?», com a RPI ainda em análise.
- **Chamadas:** `resumo_da_fila`, `prazos`, `fila`.
- **A resposta tem:** o `cobertura.aviso` como veio.
- **Errado:** dizer que a edição foi toda analisada.

## 3. Escritório em teste

- **Pergunta:** «O que tenho para esta terça?», no escritório em teste grátis.
- **Chamadas:** `resumo_da_fila`, `prazos`, `fila`.
- **A resposta tem:** `teste.abertos` e `teste.bloqueados`, e que os bloqueados abrem com a assinatura em https://nicio.com.br/plano.
- **Errado:** nome ou data de um par bloqueado.

## 4. Repetir toda terça

- **Pergunta:** «Me manda isso toda terça.»
- **Chamadas:** as do caso 1.
- **A resposta tem:** que o Claude pode agendar uma tarefa onde o plano tiver o recurso, e que os lembretes de prazo seguem vindo do Nicio por e-mail.
- **Errado:** um agendamento criado sem a pessoa confirmar; a promessa de que o Claude avisa os prazos.

## 5. Sem conexão

- **Pergunta:** «Como está minha semana?», com o conector não conectado.
- **Chamadas:** `resumo_da_fila`, que falha.
- **A resposta tem:** como conectar na aba Connectors do plugin.
- **Errado:** qualquer par, prazo ou número.
