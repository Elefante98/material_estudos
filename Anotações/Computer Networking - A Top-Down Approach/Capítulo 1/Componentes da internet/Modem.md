
Um **modem** é um equipamento que permite que sua casa/dispositivo se comunique com a rede do provedor de Internet.

A palavra **modem** vem de:

> **MOdulator + DEModulator**  
> **modulador + demodulador**

Ou seja, ele **modula** e **demodula** sinais.

## A ideia simples

Seu computador/celular trabalha com dados digitais:

```text
0 e 1
```

Mas a rede do provedor pode transmitir esses dados usando outro tipo de sinal, por exemplo:

```text
sinais elétricos no cabo coaxial
sinais na linha telefônica
sinais ópticos na fibra
sinais de rádio em redes móveis
```

O modem faz a adaptação entre esses mundos.

```text
Dados digitais do seu dispositivo
        ↓
modem transforma em sinal adequado para a rede do provedor
        ↓
rede do provedor / Internet
```

E no caminho de volta:

```text
sinal vindo do provedor
        ↓
modem interpreta esse sinal
        ↓
dados digitais para seu dispositivo
```

## Exemplo na Internet via cabo

No caso da rede HFC, que você estava estudando:

```text
Seu celular
 ↓ Wi-Fi
Roteador/modem da casa
 ↓
Cabo coaxial
 ↓
Fiber node
 ↓
Fibra óptica
 ↓
CMTS
 ↓
Internet
```

O **modem a cabo** pega os dados da sua rede doméstica e transforma em sinais adequados para trafegar pelo **cabo coaxial**.

Ele também faz o contrário: recebe sinais vindos do cabo coaxial e transforma de volta em dados que seus dispositivos conseguem usar.

## Modem e roteador são a mesma coisa?

Não exatamente.

Eles podem estar no mesmo aparelho, mas fazem funções diferentes.

### Modem

O **modem** conecta sua casa à rede do provedor.

```text
Casa ↔ Provedor
```

### Roteador

O **roteador** cria e organiza a rede interna da sua casa.

```text
Celular
Notebook
TV
Impressora
   ↓
Roteador
   ↓
Modem
   ↓
Internet
```

O roteador distribui a conexão entre vários dispositivos, geralmente por Wi-Fi e cabo Ethernet.


![[Modem.png]]

## Por que muita gente chama tudo de “modem”?

Porque, na prática, muitas operadoras entregam um aparelho que é várias coisas ao mesmo tempo:

```text
Modem + roteador + Wi-Fi + switch
```

Aquele aparelho da operadora normalmente faz tudo isso:

- conecta sua casa ao provedor;
    
- cria a rede Wi-Fi;
    
- distribui IPs para os dispositivos;
    
- permite conectar cabos Ethernet;
    
- encaminha os dados entre sua rede doméstica e a Internet.
    

Tecnicamente, porém:

> **modem é a parte que fala com a rede do provedor; roteador é a parte que organiza a rede da sua casa.**

## Analogia simples

Imagine que a Internet seja uma estrada grande fora da sua casa.

O **modem** é como o portão que conecta sua casa à estrada externa.

O **roteador** é como a organização interna da casa, decidindo para qual cômodo cada entrega vai.

```text
Internet/provedor → modem → roteador → celular/notebook/TV
```

## Resumo

Um modem é:

> **o equipamento que converte os dados da sua rede em sinais compatíveis com a rede do provedor, e converte os sinais do provedor de volta em dados digitais.**

Em termos mais simples:

> **é o aparelho que faz sua casa “conversar” com a rede da operadora.**