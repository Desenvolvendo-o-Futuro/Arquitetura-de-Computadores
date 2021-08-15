# Transistores

## Válvulas Termiônicas
Os primeiros computadores eletrônicos, como o *ENIAC* usavam as chamadas válvulas termiônicos, dispositivos eletrônicos que regulam a passagem de elétrons através deles, assim como uma válvula hidráulica regula a passagem de água.

![Válvula Termiônica](https://upload.wikimedia.org/wikipedia/commons/8/89/VacuumTube1.jpg)

Uma válvula hidráulica, como um registro de torneira, ao ficar totalmente aberta permite a passagem total de água, ao passo que ao se fechar bloqueia o fluxo da água. Se ficar parcialmente aberta, então permitirá a passagem de um pouco de água e quanto mais aberta, maior o fluxo de água que passará.

 ![Desenho de uma Válvula Hidráulica](https://upload.wikimedia.org/wikipedia/commons/f/f7/Valve_cross-section.PNG)

As válvulas termiônicas como o exemplo abaixo, de uma válvula Tíratron, são formadas por um bulbo de vidro preenchido com um gás ionizável (como vapor de mercúrio, néon ou xenônio). Neste bulbo entra um filamento, que é basicamente uma resistência elétrica que aquece o gás presente no bulbo. Outros dois elementos importantes na válvula são o catodo e o anodo, onde o primeiro é eletrodo negativo (fornece elétrons) e o segundo é positivo (recebe elétrons), mas em condições normais, mesmo que você energize o catodo, nenhuma tensão passará para o outro lado. Um fio alimenta uma grade de controle que quando atinge uma determinada tensão (voltagem), permite a passagem de elétrons entre o catodo e o anodo.

![ Válvula Tiratron](https://upload.wikimedia.org/wikipedia/commons/6/60/Thyratron_Symbols.svg)

É possível usar tais válvulas termiônicas para amplificar sinais, isto é alimentar a grade de controle com tensões fracas para que ela permita a passagem de tensões maiores, mas proporcionais ao fraco sinal. Assim, é possível pegar o sinal fraquíssimo de uma guitarra da vibração das cordas de uma guitarra e jogar em grandes caixas de som de casas de shows.

Um outro uso é trabalhar somente o ato de ligar e desligar a passagem de eletricidade, e é dessa forma que são desenhados os computadores, ligando vários elementos deste tipo em uma rede onde uma válvula liga a outra de forma coordenada.

Entretanto, as válvulas termiônicas são grandes quentes e gastam muita energia para funcionar, sendo um grande impeditivo para a popularização dos computadores.

## Transistor

Transistores funcionam de forma muito parecida com as válvulas termiônicas, porém com menos elementos e de forma mais simples. O termo provém do inglês transfer resistor (resistor/resistência de transferência), como era conhecido pelos seus inventores.

Julius Edgar Lilienfeld patenteou um transistor de efeito de campo em 1926, mas não foi possível construir um dispositivo de trabalho naquele momento. O primeiro dispositivo praticamente implementado foi um transistor de contato pontual inventado em 1947 pelos físicos estadunidenses John Bardeen, Walter Brattain e William Shockley, o que lhes rendeu o Prêmio Nobel de Física em 1956.

![Diferentes tipos de transistores](https://upload.wikimedia.org/wikipedia/commons/f/f8/Transistor-photo.JPG)

Transistores são feitos de elementos semicondutores, sendo o mais famoso o silício. Semicondutores são elementos que não são condutores e nem isolantes, mas por conta disso sob certas condições agem como condutores ou isolantes. Misturando ao semicondutor, pequenas quantidades de outros elementos químicos que ganham ou perdem elétrons com facilidade, é possível mudar tais propriedades, num processo chamado dopagem.

Quando se dopa o cristal de semicondutor com um elemento como o Índio (In), obtém-se o cristal P, que pode ser usado como anodo, e quando se dopa o cristal de semicondutor com um elemento como o Fósforo ( P ), obtém-se o cristal N, que pode ser usado como catodo.

![Símbolo do Transistor de Junção Bipolar NPN](https://upload.wikimedia.org/wikipedia/commons/c/cb/BJT_NPN_symbol_%28case%29.svg)

Quando se junta esses cristais na configuração NPN, obtêm-se um Transistor de Junção Bipolar. Tal transístor apresenta três elementos, o Emissor (E), a Base (B) e o Coletor ( C ). Quando se energiza a Base com uma pequena tensão é possível passar correntes entre o Coletor e o Emissor.

![Transistor de Junção Bipolar](https://upload.wikimedia.org/wikipedia/commons/6/6b/NPN_BJT_%28Planar%29_Cross-section.svg)

## Construindo Circuitos Digitais

Ao conectar transistores é possível criar circuitos que executam operações lógicas mais complexas. Abaixo, pode-se ver os casos das operações lógicas mais simples: E (AND) e OU (OR).

### Porta Lógica E (AND)

Essa porta lógica compara se há dois sinais iguais a 1 (verdadeiro), a saída é 1 (verdadeiro), mas se houver algum sinal 0 (falso), a saída será 0 (falso). Em tal circuito, usou-se um led para mostrar saída, acendendo quando a saída é 1 e apagando quando for 0. Foram usados dois botões para indicar as entradas representando o sinal 1 (verdadeiro) quando pressionados.
![Implementação da Porta Lógica E por https://tecdicas.com/criando-portas-logicas-com-transistores/](https://tecdicas.com/content/images/2019/11/porta-and-transistor-tabela-verdade-esquema.jpg)

Para implementar essa porta lógica, a fonte de tensão foi ligada ao Coletor do primeiro transistor e aos botões. Em seguida o Emissor do primeiro transistor foi ligado ao coletor do segundo transistor enquanto seu emissor foi ligado ao terra. A saída dos botões foram ligadas à Base de cada um dos transistores.

Quando a base do primeiro transistor é energizada, então é permitida a passagem de corrente até o segundo transistor, mas este permanece aberto enquanto sua base não for energizada. Somente quando ambas as bases forem energizadas simultaneamente é que será permitida a passagem de corrente na saída, gerando o valor 1 (verdadeiro).

### Porta Lógica OU (OR)

Essa porta lógica verifica se há ao menos um sinal igual a 1 (verdadeiro), então a saída é 1 (verdadeiro), mas se não houverem sinais 1 (verdadeiro), a saída será  0 (falso). Similarmente à Porta Lógica E, foi usado um led para indicar a saída, acendo no caso 1 (verdadeiro) e apagando no caso 0 (falso).

![Porta Lógica OU por https://tecdicas.com/criando-portas-logicas-com-transistores/](https://tecdicas.com/content/images/2019/11/porta-or-transistor-tabela-verdade-esquema.jpg)

Neste caso, para implementar tal porta, os transistores são colocados em paralelo tendo os Coletores ligado à fonte de tensão. Os botões são ligados às bases e seus emissores são aterrados. Assim, sempre que houver um sinal 1 (verdadeiro) em alguns dos botões haverá a passagem de corrente no circuito.

### Circuitos mais Complexos

Embora o funcionamento dos computadores sejam baseados nas portas lógicas apresentadas, seu funcionamento não é limitado a operações tão simples. Na realidade, dentro de um processador, por exemplo, é construída uma rede de transistores extremamente complexa composta por milhões de transistores. Um processador como o [Core i7 Broadwell-U](https://en.wikipedia.org/wiki/Broadwell_(microarchitecture) "Broadwell (microarchitecture)") (2015) pode possuir até 1,9 bilhões de transistores, cada um medindo 14 nanômetros, enquanto um processador [AMD](https://en.wikipedia.org/wiki/AMD "AMD")  [Ryzen](https://en.wikipedia.org/wiki/Zen_2#Desktop_processors "Zen 2") 7 3700X (2019) possui 5,99 bilhões de transistores, cada um medindo 7 nanômetros. Abaixo pode ser visto o exemplo de circuito de um [Amd Ryzen 7 1800X (2017)](https://en.wikichip.org/wiki/amd/ryzen_7/1800x).

![Amd Ryzen 7 1800X ](https://en.wikichip.org/w/images/3/3f/amd_zen_octa-core_die_shot.png)

## Por que trabalhar com Verdadeiro e Falso

Resposta curta: Porque é mais simples.

Transistores também têm a capacidade de trabalhar com variações contínuas de tensão e corrente e existem diversos circuitos analógicos que fazem uso dessa capacidade, incluindo diversos tipos de amplificadores que estão espalhados por todo canto, amplificando sinais de instrumentos musicais a rádio frequência.

Entretanto, até o presente momento é impraticável trabalhar com um circuito lógico mais complexo usando sinais contínuos. Na origem da computação, a abstração binária onde os valores possíveis são 0 e 1 se mostrou a mais simples de se trabalhar e em cima dela foi construída a computação moderna.

Esses zeros e uns em última instância representam a presença ou ausência de corrente elétrica, como pode ser visto nos exemplos anteriores. Em geral computadores trabalham como uma tensão contínua, normalmente algo em torno de 5 volts, que periodicamente varia entre 0 e os próprios 5 volts indicando valores binários de acordo com os diferentes processamentos que estejam sendo feitos pela máquina. A partir de então, para transpor os resultados em uma base lógica, assumiu-se que 0 representaria o valor Falso enquanto 1 representaria o valor Verdadeiro, construindo a chamada Lógica Booleana.

Em 1958, na URSS foi desenvolvido um computador de base Ternária, isto é com baseado em 3 possibilidades, um projeto desenvolvido na Moscow State University por Sergei Sobolev and Nikolay Brusentsov, mas tal tecnologia não se popularizou. 