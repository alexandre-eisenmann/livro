---
layout: post
title: O Problema da Rota Colorida
date: 2008-02-16 10:00:00 +1000
categories: mathematics blog
mathjax: true
---

# O Problema da Rota Colorida
  
A cidade de Manaus possui cerca de 2 milhões de habitantes. Apesar de não ser tão grande como São Paulo ou Rio de Janeiro, localizar um endereço em Manaus é uma das tarefas mais frustrantes que o motorista será obrigado a enfrentar. Em geral as ruas não possuem nomes (apenas apelidos) ou quando possuem não há placas informando.  
  
Quando tudo parece bem, a rua possui nome e placa, certamente a numeração das casas estará totalmente desordenada. Depois das casas, digamos, 35 e 44 podemos encontrar a casa 7 seguida da 35 (novamente) ou podemos encontrar as casas 1322 seguido das casas 511 e 688. Ímpares e pares compartilham o mesmo lado da rua sem o menor pudor.  
  
Quando você compra um eletrodoméstico numa loja de departamentos, o funcionário, além de perguntar o endereço, exige uma referência. Na verdade, o campo referência é obrigatório no seu sistema e sem isso a compra quase não pode ser feita.  
  
Dirigir na cidade de São Paulo não é muito melhor. É certo que as ruas possuem nomes e placas e a numeração é ordenada e coerente mas a malha viária é tão complexa que fica difícil para o motorista entender.  
  
Realizar retornos, corrigir rotas erradas, memorizar um trajeto são todas tarefas difíceis para o não taxista. Para piorar, você nunca está sozinho, para qualquer lugar que você vá, você terá companhia, e muita. Como todos sabemos, o trânsito em São Paulo é realmente infernal!  
  
Dependendo de como a malha viária de uma cidade for organizada e construída, a vida dos motoristas e pedestres pode ficar muito mais fácil. Quem conhece Manhatam, por exemplo, sabe como é fácil se localizar e encontrar um endereço. Lá, as próprias ruas são numeradas de maneira que, se estamos na quinta avenida e deserjarmos ir para a sétima sabemos de antemão que precisamos caminhar 2 quadras em determinado sentido.  
  
A topologia da malha viária é também bastante simples, aproximando-se de um grande quadriculado com ruas no sentido norte-sul e outras no sentido leste-oeste. Fácil não?  
  
Podemos fazer melhor? Será que é possível projetarmos uma cidade com um sistema de localização diferente, que facilite ainda mais a vida das pessoas? Que seja simples e fácil de se orientar?  
  
Incrivelmente o matemático israelense Avharam Trakhman resolveu o [Problema da Rota Colorida](https://www.blogger.com/blog/post/edit/5314484891711013222/8551492903365106386# "Problema da Rota Colorida") e esse fato nos dá certeza de que é sempre possível projetar uma cidade com endereço absoluto. Mas o que é endereço absoluto afinal? Bom, estou chamando de endereço absoluto um endereço que cumpre duas funções:  
  

- O endereço por si só pode ser utilizado para se encontrar o local não sendo necessário recorrermos a guias ou ao GPS.

- A rota sugerida pelo endereço absoluto funciona se partirmos de **qualquer** ponto da cidade. Ressalto a palavra qualquer e acrescento: O endereço absoluto é independente do ponto de partida.

  
Para exemplificar a idéia do endereço absoluto vou recorrer a um exemplo. Suponha uma mini-cidade com a malha viária representada na figura abaixo. As linhas azuis e vermelhas são as ruas, a direção permitida é representada pelas setas e os pequenos círculos são cruzamentos. O endereço do cruzamento amarelo é AVVAVVAVV enquanto o endereço do cruzamento verde é AAVAAVAAV.  
  
Cada letra do endereço representa qual rua devemos seguir, a rua (A)zul ou a rua (V)ermelha. O incrível é que a rota AVVAVVAVV levar-nos-á ao cruzamento amarelo a partir de qualquer, isso mesmo, qualquer ponto do mapa. A rota AAVAAVAAV, analogamente, levará o motorista ao cruzamento verde independente do ponto de partida. Verifique!

![[rotacolorida.png]]


Imagem retirada da wikipedia para explicação do [Problema da Rota Colorida](https://www.blogger.com/blog/post/edit/5314484891711013222/8551492903365106386# "Problema da Rota Colorida")

  
Trakhman não estava de fato preocupado com urbanismo ou melhoria do sistema de orientação das cidades. O "Problema da Rota Colorida" está relacionado a teoria dos Grafos, entidades matemáticas abstratas representadas por desenhos como a figura acima. Também não é qualquer grafo (neste contexto troque por malha viária, se quiser) que tem essa propriedade, mas sempre será possível produzir um grafo com "endereço absoluto" se seguirmos as hipóteses descritas no teorema de Trakhman. Transformadas para a linguagem da malha viária as hipóteses são:  
  

- Escolhidos dois cruzamentos quaisquer deverá ser sempre existir uma rota que parte de um cruzamento ao outro.
- Todos os cruzamentos deverão ter o mesmo número de opções de saída. Em nossa figura, esse número é igual a dois, observe que temos duas opções de saída, e somente duas, para cada um dos cruzamentos.

  
Se obedecermos as duas regras acima é possível projetarmos cidades com endereço absoluto de quaisquer dimensões.  
  
O "[Problema da Rota Colorida](https://www.blogger.com/blog/post/edit/5314484891711013222/8551492903365106386# "Problema da Rota Colorida")" estava sem solução desde que foi proposto por uma equipe de matemáticos dirigidas pelo professor Binyamin Weiss em 1970. A notícia da demonstração foi noticiada em todo o Brasil em 8 de fevereiro de 2008 e quem quiser pode consultar [aqui](https://www.blogger.com/blog/post/edit/5314484891711013222/8551492903365106386# "aqui").  
  
Na realidade não sei se construir cidades com este conceito é economicamente viável ou se de fato é simples para as pessoas memorizar grandes sequências de letras. De qualquer maneira o conceito é sedutor e surpreendente. Antes da prova de Trakhman eu não fazia idéia, e acredito que o leitor também não, de que é possível construir mapas com endereço absoluto.