# Projeto Claviculário Eletrônico

Projeto com o microcontrolador arduíno MEGA2560, utilizando linguagem de programação C.

Esse projeto consiste em um protótipo desenvolvido para instituições para facilitar o acesso e organização das chaves.

- Há uma inteface com display e teclado na parte frontal do claviculário para o usuário digitar sua senha;
- Um servomotor em posição que trava a porta do claviculário;
- Cada pessoa possui uma senha atrelada a si;
- Um sensor localizado na porta do claviculário para identificar se está fechado;
- Sensores localizados atrás das chaves;
- Um módulo rtc para identificar o horário.

No momento que um usuário digita sua senha corretamente, e o sensor da porta identifica que a porta está fechada, o microcontrolador manda um sinal para o servomotor para mudar de posição, assim destravando a porta. Assim que a porta é aberta, e o sensor da porta identifica que a porta está aberta, ele entende o usuário como "logado". A cada chave que é pega, ou devolvida, é identificado pelos sensores de cada chave, e microcontrolador envia esses dados para um arquivo txt com hora e data, criando assim, um "banco de dados". 

