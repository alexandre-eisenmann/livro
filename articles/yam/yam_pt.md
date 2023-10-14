---
layout: post
title: Yam!
date: 2007-12-08 10:00:00 +1000
categories: mathematics blog
mathjax: true
---

# Yam!

  ![[yam.jpg]]

Atendendo a pedidos finalmente desenvolvi e disponibilizei online o jogo Yam. Para jogar basta se cadastrar e jogar. É de graça! [Clique aqui para Jogar!](https://www.blogger.com/blog/post/edit/5314484891711013222/7618142785794722593# "Clique aqui para Jogar!")  
  
A versão que implementei é aquela comercializada pela Grow que muitos de vocês deverão conhecer. O Yam da Grow utiliza cartelas, lápis e dados reais, além disso pode ser jogado em grupos de pessoas, cada uma preenchendo sua própria cartela. A versão que desenvolvi deve ser jogada individualmente na Web, porém, em contrapardida, estabeleci um sofisticado sistema de ranking para enriquecer a experiência de quem joga.  

O Yam é um jogo de dados, cinco precisamente. Alguns consideram o Yam uma espécie de pôquer de dados, provavelmente motivados pelo fato de que no Yam o jogador poderá obter uma Quadra, Um Full-House ou Seguidas, resultados idênticos aos do pôquer. Porém, o Yam não envolve apostas, nem são comparados jogos entre os jogadores. Para jogar bem o Yam e conseguir um boa pontuação é necessário sorte, raciocínio lógico e uma boa dose de estratégia. Jogadores iniciantes dificilmente conseguirão bons scores mesmo com um bom grau de sorte.  
  
**Objetivo  
**O objetivo do Yam é preencher todas as células da tabela e obter o maior número possível de pontos.  
  
**Jogada**  
  
Uma jogada equivale ao resultado obtido após 3 ou menos lançamentos dos dados seguido do preenchimento de uma célula na tabela. No primeiro lançamento o jogador irá lançar necessariamente os 5 dados. Se o resultado agradar, ele para por aí, preenche uma célula da tabela e a jogada está concluída. Se quiser melhorar o resultado ele separa os dados que não quer mexer (clicando neles) e lança os demais. Novamente, se após o segundo lançamento o resultado ainda não tiver do seu agrado, ele tem sua terceira e última chance.  
  
Tipicamente o jogador irá jogar 3 vezes os dados antes de preencher uma célula, afinal não é fácil obter um bom resultado, tanto que uma jogada de apenas um lançamento recebe um nome e tratamento especial, dizemos que a jogada foi no SECO.  
  
**Tabela**  
  
A tabela é composta por quatro colunas, Descida, Subida, Desordem e Seco, cada coluna possui 13 células a ser preenchidas pelo jogador (em verde claro na tabela abaixo) e 3 células de totais que serão preenchidas automaticamente pelo jogo (verde escuro). As colunas se diferenciam pela forma como devem ser preenchidas, a coluna Descida deve ser preencida de cima para baixo, a coluna Subida, de baixo para cima. A coluna Desordem, como o próprio nome diz, pode ser preenchida em qualquer ordem.  
  
Finalmente, a coluna Seco, só poderá ser preencida após o primeiro lançamento dos dados, ou seja, o jogador deverá ter obtido o resultado desejado no primeiro lançamento. Se o jogador lançar os dados uma segunda vez, a coluna inteira será desabilitada.  
  
**Jogos  
**Em cada linha da tabela um certo tipo de jogo deverá ser obtido pelo jogador. Se for bem sucedido, o jogador irá ganhar o bônus correspondente ao jogo em questão. Por exemplo, se o jogador obter uma Quadra (quatro dados iguais) na linha Q, deverá marcar a soma dos pontos da quadra mais um bônus de 20 pontos. Isso vale para qualquer uma das quatro colunas. Abaixo, a lista de todos os jogos previstos no Yam:  
  

|   |   |   |   |
|---|---|---|---|
|1|Um|Obter a maior quantidade possível de números 1|Somar os pontos dos dados com número 1|
|2|Dois|Obter a maior quantidade possível de números 2|Somar os pontos dos dados com número 2|
|3|Três|Obter a maior quantidade possível de números 3|Somar os pontos dos dados com número 3|
|4|Quatro|Obter a maior quantidade possível de números 4|Somar os pontos dos dados com número 4|
|5|Cinco|Obter a maior quantidade possível de números 5|Somar os pontos dos dados com número 5|
|6|Seis|Obter a maior quantidade possível de números 6|Somar os pontos dos dados com número 6|
|T|SubTotal||Somar os pontos anteriores. Se o valor for maior ou igual a 60, acrescentar um bônus de 30 pontos.|
|Q|Quadra|Obter 4 dados iguais|Se obtido, somar os pontos dos dados iguais e acrescentar um bônus de 20 pontos, caso contrário marcar 0|
|F|Full|Obter uma trinca e uma dupla|Se obtido, somar os pontos de todos os dados e acrescentar um bônus de 30 pontos, caso contrário marcar 0|
|S-|Seguida Mínima|Obter 1, 2, 3, 4, 5|Se obtido, somar os pontos de todos os dados e acrescentar um bônus de 35 pontos, caso contrário marcar 0|
|S+|Seguida Máxima|Obter 2, 3, 4, 5, 6|Se obtido, somar os pontos de todos os dados e acrescentar um bônus de 40 pontos, caso contrário marcar 0|
|-|Mínimo|Somar os pontos dos dados. O resultado deve ser menor do que a célula abaixo (Mínimo).|Somar os pontos de todos os dados. Considerar 0 se o valor for maior do que a coluna abaixo|
|+|Máximo|Somar os pontos dos dados. O resultado deve ser maior do que a célula acima (Mínimo).|Somar os pontos de todos os dados. Considerar 0 se o valor for menor do que a coluna acima|
|Y|Yam|Obter 5 dados iguais|Se obtido, somar os pontos de todos os dados e acrescentar um bônus de 50 pontos, caso contrário marcar 0|
|T|Total||Somar as linhas Q,F,S-S+,-,+,Y|
|TG|Total Geral||Somar SubTotal com Total|

  
**Ranking**  
  
Criei um sistema de ranking que privilegia o jogador regular, estrategista, insensível a golpes de sorte. Existe o ranking do dia, o ranking da semana, os melhores resultados e o ranking geral. Para calcular o ranking geral devemos considerar o seguinte critério de pontos:  
  
1º colocado na semana: 8 pontos  
2º colocado na semana: 5 pontos  
3º colocado na semana: 3 pontos  
1º colocado no dia: 1 ponto  
  
Dependendo do número de semanas que você foi primeiro, segundo ou terceiro colocado terá seu score geral acrescido de 8, 5 ou 3 pontos respectivamente. Se você campeão de apenas 1 dia ganhará 1 ponto. Para os propósitos do jogo o primeiro dia da semana é domingo, portanto no próximo domingo o ranking da semana estará vazio, aproveitem! O ranking de melhores resultados não é utilizado para o ranking geral. Esta decisão foi tomada na intenção de diminuir o componente sorte do ranking geral.  
  
**O que é um bom resultado?**  
  
Adianto que um resultado superior a 1000 já é considerado bom. Se você conseguir mais do que 1100 já pode pensar em ser campeão do dia. Se conseguir mais do que 1200 tem muita chance de ser o campeão da semana. Se ultrapassar os 1300, bom já estamos lidando com profissionais. Só vi um resultado maior do que 1400 e me pergunto porque o fulano não jogou na megasena. Mais que 1500? Nunca vi!