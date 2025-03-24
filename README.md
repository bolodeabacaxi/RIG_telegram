# 🚀 Monitoramento de Rig com ESP32 e Telegram

Este projeto utiliza o **ESP32** para monitorar sua rig de mineração e enviar atualizações periódicas para o **Telegram**. Ideal para quem quer acompanhar a performance da sua rig em tempo real, sem precisar ficar verificando fisicamente.

---

## 🔧 Funcionalidades

- Conexão automática ao Wi-Fi.
- Envio de mensagens para o Telegram utilizando a API do Telegram Bot.
- Envio de atualizações a cada 1 minuto, informando o status da rig.

---

## 📦 Requisitos

- **ESP32** (Placa de desenvolvimento)
- **Arduino IDE** ou **PlatformIO**
- Bibliotecas `WiFi.h` e `HTTPClient.h` para ESP32
- **Token do Bot do Telegram** e **Chat ID**

---

## ⚙️ Como Usar

1. **Configuração do Wi-Fi**:
    - Substitua os valores de `ssid` e `password` com as credenciais da sua rede Wi-Fi.

2. **Configuração do Telegram**:
    - Crie um **bot** no Telegram usando o [BotFather](https://core.telegram.org/bots#botfather).
    - Após criar o bot, obtenha o **botToken** e **chatID** para substituir nas variáveis `botToken` e `chatID` no código.

3. **Carregue o Código no ESP32**:
    - Após fazer as alterações necessárias, carregue o código no seu ESP32 utilizando o **Arduino IDE** ou **PlatformIO**.

4. **Monitoramento**:
    - O ESP32 começará a monitorar a rig e enviará atualizações para o seu Telegram a cada 1 minuto.

---

## 📱 Como Funciona

1. **Conexão Wi-Fi**: O ESP32 se conecta à rede Wi-Fi usando as credenciais fornecidas.
2. **Primeira Mensagem**: Assim que a conexão Wi-Fi é estabelecida, o ESP32 envia uma mensagem para o Telegram informando que ele está pronto para monitorar sua rig.
3. **Atualizações Periódicas**: A cada 1 minuto, o ESP32 envia outra mensagem para o Telegram confirmando que sua rig está funcionando normalmente.

---

## 📥 Dependências

- **ESP32**: Certifique-se de ter a biblioteca ESP32 instalada no seu Arduino IDE.
- **Bibliotecas WiFi e HTTPClient**: Bibliotecas padrão para comunicação Wi-Fi e requisições HTTP.
