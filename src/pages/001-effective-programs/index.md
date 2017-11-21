---
title: Effective Programs
date: "2017-11-21"
---

10 Years of Clojure - Rich Hickey https://youtu.be/2V1FtfBDsLU

Visão do criador sobre que tipo de programas a linguagem destina.  Descreve information-driven situated programs como algo próximo a sistemas que tratam informação real, com protocolos, banco de dados, abstrações de dados e UI, tudo isso mudando com o tempo. Esses programas estão no extremo oposto de peças de software como compiladores que tem entrada e saída bem definida.

Crê que linguagens com tipagem estática não adicionam muita coisa para resolver essa classe problemas, ao contrário podem criar problemas na integração/comunicação. Sugere que quanto mais elaborado for o esquema de tipos mais a chance desses problemas ocorrerem. 
Ex: 832 classes java para descrever o vocabulário de um domínio. 
Clojure utiliza estruturas simples: mapas e chaves com namespaces. Uma checagem extra pode ser realizada utilizando Specs mas isso claramente é uma coisa opcional.

Insight: Formulário web deve ser tratado com Mapa de Strings e não com um tipo java, ex: Solicitação.

Insight: Possíveis boas práticas esquema GraphQL
- mais horizontal (colocar acesso da raiz)
 - menos profundo
 - utilizar tipos básicos ( quanto mais tipos mais difícil de se comunicar) paroquialism, faça o simples de sibelius

Provocação
será que os novos programas que processam informação não se transformarão apenas em nas pernas e pés (script de crawling) para alimentar apenas peças de algum esforço de  machine learning .
programmable programs, um programa pode afetar outro



