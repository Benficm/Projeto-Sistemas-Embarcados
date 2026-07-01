
# Materiais

Os materiais utilizados no desenvolvimento do projeto foram:

ESP32;
Sensor de temperatura e umidade DHT11;
Protoboard;
Jumpers;
Cabo USB para alimentação e programação do ESP32;
Computador para desenvolvimento e testes.

Além dos componentes eletrônicos, foram utilizadas ferramentas de software para programação, testes e organização do projeto, como Arduino IDE, GitHub e Trello.

# Desenvolvimento

O desenvolvimento do projeto foi dividido em etapas, permitindo que a equipe validasse o funcionamento de cada componente antes da integração completa do sistema.

Inicialmente foi realizado o levantamento dos requisitos e a definição da arquitetura do projeto, escolhendo o ESP32 como plataforma principal devido ao seu baixo custo, capacidade de processamento e conectividade Wi-Fi integrada.

Em seguida foi realizada a montagem do circuito eletrônico em protoboard, conectando o sensor DHT11 ao ESP32 conforme sua pinagem. Após essa etapa, iniciou-se o desenvolvimento do software responsável pela leitura dos dados do sensor.

Os primeiros testes consistiram na verificação da comunicação entre o microcontrolador e o sensor, validando a leitura correta da temperatura e da umidade do ar através do Monitor Serial da Arduino IDE.

Após a validação das leituras, foram implementadas melhorias no código para tornar a coleta dos dados mais estável, além da integração com a interface de visualização utilizada pelo projeto.

Durante todo o desenvolvimento foram realizados testes funcionais para verificar a confiabilidade das medições e corrigir eventuais falhas de comunicação entre hardware e software.

Ao final, o sistema apresentou funcionamento satisfatório, realizando continuamente a coleta e a disponibilização das informações meteorológicas.


### Interface

Foi desenvolvida uma interface simples e intuitiva para apresentar ao usuário as informações coletadas pelo sistema meteorológico.

A interface permite visualizar em tempo real os valores de temperatura e umidade do ambiente, facilitando o acompanhamento das condições climáticas.

O objetivo principal foi criar uma visualização clara, organizada e de fácil interpretação, permitindo que qualquer usuário consiga consultar as informações sem necessidade de conhecimentos técnicos.

### Código

O desenvolvimento do código da interface foi realizado de forma modular, permitindo a atualização automática dos dados enviados pelo ESP32.

Foram implementadas funções responsáveis por receber os valores enviados pelo microcontrolador, processar essas informações e apresentá-las ao usuário de maneira organizada.

A estrutura do código foi desenvolvida visando facilitar futuras expansões do sistema, permitindo adicionar novos sensores e novas funcionalidades sem grandes alterações na arquitetura do projeto.

## Desenvolvimento do Hardware

### Montagem

A montagem do hardware foi realizada inicialmente em uma protoboard, facilitando a realização de testes e possíveis alterações durante o desenvolvimento.

O sensor DHT11 foi conectado ao ESP32 utilizando cabos jumper, respeitando a alimentação e os pinos de comunicação especificados pelo fabricante.

Após a montagem, foram realizados testes elétricos para verificar a alimentação correta dos componentes e garantir o funcionamento adequado do circuito antes da execução do software.

Essa abordagem permitiu corrigir rapidamente possíveis erros de ligação durante o processo de desenvolvimento.

### Desenvolvimento do Código

O código embarcado foi desenvolvido utilizando a linguagem C++ na Arduino IDE.

Inicialmente foram configuradas as bibliotecas necessárias para comunicação com o sensor DHT11 e com o ESP32.

Posteriormente foram implementadas as funções responsáveis por inicializar os dispositivos, realizar a leitura periódica da temperatura e da umidade e disponibilizar essas informações para visualização.

Durante o desenvolvimento foram realizados diversos testes para garantir a estabilidade das leituras, reduzindo erros ocasionais do sensor e assegurando o funcionamento contínuo do sistema.
