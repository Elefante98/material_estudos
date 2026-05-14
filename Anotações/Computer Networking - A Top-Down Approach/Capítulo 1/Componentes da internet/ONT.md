Um **ONT** é o equipamento que fica na casa do cliente em uma conexão de fibra óptica.

**ONT** significa:

> **Optical Network Terminator**  
> **Terminador de Rede Óptica**

Em português mais natural:

> **equipamento que termina a rede óptica dentro da residência.**

Ele é a “ponta do cliente” na rede de fibra.

```text
Central da operadora
        ↓
       OLT
        ↓
fibra óptica
        ↓
divisor óptico
        ↓
       ONT
        ↓
roteador Wi-Fi
        ↓
celular / notebook / TV
```

## O que o ONT faz?

A fibra óptica transporta dados como **sinais de luz**. Só que os dispositivos da sua casa — roteador, computador, celular, TV — não trabalham diretamente com sinal óptico.

Então o ONT faz a conversão:

```text
sinal óptico da fibra → sinal elétrico/Ethernet
```

E no caminho contrário:

```text
sinal elétrico/Ethernet → sinal óptico para a fibra
```

Ou seja, ele permite que a rede de fibra da operadora se comunique com a rede doméstica.

## ONT é modem?

Didaticamente, sim, dá para pensar nele como o **“modem da fibra”**.

Mas tecnicamente, em redes FTTH/PON, o nome correto é **ONT**.

Comparando:

|Tecnologia|Equipamento na casa|
|---|---|
|Internet via cabo/HFC|modem a cabo|
|Internet via DSL|modem DSL|
|Internet via fibra/FTTH|ONT|

A função parecida é:

> receber o sinal da rede da operadora e entregar uma conexão utilizável para a rede da casa.

## ONT e roteador são a mesma coisa?

Não necessariamente.

O **ONT** conecta sua casa à fibra da operadora.

O **roteador** distribui a conexão dentro da sua casa.

```text
Fibra óptica → ONT → roteador → dispositivos
```

Mas muitas operadoras entregam um aparelho que junta tudo:

```text
ONT + roteador + Wi-Fi + switch Ethernet
```

Por isso, às vezes o usuário chama tudo de “roteador da fibra” ou “modem da fibra”.

## Resumo simples

Um **ONT** é:

> **o equipamento instalado na casa do cliente que recebe a fibra óptica, converte o sinal de luz em dados utilizáveis pela rede doméstica e se comunica com o OLT da operadora.**


![[ONT.png]]
