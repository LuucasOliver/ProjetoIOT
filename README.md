# Projeto ESP32: Monitoramento de Temperatura e Umidade com DHT11

## Descrição

Este projeto utiliza um ESP32 para monitorar a temperatura e a umidade ambiente usando um sensor DHT11. Os dados coletados são exibidos em uma página web hospedada no próprio ESP32, permitindo acesso fácil e visualização em tempo real dos dados ambientais.

## Funcionalidade

- Conexão à rede Wi-Fi.
- Coleta de dados de temperatura e umidade usando o sensor DHT11.
- Exibição dos dados em uma página HTML acessível via navegador.
- Atualização automática dos dados a cada 2 segundos, sem a necessidade de recarregar a página.

## Componentes Necessários

- **ESP32**: Microcontrolador que será utilizado para coletar os dados e hospedar o servidor web.
- **Sensor DHT11**: Sensor para medir a temperatura e umidade.
- **Fios de Conexão**: Para conectar o sensor ao ESP32.
- **Fonte de Alimentação**: Para alimentar o ESP32.

## Configuração

### 1. Instalação das Bibliotecas

Certifique-se de que as bibliotecas necessárias estão instaladas no seu ambiente de desenvolvimento:

- **DHT Sensor Library**
- **ESP32 Board Package**

Essas bibliotecas podem ser instaladas pelo gerenciador de bibliotecas do Arduino IDE.

### 2. Conexão do Hardware

Conecte o sensor DHT11 ao ESP32 da seguinte forma:

- **VCC** do DHT11 ao **5V** do ESP32
- **GND** do DHT11 ao **GND** do ESP32
- **DATA** do DHT11 ao pino **4** do ESP32

### 3. Configuração do Código

Edite as linhas no código para inserir seu SSID e senha da rede Wi-Fi:

```cpp
const char* ssid = "SEU_SSID";  // Insira seu SSID aqui
const char* password = "SUA_SENHA";  // Insira sua senha aqui
