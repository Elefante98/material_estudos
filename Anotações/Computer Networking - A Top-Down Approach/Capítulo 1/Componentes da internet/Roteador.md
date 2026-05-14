Um **roteador** é um equipamento que conecta **redes diferentes** e decide por qual caminho os dados devem seguir.

Em redes de computadores, ele é chamado de **router** em inglês.

A ideia central é:

> **o roteador encaminha pacotes de dados entre redes.**

---

## Exemplo simples: sua casa

Na sua casa, o roteador normalmente conecta a sua **rede doméstica** à **rede da operadora/Internet**.

```text
Celular
Notebook
TV
   ↓
Rede da sua casa / Wi-Fi
   ↓
Roteador
   ↓
Modem / operadora
   ↓
Internet
```

Quando você acessa o YouTube, por exemplo:

```text
Seu celular → roteador → operadora → Internet → servidor do YouTube
```

Na volta:

```text
Servidor do YouTube → Internet → operadora → roteador → seu celular
```

---

## O que o roteador faz?

Ele recebe pacotes de dados e decide para onde enviá-los.

Um pacote pode ser imaginado como uma “cartinha” com endereço de origem e destino.

Exemplo simplificado:

```text
Origem: seu celular
Destino: servidor do YouTube
Conteúdo: quero acessar este vídeo
```

O roteador olha principalmente para o **endereço IP de destino** e decide o próximo caminho.

---

## Roteador usa IP

O roteador trabalha principalmente na **camada de rede**, ou **camada 3**, e usa endereços **IP**.

Exemplo de IP:

```text
192.168.0.10
```

ou

```text
8.8.8.8
```

Então:

```text
Roteador → usa IP para encaminhar pacotes
Switch → usa MAC para encaminhar quadros dentro da rede local
```

---

## Diferença entre roteador e switch

Essa diferença é muito importante.

### Switch

O **switch** conecta dispositivos dentro da mesma rede local.

```text
PC A ─┐
PC B ─┼── Switch
PC C ─┘
```

Ele funciona como uma “central interna” da rede local.

### Roteador

O **roteador** conecta redes diferentes.

```text
Rede da sua casa ── Roteador ── Internet
```

Comparando:

|Equipamento|Função principal|Usa principalmente|
|---|---|---|
|Switch|Conectar dispositivos na mesma rede local|Endereço MAC|
|Roteador|Conectar redes diferentes|Endereço IP|


![[Roteador.png]]

---

## Roteador residencial e roteador da operadora

O roteador da sua casa é uma versão pequena dessa ideia.

Mas existem roteadores muito maiores nas operadoras e na Internet.

Na imagem da rede HFC, depois do CMTS aparecem roteadores da operadora:

```text
Casas
 ↓
Cabo coaxial
 ↓
Nó de fibra
 ↓
Fibra
 ↓
CMTS
 ↓
Roteadores da operadora
 ↓
Internet
```

Esses roteadores encaminham pacotes entre a rede da operadora e outras redes da Internet.

---

## O roteador também cria o Wi-Fi?

No uso doméstico, geralmente sim, mas tecnicamente são funções diferentes.

Aquele aparelho da sua casa costuma ser vários equipamentos em um só:

```text
Modem + roteador + ponto de acesso Wi-Fi + switch
```

Por isso muita gente chama tudo de “roteador”.

Mas tecnicamente:

- **modem**: conecta sua casa à rede da operadora;
    
- **roteador**: conecta sua rede doméstica à Internet e encaminha pacotes;
    
- **Wi-Fi/access point**: cria a rede sem fio;
    
- **switch**: permite conectar dispositivos por cabo dentro da rede local.
    

---

## Analogia simples

Imagine que redes sejam bairros.

O **switch** entrega mensagens dentro do mesmo prédio ou condomínio.

O **roteador** decide para qual bairro, cidade ou estrada a mensagem deve ir.

```text
Dentro da sua casa/rede → switch/Wi-Fi
Entre redes diferentes → roteador
```

---

## Resumo

Um roteador é:

> **um equipamento que conecta redes diferentes e encaminha pacotes usando endereços IP.**

Em termos simples:

> **ele é o “guia de caminho” dos dados entre sua rede e outras redes, como a Internet.**