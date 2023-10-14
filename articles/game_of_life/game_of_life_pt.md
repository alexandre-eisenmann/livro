---
layout: post
title: O Jogo da Vida
date: 2007-05-26 10:00:00 +1000
categories: mathematics blog
mathjax: true
---

# O Jogo da Vida

Gostaria de apresentar o viciante e pouco conhecido "Jogo da Vida". Empresários, cuidado! O Jogo da Vida pode parar um departamento inteiro durante toda a tarde de forma mais eficiente do que o Orkut. Sob sua aparência ingênua e trivial se esconde um voraz devorador de cérebros.  
  
Deixando a brincadeira de lado, o Jogo da Vida (_Game of Life_) foi inventado pelo matemático inglês e professor da Universidade de Princeton John Horton Conway em 1970 e desde lá tem despertado nossa curiosidade e imaginação. Ele não é propriamente um jogo no sentido clássico, não há objetivo, não há jogadores, vencedores ou perdedores. Definida uma posição inicial para as peças do jogo (células) , regras simples determinarão os acontecimentos que estão por vir. O Jogo da Vida é surpreendente em muitos aspectos, com várias facetas e desdobramentos, um ambiente muito rico para novas descobertas.  
  
O Jogo da Vida é composto de um grande tabuleiro infinito, inteiramente quadriculado onde cada um dos quadradinhos representa uma célula que poderá estar _viva_ ou _morta._ Inicialmente todas as células estarão mortas, no ponto em que nós, em nossas raras intervenções (na verdade a única), iremos definitivamente criar vida e compor o que chamamos de padrão inicial (ou configuração inicial). A seguir, comandamos uma espécie de _Big Bang_, isto é, damos início ao jogo e observamos seu comportamento. Conway definiu cuidadosamente 3 simples regras que irão reger o comportamento do jogo, uma regra para os nascimentos, outra para a morte e outra para a sobrevivência:  
  

- Regra para _nascimento_: Toda célula morta se tornará viva quando exatamente 3 de suas 8 células vizinhas estiverem vivas.
- Regra para _sobrevivência_: Toda célula viva que possui 2 ou 3 células vizinhas vivas, continuará viva.
- Regra para _morte_: Em todos os outros casos, uma célula morrerá (ou permanecerá morta), ou por solidão (1 ou menos vizinhos vivos) ou por lotação (4 ou mais vizinhos vivos).

  
Apesar de simples, estas regras costuma gerar alguma confusão. As pessoas normalmente perguntam: "Mas o que devo fazer primeiro? Eliminar as células mortas ou incluir as que irão nascer?". A resposta é nenhum nem outro! As duas operações deverão ser feitas ao mesmo tempo. Dito de outra maneira, é irrelevante a ordem em que as operações são feitas, o resultado é sempre o mesmo. Um dica é marcar as que vão nascer e as que irão morrem sem alterar o estado do jogo, depois disso pode-se de fato criar as células maracadas para nascer e apagar aquelas marcadas para morrer. Certifique-se que você compreendeu esta sutilieza acompanhando o exemplo abaixo.  
  
Suponha a execução do Jogo da Vida a partir de um padrão inicial composto de 5 células vivas enfileiradas. Esse tipo de padrão é conhecido como pentaminó, isto é, um padrão formado por cinco quadradinhos onde cada uma delas compartilha no mínimo uma face com qualquer um dos outros. O pentaminó é, enfim, uma generalização do dominó, porém com cinco quadradinhos ao invés de dois.  
  
Quando submetemos este padrão às regras, ele se transformará no oitavo desenho sete passos após o Big Bang. Depois disso, surpreendentemente, o nono padrão será exatamente igual ao sétimo que por sua vez gera novamente o oitavo, resultando finalmente num padrão oscilante depois de 7 gerações


![[jogovida-1.png]]![[jogovida-2.png]]![[jogovida-3.png]]![[jogovida-4.png]]![[jogovida-5.png]]![[jogovida-6.png]]![[jogovida-7.png]]

  
Nem sempre o padrão inicial resulta em um padrão oscilante. Em muitos casos a população inicial caminha para sua total extinção, onde depois de algum tempo todas as células estão novamente mortas. É o que ocorre com este outro pentaminó, extinto em apenas 3 passos (ou gerações).  

  ![[jogovida-8.png]]
  
Ao conceber seu jogo, Conway testou todos os 12 pentaminós existentes e logo percebeu que ou eles se tornavam oscilantes, ou eram extintos. Havia, porém uma única exceção, um dos pentaminós (abaixo) se recusava a estabilizar depois de um número significativo de passos. Lembrem-se vocês leitores que Conway testou estes padrões em um tabuleiro ou em um papel milimetrado, afinal eram os anos 70 e os computadores não eram assim tão disponíveis, mesmo para acadêmicos de porte.  
  
![[jogovida-9.png]]
  
Felizmente, preparei uma surpresa para vocês, aqui mesmo neste blog. Basta rolar a página até o final que vocês verão um simulador do Jogo da Vida que desenvolvi para testarmos quantos padrões desejarmos. Ele foi desenvolvido em Java e só irá funcionar se o plug-in do Java estiver devidamente instalado no browser de vocês, se não for esse o caso basta entrar no site [http://www.java.com/pt_BR/](http://www.java.com/pt_BR/) e clicar numa seta amarela enorme que aparece logo de cara que a atualização será efetuada. É de graça!.  
  
Para criar vida, basta clicar em qualquer quadradinho que eles viverão, tornando-se pretos. Um novo clique, e eles morrerão novamente. Uma vez definida a posição desejada, basta clicar no botão ON em cima à esquerda. Se desejarem pausar a simulação cliquem novamente neste botão que agora tem o nome de OFF.  
  
Vocês logo perceberão que um intuitivo seletor de velocidade fica à direita deste botão e pode ser usado à vontade. As duas informações que ficam em cima e à direita são respectivamente, o número de células vivas e a quantidade de gerações (passos) realizados. Finalmente, na parte inferior há uma versão do mesmo universo, porém reduzido de maneira que possamos visualizar a ação de uma perspectiva mais ampla. É possível arrastar o retângulo vermelho posicionado no centro desta região para selecionar áreas distantes deste mesmo universo. Experimente!  
  
Bom, por hora não vou estragar a surpresa de vocês. Há ainda muito o que dizer mas vou deixar vocês se divertirem um pouco...