O desafio proposto nesta atividade é desenvolver um programa que utilize a USART para transmitir uma mensagem ao computador que informe o estado de um botão conectado ao terminal PB1 do microcontrolador. O monitoramento do botão e a verificação do término da transmissão de cada caractere devem ser implementados utilizando a estratégia de varredura.

O botão é monitorado todo o tempo e, se ele não está pressionado, deve ser enviada a mensagem:
char msg_np[] = "Transmissao serial utilizando a USART: verificacao do termino da transmissao por varredura. O botao nao esta pressionado.\n\n";

Cada vez que a sequência inteira de caracteres da mensagem for transmitida, o programa deve aguardar 500ms antes de enviar a próxima mensagem. Se o botão estiver pressionado, a seguinte mensagem deve ser enviada:

char msg_p[] = "Transmissao serial utilizando a USART: verificacao do termino da transmissao por varredura. O botao esta pressionado.\n\n";

Utilize o resistor de pullup interno da porta no acionamento do botão, como feito em na Atividade 3. As configurações da USART são as mesmas discutidas na atividade de aula. O fluxograma a seguir sumariza o funcionamento do sistema.

![alt text](https://github.com/AlefeTiago/serial-transmission/blob/main/Fluxograma.PNG)
