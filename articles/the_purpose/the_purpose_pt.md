---
layout: post
title: Uma Proposta para o Ensino de Combinatória
date: 2007-09-22 10:00:00 +1000
categories: mathematics blog
mathjax: true
---

# Uma Proposta para o Ensino de Combinatória


Combinatória é um assunto difícil, acho que todos concordamos com isso. Num curso típico sobre o assunto, logo na primeira ou segunda aula, conceitos sofisticados como combinação, arranjo, permutação são esparramados no quadro negro. Em breve virá a combinação com repetição e probabilidades e a coisa toda piora.

O aluno típico, frente a esta coleção de nomes e fórmulas procura desesperadamente respostas para suas angústias e invariavelmente ouvimos: "... mas neste exercícios, usamos combinação ou arranjo?"

Ensinar combinatória é igualmente frustrante, uma vez que não há uma sistemática a seguir e muitas vezes os professores são obrigados a tentar expressar sua própria intuição em palavras. Além disso a dificuldade de ensinar assunto tão simples agrava a sensação de frustração.

## Princípio da Equiparação

Inspirado na forma como nossos antepassados realizavam contagem sem a utilização de números, vou propor uma nova abordagem para resolvermos exercícios de combinatória. Não é claro que ajudará todos os professores ou alunos mas é uma forma diferente que pode, acredito, ser bastante útil.

O grande segredo de nossos antepassados para contar, por exemplo, ovelhas de um rebanho é o chamado princípio da equiparação. Para cada ovelha do rebanho fazemos um talho num pedaço de pau. Assim, a quantidade de talhos na madeira é equivalente a quantidade de ovelhas. Se, no dia seguinte, houverem mais talhos do que ovelha é provável que algumas tenham sido roubadas ou mortas.

Se ao invés de talhos na madeira, utilizássemos pedras em um saco, não faria diferença nenhuma e o princípio da equiparação estaria sendo utilizado da mesma maneira. De fato muitas outras maneiras são possíveis e, se pensarmos um pouco, a escala numérica é apenas um substituto abstrato para o conjunto de talhos ou pedras em um saco.

Desta forma, contar uma coleção de elementos equivale a encontrar um conjunto de mesmo tamanho. Se este tamanho já é conhecido, não é necessário contar os elementos da coleção para conhecermos a resposta desejada. Por exemplo, apresento para vocês um auditório e informo que há 150 poltronas, na sequência pergunto: quantas pessoas sentadas poderemos acomodar? A resposta é óbvia; 150 pessoas.

## Um Problema

O princípio da equiparação é uma ferramenta poderosa de contagem e procurarei ilustrar esta idéia através de um exercício bastante conhecido:

Suponha uma grade com 5 de largura e 3 de altura. Você está localizado no canto inferior esquerdo e deseja alcançar o canto superior direito. Só é possível a locomoção para a direita ou para cima. Quantos caminhos existem?

Certifique-se de que entendeu o problema. Desenhe a grade e trace alguns caminhos possíveis. Afinal, quantos existem? Se quiser pensar um pouco no problema interrompa a leitura neste ponto e volte mais tarde.

Adiantando já para a resolução, é possível perceber que cada caminho envolve 5 passos para a direita e 3 passos para cima. Se representarmos um passo para a direita pela letra D e um passo para cima pela letra C, todos os caminhos procurados podem ser representados por uma palavra de 5 letras D e 3 letras C's. Por exemplo, a palavra DCDDCCDD representa um dos caminhos enquanto CCCDDDDD representa outro.

Se pudermos concluir que a quantidade de palavras com 5 D's e 3 C's é exatamente igual a quantidade de caminhos que pretendemos contar, podemos contar as palavras ao invés dos caminhos e resolver o problema. Esta é a essência do princípio da equiparação.

## Anagramas

Um anagrama é uma palavra formada a partir da reorganização das letras de outra palavra. Assim ROMA é um anagrama de AMOR. Palavra, no contexto que estou usando, não precisa ter nenhum significado, assim, a palavra MRAO também é um anagrama de AMOR.

A quantidade de anagramas de determinada palavra é assunto bastante estudado no ensino médio e não tratarei do assunto aqui. Digamos que no momento, calcular esta quantidade é um processo simples e de fácil entendimento.

Um pouco mais complicado é calcular a quantidade de anagramas de palavras com caracteres repetidos com por exemplo a palavra PASSEIO ou a palavra AUTOMATICO, mas novamente, há uma forma simples e sistemática de realizar esta contagem.

Se temos uma ferramenta para contar a quantidade de anagramas, por que não usá-la para resolver o problema proposto anteriormente, afinal a resposta do problema é a quantidade de anagramas que a palavra CCCDDDDD possui. Todos concordam?

Enfim, tínhamos um problema bem definido, conseguimos mapeá-lo para outro contexto, no caso o contexto dos anagramas que possuímos procedimentos fáceis de cálculo. Assim, usando o princípio da equiparação, contamos a quantidade de anagramas possíveis e automaticamente resolvemos o problema.

## Um outro problema

Pensar em anagramas é uma boa maneira de resolver problemas de contagem em geral. Não estou querendo dizer que podemos sempre mapear um problema para um conjunto de anagramas, mas sim que sempre que pudermos a solução é imediata.

Um outro exemplo cuja solução por anagramas é simples é o seguinte:

Em um grupo de 9 pessoas conhecidas gostaríamos de eleger 2 presidentes, 3 diretores e 4 gerentes. De quantas maneiras podemos realizar a divisão?

Mais uma vez é possível modelar este problema usando a idéia de anagramas. Numere as pessoas de 1 a 10 e escreva na sequencia. Imediatamente abaixo destes números enfilere 9 letras, 2 P's para presidentes, 3 D's para diretores e 4 G's para gerentes.

123456789
PPDDDGGGG

Suponha que esta representação indica que as pessoas 1 e 2 são presidentes, as pessoas 3, 4, 5 são diretores enquanto as pessoas restantes são gerentes. É claro, muitas outras formações são possíveis, cada uma delas representada por um diferente anagrama da palavra PPDDDGGGG.

123456789
PPDDDGGGG
PDPGGGDGP
DGGGDPPDG
etc...

Assim o número procurado é exatamente igual ao número de anagramas da palavra PPDDDGGGG.

## Generalização

Anagramas são ferramentas poderosas e na verdade generalizam os conceitos conhecidos de combinação, arranjo e permutação. Com isso quero dizer que toda combinação pode ser representada por um anagrama assim como todo arranjo e toda a permutação.

Por exemplo toda a combinação C(n,p) pode ser representada como a quantidade de anagramas de p X's e n-p Y's. Por exemplo C(7,3) é igual a quantidade de anagramas da palavra XXXYYYY.

Um arranjo A(n,p) pode ser representado pela busca de todos os anagramas de uma palavra com n-p letras distintas e n-p letras iguais. Assim A(7,3) é equivalente a quantidade de anagramas da palavra ABCXXXX.

Uma permutação de n elementos P(n) é sempre igual a quantidade de anagramas de uma palavra com n letras distintas. Exemplificando P(4) é equivalente a quantidade de anagramas da palavra AMOR.

## Conclusão

O princípio da equiparação é muito útil para resolver um sem número de problemas. Suponho que aulas de combinatória focadas neste tipo de raciocínio caminharão no sentido do fortalecimento de conceitos ao invés de memorização de fórmulas. Os anagramas são apenas um exemplo de conjunto que podemos utilizar na aplicação do princípio da equiparação. Eles naturalmente não esgotam o assunto mas é uma nova ferramenta na tentativa de despertar a intuição de alunos e professores.








