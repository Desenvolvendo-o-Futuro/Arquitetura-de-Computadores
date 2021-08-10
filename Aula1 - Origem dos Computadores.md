# História da Computação

## O que é um Computador?
**Etimologia:** Que computa, que faz cômputos (cálculos) de; calculador.

No século XIX e XX o termo era designado para pessoas responsáveis por fazer cálculos para diversos fins. Era considerado uma tarefa considerada "inferior" de suporte à pesquisa e engenharia, mas de suma importância em muitos aspectos. Um exemplo pode ser visto no filme **Estrelas Além do Tempo** (Hidden Figures - 2016) que narra a história de um grupo de computadoras negras que trabalharam para a NASA  durante a década de 1960 em projetos como Mercury e Geminy.

## Os Primeiros Computadores

### Primórdios

Desde o início da civilização, seres humanos buscaram criar mecanismos para auxiliar nos cálculos, como o ábaco que provavelmente foi criado na Mesopotâmia há mais de 7.500 anos atrás.

Mas em 1901 foi encontrado um mecanismo, bastante curioso na costa da ilha grega de Anticítera, que ficou conhecido como a **Máquina de Anticítera**. Um mecanismo de engrenagens capaz de calcular com bastante precisão a órbita de estrelas, as posições das constelações e eclipses, sendo este provavelmente o primeiro computador mecânico.

![ Restos da Máquina de Anticítera](https://upload.wikimedia.org/wikipedia/commons/6/66/NAMA_Machine_d%27Anticyth%C3%A8re_1.jpg)

![Reconstrução da Máquina de Anticítera](https://upload.wikimedia.org/wikipedia/commons/thumb/7/76/Antikythera_model_front_panel_Mogi_Vicentini_2007.JPG/250px-Antikythera_model_front_panel_Mogi_Vicentini_2007.JPG)

### Computadores Mecânicos Multifuncionais

A primeira máquina computadora de verdade foi construída por [Wilhelm Schickard](https://pt.wikipedia.org/wiki/Wilhelm_Schickard "Wilhelm Schickard") sendo capaz de somar, subtrair, multiplicar e dividir. Essa máquina foi perdida durante a [guerra dos trinta anos](https://pt.wikipedia.org/wiki/Guerra_dos_trinta_anos "Guerra dos trinta anos"), sendo que recentemente foi encontrada alguma documentação sobre ela. Durante muitos anos nada se soube sobre essa máquina, por isso, atribuía-se a [Blaise Pascal](https://pt.wikipedia.org/wiki/Blaise_Pascal "Blaise Pascal") ([1623](https://pt.wikipedia.org/wiki/1623 "1623")-[1662](https://pt.wikipedia.org/wiki/1662 "1662")) a construção da primeira máquina calculadora, que fazia apenas somas e subtrações.

![Pascaline, máquina calculadora feita por [Blaise Pascal](https://pt.wikipedia.org/wiki/Blaise_Pascal "Blaise Pascal")](https://upload.wikimedia.org/wikipedia/commons/thumb/8/80/Arts_et_Metiers_Pascaline_dsc03869.jpg/150px-Arts_et_Metiers_Pascaline_dsc03869.jpg)

No século XIX, o matemático Charles Babbage propôs uma máquina de calcular que poderia ser programada através de cartões e capaz de imprimir seus resultados em papel, porém não conseguiu fundos suficientes para construir uma versão funcional do [calculador analítico](https://pt.wikipedia.org/wiki/Engenho_anal%C3%ADtico "Engenho analítico"). A matemática e escritora Ada Lovelace desenvolveu um algoritmo para ser executado no Calculador Analítico de Babbage, sendo considerada a primeira programadora da história.
[![Réplica (parte) do Calculador Diferencial criado por  [Charles Babbage](https://pt.wikipedia.org/wiki/Charles_Babbage "Charles Babbage").](https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/BabbageDifferenceEngine.jpg/220px-BabbageDifferenceEngine.jpg)](https://pt.wikipedia.org/wiki/Ficheiro:BabbageDifferenceEngine.jpg)

### Máquina de Turing

A ***Máquina de Turing*** foi um modelo de computador teórico proposto pelo matemático Alan Turing em 1936, conhecido também como a *máquina universal*. Tal máquina é capaz de receber programas indicando quais ações ela deve tomar, sendo que tal programa pode ser a definição de outra Máquina de Turing.

Uma máquina de Turing consiste em:

1.  Uma  _fita_  que é dividida em células, uma adjacente à outra. Cada célula contém um símbolo de algum alfabeto finito. O alfabeto contém um símbolo especial  _branco_  (aqui escrito como ¬) e um ou mais símbolos adicionais. Assume-se que a fita é arbitrariamente extensível para a esquerda e para a direita, isto é, a máquina de Turing possui tanta fita quanto é necessário para a computação. Assume-se também que células que ainda não foram escritas estão preenchidas com o símbolo branco.
2.  Um  _cabeçote_, que pode ler e escrever símbolos na fita e mover-se para a esquerda ou para a direita.
3.  Um  _registrador de estados_, que armazena o estado da máquina de Turing. O número de estados diferentes é sempre finito e há um estado especial denominado  _estado inicial_  com o qual o registrador de estado é inicializado.
4.  Uma  _tabela de ação_  (ou  _função de transição_) que diz à máquina que símbolo escrever, como mover o cabeçote (![\leftarrow ](https://wikimedia.org/api/rest_v1/media/math/render/svg/3c0fb4bce772117bbaf55b7ca1539ceff9ae218c)  para esquerda e  ![\rightarrow ](https://wikimedia.org/api/rest_v1/media/math/render/svg/53e574cc3aa5b4bf5f3f5906caf121a378eef08b)  para direita) e qual será seu novo estado, dados o símbolo que ele acabou de ler na fita e o estado em que se encontra. Se não houver entrada alguma na tabela para a combinação atual de símbolo e estado então a máquina para.

Note que cada parte da máquina é finita e sua quantidade de fita potencialmente ilimitada dá uma quantidade ilimitada de espaço de memória.

## Computadores Eletrônicos

Durante a Segunda Guerra Mundial foi desenvolvido o primeiro computador eletrônico, o _Eletronic Numeric Integrator And Calculator_ (**ENIAC**), capaz de fazer 500 multiplicações por segundo, sendo usado para calcular trajetórias de mísseis e mantido em segredo até o fim da guerra e era programado através do rearranjamento de fios em um painel.

![ENIAC](https://upload.wikimedia.org/wikipedia/commons/a/aa/Reprogramming_ENIAC.png)

## Arquitetura Von Neumman

John Von Neumman propôs uma modelagem dos computadores de forma inspirada em um sistema nervoso central, organizando-os da seguinte forma:

Para isso, eles teriam que ter três características:

1.  Codificar as instruções de uma forma possível de ser armazenada na  [memória do computador](https://pt.wikipedia.org/wiki/Mem%C3%B3ria_(computador)). Von Neumann sugeriu que fossem usados uns e zeros.
2.  Armazenar as instruções na memória, bem como toda e qualquer informação necessária a execução da tarefa, e
3.  Quando processar o programa, buscar as instruções diretamente na memória, ao invés de lerem um novo  "Cartão perfurado" a cada passo.

![Visão simplificada da arquitetura de Von Neumann.
](https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Arquiteturavn.png/220px-Arquiteturavn.png)

Este é o conceito de programa armazenado, cujas principais vantagens são: rapidez, versatilidade e automodificação. Assim, o computador programável que conhecemos hoje, onde o programa e os dados estão armazenados na memória ficou conhecido como Arquitetura de von Neumann, sendo usada até hoje nos computadores modernos.