9.       Deve ser inserido no relatório um link para um repositório em github.com (inserido na seção Resultados de seu artigo) contendo a documentação do projeto apresentado. O repositório deve conter:

i)         Uma breve descrição do funcionamento e uso para quem quiser reproduzir.

Primeiro iremos conectar o sensor na saída 5 do Arduino. Assim como na imagem1 abaixo:
![descrição-img](/Docs/img/img1.jpeg)

Em seguida vamos usar nosso sensor na porta 6, ligando o Ecko nesta porta número, como na imagem2.
![descrição-img](/Docs/img/img2.jpeg)

Agora nesta parte será conectada o motor junto com o fio amarelo ligado na porta 7 do nosso Arduino

![descrição-img](/Docs/img/img3.jpeg)

Na sequência iremos conectar o GMD do nosso sensor com o GND do Arduino, e o vcc remos ligar em 5V, 
Deixando assim nosso sensor totalmente ligado. Veja na imagem abaixo:

![descrição-img](/Docs/img/img4.jpeg)

Vamos ligar o serve motor, o negativo dele iremos ligar no GND, e o positivo dele no 0,3,3V do nosso Arduino

![descrição-img](/Docs/img/img5.jpeg)

Vamos conectar a bateria , o positivo irá ligar no win e o negativo no primeiro GND .

![descrição-img](/Docs/img/img6.jpeg)

Adicionando Componentes no Hadware:

Iremos adicionar os componentes Arduino e sensor ao lado da lixeira, de preferencia uma lixeria quadrada pois nossos componentes irá se adequar melhor.
assim  como na imagem abaixo: 

![descrição-img](/Docs/img/img7.jpg)

neste imagem acima, foi colocado os componentes usando fitas para que os componentes fiquem seguro. 

Na parte da tampa da lixeira, usamos um papelão para servir como tampa, pois nosso motor irá puxar ela para abrir e fechar. Segue a imagem abaixo: 

![descrição-img](/Docs/img/img9.jpg)
![descrição-img](/Docs/img/img10.jpg)


Depois de ter feito esse processo iremos subir o nosso código que está neste repositório do GitHub na parte README.

Agora vamos conhecer um pouco de cada componente utilizado:

Sensor de Ultrassom HC-SR04:

![descrição-img](/Docs/img/sensor.jpeg)

O sensor de ultrassom HC-SR04 é posicionado estrategicamente próximo à abertura da lixeira, direcionado para a área onde os objetos seriam descartados.

O microcontrolador (ou qualquer outro dispositivo de controle) conectado ao sensor envia um sinal para iniciar a emissão do pulso ultrassônico.

O sensor emite o pulso de ultrassom e aguarda o retorno do sinal refletido.

Quando o sinal refletido é detectado, o sensor mede o tempo decorrido entre a emissão e o retorno do sinal.

Com base no tempo medido, o microcontrolador calcula a distância entre o sensor e o objeto em frente à lixeira.

Se a distância medida estiver dentro de um limite pré-definido, o microcontrolador aciona um mecanismo para abrir a tampa ou o compartimento da lixeira.

Após o descarte do objeto, o sensor de ultrassom continua a monitorar a área e, caso não detecte mais nenhum objeto próximo, o microcontrolador pode acionar um mecanismo para fechar a tampa ou o compartimento da lixeira.

Sensor de Ultrassom HC-SR04;

![descrição-img](/Docs/img/motor.jpeg)

O Micro Servo Motor de 9g é conectado a um microcontrolador ou a outro dispositivo de controle eletrônico. Geralmente, utiliza-se uma placa de desenvolvimento como Arduino ou Raspberry Pi para esse propósito.

O motor possui três fios: um fio de alimentação (VCC), um fio de terra (GND) e um fio de sinal (sinal). O fio de alimentação é conectado a uma fonte de energia, como uma bateria ou uma fonte de alimentação.

O fio de sinal é conectado a uma porta de saída do microcontrolador. O microcontrolador envia pulsos elétricos de largura variável através desse fio para controlar a posição do motor.

O microcontrolador ajusta a largura do pulso enviado ao motor para determinar a posição em que a tampa da lixeira deve ser aberta ou fechada. Por exemplo, um pulso de largura mínima pode representar a tampa fechada, enquanto um pulso de largura máxima pode representar a tampa completamente aberta.

Quando o microcontrolador envia um pulso para o motor, ele gira em uma determinada direção até alcançar a posição desejada.

O motor é equipado com um pequeno conjunto de engrenagens internas que amplificam o torque do motor, permitindo que ele mova a tampa ou o compartimento da lixeira.

O microcontrolador pode controlar o motor para abrir ou fechar a tampa da lixeira com base em comandos específicos, como a detecção de um objeto próximo por meio do sensor de ultrassom HC-SR04.

 Arduíno Uno;

 ![descrição-img](/Docs/img/arduinouno.jpeg)

 O Arduino Uno é conectado a diferentes componentes da lixeira eletrônica, como o sensor de ultrassom HC-SR04 e o Micro Servo Motor de 9g. Essa conexão pode ser feita por meio de fios e pinos na placa.

O sensor de ultrassom HC-SR04 é conectado a portas digitais do Arduino Uno. Essas portas são responsáveis por enviar e receber sinais digitais para interagir com o sensor.

O Micro Servo Motor de 9g é conectado a uma porta de saída PWM (Pulse Width Modulation) do Arduino Uno. As portas PWM permitem que o microcontrolador envie pulsos elétricos de largura variável para controlar a posição do motor.

O Arduino Uno é programado para ler os dados provenientes do sensor de ultrassom. Isso pode ser feito por meio de bibliotecas e funções específicas disponíveis no ambiente de programação do Arduino.

Com base nas leituras do sensor de ultrassom, o Arduino Uno decide quando abrir ou fechar a tampa da lixeira eletrônica. Ele pode enviar os sinais apropriados para o Micro Servo Motor de 9g para controlar a posição da tampa.

Além disso, o Arduino Uno pode ser programado para realizar outras funcionalidades, como exibir informações em um display LCD, registrar dados em um cartão SD ou se comunicar com outros dispositivos por meio de protocolos de comunicação, como Bluetooth ou Wi-Fi.

O Arduino Uno também pode ser alimentado por uma fonte de energia externa, como uma bateria ou uma fonte de alimentação.

A programação do Arduino Uno é feita em uma linguagem baseada em C/C++, utilizando o ambiente de desenvolvimento Arduino IDE. O código é escrito para definir as interações entre os componentes da lixeira eletrônica, como o sensor de ultrassom e o motor servo, e as ações a serem executadas com base nos dados recebidos.

Jumpers;


 ![descrição-img](/Docs/img/Jumpers.jpeg)


Na lixeira eletrônica, os jumpers podem ser utilizados para realizar conexões entre os diferentes componentes do sistema, como o sensor de ultrassom, o micro servo motor, o Arduino Uno e outros dispositivos eletrônicos.

Conexão entre o sensor de ultrassom e o Arduino Uno: Os jumpers podem ser usados para conectar os pinos de sinal do sensor de ultrassom às portas digitais do Arduino Uno. Isso permite que o Arduino leia os dados do sensor e tome decisões com base nessas informações.

Conexão entre o micro servo motor e o Arduino Uno: Os jumpers são usados para conectar o pino de controle PWM do micro servo motor a uma porta PWM do Arduino Uno. Isso permite que o Arduino envie os pulsos elétricos necessários para controlar a posição do motor e, assim, abrir e fechar a tampa da lixeira.

Conexões entre outros componentes: Dependendo do design e das funcionalidades desejadas, podem ser necessárias conexões adicionais entre o Arduino Uno, um display LCD, botões, LEDs ou outros dispositivos. Os jumpers podem ser usados para estabelecer essas conexões entre os pinos correspondentes.

Alterações e ajustes: À medida que o projeto evolui, é possível que seja necessário modificar as conexões entre os componentes. Os jumpers permitem que você faça alterações facilmente, desconectando-os de um local e conectando-os em outro conforme necessário.


iii)      A descrição do hardware utilizado (plataformas de desenvolvimento, sensores, atuadores, impressão 3D de peças, medidas de peças e caixas etc.)

iv)      A documentação das interfaces, protocolos e módulos de comunicação.

v)       O projeto deve possuir comunicação/controle via internet (TCP/IP) e uso do Protocolo MQTT.

<<<<<<< HEAD:Docs/index.md

# Diagrama de casos de uso

*&lt;Diagrama de casos de uso&gt;*
![descrição-dos-casos-de-uso](casosdeuso.jpeg)
=======
# Diagrama de casos de uso

*&lt;Diagrama de casos de uso&gt;*
![descrição-dos-casos-de-uso](casosdeuso.jpeg)
>>>>>>> 60c2f3b4e5cd42dcda110ac678bf9def5cf81e01:Docs
