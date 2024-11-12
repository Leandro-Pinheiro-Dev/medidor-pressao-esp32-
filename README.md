# Medidor de pressão utilizando uma Lilygo TTGO ESP32 com display OLED integrado

Medidor de pressão utilizando uma Lilygo TTGO ESP32 com display OLED integrado e sensores BMP280, de temperatura e pressão barométrica, e SMP3011, de pressão.

# Antes de começar

- O código foi projetado para a IDE ESP-IDF - que depende do Python - no Visual Studio Code, e utilizando-se do CMake junto às C++ Build Tools do Visual Studio 2019, portanto, todos estes serão necessários para a compilação;
- É necessário que o sistema possua as variáveis de ambiente `PATH`, contendo o diretório `\.espressif\` e `%IDF_PATH%\tools`, e `IDF_PATH`, contendo o diretório onde está instalado o ESP-IDF, para que o código do projeto carregue todas as dependências;

Para funcionamento dos sensores e display:
- Abra o temrminal do Visual Studio Code e execute `git clone --recursive https://github.com/eng-software/ComponentesESP32.git components\tex` para obter os componentes herdados para o projeto;
- Na aba da extensão ESP-IDF, vá em `SDK Config`;
  ![image](https://github.com/user-attachments/assets/2b6b6b0f-429e-4d2f-946e-f8e7b53aa563)

- Role até a seção `Font usage`;
  ![image](https://github.com/user-attachments/assets/d1f4139c-9836-4465-ba29-184c1d90ded6)

- Marque as caixas mostradas na imagem:
  ![image](https://github.com/user-attachments/assets/e35f3a0f-8889-4c2b-9920-4e641ec7ef48)
- Na seção `Others` marque as opções abaixo:
  ![image](https://github.com/user-attachments/assets/49bfdab3-1f41-4cee-abf9-252d26c3d275)

Para carregar o software para a placa ESP32:

- Na aba da extensão do IDF, selectione `Set Espressif Target`;
  ![image](https://github.com/user-attachments/assets/91520245-6b44-4939-8ce8-ca122ea4ca93)

- Selecione a primeira opção, `esp32` e pressione enter;
  ![image](https://github.com/user-attachments/assets/deb865c9-0e03-4af7-992e-e7e1e5cee91e)

- Depois, selecione a última opção, `Custom board` e pressione enter;
  ![image](https://github.com/user-attachments/assets/d841c316-f0b5-4156-a937-deb7f62bc332)

- Ainda na aba da extensão, selecione a opção `Build` para compilar o código;
  ![image](https://github.com/user-attachments/assets/9ee2936d-687a-40b8-a9a4-ae7cf1be2299)

- E por fim, selecione a opção `Flash` - *não se esqueça de segurar o botão 'boot' em sua placa ESP32 ao início do processo de flash, quando aparecer a mensagem `Connecting...`.
  ![image](https://github.com/user-attachments/assets/ebb47c55-2518-4132-adf2-996feb566a0c)


