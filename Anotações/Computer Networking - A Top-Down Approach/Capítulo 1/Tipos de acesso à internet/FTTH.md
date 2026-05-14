
O modelo FTTH (Fiber To The Home), como o nome sugere, provê um [[cabo de fibra óptica]] do central office diretamente para as residências. Esse é um modelo de altíssima velocidade.

O FTTH pode ocorrer no modo Fibra direta, que leva um cabo de fibra óptica diretamente para cada casa, mas é mais comum que um cabo de fibra óptica seja compartilhado por várias residências. Quando está próximo das casas que ele vai servir, um dispositivo chamado [[Divisor óptico]] separa o cabo principal em vários cabos de fibra ópticos específicos de cada residência.

No modelo FTTH existem 2 arquiteturas: [[AON]] (Active Optical Network) e [[PON]] (Passive Optical Network).

No Central office existe os roteadores da provedora e um [[OLT]] que faz uma função parecida com a de um [[CMTS]] que é de conectar os roteadores da provedora com os das casas dos clientes (não necessariamente de forma direta nos dois). 

Esse [[OLT]] recebe os dados do roteador de borda da provedora e encaminha para o Divisor óptico referente ao destino da mensagem. Esse divisor óptico, na arquitetura PON (Passive Optical Network), não endereça os dados para um cabo específico (inclusive funciona sem energia), envia para todas as ramificações do cabo que o Divisor óptico criou, de forma semelhante a um [[nó de fibra]] no modelo de [[acesso à internet via cabo]].

Em cada casa, existe um [[ONT]] que acata apenas os pacotes endereçados a ele. Esse ONT geralmente está conectado a um roteador + ponto de acesso que faz os dados chegarem no dispositivo correspondente, de forma semelhante a um [[modem]].