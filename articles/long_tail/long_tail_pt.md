---
layout: post
title: The Long Tail
date: 2007-05-18 10:00:00 +1000
categories: mathematics blog
mathjax: true
---

# The Long Tail

Não resisti, forças misteriosas forçaram-me a investigar um pouquinho mais a natureza do número 9376, este número estranho de caráter auto-reprodutivo que quando multiplica-mo-lo (gostaram da mesóclise? Corrijam-me se a usei errado) por ele mesmo resulta em um novo número com o mesmo "código genético".

Encarei ele de frente e algo novo surgiu. Qualquer "cauda" do número 9376 também é auto-reprodutiva! Ok, vocês não endenderam nada, afinal o que é a "cauda" de um número? Bom, foi o nome que encontrei para designar o número encontrado em qualquer trecho à direita do número original. Assim, 9376 tem 4 caudas, o número 6, o número 76, o número 376 e ele próprio, o número 9376. Fazendo as contas, logo vi que as 4 caudas de 9376 também são auto-reprodutivas:

9376 x 9376	=	87909376
376 x 376	=	141376
76 x 76	=	5776
6 x 6	=	36
Pensei um longo tempo neste assunto e percebi que este fato é necessário para que o número seja auto-reprodutivo, ou seja: todas as caudas de um número auto-reprodutivo deverão ser necessariamente números auto-reprodutivos. É simples demonstrar este resultado e sugiro que vocês tentem, não envolve nada além do que vocês aprenderam até a sétima série. Para aqueles de menor magnetismo pessoal aconselho apresentar este resultado num sábado a noite qualquer. Vocês verão o sucesso que irão fazer ! É melhor do que carro importado.

Neste ponto, um sentimento megalomaníaco apareceu em meu peito. Será que eu não poderia construir números auto-reprodutivos maiores, com digamos mil dígitos, ou dez mil, talvez 1 milhão? Lá fui eu para o caderno de alemão de minha esposa rabiscar e rabiscar durante horas. Depois de uma eternidade finalmente eu desisti frustrado. O que eu estava procurando era uma regra para encontrar um número reprodutivo a partir de uma de suas caudas. Por exemplo, gostaria de, a partir de, digamos 76, encontrar 376 ou 9376. É claro, esta regra deveria ser suficientemente poderosa para eu encontrar números reprodutivos maiores do que 9376.

Como não podia deixar de ser sofri uma reprimenda da minha esposa. Onde já se viu, disse ela, estragar todo o meu caderno com esses rabiscos? (sim, ela os chamou de rabiscos toda a minha arte). Abalado e com um caderno novinho e sem pautas que ganhei dela, resolvi apelar, fazer uso de um arsenal matemático bem além da sétima série. Com caderno novo, técnica nova e esposa trabalhando fora, pude me deliciar com o melhor que a internet pode oferecer... é claro, dicas sobre a aritmética modular.

Esse relato tinha tudo para acabar aqui, mas contrariando todas as probabilidades eu encontrei a tal regra que gera números auto-reprodutivo cada vez maiores. Ela é simples e bela, quase uma pintura. Aprecie:

3n2-2n3 (mod 102d(n))

onde n é um número auto-reprodutivo e d(n) é o número de dígitos deste número. O resultado da expressão acima é um novo número auto-reprodutivo com o dobro de dígitos do anterior. Calma, não é motivo para pânico, posso reescrever a fórmula acima sem usar a palavra "mod". De fato, a expressão é equivalente a:

Resto da divisão de 3n2-2n3 por 102d(n)

Além de produzir um número auto-reprodutivo maior do que o número utilizado (que chamarei de "semente") a demonstração da fórmula acima trouxe uma informação muito mais sutil e importante. Existem infinitos números auto-reprodutivos, afinal, sempre será possível construir um maior a partir da "semente" anterior.

Para os que tentarem fazer as contas com uma calculadora simples tenho dois avisos: primeiro, vocês não irão muito longe pois como o tamanho dos números dobra a cada iteração, logo o limite de suas calculadoras irá estourar; segundo, é necessário saber como calcular "restos de divisão" quando o dividendo é negativo. No meu caso, preferi não perder muito tempo e lancei mão de recursos computacionais mais poderosos. Enfim, a partir do número 6 como "semente", obtive a uma boa sequência de números auto-reprodutivos, cada um com tamanho duas vezes maior do que o anterior.

6
76
9376
87109376
3740081787109376
95893380022607743740081787109376

Observe o poder do algoritmo, com apenas 5 iterações obtive, não 5 como pode parecer a primeira vista, mas 32 números auto-reprodutivos. Basta pegar o maior deles e listar todas as suas caudas. E para isso foi necessário partir de uma semente minúscula que é o número 6, que é claro, é um número auto-reprodutivo.

6
76
376
9376
09376
109376
7109376
87109376
787109376
1787109376
81787109376
etc...

A pergunta seguinte surgiu naturalmente, como deverá ter ocorrido para alguns de vocês (ou você... se apenas uma pessoa ler isso aqui. Oi mãe!) caros leitores. Não existe outra semente pequena diferente de 6? Uma coisa é claro, se outra semente existe, ela deverá ter apenas 1 dígito, pois o fato de ter mais do que 1 dígito implica que sua cauda de tamanho 1 também seja auto-reprodutiva. Bom, agora ficou fácil, basta testar todos os números de 1 dígito e... Voilà !!! o número 5 também é auto-reprodutivo, afinal 5 x 5 = 25. Quantos aos outros números, nenhum deles é auto-reprodutivo.

A fórmula é bem poderosa, e funciona com qualquer semente, então foi simples calcular toda um nova família de números auto-reprodutivos a partir da semente 5.

5
25
625
0625
90625
890625
2890625
12890625
212890625
8212890625
18212890625
918212890625
etc...

Incansável e motivado pela últimas realizações, fui atrás de novas regularidades e resolvi somar os números das duas famílias usando a expressão R5(d) + R6(d), onde R5(d) representa o maior número auto-reprodutivo de cauda 5 que possui d ou menos dígitos, analogamente R6(d) é o maior número auto-reprodutivo de cauda 6 que possui d ou menos dígitos. Bom, realizei a soma e obtive a tabela abaixo:


n	R5(n)	R6(n)	R5(n)+R6(d)
1	 5	6	11
2	 25	76	101
3   625	376	1001
4	 625	9376	10001
5	 90625	9376	100001
6	 890625	109376	1000001
7   2890625	7109376	10000001
8	 12890625	87109376	100000001
9   212890625	787109376	1000000001
10  8212890625	1787109376	10000000001
11	  18212890625	81787109376	100000000001
12  918212890625	81787109376	1000000000001
13	9918212890625	81787109376	10000000000001
14	59918212890625	40081787109376	100000000000001
15	259918212890625	740081787109376	1000000000000001
16	6259918212890625	3740081787109376	10000000000000001
17	56259918212890625	43740081787109376	100000000000000001
18	256259918212890625	743740081787109376	1000000000000000001
19	2256259918212890625	7743740081787109376	10000000000000000001


Incrível, não é mesmo? A soma entre os números reprodutivos das famílias de cauda 5 e de cauda 6 resultam sempre em um mesmo padrão, independentemente do tamanho do número, ou da cauda se preferir. A expressão que ilustra esse resultado é:

R5(d) + R6(d) = 10d + 1

Gostei muito desta conjectura e ainda me espanto com ela, dois números de famílias diferentes de números auto-reprodutivos quando somados resultam em uma família de números capicuas. Para quem não sabe, números capicuas são aqueles que lido da direita para esquerda ou da esquerda para a direita resultam sempre no mesmo número. Para os mais letrados, capicua é o equivalente numérico dos palíndromos.

Após tantas regularidades e da existência de uma família infinita de números auto-reprodutivos, desconfiei que alguém já tenha trabalhado com isso e mais uma vez recorri ao Oráculo. "Oh Oráculo. Existe alguém que descobriu os números auto-reprodutivos antes de mim?". Aguardei um pouco e obtive: "Sim, caro mortal, muitas pessoas trabalharam com isso e já haviam percebido isso há muito tempo, porém deram outro nome, chamaram de números automórficos". Bom, um pouco decepcionado, confesso, voltei a minha insignificância e escrevi este pequeno artigo.

Um último comentário é de que não encontrei no Oráculo qualquer referência à conjectura acima. Isso significa que é possível que ainda não tenha sido batizada por ninguém. Como prêmio para quem leu até aqui (viu mãe) prometo batizar a conjectura acima com o nome da pessoa que a demonstrá-la e mandar um post com a demonstração. Lembro que uma conjectura ainda não demonstrada pode se mostrar falsa para algum valor de n maior, portanto uma demonstração se faz necessária. Se a conjectura é demonstrada, ela não é mais uma conjectura e sim um Teorema.
