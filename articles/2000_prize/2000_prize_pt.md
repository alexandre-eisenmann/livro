---
layout: post
title: Prêmio de 2000 R$!
date: 2008-01-12 10:00:00 +1000
categories: mathematics blog
mathjax: true
---

# Prêmio de 2000 R$!


Ofereço 2000 reais para o primeiro que resolver o desafio abaixo.

Deslizar as placas numéricas de forma a alterar o número 14 com número 15 e ordenar todo o conjunto. Como todos sabem este clássico brinquedo só permite movimentos em direção ao espaço vazio das placas imediatamente adjacentes, posicionadas em cima, abaixo ou dos lados, não sendo possível destacar placas ou outras malandragens do tipo. A figura à esquerda mostra o ponto de partida enquanto a figura da direita mostra aonde devemos chegar para completar o desafio.


![[left.png]]![[right.png]]



Considerei 2000 reais um valor adequado. Se oferecesse mais não me levariam a sério, se oferecesse menos não levariam a tarefa a sério. Além disso, 2000 R$ é equivalente a 1000 dólares, quantia que Sam Loyd ofereceu em 1878 para quem resolvesse o mesmo problema, então, porque não seguir a tradição.

Sam Loyd foi o maior expert americano em puzzles da época. Em suas próprias palavras, ele “deixou o mundo inteiro doido” ao propor “seu” recém descoberto puzzle 14-15. Na verdade a história provou não ter sido ele o primeiro a propor o puzzle. De fato o criador foi o agente postal Noyes Chapmak que inclusive solicitou a patente da descoberta. Para conhecer mais a história consulte http://bd.thrijswijk.nl/15puzzle/15puzzen.htm

Porque Sam Loyd esbanjou tanto dinheiro assim? Porque eu mesmo, seguindo os passos dele também estou esbanjando? Simples, Sam Loyd não precisou pagar um centavo pois ninguém resolveu o problema. E eu também não vou perder nada, pois o problema não possui solução, é impossível resolvê-lo.

Sam Loyd foi bem mais longe, ele não disse que era impossível e deixou algumas pessoas realmente enfurecidas. Eu adotarei outra abordagem, tentarei provar sem usar uma linguagem muito técnica que é impossível.

Como é possível provar que algo é impossível?

Provar que algo é impossível sempre despertou minha curiosidade. É simples imaginar como provar que algo é possível, basta fazê-lo e pronto, é possível. Por outro lado, provar que algo é impossível sempre me soou como uma desculpa para... Ora... é impossível porque ninguém ainda fez.

Não era possível ir até a Lua até que alguém foi lá e fez! Não era possível alguém ser atingido por um raio 7 vezes até que alguém foi lá e tomou! Bom, para aqueles inclinados a fazer os comentários ao lado sugiro acompanhar a demonstração abaixo, onde de fato é possível provar que resolver o puzzle 14-15 é impossível a ponto de eu oferecer 2000 reais ou muito mais para quem resolvê-lo.

Um passeio pelo problema

Uma tentativa de solução pode ser entendida com um "passeio" do espaço vazio através do tabuleiro. O passeio deverá começar e terminar na mesma posição, isto é, abaixo e à direita. Por exemplo, suponha que durante uma tentativa o espaço vazio realize o seguinte passeio, representado na figura pela seta em azul: Esquerda-Esquerda-Cima-Direita-Cima-Direita-Baixo-baixo. Esse passeio possui, portanto, 8 passos de comprimento, mas como vocês podem verificar, não resultou na configuração desejada.

![[A.png]]![[B.png]]![[C.png]]

Todo passeio (e somente) que comece e termine no canto inferior direito é um candidato a solução. Observe, portanto, que a solução deverá necessariamente ser um passeio com um número par de passos. É fácil perceber isso se levarmos em conta que o número de passos para a esquerda deverá ser igual ao número de passos para a direita, da mesma forma, o números de passos para cima deverá ser igual ao número de passos para baixo. Só assim voltaremos ao ponto em que saímos, e obviamente esta exigência resulta em um número par de passos.

Esse é nosso primeiro resultado e vou destacá-lo para utilizarmos futuramente.

Uma solução, se existir, deverá necessariamente possuir um número par de passos.
Uma medida para a organização

Cada passo ou movimento altera a organização do jogo, porém não temos uma medida de organização que possa servir de parâmetro para cada movimento. Por exemplo, dado duas configurações, é difícil dizer qual é a que está mais organizada. Bom, vou propor uma medida e o leitor irá verificar que ela será muito útil para a solução do problema. Chamarei esta medida de medida I.

Primeiramente, vou estabelecer que quando a configuração está o mais organizada possível, isto é, totalmente ordenada, ela possui medida I = 0. Assim, representando a configuração em apenas uma tira de números temos (note que representei o espaço vazio com o número 16):

1	2	3	4	5	6	7	8	9	10	11	12	13	14	15	16
Medida I = 0

Toda a vez que um número possui números menores a sua direita, contamos um. Por exemplo, a partir da sequência totalmente ordenada (I=0), invertemos o número 6 com o número 10. A tabela abaixo apresenta esta nova disposição, que por sua vez terá I=7, resultado da soma 4+1+1+1.

1	2	3	4	5	10	7	8	9	6	11	12	13	14	15	16
0	0	0	0	0	4	1	1	1	0	0	0	0	0	0	0
Medida I = 7

Abaixo da sequência que queremos analisar inclui uma linha suporte. Cada posição da linha suporte, deverá conter a quantidade de números da linha original que são menores do que o que está acima. Note que o número 10 possui 4 números menores do que ele à sua direita, a saber, 7, 8, 9 e 6. Já o número 7, possui apenas 1 número menor que ele posicionado a sua direita, o número 6. Enfim, somando os números da linha suporte obteremos a medida I.

Análise dos movimentos no puzzle 14-15

São quatro os movimentos possíveis no puzzle 14-15. Podemos ir para a esquerda, para a direita, para cima ou para baixo. Como estes movimentos podem alterar a medida I? Vamos começar com o fácil, os movimentos na horizontal. Observe que quando caminhamos para a esquerda ou para a direita, realizaremos a inversão entre dois, e apenas dois vizinhos, de maneira que nossa medida I será acrescida ou diminuída de 1 unidade na nova configuração. Para facilitar, vamos dar um nome a este movimento simples. A partir de agora, quando trocamos de posição dois vizinhos estaremos fazendo uma Inversão.

Um pouco mais difícil é a análise do que ocorre com a medida I como reflexo dos movimentos verticais. Note que qualquer movimento vertical irá trocar de posição dois números que estão distante entre si em 4 unidades, em função da dimensão do tabuleiro. Assim, independente dos valores originais, um movimento vertical, seja para cima ou para baixo, deverá transformar uma configuração da forma

A	B	C	D	E	F	G	H	I	J	K	L	M	N	O	P
a	b	c	d	e	f	g	h	i	j	k	l	m	n	o	p
numa configuração, por exemplo, da forma

A	B	C	H	E	F	G	D	I	J	K	L	M	N	O	P
a	b	c	?	?	?	?	h	i	j	k	l	m	n	o	p
Cada letra minúscula é o valor suporte para a determinação da medida I. Note que quase todos eles permanecerão o mesmo depois do movimento vertical HD. Assim, o novo valor da medida I depende exclusivamente dos valores representados pelos pontos de interrogação.

Como não conhecemos os valores representados pelas letras maiúsculas, decisão que tomei para deixar o argumento genérico, fica difícil conhecermos estes novos valores. Porém, há um forma; podemos calcular quantas Inversões são necessárias para alcançarmos a segunda configuração a partir da primeira, lembrando que uma Inversão no sentido que discuto aqui é a troca de posição entre dois vizinhos. Acompanhe o desenvolvimento na tabela abaixo.

A	B	C	D	E	F	G	H	I	J	K	L	M	N	O	P
A	B	C	E	D	F	G	H	I	J	K	L	M	N	O	P
A	B	C	E	F	D	G	H	I	J	K	L	M	N	O	P
A	B	C	E	F	G	D	H	I	J	K	L	M	N	O	P
A	B	C	E	F	G	H	D	I	J	K	L	M	N	O	P
A	B	C	E	F	H	G	D	I	J	K	L	M	N	O	P
A	B	C	E	H	F	G	D	I	J	K	L	M	N	O	P
A	B	C	H	E	F	G	D	I	J	K	L	M	N	O	P
Foram necessárias 7 inversões para alcançarmos a segunda configuração. Como cada inversão acresce +1 ou -1 à medida I, um movimento vertical poderá acrescentar:

+1+1+1+1+1+1+1 = +7
+1+1+1+1+1+1-1 = +5
+1+1+1+1+1-1-1 = +3
+1+1+1+1-1-1-1 = +1
+1+1+1-1-1-1-1 = -1
+1+1-1-1-1-1-1 = -3
+1-1-1-1-1-1-1 = -5
-1-1-1-1-1-1-1 = -7

Paridade

Parece que pouco caminhamos para a resolução do problema, porém é apenas aparência, de fato já temos todos os elementos para provar que é impossível resolver o puzzle 14-15.
Sabemos que qualquer movimento horizontal irá alterar a medida I em +1 ou -1 e que qualquer movimento horizontal irá alterar a medida I em -7,-5,-3,-1,1,3,5 ou 7. Então, resumindo, podemos ter certeza de que qualquer movimento no puzzle irá alterar a medida I em um número ímpar, seja positivo ou negativo.

Ora, também sabemos que qualquer solução possível deverá conter um número par de movimentos. Como cada movimento é um número ímpar e par vezes ímpar é um número par, podemos concluir que qualquer solução possível irá alterar a medida I em um número par. Para ressaltar a importância deste resultado, irei emoldurá-lo abaixo:
Qualquer solução possível deverá alterar a medida I em um número par.

O golpe final

A resolução do puzzle 14-15 envolve a transformação da configuração 1-2-3-4-5-6-7-8-9-10-11-12-13-15-14-16 de medida I=1 na configuração 1-2-3-4-5-6-7-8-9-10-11-12-13-14-15-16 de medida I=0. Como qualquer solução possível altera a medida I em um número par, é impossível resolver o problema.

Então não ganharei dinheiro?

Não, você não ganhará dinheiro algum pois não é possível resolver o problema. Porém, para quem ficou frustrado tenho uma receita infalível para ganhar algum. Basta seguir o procedimento abaixo:

De algum jeito faça com que seus amigos tomem conhecimento da insolubilidade do puzzle 14-15. É muito importante que eles não saibam que você sabe que eles sabem disso.
Finja que você está se descabelando para resolver o puzzle que apresentarei logo abaixo. O puzzle é muito parecido com o 14-15.
Em algum momento eles irão comentar. "Seu burro, isso não tem solução".
Diga que tem sim uma solução e que logo você vai descobrir.
Ele, no alto de sua arrogância, dirá algo do tipo: "Não tem não, você é muito burro".
Ele está pronto! Agora é a sua deixa, aposte com ele que tem sim. Sugiro 10 ou 20 reais, talvez um almoço.
Se tudo der certo ele cairá como um patinho e aceitará a aposta.
Resolva o problema na frente dele e pegue o dinheiro.

Abaixo o puzzle "Resolva! Se puder". O objetivo é corrigir a grafia da frase invertendo as duas últimas letras. A primeira vista parece ser igual ao puzzle 14-15, porém por algum motivo, que desafio o leitor a descobrir, é possível resolvê-lo.


![[resolva.png]]

Bom almoço.