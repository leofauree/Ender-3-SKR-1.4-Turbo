# Ender-3-SKR-1.4-Turbo

Adicionando aqui o firmware que compilo para a minha Ender 3 Pro, que usa a placa SKR 1.4 Turbo da Bigtreetech. 

Até o momento, foram adicionadas algumas mudanças, que no momento do primeiro commit são:

Configuration.h
-Velocidade e aceleração levemente aumentadas do original (DEFAULT_MAX_FEEDRATE          { 500, 500, 20, 50 }, DEFAULT_MAX_ACCELERATION      { 500, 500, 200, 5000 })
-Utilização para Drivers TMC2208 nos motores X,Y,Z e E0
-Hybrid Treshold alterado para que somente acima de 120mm/s faça algum barulho de drivers
-Mesh Bed Leveling habilitado com uma matriz de 4x4
-Menu de Nivelamento direto no LCD
-Nivelamento de 4 pontos no LCD
-Modificado valor de E-Steps para utilização de extrusora com dupla engrenagem (80, 80, 400, 142)
-Cooler da extrusora só é acionado á partir de 50graus
-Máxima temperatura da mesa de 125 graus celsius
-Mínima temperatura do bico para extrusão de 180 graus
-PID refeito para uso do sistema Bullseye
-Adicionado menu de PID no LCD
-Adicionado opção de PID da Mesa
-Setado limite de volume real a ser utilizado (#define X_BED_SIZE 235 #define Y_BED_SIZE 235 	#define Z_MAX_POS 250)
-Sensor de fim de filamento ativado utilizando um switch comum
-Habilitado gravação da EEPROM

Configuration_adv.h
-Configurado pin do cooler da extrusora
-Habilitada função de Quick Home (movimentos simultaneos de todos os motores)
-Alterado feedrate da extrusora para movimentos no LCD
-Adicionado menu de Info no LCD
-Adicionado Scroll quando a informação é maior que o display permite enxergar
-Configurada entrada de SD Card
-Adicionada função de BabyStepping com o duplo clique na tela inicial
-Adicionado Advanced Pause
-Configurados valores de tensão e corrente para os drivers TMC2208
-Configurado drivers TMC 2208 em modo UART


Qualquer dúvidas estou disponível :)
