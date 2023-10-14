---
layout: post
title: A Matemática do Playlist
date: 2012-02-02 10:00:00 +1000
categories: mathematics blog
mathjax: true
---

# A Matemática do Playlist
  
Meu irmão ligou dizendo que já estava perto e que eu deveria descer para ganhar tempo. Era sexta-feira, fim do dia e estávamos nos preparando para irmos ao litoral. Logo ao entrar no carro ele pediu para que eu colocar o novo CD que ele tinha comprado. Tinha 100 músicas e deveria durar a viagem toda e ainda sobrar.  
  
Ele sugeriu que eu selecionasse o modo "randômico", porém frustado, fez o seguinte comentário:  
  
- O randômico desse rádio tá quebrado!  
- Como assim, quebrado - disse eu.  
- Bom, você vai ver, daqui a pouco vai repetir uma música.  
- Ué, e daí, o randômico não garante que as músicas não vão repetir. Já tentou o modo "sequencial"? -respondi irônico.  
- Cara, tem 100 músicas no CD, toda a vez que vou pro escritório acabo ouvindo uma música repetida no caminho.  
  
Fiquei intrigado com o comentário, e ainda mais intrigado com o gosto musical do meu irmão, mas afinal o carro era dele. Como fuga para o inferno musical a que fui exposto, meu cérebro logo encontrou consolo nas abstrações platônicas matemáticas, uma higiene mental.  
  
No íntimo eu duvidava que o modo randômico estava quebrado uma vez que é tão fácil implementá-lo computacionalmente. Tentei modelar o problema de maneira a poder tratá-lo, assumi que o modo randômico no caso é equivalente a jogar um dado de 100 lados toda a vez para definir a música que será tocada. É claro que em algum momento repetições irão acontecer, mas a pergunta era, quando?  
  
Matematicamente o que eu buscava era responder qual era o número esperado de músicas a ouvir até que haja a primeira repetição. Na estatística esse conceito tem um nome curioso, se chama "Esperança".  
  
O conceito de Esperança tem um relação forte com a média, por exemplo, suponha que meu irmão anotasse quantas músicas escutou até a primeira repetição todas as vezes que foi ao escritório (assumindo que haja sempre tempo para que alguma repetição ocorra, o que não é verdade). A média deste valor é próximo ao valor esperado que estamos procurando.  
  
Ele poderia tabular os valores conforme a tabela abaixo. Suponha que tenha ouvido o CD 1000 vezes, então a tabela seria algo assim.  
  
| número de músicas sem repetição | quantidade de vezes |
| --- | --- |
| 1 | 3 |
| 2 | 5 |
| 3 | 8 |
| 4 | 12 |
| … | … |
| 100 | 0 |
| Total | 1000 |

Formalmente esse valor deverá ser próximo a expressão abaixo onde P(x) significa Probabilidade de que x ocorra:  
  
1 x P(1 música sem repetição) + 2 x P(2 músicas sem repetição) + ... + 100 x P(100 músicas sem repetição)  
  
O leitor paciente irá constatar que calcular a média aritmética de quantas músicas até a primeira repetição da tabela é próximo ao conceito platônico de "Esperança" dado em função de probabilidades. A pergunta que resta é como calcular as probabilidades. Para ajudar o raciocínio vamos calcular a probabilidade de  ouvirmos exatamente 4 músicas não repetidas, isto é, a repetição ocorrerá necessariamente na quinta música.  
  
$$
1 \times \frac{99}{100} \times \frac{98}{100} \times \frac{97}{100} \times \frac{4}{100}
$$

O que é equivalente a:
$$
\frac{100!}{96! \times 100^5} \times 4
$$

Convertendo os valores para uma forma geral teremos:
$$
\frac{n!}{(n-k)!n^{k+1}} k
$$
onde n = 100 e k = 4


Enfim, reconstruindo a fórmula acima em função dos resultados obtidos acima teremos:

$$
\sum_{k=0}^{n} \frac{k^2n!}{n^{k+1}(n-k)!}
$$   
Não consegui ainda uma forma fechada, ou seja, não consegui me livrar do somatório para a fórmula, o que significa que vou precisar usar arsenal computacional. Felizmente o leitor poderá contar com a widget que eu criei para calcular o número esperado de músicas em função do número total do CD.  
  
Por exemplo, meu irmão ficou surpreso em saber que para seu CD esse número é 12, isto é, considerando uma média de 3 minutos para cada música, é esperado que ocorra a primeira repetição 36 minutos depois.  
  
De fato, com o trânsito de São Paulo sexta-feira à noite, ouvimos a primeira repetição antes de chegarmos na imigrantes, onde fui acordado do meu transe matemático com um grito desproporcionalmente estridente do meu irmão:  
  
- AhÁ, eu te disse, o randômico tá quebrado!!!!