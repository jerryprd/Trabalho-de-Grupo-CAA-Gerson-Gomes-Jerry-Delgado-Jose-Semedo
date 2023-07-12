![](Aspose.Words.fd4c8fda-61d8-42a3-8a5f-623013dfa1a4.001.png)

[***CIÊNCIAS DA SAÚDE, AMBIENTE E TECNOLOGIAS** ](https://us.edu.cv/usSITE/index.php/departamentos/ciencias-da-saude-ambiente-e-tecnologias)*(DCSAT)* **LICENCIATURA EM ENGENHARIA INFORMÁTICA** 

**2º ANO / 2º SEMESTRE** 

**CONCEPÇÃO E ANÁLISE DE ALGORÍTMOS** 

*RELATÓRIO FINAL:* 

*JOGO DE GESTÃO BIBLIOTECÁRIA* 

**DOCENTE:** VALÉRIO SANTOS 

**DISCENTES:**                                                                                                GERSON GOMES – Nr: 5876 

`                                                                                    `JERRY DELGADO – Nr: 5686                                                                             JOSÉ SEMEDO – Nr: 6370 

Julho de 2023 

Índice 

[Introdução ........................................................................................................................................... 1 ](#_page2_x82.00_y71.00)[Objetivos: ............................................................................................................................................ 2 ](#_page3_x82.00_y71.00)[Estrutura de dados: .............................................................................................................................. 3 ](#_page4_x82.00_y71.00)[Algoritmos........................................................................................................................................... 3 ](#_page4_x82.00_y295.00)[Análise da complexidade .................................................................................................................... 5 ](#_page6_x82.00_y132.00)[Justificativa da Estrutura e Serviços.................................................................................................... 5 ](#_page6_x82.00_y267.00)[Resultado da execução do programa ................................................................................................... 6 ](#_page7_x82.00_y71.00)[Interface............................................................................................................................................... 6 ](#_page7_x82.00_y466.00)[Manual do Utilizador .......................................................................................................................... 7 ](#_page8_x82.00_y71.00)[Justificação de Erros ........................................................................................................................... 8 ](#_page9_x82.00_y71.00)[Resultados esperados .......................................................................................................................... 9 ](#_page10_x82.00_y71.00)[Melhoramento ................................................................................................................................... 10 ](#_page11_x82.00_y71.00)[Conclusão .......................................................................................................................................... 11 ](#_page12_x82.00_y71.00)[Bibliografia ....................................................................................................................................... 12 ](#_page13_x82.00_y71.00)

<a name="_page2_x82.00_y71.00"></a>Introdução 

Este relatório aborda o desenvolvimento de um jogo de biblioteca no Scratch, um ambiente de programação visual. O jogo simula uma experiência de exploração de uma biblioteca virtual, onde os usuários podem interagir com prateleiras de livros, abrir e ler informações sobre os livros, além de decidir se desejam adicioná-los a uma lista de livros levados. Para implementar o jogo, foram consideradas estruturas de dados e algoritmos adequados, visando uma organização eficiente do código e uma experiência fluida para o usuário. 

A criação de um jogo de biblioteca no Scratch é um processo complexo que envolve a organização cuidadosa do programa em diferentes módulos. Essa estrutura modular permite uma melhor legibilidade e manutenção do código, além de facilitar a reutilização de trechos específicos em futuros projetos. Neste relatório, vamos explorar em detalhes a estrutura do programa e descrever os principais módulos e serviços oferecidos por cada um deles, levando em consideração a utilização do Scratch como ambiente de desenvolvimento. 

<a name="_page3_x82.00_y71.00"></a>Objetivos: 

**Objetivo principal** 

Desenvolver um jogo de biblioteca no Scratch, um ambiente de programação visual. O jogo tem como propósito simular uma experiência de exploração de uma biblioteca virtual, onde os usuários podem interagir com prateleiras de livros, ler informações sobre os livros e decidir se desejam adicioná-los a uma lista de livros levados. 

**Objetivos específicos:** 

1. Criar uma estrutura modular para o programa do jogo, dividindo-o em módulos que lidam com diferentes aspectos, como controle principal, som, modos de jogo gráfico e consola. 
1. Implementar a funcionalidade de reprodução de sons no jogo, incluindo sons de fundo e efeitos sonoros para melhorar a experiência do usuário. 
1. Desenvolver os modos de jogo gráfico e consola, permitindo que os usuários interajam com os livros de diferentes formas, seja clicando visualmente nas prateleiras ou digitando o número correspondente ao livro desejado. 
1. Criar atores virtuais que fornecem informações sobre os livros selecionados e fazem perguntas aos usuários para determinar se eles desejam levar o livro ou retornar à prateleira. 
1. Implementar a funcionalidade de adicionar livros selecionados à lista de livros levados, permitindo aos usuários acompanharem os livros que escolheram durante o jogo. 

<a name="_page4_x82.00_y71.00"></a>Estrutura de dados: 

Na concepção do jogo, foram utilizadas as seguintes estruturas de dados: 

- **Listas:** As listas foram utilizadas para armazenar as prateleiras de livros, a lista de livros levados e a lista de informações dos livros. Cada elemento da lista representa um livro, contendo suas informações, como título, autor e sinopse. 
- **Variáveis:** Variáveis foram usadas para controlar o fluxo do jogo, armazenar o modo de jogo selecionado e acompanhar o livro atualmente aberto. 

<a name="_page4_x82.00_y295.00"></a>Algoritmos 

Os principais algoritmos utilizados no jogo de biblioteca são responsáveis por lidar com as interações do usuário e controlar o fluxo do jogo. São eles: 

- **Algoritmo de seleção de livro:** Esse algoritmo verifica qual livro foi selecionado pelo usuário, seja clicando visualmente ou digitando o número correspondente no modo consola. Ele identifica o livro na lista de prateleiras e o abre para exibir suas informações. 
- **Algoritmo de adição de livro à lista:** Esse algoritmo é acionado quando o usuário decide levar um livro. Ele adiciona o livro à lista de livros levados, permitindo ao usuário acompanhar suas escolhas durante o jogo. 

**Módulo Principal** 

O módulo principal, representado pela classe "Main", desempenha um papel fundamental no controle da execução do jogo. Sua função é inicializar o programa, criar os objetos e variáveis necessárias e apresentar o menu principal ao usuário. Esse módulo também é responsável por receber as opções escolhidas pelo usuário, como "Play", "Sound" e "Quit", e encaminhar o fluxo do programa para os módulos correspondentes de acordo com a opção selecionada. A escolha dessa estrutura de módulo principal ajuda a manter o código organizado e facilita a compreensão da lógica de controle do jogo. 

**Módulo de Som** 

O módulo de som, representado pela classe "SoundModule", é responsável por todas as interações sonoras do jogo. Ele oferece serviços para reproduzir sons de fundo durante o jogo, criando uma atmosfera adequada e imersiva. Além disso, o módulo de som também fornece efeitos sonoros para as interações do usuário, como o clique em um livro ou a resposta a uma pergunta. Esses efeitos sonoros contribuem para a experiência do usuário, fornecendo um feedback auditivo que reforça as ações realizadas no jogo. A escolha de um módulo separado para o som permite um controle mais granular dos recursos sonoros e facilita a adição e modificação de sons no jogo. 

**Módulo de Modo de Jogo** 

O módulo de modo de jogo, representado pela classe "GameModeModule", gerencia a escolha e execução dos diferentes modos de jogo disponíveis. Ele apresenta ao usuário as opções de modo de jogo, como "Consola" ou "Gráfico", e permite que ele selecione o modo de sua preferência. Com base na escolha do usuário, o módulo de modo de jogo encaminha 

- fluxo do programa para os módulos correspondentes a cada modo selecionado. 

**Módulo de Modo Gráfico** 

O módulo de modo gráfico, representado pela classe "GraphicModeModule", lida com a exibição visual das prateleiras de livros e as interações gráficas no jogo. Esse módulo é responsável por criar e exibir as prateleiras de livros na tela, proporcionando uma representação gráfica das opções disponíveis ao usuário. Quando o usuário clica em um livro, o módulo de modo gráfico é acionado para abrir o livro selecionado. Essa abertura revela suas informações e apresenta uma pergunta ao usuário sobre seu interesse em levá- lo. Dependendo da resposta do usuário, o livro é adicionado à lista de livros levados ou o usuário retorna à prateleira. O uso de um módulo específico para o modo gráfico permite a implementação de recursos visuais atraentes e interativos no jogo, tornando a experiência mais imersiva e envolvente para o usuário. 

**Módulo de Modo Consola** 

O módulo de modo consola, representado pela classe "ConsoleModeModule", oferece uma alternativa ao modo gráfico, focada em interações baseadas em texto. Nesse modo, o usuário não interage visualmente com os livros, mas em vez disso, digita o número correspondente ao livro que deseja abrir. O módulo de modo consola exibe a lista de livros disponíveis e recebe a entrada do usuário por meio do teclado. Em seguida, ele abre o livro correspondente ao número digitado, exibindo suas informações e perguntando ao usuário se deseja levá-lo. Assim como no modo gráfico, o livro selecionado é adicionado à lista de livros levados ou o usuário retorna à lista de livros disponíveis. A inclusão de um módulo específico para o modo consola permite acomodar usuários que preferem interações baseadas em texto ou situações em que a interface gráfica não é possível ou desejada. 

<a name="_page6_x82.00_y132.00"></a>Análise da complexidade 

Os algoritmos implementados no jogo de biblioteca possuem complexidade linear, uma vez que a busca do livro selecionado ocorre percorrendo a lista de prateleiras até encontrar o livro desejado. A adição de um livro à lista de livros levados também é uma operação de complexidade constante, pois envolve apenas a inserção de um elemento na lista. 

<a name="_page6_x82.00_y267.00"></a>Justificativa da Estrutura e Serviços 

A escolha de uma estrutura modular para o programa do jogo de biblioteca no Scratch é essencial para garantir a organização e manutenção adequadas do código. A divisão em módulos permite que cada componente do jogo tenha uma responsabilidade específica e claramente definida. Isso facilita a compreensão do código, torna a solução mais modular e reutilizável e promove uma colaboração eficiente entre os desenvolvedores. 

Ao separar o módulo principal do programa, é possível concentrar-se na lógica de controle central e no gerenciamento do fluxo de execução do jogo. Isso torna o código mais legível e ajuda a evitar problemas de complexidade excessiva. Além disso, a separação dos serviços de som em um módulo específico oferece flexibilidade para controlar as configurações sonoras e permite uma fácil manutenção e expansão do sistema sonoro no jogo. 

Os módulos de modo de jogo, modo gráfico e modo consola foram desenvolvidos para atender às necessidades dos usuários, oferecendo diferentes formas de interação com o jogo. O modo gráfico, com sua representação visual das prateleiras e livros, proporciona uma experiência imersiva para os jogadores que preferem uma abordagem mais interativa. Já o modo consola oferece uma alternativa baseada em texto, adequada para usuários que preferem uma interação mais direta e sucinta. Essa variedade de modos de jogo torna o jogo de biblioteca mais acessível e atraente para diferentes tipos de jogadores. 

<a name="_page7_x82.00_y71.00"></a>Resultado da execução do programa 

O programa do jogo de biblioteca no Scratch, com sua estrutura modular bem definida, permite aos usuários desfrutarem de uma experiência interativa e envolvente. Ao executar o programa, os usuários são apresentados ao menu principal, onde podem escolher entre as opções "Play", "Sound" e "Quit". A seleção da opção "Play" direciona os usuários para escolher o modo de jogo, seja "Consola" ou "Gráfico". Cada modo oferece uma experiência única. 

No modo gráfico, os usuários são transportados para a página com as prateleiras de livros. Eles podem navegar pelas prateleiras e clicar em um livro para abri-lo. Ao abrir um livro, eles têm acesso a informações detalhadas sobre o livro e são questionados se desejam levá- lo. Caso optem por levar o livro, ele é adicionado à lista de livros levados. Se não desejarem, podem retornar à prateleira para explorar outros livros. 

No modo consola, os usuários são direcionados a digitar o número correspondente ao livro que desejam abrir. A lista de livros disponíveis é exibida, e o usuário pode inserir o número do livro desejado. O livro é então aberto, fornecendo informações sobre ele e fazendo a pergunta sobre o desejo de levá-lo. O livro é adicionado à lista de livros levados se o usuário optar por levá-lo. 

<a name="_page7_x82.00_y466.00"></a>Interface 

A interface do jogo de biblioteca foi projetada para ser intuitiva e amigável ao usuário. Ela apresenta as prateleiras de livros, permitindo ao usuário clicar visualmente em um livro para abri-lo ou digitar o número correspondente no modo consola. Ao abrir um livro, são exibidas suas informações, incluindo título, autor e sinopse. Além disso, um ator virtual fornece detalhes adicionais sobre o livro e faz uma pergunta ao usuário para determinar se ele deseja levá-lo ou retornar à prateleira. 

<a name="_page8_x82.00_y71.00"></a>Manual do Utilizador 

O programa do jogo de biblioteca no Scratch oferece uma variedade de funcionalidades para os usuários aproveitarem ao máximo sua experiência. Abaixo está uma sequência correta de operações para utilizar o programa em todas as funcionalidades disponíveis: 

Ao iniciar o programa, será exibido o menu principal. 

Clique na opção "Play" para selecionar o modo de jogo. 

Escolha entre os modos "Gráfico" ou "Consola" e siga as instruções fornecidas. 

**No modo gráfico:** 

1. Navegue pelas prateleiras clicando nos livros. 
1. Ao encontrar um livro de interesse, clique nele para abri-lo. 
1. Leia as informações fornecidas pelo ator virtual e responda à pergunta no final. 
1. Se desejar levar o livro, clique em "Sim". Caso contrário, clique em "Não" para retornar à prateleira. 
1. O livro levado será adicionado à sua lista. 
1. Continue explorando as prateleiras e repetindo o processo. 

**No modo consola:** 

1. Digite o número correspondente ao livro que deseja abrir, de acordo com a lista exibida. 
1. O livro será aberto, e você poderá ler as informações fornecidas. 
1. Responda à pergunta no final digitando "Sim" ou "Não". 
1. Se desejar levar o livro, digite "Sim". Caso contrário, digite "Não" para retornar à lista. 
1. O livro levado será adicionado à sua lista. 
1. Repita o processo para outros livros. 

Ao terminar o jogo, pode-se selecionar outras opções no menu principal, como "Sound" para configurar as opções de som ou "Quit" para sair do jogo. 

<a name="_page9_x82.00_y71.00"></a>Justificação de Erros 

Durante a execução do programa, podem ocorrer alguns erros comuns, que podem ser justificados da seguinte forma: 

- **Erro ao abrir um livro:** Se o usuário encontrar dificuldades em abrir um livro, é possível que o número digitado ou o livro clicado não esteja correto. Certifique-se de escolher o número correto na lista ou clicar no livro desejado. 
- **Erro ao adicionar um livro à lista:** Caso o livro não seja adicionado corretamente à lista de livros levados, verifique se você respondeu corretamente à pergunta sobre levar o livro e seguiu todas as instruções fornecidas pelo ator virtual. 
- **Erro de som:** Se houver problemas com a reprodução de sons no jogo, verifique se 
- som está ativado e se o volume está ajustado corretamente. Caso persista o problema, verifique as configurações de áudio do seu dispositivo. 

É importante destacar que essas justificativas são apenas exemplos e que, durante o desenvolvimento do jogo, será necessário identificar e tratar os possíveis erros que podem ocorrer, fornecendo mensagens claras ao usuário para orientá-lo na resolução desses problemas. 

<a name="_page10_x82.00_y71.00"></a>Resultados esperados 

Espera-se que, ao finalizar este trabalho, o jogo de biblioteca no Scratch ofereça uma experiência interativa e divertida para os usuários. Os resultados esperados incluem: 

- Um programa funcional que permite aos usuários explorarem uma biblioteca virtual, interagir com prateleiras de livros e ler informações detalhadas sobre cada livro. 
- A capacidade de reproduzir sons de fundo e efeitos sonoros para tornar a experiência do jogo mais imersiva. 
- A implementação de modos de jogo gráfico e consola, oferecendo aos usuários diferentes formas de interagir com os livros. 
- A presença de atores virtuais que fornecem informações sobre os livros e fazem perguntas, adicionando uma camada de interatividade e engajamento ao jogo. 
- A funcionalidade de adicionar livros selecionados à lista de livros levados, permitindo aos usuários acompanharem e revisitar suas escolhas durante o jogo. 

<a name="_page11_x82.00_y71.00"></a>Melhoramento 

Embora o programa do jogo de biblioteca no Scratch já apresente uma estrutura sólida, há oportunidades para melhorias e expansões futuras. Algumas funcionalidades adicionais que poderiam ser implementadas incluem: 

- Sistema de pontuação: Adicionar um sistema de pontuação que recompense os jogadores por cada livro levado ou respostas corretas nas perguntas feitas pelos atores no modo gráfico. 
- Recursos de pesquisa: Implementar uma funcionalidade de pesquisa para permitir que os usuários encontrem livros específicos com base em critérios, como autor, título ou gênero. 
- Modo multiplayer: Adicionar um modo multiplayer que permita aos jogadores interagirem entre si, compartilhando suas listas de livros levados ou competindo em desafios. 
- Minijogos educativos: Incluir minijogos educativos relacionados a livros e literatura, como quizzes sobre autores famosos, enigmas relacionados a histórias ou quebra-cabeças de palavras. 

Aumentar a eficiência do programa é um objetivo importante. Para isso, poderiam ser implementadas as seguintes melhorias: 

- Otimização de código: Rever o código existente em busca de possíveis melhorias de desempenho e eficiência, como evitar repetições desnecessárias e otimizar loops. 
- Gerenciamento de recursos: Implementar um gerenciamento eficiente dos recursos do jogo, como memória e processamento, para garantir um desempenho suave e evitar travamentos. 
- Melhoria da interface do usuário: Aprimorar a interface gráfica para torná-la mais intuitiva e amigável, garantindo que os usuários possam navegar facilmente pelas opções do jogo e entender as ações disponíveis. 

<a name="_page12_x82.00_y71.00"></a>Conclusão 

Durante o desenvolvimento do jogo de biblioteca, algumas dificuldades foram encontradas, como a necessidade de equilibrar a interação visual e a interação baseada em texto no modo consola. Foi necessário dedicar tempo à compreensão do problema e à concepção de uma solução que atendesse aos requisitos do jogo. A implementação envolveu a criação das estruturas de dados, a codificação dos algoritmos e a integração da interface gráfica e sonora. 

O jogo de biblioteca desenvolvido no Scratch alcançou os resultados esperados, proporcionando uma experiência interativa e envolvente aos usuários. Os objetivos de implementar a exploração das prateleiras de livros, exibir informações detalhadas e permitir ao usuário adicionar livros à lista foram alcançados. No entanto, é importante mencionar que o jogo pode ter limitações em relação à quantidade de livros disponíveis e à diversidade das interações. Para uma nova versão, seria interessante expandir o número de livros e incluir funcionalidades adicionais, como sistema de pontuação, pesquisa de livros e minijogos educativos. 

As estruturas de dados utilizadas no jogo, como listas e variáveis, mostraram-se adequadas para armazenar e gerenciar as informações dos livros e o estado do jogo. Elas forneceram uma organização eficiente dos dados e facilitaram o controle do fluxo do jogo. 

A estrutura modular do programa do jogo de biblioteca no Scratch se mostrou eficiente na organização do código e na manutenção do projeto. A divisão em módulos permitiu um desenvolvimento mais claro e modular, facilitando a adição de novas funcionalidades e a manutenção das existentes. 

A utilização do ambiente Scratch proporcionou uma implementação interativa e envolvente do jogo de biblioteca. Os diferentes modos de jogo oferecidos (gráfico e consola) atendem a diferentes preferências dos usuários, permitindo uma experiência personalizada. 

Espera-se que este trabalho resulte em um jogo de biblioteca no Scratch que proporcione uma experiência envolvente e educativa para os usuários, incentivando a exploração e a descoberta de novos livros e conhecimentos. 

<a name="_page13_x82.00_y71.00"></a>Bibliografia 

[Estruturas de dados: uma introdução | Alura ](https://www.alura.com.br/artigos/estruturas-de-dados-introducao?fbclid=IwAR1XFjz1u8KrZ3k3m2HHPnpbneKNFyqdQsasDvb-wyvNg15ouRFD2ITl0xM)

[Estrutura de Dados: entenda o conceito e os principais tipos (awari.com.br) ](https://awari.com.br/estrutura-de-dados/?utm_source=blog&utm_campaign=projeto+blog&utm_medium=Estrutura%20de%20Dados:%20entenda%20o%20conceito%20e%20os%20principais%20tipos)

[Como Programar um Jogo: 10 Passos (com Imagens) - wikiHow ](https://pt.wikihow.com/Programar-um-Jogo?fbclid=IwAR1hN4bYXK7Eu39EsTQbI1nFXIrDyGBpUhqbKple1xN050YmOETPaEcxRQM)

[AULA DE PROGRAMAÇÃO - Jogo das maças no Scratch. - YouTube ](https://www.youtube.com/watch?v=DRaKvVmsMFM)

[CRIANDO BOTÕES TOUCH NO SCRATCH - YouTube ](https://www.youtube.com/watch?v=nosj1m4llF8)

[Scratch - Imagine, Program, Share (mit.edu) ](https://scratch.mit.edu/)

[Romeu e Julieta - Loja Nova Fronteira - Nova Fronteira Editora de Livros ](https://www.novafronteira.com.br/produto/romeu-e-julieta-cpt.html)

[Quem É Homero E Ele É O Autor Da Ilíada E Da Odisséia? (enigmas-do-mundo.com) ](http://www.enigmas-do-mundo.com/homero.php)[William Shakespeare and Leonardo da Vinci by Ashley Griffith (prezi.com) ](https://prezi.com/hxwhjxgz3xbw/william-shakespeare-and-leonardo-da-vinci/)
12 
