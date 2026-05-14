
Em Ciência da Computação, a ideia de **rede** é:

> **um conjunto de elementos conectados entre si, capazes de trocar informações, recursos ou serviços.**

No contexto de **redes de computadores**, uma rede é um conjunto de dispositivos conectados para se comunicarem.

Exemplo simples:

```text
Notebook ── Roteador ── Internet ── Servidor do YouTube
```

Esses elementos podem ser:

- computadores;
    
- celulares;
    
- servidores;
    
- roteadores;
    
- switches;
    
- impressoras;
    
- sensores;
    
- cabos;
    
- antenas;
    
- enlaces sem fio.
    

A ideia central é **comunicação**.

## Rede não é só “Internet”

A Internet é uma rede gigantesca, mas existem redes menores.

Por exemplo:

```text
Sua casa:
Celular ─┐
Notebook ├── Roteador Wi-Fi ── Internet
TV      ─┘
```

Isso já é uma rede local.

Uma empresa também tem sua rede:

```text
Computadores ── Switch ── Servidor interno ── Roteador ── Internet
```

Uma faculdade, banco, hospital ou datacenter também possuem redes próprias.

## O que uma rede permite?

Uma rede permite que dispositivos:

1. **troquem dados**
    

Exemplo: seu navegador pede uma página para um servidor.

```text
Seu computador → pedido → servidor
Seu computador ← resposta ← servidor
```

2. **compartilhem recursos**
    

Exemplo: vários computadores usando a mesma impressora.

3. **acessem serviços remotos**
    

Exemplo: acessar Google Drive, YouTube, Netflix, WhatsApp, banco online etc.

4. **trabalhem de forma distribuída**
    

Exemplo: uma aplicação em que o frontend roda no seu navegador, o backend roda em um servidor e o banco de dados roda em outro.

## A ideia mais abstrata de rede

De forma mais geral, uma rede é composta por:

```text
Nós + conexões
```

Ou seja:

- **nós**: os pontos da rede;
    
- **conexões**: os caminhos entre esses pontos.
    

Exemplo em redes de computadores:

```text
Nós = computadores, roteadores, servidores
Conexões = cabos, fibra, Wi-Fi, enlaces de rádio
```

Visualmente:

```text
A ─── B ─── C
│     │
D ─── E
```

Cada letra pode representar um dispositivo, e cada linha representa uma conexão.

## Em redes de computadores, o que trafega?

O que trafega são **dados**.

Mas esses dados normalmente não vão como um bloco único. Eles são divididos em pequenas partes chamadas **pacotes**.

Exemplo:

```text
Mensagem original:
"Olá, servidor, quero acessar este site"

Dividida em pacotes:
[Pacote 1] [Pacote 2] [Pacote 3]
```

Esses pacotes passam por vários equipamentos até chegar ao destino.

## Por que isso importa?

Porque quase tudo que usamos hoje depende de redes:

```text
WhatsApp
Pix
YouTube
Netflix
Jogos online
Sistemas de empresa
APIs
Banco de dados na nuvem
Sites
E-mails
Aplicativos de entrega
```

Quando você faz uma requisição para uma API, por exemplo, seu computador está usando uma rede para enviar dados até um servidor e receber uma resposta.

## Resumo simples

Em Ciência da Computação, uma rede é:

> **uma estrutura de dispositivos conectados que permite comunicação e troca de dados.**

Em termos ainda mais simples:

> **rede é o caminho organizado que permite que computadores conversem entre si.**