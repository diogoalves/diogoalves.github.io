---
title: "Primeiro contato com aplicativos baseados em blockchain"
date: "2017-12-10"
---

Fiquei fascinado com as possibilidades de smart contracts após um amigo me apresentar o [CryptoKitties](https://www.cryptokitties.co/). Sempre imaginava a blockchain como simplesmente
uma assinatura de chave pública encadeada com objetivo de manter certa integridade nas 
transações. Não é só isso, a possibilidade de rodar código de forma descentralizada
abre espaço para mudar várias regras do jogo. 

Ao ler [How to Code Your Own CryptoKitties-Style Game on Ethereum](https://medium.com/loom-network/how-to-code-your-own-cryptokitties-style-game-on-ethereum-7c8ac86a4eb3), fica mais claro que o jogo não é 100% baseado em blockchain mas apenas utiliza a blockchain com estrutura de dados persistente e com backend para rodar alguns smart contracts. Genial.

Parte do [código](https://ethfiddle.com/09YbyJRfiI) está aberto e já da pra sentir que a linguagem de programação é um frankstein meio pé-duro. Talvez, limitações de segurança forçaram a certos decisões defensivas no design na linguagem. Ainda não programei nada nela mas parece mais uma pedra brilhante que já já vou tentar pegar.

O mesmo amigo que mostrou o Cryptokitties me enviou o link dessa [playlist](https://www.youtube.com/watch?v=zVqczFZr124&list=PLzvRQMJ9HDiTqZmbtFisdXFxul5k0F-Q4) que apresenta uma introdução gentil como criar uma blockchain em javascript. Esse [vídeo](Esse vídeo da khan academy mostra um pouco sobre o funcionamento 
) da khan academy mostra um pouco sobre o funcionamento de proof-of-work.

```
f(c, p) = resultado
f -> função de hash criptográficamente segura
c -> challenge
p -> proof-of-work string
resultado -> deve obdecer alguma restrição que obrigue algum esforço computacional, por exemplo começar com 40 zeros.
``` 
A primeira coisa que penso é será que conseguiriamos pré-calcular alguma parte do proof-of-work??? Será que fpgas, asics, gpus, computação quântica podem ser utilizados para isso? Qual a função de hash do bitcoin, ethereum? 

E se surgirem dois p diferentes, quem decide? Será que um ator grande pode aceitar apenas um subconjunto de Ps?
>Nodes always consider the longest chain to be the correct one and will keep working on
extending it. If two nodes broadcast different versions of the next block simultaneously, some
nodes may receive one or the other first. In that case, they work on the first one they received,
but save the other branch in case it becomes longer. The tie will be broken when the next proofof-work
is found and one branch becomes longer; the nodes that were working on the other
branch will then switch to the longer one. 

Qual o custo de transação de bitcoin e ethereum? [Aqui](https://bitinfocharts.com/comparison/transactionfees-btc-eth.html). Um [panorama](https://bitinfocharts.com/) geral das principais moedas.

Incentivo para permanecer honesto.
> The incentive may help encourage nodes to stay honest. If a greedy attacker is able to
assemble more CPU power than all the honest nodes, he would have to choose between using it
to defraud people by stealing back his payments, or using it to generate new coins. He ought to
find it more profitable to play by the rules, such rules that favour him with more new coins than
everyone else combined, than to undermine the system and the validity of his own wealth. https://bitcoincore.org/bitcoin.pdf


