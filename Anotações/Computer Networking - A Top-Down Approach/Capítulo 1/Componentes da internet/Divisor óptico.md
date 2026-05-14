Um **divisor óptico** é um componente usado em redes de fibra óptica para **dividir um sinal de luz em vários caminhos**.

Em inglês, ele aparece como:

> **optical splitter**  
> **splitter óptico**  
> **divisor óptico**

No contexto de FTTH/PON, ele fica entre a central da operadora e as casas.

```text
OLT da operadora
      ↓
fibra óptica principal
      ↓
divisor óptico / splitter
   ↓      ↓      ↓
ONT1   ONT2   ONT3
casa1  casa2  casa3
```

A função dele é permitir que **uma única fibra que sai da central** seja compartilhada por várias residências.

## Por que ele é “passivo”?

Na arquitetura **PON**, o divisor é chamado de passivo porque ele não precisa tomar decisões inteligentes nem, em geral, de energia elétrica para funcionar.

Ele não age como um switch, que lê endereços e decide para onde mandar o pacote.

O divisor óptico simplesmente faz algo físico:

> ele pega a luz que chega por uma fibra e a divide entre várias fibras de saída.

Por exemplo:

```text
1 fibra de entrada
      ↓
divisor 1:4
 ↓    ↓    ↓    ↓
4 fibras de saída
```

Ou:

```text
1 fibra de entrada
      ↓
divisor 1:8
 ↓ ↓ ↓ ↓ ↓ ↓ ↓ ↓
8 fibras de saída
```

Também existem divisores 1:16, 1:32, 1:64 etc.

## O que acontece no downstream?

No sentido **downstream**, ou seja, da operadora para as casas:

```text
OLT → divisor óptico → ONTs das casas
```

O sinal enviado pelo OLT chega ao divisor, e o divisor replica/divide esse sinal para todas as casas conectadas a ele.

Então, se o OLT manda dados para a casa 3, fisicamente o sinal pode chegar também às casas 1, 2 e 4.

```text
OLT envia dados para ONT3
        ↓
   divisor óptico
 ↓      ↓      ↓      ↓
ONT1   ONT2   ONT3   ONT4
```

Mas apenas o **ONT3** processa os dados destinados a ele. Os outros ONTs ignoram.

## O que acontece no upstream?

No sentido **upstream**, ou seja, das casas para a operadora:

```text
ONTs das casas → divisor óptico → OLT
```

O divisor faz o caminho inverso: combina os sinais vindos das várias casas em direção à fibra principal que vai para o OLT.

Mas como várias casas compartilham essa mesma fibra principal, os ONTs precisam transmitir de forma coordenada, para evitar que os sinais se misturem.

## Analogia simples

Imagine uma mangueira que chega em um adaptador com várias saídas:

```text
uma entrada → várias saídas
```

No caso da fibra, em vez de água, é luz.

Ou pense em uma tomada com benjamin/filtro de linha, mas para sinal óptico: uma entrada é distribuída para várias saídas. A diferença é que, na fibra, essa divisão reduz a potência do sinal, porque a mesma luz é repartida entre vários caminhos.

## Resumo

Um **divisor óptico** é:

> **um componente passivo da rede de fibra que divide um sinal óptico vindo da operadora para várias fibras que vão até diferentes casas.**

Em termos simples:

> **é o ponto onde uma fibra principal é repartida para atender vários clientes.**


![[Divisor óptico.png|655]]

