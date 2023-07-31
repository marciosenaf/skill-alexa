[![NPM](https://img.shields.io/npm/l/react)](https://github.com/marciosenaf/skill-alexa/blob/main/LICENSE)

# Layout
<img src="https://github.com/marciosenaf/skill-alexa/blob/main/imagesreadme/Images2.jpg" alt="Texto alternativo" width="300" height="500">

# Visão geral
Uma visão geral de uma habilidade Alexa de amostra para tocar uma estação de rádio que
transmite música rock. A habilidade é implementada usando o Alexa Skills Kit (ASK) SDK (v2) e suporta a interface
AudioPlayer para reprodução de áudio. A habilidade usa uma tabela DynamoDB para persistência de sessão, que é
configurada automaticamente para habilidades hospedadas do Alexa. A URL da estação de rádio usada na habilidade é uma
URL de amostra e pode ser substituída pela URL da estação de rádio real que você deseja transmitir.# Autor

# Funcionalidade da habilidade

- A habilidade é acionada com a invocação "Open Rock Radio" ou frases semelhantes.
- Quando aberto, ele dá as boas-vindas ao usuário e começa a reproduzir o fluxo de música rock automaticamente.
- O usuário pode dizer "Pausar" para interromper a reprodução da música.
- O usuário pode dizer "Play" ou "Resume" para retomar a reprodução da música.
- A habilidade lida com intents integrados como "AMAZON.HelpIntent", "AMAZON.StopIntent" e "AMAZON.CancelIntent".
- A habilidade oferece suporte a eventos AudioPlayer como "PlaybackStarted", "PlaybackFinished", "PlaybackStopped", "PlaybackNearlyFinished" e "PlaybackFailed".
- A habilidade fornece um manipulador de erro genérico para lidar com qualquer sintaxe ou erros de roteamento.

# Estrutura de código

O código de habilidade é estruturado em manipuladores de intenção separados, interceptadores de solicitação, interceptadores de resposta e manipuladores de erro. Abaixo estão os principais componentes do código:

# Tabela do DynamoDB

Essa habilidade usa uma tabela do DynamoDB para armazenar atributos persistentes, que incluem informações de reprodução, como offsetInMilliseconds, token, inPlaybackSession e hasPreviousPlaybackSession. A tabela é criada automaticamente ao usar habilidades hospedadas no Alexa.

# Implantação

O código de habilidade é estruturado em manipuladores de intenção separados, interceptadores de solicitação, interceptadores de resposta e manipuladores de erro. Abaixo estão os principais componentes do código:

1. Crie uma habilidade hospedada pela Alexa no Amazon Developer Console.
2. Copie o código fornecido acima e cole-o na função Lambda associada à habilidade.
3. Salve e implante a função Lambda.
4. Adicione o modelo de interação necessário e a configuração de habilidades no console do desenvolvedor.
5. Teste a habilidade usando dispositivos Alexa ou o Simulador Alexa.

Nota: Lembre-se de substituir o URL da estação de rádio de exemplo pelo URL real que você deseja usar para streaming de música.

# Conclusão

O código de habilidade Alexa Rock Radio e sua funcionalidade. A habilidade permite aos usuários ouvir uma estação de rádio de rock invocando a habilidade e fornece controles básicos de reprodução. Ao personalizar e estender essa habilidade de amostra, você pode criar suas próprias habilidades Alexa para reproduzir diferentes fluxos de áudio ou implementar recursos de reprodução de áudio mais avançados.

Márcio Sena 

https://www.linkedin.com/in/marciosenaf/
