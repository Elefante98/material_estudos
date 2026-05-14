
Um **OLT** é o equipamento da operadora que fica na **central** e controla a rede de fibra óptica que chega até várias casas.

**OLT** significa:

> **Optical Line Terminator**  
> **Terminador de Linha Óptica**

Em uma rede FTTH/PON, a estrutura fica assim:

```text
Internet
   ↓
Roteadores da operadora
   ↓
OLT
   ↓
Fibra óptica principal
   ↓
Divisor óptico / splitter
   ↓
ONTs nas casas
```

## Função principal do OLT

O OLT é o equipamento que faz a ponte entre:

```text
Rede da operadora / Internet
        ↕
Rede óptica de acesso até os clientes
```

Ele conversa com vários **ONTs**, que são os equipamentos instalados nas residências.

```text
OLT da operadora ↔ ONT da casa
```

De forma simples:

> **O OLT é a “ponta da operadora” na rede de fibra. O ONT é a “ponta do cliente”.**

## O que o OLT faz?

Ele tem várias funções importantes:

1. **Envia dados para as casas**
    

No downstream:

```text
OLT → splitter → ONTs das casas
```

O OLT envia os dados pela fibra. O sinal chega ao splitter, que replica o sinal para várias casas. Cada ONT processa apenas os dados destinados a ele.

2. **Recebe dados das casas**
    

No upstream:

```text
ONTs das casas → splitter → OLT
```

Vários ONTs compartilham a mesma fibra principal até o OLT. Por isso, o OLT ajuda a coordenar quando cada ONT pode transmitir, para evitar que os sinais se misturem.

3. **Gerencia os ONTs**
    

O OLT identifica e controla os ONTs conectados à rede. Ele sabe quais clientes estão associados àquela porta/rede óptica e gerencia o tráfego de cada um.

4. **Conecta a rede óptica à rede IP da operadora**
    

Depois que o tráfego chega ao OLT, ele segue para os roteadores da operadora e depois para a Internet.

```text
ONT → splitter → OLT → roteadores da operadora → Internet
```

## Analogia com CMTS

Na comparação com Internet via cabo/HFC:

```text
HFC/cabo:
modem a cabo da casa ↔ CMTS da operadora

FTTH/PON:
ONT da casa ↔ OLT da operadora
```

Então, sim: o **OLT** é parecido com o **CMTS** no sentido de ser o equipamento central da operadora que gerencia vários clientes daquela tecnologia de acesso.

## Resumo simples

Um **OLT** é:

> **o equipamento da operadora que controla a rede de fibra óptica, comunica-se com os ONTs das casas e conecta esses clientes à rede da operadora/Internet.**

Em uma frase bem simples:

> **o ONT da sua casa fala com o OLT da operadora; o OLT fala com a Internet.**


![[OLT.png]]

