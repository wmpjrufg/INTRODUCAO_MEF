As atividades habituais dos profissionais dos diversos ramos da engenharia geralmente os colocam diante de problemas técnicos que nem sempre possuem soluções simples. Para que seja possível resolver uma maior gama destes problemas de maneira satisfatória, a área da engenharia recorre a diversos métodos.

   No caso da engenharia civil, essa maneira satisfatória está associada à uma análise da estrutura de forma que esta não estará sujeita a falhas sob  as condições normais de seu uso.
    
   Para que seja possível desenvolver essa análise representando o comportamento mais aproximado ao real dessa estrutura em serviço, premissas baseadas em conceitos da teoria da resistência dos materiais baseados na rigidez de seus elementos, conceitos de estática e mecânica geral são utilizadas como subsídios para os cálculos da modelagem.
    
   É importante ressaltar que aliado aos conhecimentos dos métodos matemáticos empregados para essa análise, o engenheiro deve conhecer a natureza física a que o elemento analisado está submetido. Somente a partir desse conhecimento será possível produzir hipóteses sobre seu comportamento individual e como este afeta o comportamento geral da estrutura, conceito base do MEF.
    
   O modelo de cálculo nada mais é que a representação do objeto de análise de acordo com suas características geométricas e cargas atuantes, idealizando essa estrutura original de forma a roterizar seu esquema de cálculo.
    
   Para a modelagem desses sistemas, existem duas vertentes:
     
   - *Modelagem contínua*;
    
   - *Modelagem discreta*.
    
   Em termos práticos, modelar um problema real de forma contínua ou discreta são dois modos distintos de se chegar ao mesmo objetivo.
    
   Matematicamente, os modelos contínuos são representados por um número infinito de graus de liberdade*, porém suas soluções são  restritas a casos ou geometrias conhecidas, o que não se aplica a grande maioria dos problemas práticos.
    
   Já os *modelos discretos* são sistemas representados por um número finito de graus de liberdade, onde problemas contínuos são discretizados através da divisão da estrutura em partes distintas de comprimento finito mas conectadas entre si por pontos doniminados nós. Esse procedimento permite que um estrtura incialmente tida como complexa seja dividida em um conjunto de estruturas simples.
    
   *O que é grau de liberdade?*
    
   Grau de liberdade, em matemática, é o número de variáveis independentes que dispomos para descrever de forma completa um sistema [1], por exemplo em mecânica computacional graus de liberdade equivale as capacidades de movimento que uma estrutura poderá ter. Um pórtico plano possui 3 graus de liberdade por nó, ou seja, dois movimentos de translação e um movimento de rotação.
    
   Vale ressaltar que essa divisão deve ser feita de modo que o número de pontos escolhidos consiga representar de maneira satisfatória o comportamento do conjunto como um todo.
    
   A abordagem discreta amplamente utilizada em técnicas refinadas de engenharia não é nenhuma novidade da modernidade e sim um recurso utilizado desde a antiguidade para facilitar a solução de problemas complexos.
    
   Os egípcios já utilizavam aproximações numéricas para determinar a área de circunferências conforme descrito nos Papiros de Ahmes (também conhecido como Papiro de Rhind) [2]. Portanto é possível afirmar que técnicas de modelagem discreta possuem um vasto campo de aplicações. 
     
   *Imagem com exemplo de discretização? Slides 7 e 8*
    
   A análise de estruturas via processo discreto é um recurso extremamente importante para o desenvolvimento de projetos de engenharia. Nos cursos de graduação em Engenharia dois métodos discretos para análise de estruturas destacam-se, o Método das Forças e o Método dos Deslocamentos, sendo que o último deles é um recurso amplamente empregado em softwares desse tipo de análise.
    
   Esses métodos de análise de estruturas utilizam a superposição de efeitos para determinação do comportamento global de uma estrutura. No Método das Forças os casos básicos são soluções estaticamente determinadas (isostáticas) e no Método dos Deslocamentos são soluções cinematicamente determinadas (configurações deformadas conhecidas) [4].
    
   Apesar dos dois métodos serem de extrema importância para realização de análise de estruturas o Método dos Deslocamentos é o que ganha uma roupagem comercial e é largamente empregado nos softwares comerciais de projeto como SAP, TQS, EBERICK e outros. Tal situação deve-se ao fato que o Método das Forças admite inúmeras soluções estaticamente determinadas, portanto há modos diferentes de se estabelecer o sistema estrutural equivalente. Já no Método dos Deslocamentos existe um único sistema equivalente portanto do ponto de vista computacional isso representa uma vantagem no ato de se implementar a forma genérica e computacional do Método dos Deslocamentos.
   
   Em termos de análise estrutural a mesma poderá ser feita de duas formas:
    
   (a) Análise Linear;
    
   (b) Análise Não Linear.
    
   Nesse material estarão contidos os casos da análise linear por estes serem o ponto de partida do estudo.
   
   Como o próprio nome afirma a análise linear é formada por um conjunto finito de equações lineares que matricialmente podem ser escritas no modo *𝐴.𝑥=𝐵*.
    
   No âmbito da análise linear são admitidas as seguintes hipóteses:
   
   - Os deslocamentos da estrutura são relativamente pequenos em relações as dimensões da estrutura;
   
   - O material possui comportamento elástico respeitando a Lei de Hooke (σ=E.ε);
   
   - As condições de contorno permanecem inalteradas durante a análise.
    
   Soluções com formulação linear são aplicadas em diversos casos práticos de engenharia devido a sua condição levar a soluções aceitáveis na prática corrente de projetos. Porém, existem situações que necessitam de formulações não lineares para representar o comportamento de uma estrutura qualquer. São exemplos de análise não-linear:
   
   - Comportamento pós-crítico de pilares pré-moldados;
    
   - Análise de fadiga em um tabuleiro de ponte submetida a carga de natureza móvel;
    
   - Estruturas de concreto ou de aço com partes danificadas;
   
   - Determinação da flecha em estruturas de CRFA considerando o panorama de fissurações;
   
   - Mudanças das condições de contorno em uma estrutura metálica devido a plastificação das ligações;

   - Efeitos de vibração na asa de uma avião;

   - Efeito do escoamento de um fluído na superfície de um veículo de corrida.
 
   Outras diversas situações podem ser exemplificadas. No entanto essas análises não-lineares podem-se dividir em alguns tipos específicos. São eles:

   - Análise Não-Linear Geométrica (NLG);
   
   - Análise Não-Linear de Contato (NLC);
    
   - Análise Não-Linear Física (NLF).
    
   Para casos onde fontes não lineares são admitidas no estudo do problema, faz–se necessário o uso de métodos numéricos para solução do sistema de equações. Tais procedimentos usam de procedimentos incrementais-iterativos como o controle de forças ou controle de deslocamentos. 
   
   Os gráficos a seguir apresentam a trajetória de equilíbrio para casos de controle de força e deslocamento para solução de problemas não lineares.
    
   *Mas afinal, o que é MEF?*
    
   A técnica de Elementos Finitos é uma ferramenta numérica bastante consagrada na área de ciências exatas. Tal procedimento foi inicialmente desenvolvido com intuito de solucionar equações diferenciais que representavam determinados fenômenos na indústria aeroespacial, especialmente os problemas que envolviam mecânica dos sólidos.
    
   A ideia básica dos Elementos Finitos é aproximar a resposta de uma equação diferencial. Reddy [6] afirma que a técnica de elementos finitos é similar a técnica de diferenças finitas sendo que ela é mais robusta e pode ser utilizada de forma mais genérica.
   
   Tal método teve sua primeira apresentação a comunidade científica por volta dos anos 50 com o artigo: Stiffness and Deflection Analysis of Complex Structures [7]. Empresas como a Boeing, Rolls Royce e Ball Aerospace tiveram uma contribuição determinante no financiamento da criação dessa técnica.
    
   O funcionamento do método é baseado na discretização de um sistema contínuo conforme apresentado no exemplo a seguir:
   
    
   Em geral os fenômenos físicos na mecânica dos sólidos podem ser representados por Equações Diferenciais Parciais (EDP) sujeita a um conjunto de restrições adicionais. Essas restrições adicionais podem gerar um Problema de Valor Inicial (PVI) ou Problema de Valor de Contorno (PVC).
    
   Aqui nos Elementos Finitos aplicados a mecânica dos sólidos estaremos interessados nos Problemas de Valor de Contorno visto que esses são amplamente difundidos nas grandes área de ciências exatas e tecnológicas. Dentro dessa linha de problemas estamos interessados nos problemas de potencial.
    
   *O que é potencial?*
    
   É uma quantidade a partir da qual um campo de forças conservativas poderia ser obtido. Portanto toda força conservativas tem um potencial associado.
    
   Portanto é comum em problemas mais complexos tomar o sentido de uma abordagem potencial, pois nesse modelo de abordagem eliminamos complicações adicionais como a delimitação das componentes vetoriais do campo de forças.
    



O exemplo de solução de uma aplicação simplificada de MEF pode ser consultado em: [link](https://nbviewer.jupyter.org/github/wmpjrufg/INTRODUCAO_MEF/blob/gh-pages/notebook2.ipynb)
