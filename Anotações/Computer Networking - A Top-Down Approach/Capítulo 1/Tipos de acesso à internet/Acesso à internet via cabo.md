
Enquanto a conexão [[DSL]] usa uma infraestrutura telefônica existente, o acesso à internet via cabo usa o cabo de televisão que já existe. A residência obtém acesso à [[internet]] pela companhia que opera a infraestrutura de cabo, muitas vezes a mesma usada historicamente para TV a cabo.  

Na imagem abaixo, você consegue entender como funciona o acesso à internet via cabo, que também é conhecido como HFC (Hybrid Fiber-Coaxial) porque emprega tanto [[Cabo de fibra óptica]] como [[Cabo coaxial]].

Esse tipo de conexão acontece da seguinte forma (partindo do seu celular, conectado à internet via Wi-fi, para a internet):

1- Você acessa o youtube
2- Essa informação é enviada via [[Ondas de rádio]] para seu [[Modem]].
3- Seu modem transforma a sua requisição que chegou em formato de [[Ondas de rádio]] em sinais elétricos adequados para trafegar pelo [[Cabo coaxial]]
4- O [[Cabo coaxial]] (que pode ser usado por várias outras residências da região) transporta esses sinais elétricos até o [[Nó de fibra]] da região.
5- O nó de fibra converte os sinais elétricos vindos do cabo coaxial em sinais ópticos, isto é, sinais de luz, para que possam trafegar pelo [[Cabo de fibra óptica]].
6- O cabo de fibra óptica leva os dados até a central da operadora de TV/Internet a cabo.
7- O [[CMTS]] (_Cable Modem Termination System_) recebe o tráfego vindo do [[Modem]], gerencia essa comunicação e encaminha os dados para a rede IP da operadora.
8- O [[Roteador]] encaminha os pacotes para a Internet, até que eles cheguem ao servidor solicitado.

![[Acesso Hibrido Fibra_Coaxial.png]]


Acesso à internet via cabo requer um modem a cabo. Em uma conexão [[DSL]], o modem a cabo é um dispositivo externo e se conecta ao PC caseiro através de uma porta Ethernet. 

Os modens a cabo dividem a rede HFC em dois canais: downstream e upstream. Assim como no modelo [[DSL]], o acesso é assimétrico, sendo o canal mais rápido o de downstream. 

Padrões de velocidade máxima teórica:

| Padrão         | Downstream máximo | Upstream máximo |
| -------------- | ----------------: | --------------: |
| **DOCSIS 2.0** |          ~40 Mbps |        ~30 Mbps |
| **DOCSIS 3.0** |         ~1,2 Gbps |       ~100 Mbps |
| **DOCSIS 3.1** |   até **10 Gbps** |  até **1 Gbps** |
| **DOCSIS 4.0** |   até **10 Gbps** |  até **6 Gbps** |

 Assim como no modelo [[DSL]], o máximo da velocidade geralmente não é atingido, por conta de pacotes com valores diferentes vendidos pela operadora, ou interferência externa.

Uma característica importante do acesso à internet via cabo é que ele é um meio de transmissão compartilhado por difusão. Isso é: os dados enviados pela provedora percorrem a rede comum e cada modem residencial pega apenas o que for destinado a ele. Isso faz com que a taxa de transmissão também seja compartilhada. Se muitos usuários estão baixando um arquivo pelo canal de downstream simultaneamente, a taxa que cada usuário recebe seu arquivo será menor que a taxa do cabo ou o plano contratado junto à operadora. Isso vale para ambos os canais.

