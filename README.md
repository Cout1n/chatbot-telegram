
#  Chatbot Previsão do Tempo (n8n + Telegram)

Automação que recebe o nome de uma cidade via **Telegram**, consulta a API do **OpenWeather** e retorna o clima em tempo real.


###  Como Importar

1. No **n8n**, crie um novo workflow.
2. Copie o código JSON do projeto e dê **Ctrl+V** diretamente no canvas (ou use *Import from File*).
 
###  Configuração de Credenciais

Crie as seguintes credenciais no menu **Credentials** do n8n:

* **Telegram API:** Insira seu `TELEGRAM_BOT_TOKEN` (obtido no [@BotFather](https://t.me/botfather)).
* **OpenWeatherMap API:** Insira sua `OPENWEATHER_API_KEY` (obtida no [site oficial](https://openweathermap.org/api)).

> **Importante:** Verifique se cada nó (node) do workflow está com a credencial correspondente selecionada.


###  Como Testar

1. Ative o workflow (**Active** no canto superior).
2. No Telegram, envie o nome de uma cidade para o seu bot (ex: `São Paulo`).
3. **Retorno esperado:** Uma mensagem com a descrição do clima e a temperatura atual da cidade enviada.



###  Variáveis Utilizadas

* `TELEGRAM_BOT_TOKEN`: Token de acesso do seu bot.
* `OPENWEATHER_API_KEY`: Chave da API de clima.