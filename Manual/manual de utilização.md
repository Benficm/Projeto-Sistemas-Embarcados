
Instruções de Utilização

Para executar o projeto de monitoramento meteorológico, é necessário realizar a configuração do hardware e do software utilizados no desenvolvimento. O sistema foi desenvolvido utilizando a plataforma ESP32 e sensores ambientais conectados ao microcontrolador.

1. Requisitos de Hardware

Os principais componentes utilizados no projeto são:

Placa ESP32
Sensor de temperatura e umidade 
Sensor de pressão atmosférica 
Protoboard
Jumpers
Cabo USB para programação e alimentação
2. Requisitos de Software

As ferramentas necessárias para execução do projeto são:

Arduino IDE
Drivers da placa ESP32 instalados no computador
Bibliotecas dos sensores utilizadas no código
Conexão com a internet (para funcionalidades IoT)
3. Configuração do Ambiente
Instalar a Arduino IDE no computador.
Adicionar o suporte à placa ESP32 através do gerenciador de placas da IDE.
Instalar as bibliotecas necessárias para os sensores utilizados no projeto.
Conectar a placa ESP32 ao computador utilizando um cabo USB.
Selecionar a porta COM correspondente e o modelo correto da placa na IDE.
Abrir o código-fonte do projeto e realizar o upload para o ESP32.
4. Configuração da Rede Wi-Fi

No código-fonte do projeto, o usuário deverá configurar as credenciais da rede Wi-Fi:

const char* ssid = "NOME_DA_REDE";
const char* password = "SENHA_DA_REDE";

Essas informações são necessárias para que o ESP32 envie os dados coletados para a plataforma de monitoramento ou dashboard.

5. Execução do Sistema

Após o upload do código:

O ESP32 iniciará a leitura dos sensores automaticamente.
Os dados serão exibidos no monitor serial da IDE.
Caso o sistema utilize dashboard web ou aplicativo, os dados também serão enviados em tempo real pela rede Wi-Fi.
6. Informações Importantes
Verificar se todos os sensores estão conectados corretamente antes de energizar o circuito.
Utilizar uma fonte de alimentação adequada para evitar falhas no funcionamento.
Conferir se as bibliotecas instaladas são compatíveis com a versão utilizada da ESP32.
Em caso de falha na conexão Wi-Fi, o sistema poderá não enviar os dados para a plataforma online, mas continuará realizando as leituras localmente.
