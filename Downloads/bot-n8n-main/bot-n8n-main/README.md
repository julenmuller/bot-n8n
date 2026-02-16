# Telegram Weather Bot N8N

Este projeto consiste em um chatbot automatizado via N8N que consulta a temperatura de cidades brasileiras em tempo real utilizando a API do OpenWeatherMap.

## 🚀 Funcionalidades
- Recebe mensagens via Telegram.
- Normalização de texto (remoção de espaços e padronização).
- Consulta de clima com resposta em Graus Celsius.
- Tratamento de erro para cidades não encontradas.

## 🛠️ Tecnologias Utilizadas
- **N8N**
- **Telegram Bot API**
- **OpenWeatherMap API**
- **Google Gemini API**

## 📋 Pré-requisitos
Antes de importar, você precisará das seguintes chaves:
1. `TELEGRAM_BOT_TOKEN`: Obtido com o [@BotFather](https://t.me/botfather).
2. `OPENWEATHER_API_KEY`: Obtido no painel da [OpenWeather](https://openweathermap.org/api).
3. `GOOGLE_API_KEY`: (Opcional) Obtido no Google AI Studio.

## 📥 Como Importar o Projeto
1. No seu N8N, clique em **Workflows** > **Import from File**.
2. Selecione o arquivo `workflow-chatbot-telegram.json` deste repositório.
3. Clique em **Credentials** no menu lateral e configure:
   - **Telegram API**: Insira seu Token.
   - **OpenWeatherMap API**: Crie uma credencial de "Header Auth" ou use o campo de parâmetros no nó.
4. Clique em **Execute Workflow** para ativar o modo de escuta.

## 🤖 Como Usar
Envie uma mensagem para o seu bot no Telegram informando a cidade:
- **Exemplo:** `Belo Horizonte, MG`
- **Retorno esperado:** `🌤️ A temperatura em Belo Horizonte é de 25°C.`

## ⚠️ Tratamento de Erros
Se o usuário enviar uma cidade inexistente, o bot responderá:
> ❌ Cidade não encontrada. Use o formato Cidade,UF (ex.: São Paulo,SP).


<img width="1136" height="1600" alt="image" src="https://github.com/user-attachments/assets/c07bdab4-873b-45c8-9655-d56673766428" />