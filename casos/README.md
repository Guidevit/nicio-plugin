# Casos das skills

Cada skill tem cinco casos. Cada caso roda duas vezes numa conta do Claude com o plugin enviado e o escritório de teste conectado. A transcrição de cada rodada fica ao lado do caso, em `casos/<skill>/<caso>-<rodada>.md`.

Uma rodada passa quando a resposta tem todos os fatos do caso, nenhuma das respostas erradas, e cada fato aparece numa chamada de ferramenta da mesma conversa, conferida no registro de chamadas do escritório (Configurações › Assistentes).

O escritório de teste tem pares inventados: um com a especificação cortada, um bloqueado pelo teste grátis, um com o prazo vencido e um marcado como provável marca do próprio cliente.

Meta: 9 de 10 rodadas por skill.
