---
layout: post
title: Intervalo entre Números Primos
date: 2008-04-04 10:00:00 +1000
categories: mathematics blog
mathjax: true
---

# Intervalo entre Números Primos

  
Minha mulher me pediu 5 números consecutivos que não fossem números primos.  
  
Não acreditam? Ok, ela não pediu isso mesmo, é claro, fui eu quem a induzi a fazer esta pergunta. Em resposta apresentei a lista, que já havia calculado anteriormente: 24,25,26,27,28  
  
Ela não se impressionou e ainda me olhou com uma cara esquisita do tipo: “Você está com algum problema?”. Não desanimei e lembrei-a que todos os números da minha lista não eram primos. Ela deu de ombros e continuou a fazer coisas menos nobres e importantes como, por exemplo, o meu jantar. (em minha defesa, eu faço o jantar às vezes, faço uma pizza maravilhosa, vem até com embalagem da pizzaria da esquina).  
  
Desafiei-a a fazer o mesmo, e pedi para me fornecer 3 números consecutivos não primos. Ela, jubilosa, disse: 14,15,16.  
  
Fiz contato!  
  
Ela investiu novamente, exigindo uma lista de 10 números. Já treinado, disparei: 114, 115, 116, 117, 118, 119, 120, 121, 122, 123.  
  
Antes que o leitor me julgue um _idiot savant_, acrescento que já havia calculado alguns valores adiantando os números que ela tipicamente iria escolher.  
  
Era minha vez novamente. Pedi entusiasmado: "Quero uma lista com 14000 números." Ela respondeu : "O jantar está na mesa!". Pronto, fim da brincadeira.  
  

>**_Espaço Mobral_**_: Um_ **_número primo_** _é um número que só pode ser dividido por 1 e por ele mesmo sem deixar resto. Os primeiros números primos são: 2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, ..._

  
Matemáticos dificilmente encontram apoio social para conversar sobre seus assuntos prediletos, de maneira que muitas vezes fragmentos de atenção de baixa qualidade como esse são suficientes para despertar nossa vontade de pesquisar um pouco mais profundamente.  
  
**Uma chance para a computação**  
  
Instintivamente não é óbvio que uma lista tão grande possa existir, afinal a lista de números primos é infinita e eles não parecem estar muito espaçados.  
  
Enfim, a pergunta é: É possível encontrar uma lista de 14000 números consecutivos que não são primos?  
  
Esta pergunta, que eu mesmo fiz (matemáticos muitas vezes falam sozinhos) me inspirou a utilizar artilharia mais pesada. Desenvolvi um programa para encontrar a tal mega lista, se é que ela existe. Para testá-lo, comecei com listas pequenas, pedi 10 números e o programa respondeu os mesmos 10 que eu havia dito para minha esposa. Bom sinal.  
  
Pedi 20 números e obtive: 1130 , 1131, 1132,...  
  
Pedi 100 números e obtive: 370262, 370263, 370264, ...  
  
Guloso, pedi 14000 e ... esperei... Esperei tanto que desisti . O programa simplesmente não parou de rodar. Diante deste quadro, a única conclusão é que o programa procurou (e procurou muito) mas não encontrou a lista nos primeiros milhões, ou bilhões (quem sabe) de números. Ainda assim não é possível afirmar que tal lista não existe, apenas que o computador ou o programa são lentos demais. Frustrante!  
  
**Um belo teorema**  
  
Sempre acreditei que quando a computação falha devemos recorrer a matemática, e parece que isso se encaixa perfeitamente a esse caso. Existe um belíssimo teorema sobre o assunto. O teorema diz que: “É possível conseguir listas de números não primos de QUALQUER tamanho”. Que 14000 que nada! Eu quero agora uma lista de 1.000.000!  
  
O teorema ilustra uma técnica para se construir o primeiro número da lista desejada. A receita é a seguinte:  
  
Suponha que queremos uma lista com 5 números consecutivos não primos. Então devemos:  
  

- Escolher um número inteiro maior do que 1, digamos _n_

- Obter o primeiro número da lista calculando _n(n+1)(n+2)(n+3)(n+4) + n_

  
Por exemplo, considerando _n = 2_, teríamos 2 x 3 x 4 x 5 x 6 + 2 = 722. De fato a lista 722, 723, 724, 725, 726 só possui números não primos. Podemos escolher qualquer valor para n. No caso _n = 3_, a lista seria 2523, 2524, 2525, 2526, 2527, também uma lista válida.  
  
Observe que a fórmula não diz nada sobre encontrar a lista cujos números são os menores possíveis, ela apenas garante que encontraremos alguma lista do tamanho desejado. Como vimos anteriormente, a lista 24, 25, 26, 27, 28 é uma lista com números menores.  
  
Para construir listas maiores basta estender a formula com mais fatores. Por exemplo, a fórmula para encontrarmos uma lista com 7 números será _n(n+1)(n+2)(n+3)(n+4)(n+5)(n+6) + n_.  
  
Ora, mais por que isso funciona? Simples, observe que o número _n(n+1)(n+2)(n+3)(n+4) + n_ é divisível por _n_, portanto um número não primo (já que _n_ é maior do que 1). O próximo número _n(n+1)(n+2)(n+3)(n+4) + (n+1)_ também não é primo pois é divisível por _(n+1)_. Enfim, o raciocínio pode ser estendido para todos os números consecutivos até _n(n+1)(n+2)(n+3)(n+4) + (n+4)_ que obviamente é divisível por _(n+4)_.  
  
Enfim, existem infinitos números primos e, mesmo assim, sempre é possível encontrar qualquer intervalo de números sem que ao menos 1 primo apareça. Este intervalo pode ser tão grande quanto desejarmos. Sabemos então que uma lista de 14000 números consecutivos não primos existe, só não conseguimos calcular seus números devido ao tamanho imenso do mesmo. Mesmo uma lista de 117 números, que meu computador conseguiu calcular, começa no número 1.349.534.