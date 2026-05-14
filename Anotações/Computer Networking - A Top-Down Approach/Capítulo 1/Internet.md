
## Visão geral (Componentes - Nuts-and-Bolts)

Para aprender [[rede]]s de computadores, usaremos a internet de exemplo.

Podemos descrever os componentes básicos (hardware) da internet. Depois, definiremos a internet como uma estrutura de rede interligando vários dispositivos.

A internet é uma [[rede]] de computadores que conecta bilhões de dispositivos. Talvez, chamar de rede de computadores seja até antiquado, já que a mais diversa sorte de dispositivos se conecta na Internet hoje em dia. Todos esses dispositivos conectados na internet sao chamados de "Hosts" ou "[[End system]]". Existem cerca de 30 bilhões de dispositivos conectados em 2026.


[[End system]]s são conectados por uma rede de enlace (cabos, fibra ótica e etc.) e comutadores de  pacotes (dispositivos que recebem um pacote e enviam para o próximo ponto da rede). Existem vários tipos de enlaces, como cabos de cobre, fibra óptica e onda de rádio. Enlaces diferentes, transmitem dados em velocidades diferentes. A taxa de transferência de dados é medida em bits/segundo. 

Quando um end system tem que enviar dados para outro, ele separa o dado em vários pacotes, adicionando dados no header para identificar cada parte. O end system receptor, recebe o dados, lê esses metadados e reorganiza os pacotes formando o dado original.

Comutadores de pacotes existem em muitos tipos e variedades, mas os mais comuns são Roteadores e Switches da camada de enlace. Um comutador de pacotes recebe um pacote entrando por algum de suas  entradas de enlace e encaminha por uma saída de enlace para o ponto mais próximo da rede.

A sequencia de enlace e comutadores de pacotes que um pacote atravessa da saída do remetente até o destinatário é chamada de Rota ou Caminho (route/path).

Pensar na rede como uma empresa de logistica de, por exemplo, peças de foguetes. Para transformar até a plataforma, vários caminhões transportam partes do foguete. No local de lançamento, temos uma ordem para montar o foguete funcionalmente.

Um [[End system]] acessa a internet através dos [[ISP]]s (Internet Service Providers). [[ISP]]s são redes de comutadores de pacotes e switches de enlace. Eles provém diversos tipos de conexão à rede, como . A internet se resume a conectar os end systems uns aos outros, então os [[ISP]]s também devem estar conectados. Os [[ISP]]s menores são conectados indiretamente via [[ISP]]s maiores (nacionais/internacionais), e esses [[ISP]]s maiores são conectados diretamente entre si. 

Isso quer dizer que a [[internet]] não é uma rede só dominada ou monopolizada, mas uma rede de redes menores.

[[End system]], packet switches e outras partes da [[internet]] operam seguindo algum [[protocolo]] (geralmente vários) que controlam o envio e recebimento de informações dentro da [[internet]]. Entre os [[protocolo]]s mais importantes, estão os TCP (Transmission Control Protocol) e IP (Internet Protocol).  Esses dois protocolos citados são usados geralmente coletivamente como TCP/IP!

É muito importante que todos operem de forma padronizada na internet, para que os sistemas interoperem.  Pra isso existem os padrões da internet, desenvolvidos pela IETF (Internet Engineering Task Force). Os documentos de padrão deles são chamados RFCs (Request for comments)

## Visão geral (Infraestrutura que provê serviços para aplicações)

Acima, a gente falou sobre uma descrição focada nos componentes (hardware) que formam a rede de redes que é a [[Internet]]. Agora, abordaremos uma visão de outro ângulo totalmente diferente.

A segunda maneira de descrever a internet é **"Um provedor de infraestrutura/serviço para aplicações"**.

Uma boa forma de exemplificar isso está abaixo.

Hoje em dia, a [[internet]] não interliga apenas computadores, mas também dispositivos mobile, eletrodomésticos, veículos e etc. No meio disso, existe um tipo especifico de aplicação chamado **Sistema distribuído**.

Sistemas distribuídos são aplicações onde acontece a troca de dado entre diferentes end systems que rodam a aplicação. Por exemplo um GPS que possui informações ao vivo sobre tráfego e acidentes na via.

Lembrando que uma aplicação não roda nos comutadores de pacotes, que, como o nome diz, apenas transfere dados para um destino. As aplicações rodam em end systems.

Voltando ao assunto, a [[internet]] serve como infraestrutura que viabiliza essa troca de dados, por exemplo.


![[Internet.png]]