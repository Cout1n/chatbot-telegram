
#  Chatbot Previsão do Tempo (n8n + Telegram)

Este repositório contém um workflow avançado para n8n que transforma o Telegram em um assistente meteorológico inteligente. O bot combina dados em tempo real da OpenWeather com a capacidade de reescrita natural do Google Gemini.


###  Pré-requisitos

1. n8n instalado (v1.114.3+)
2. Telegram Bot Token: Obtido via @BotFather.
3. OpenWeather API Key: Obtida no OpenWeatherMap.
4. Google Gemini API Key: Obtida no Google AI Studio.
 
###  Como Importar

* Faça o download do arquivo workflow-telegram-chatbot.json.
* No seu n8n, clique em Workflows > Import from File.
* Selecione o arquivo baixado.


###  Configuração das Credenciais

Após importar, você deve configurar as credenciais no painel do n8n para que o bot funcione:
1. Telegram API: Crie uma credencial de Telegram e insira seu Token.
2. OpenWeather API (Query Auth): * Crie uma credencial do tipo Query Auth.
 Name: OpenWeather API
 Query Name: appid
 Value: Sua chave da OpenWeather.
3. Google Gemini API: Crie uma credencial de Gemini e insira sua API Key.



###  Como Executar e Testar

* O que enviar: O nome de uma cidade (ex: Curitiba ou Recife-PE).
* O que esperar: Uma resposta natural e amigável informando a temperatura atual e as condições do céu.
*  Exemplo: "🌤️ Em Curitiba, a temperatura atual é de 18°C agora.".


