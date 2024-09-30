Projeto de Monitoramento de Temperatura, Umidade e Movimento
Este projeto utiliza um microcontrolador (como o Arduino) para ler dados de temperatura e umidade usando um sensor DHT11 e dados de movimento utilizando um MPU-6050. Os dados são processados e exibidos no monitor serial.
Componentes Necessários
• Arduino (ou compatível)
• Sensor DHT11 (para temperatura e umidade)
• Sensor MPU-6050 (acelerômetro e giroscópio)
• Fios de conexão
• Breadboard (opcional)
Bibliotecas Necessárias
•
Wire.h
: Para comunicação I2C.
•
DHT.h
: Para o funcionamento do sensor DHT11.
•
math.h
: Para funções matemáticas.
Conexões
DHT11
•
VCC
: Conecte ao pino de 5V do Arduino
•
GND
: Conecte ao GND do Arduino
•
DATA
: Conecte ao pino digital 10 do Arduino
MPU-6050
•
VCC
: Conecte ao pino de 5V do Arduino
•
GND
: Conecte ao GND do Arduino
•
SDA
: Conecte ao pino A4 do Arduino
•
SCL
: Conecte ao pino A5 do Arduino
Código
O código realiza as seguintes funções:
1. Inicializa a comunicação serial e os sensores.
2. A cada 2 segundos, lê a temperatura, umidade, aceleração e rotação do MPU-6050.
3. Calcula a magnitude da aceleração e da rotação.
4. Imprime os dados lidos no monitor serial.
Estrutura do Código
•
Setup
: Inicializa os sensores e configura a comunicação.
•
Loop
: Lê os dados dos sensores e os imprime no monitor serial.
Compilação e Execução
1. Conecte seu Arduino ao computador.
2. Abra o Arduino IDE e copie o código fornecido.
3. Cole o código no editor do Arduino IDE.
4. Selecione a placa e a porta corretas nas configurações do Arduino IDE.
5. Carregue o código para o Arduino.
6. Abra o Monitor Serial para visualizar os dados.
Exemplo de Saída
bashCopiar códigoTemperatura: 25.0 °C, Umidade: 50.0 %, Aceleração: 0.5 km/h, Rotação: 0.3 giro/s

Observações
• Certifique-se de que os sensores estão conectados corretamente para evitar erros de leitura.
• O DHT11 pode demorar um pouco para estabilizar, especialmente se usado pela primeira vez.
Contribuições
Se você deseja contribuir para este projeto, sinta-se à vontade para fazer sugestões ou correções!
Sinta-se à vontade para modificar ou adicionar qualquer informação que considerar necessária!
