---
layout: post
title: Paradoxo dos Aniversários
date: 2013-04-24 10:00:00 +1000
categories: mathematics blog
mathjax: true
---

# Paradoxo dos Aniversários
  
Experimente perguntar a seus colegas de trabalho qual é a chance de que duas pessoas ao menos compartilhem o mesmo dia de aniversario entre as 23 pessoas de um jogo de futebol (11 de cada lado mais o juiz).

As respostas irão variar, é claro, mas entre não iniciados na arte matemática, elas gravitarão em torno de "baixa", "muito baixa" e "pequena".  Alguns terão a oportunidade de mostrar o desinteresse típico a assuntos quantitativos dando de ombros enquanto outros sorrateiramente caminharão para o cafezinho disfarçando certa fobia que carregam desde os tempos de escola.

Porém alguns estarão lá, abertos a sua pergunta, ansiosos por declarar sua opinião, esses poderão ser salvos. Para estes, mantenha a tez serena, a voz baixa porém firme, e no tom mais arrogante que conseguir professe casualmente: "Bom, as chances são maiores do que sair cara no cara ou coroa". 

Nesse momento você ainda perderá mais algumas almas. Os motivos são diversos e desconhecidos em sua totalidade, variam desde o total não entendimento do problema até a aversão ao convite para uma digressão quantitativa. Espere neste ponto ouvir frases como "Não me interesso muito por futebol", "Sempre fui mal em matemática" ou "Viu o jogo ontem?"

Por outro lado se ouvir frases como "Impossível!", "Você esta errado" ou "Claro que não, as chances são 1/365" tenha certeza que está lidando com um público de maior sofisticação quantitativa. Neste caso é sua hora de brilhar, terá enfim a oportunidade de explicar porque as chances são tal altas assim, maiores do que 50%.

O que confunde as pessoas é a tendência de imaginar este problema sob o ponto de vista pessoal, isto é, as pessoas imaginam que não é fácil encontrar alguém com a mesma data de aniversario delas próprias, portanto a ocorrência deste fenômeno deve ser bastante baixa. 

Porém, esta não é a perspectiva correta, lembre-se que o problema não é sobre as chances de encontrar alguém com o mesmo aniversário do que você num grupo de 23 pessoas, o problema é sobre encontrar colisões de aniversários entre todas as duplas possíveis de se formar com 23 pessoas. 

Enfim, num grupo de 23 existem 253 duplas (combinação 23, 2 a 2). Para que não ocorram conflitos de aniversario, nenhuma dupla devera compartilhar as mesmas datas. A probabilidade de que uma dupla não compartilhe aniversários é alta, exatamente igual a 364/365.  
  
Para ver isso, note que as chances de jogarmos 2 dados e não obtermos dois números iguais é 5/6. Pode parecer trivial para alguns, mas confiem em mim, muitos irão desistir da leitura nesse ponto (como meu irmão por exemplo). Novamente, independente do resultado do primeiro dado, o segundo não poderá ser igual, então as chances são 5/6. Analogamente as chances de que uma dupla não compartilhe aniversário é 364/365. (ignoremos anos bissextos por favor)  
  
Portanto, as chances de que não hajam compartilhamento de aniversários em nenhuma das 253 duplas é igual a:

364/365 x 364/365 x 364/365 x … x 364/365 (253 vezes)

isto é igual a (364/365)^253

Inversamente, as chances de que haja ao menos uma ocorrência de compartilhamento de aniversario é exatamente 1-(364/365)^253, o que resulta em algo um pouco maior do que 50%

Em teoria, estas chances são ainda maiores do que encontrar duas pessoas com o mesmo primeiro nome, afinal o tamanho do conjunto de nomes disponíveis é bem maior do que 365 ocasionando em menos colisões de nomes em potencial. (o que não é bem verdade, pois os nomes da moda são escolhidos com muito maior frequência do que nomes mais raros) 

Para terminar sua exposição, inquira a audiência (se é que ainda sobrou alguém) para saber se há alguma colisão de aniversários insuspeitos até o momento. Se tiver essa sorte passará a ser respeitado como um novo guru do escritório. Apesar de não provar nada, esse simples fato, ao invés das contas anteriores, parece dar certeza as pessoas de que você estava de fato certo afinal.

Como desafio final a seus colegas pergunte quais são as chances de encontrar, no mesmo grupo, duas pessoas que compartilhem o mesmo mês de aniversário. Sua audiência, agora já treinada, irá responder com segurança que as chances são altas ou bem altas, afinal a chance de colisão é muito mais alta agora. Os mais matematicamente inclinados irão até rabiscar 1-(11/12)ˆ66, porém eles estarão novamente enganados! As chances são 100%, ou seja não há como não haver colisões de meses de aniversário entre um grupo maior do que 12 pessoas. Deixo ao leitor a tentativa de encontrar uma explicação para este fato.