
# **m-Labs: Laboratórios de física em dispositivos móveis**

:material-cursor-default-click-outline: Clique no botão abaixo para alternar visualização:

<div class="tx-switch">
  <button data-md-color-scheme="default"><code>Visualização normal</code></button>
  <button data-md-color-scheme="slate"><code>Visualização contraste</code></button>
</div>

<script>
  var buttons = document.querySelectorAll("button[data-md-color-scheme]")
  buttons.forEach(function(button) {
    button.addEventListener("click", function() {
      var attr = this.getAttribute("data-md-color-scheme")
      document.body.setAttribute("data-md-color-scheme", attr)
      var name = document.querySelector("#__code_0 code span:nth-child(7)")
      name.textContent = attr
    })
  })
</script>



<style>

body {text-align: justify}

div.a {
  text-indent: 50px;
}

p.recuo {
  padding-left: 130px;
  font-size: small;
  text-align: justify;
}

p.combinado:first-letter { 
	color: #F5843A; 
	font-size:xx-large; 
}
.info {
  background-color: #e7f3fe;
  border-left: 6px solid #2196F3;
}
.success {
  background-color: #ddffdd;
  border-left: 6px solid #4CAF50;
}

.danger {
  background-color: #ffdddd;
  border-left: 6px solid #f44336;
}

.block {
  display: block;
  width: 100%;
  border: none;
  background-color: #4CAF50;
  color: white;
  padding: 14px 28px;
  font-size: 16px;
  cursor: pointer;
  text-align: center;
}

.block:hover {
  background-color: #ddd;
  color: black;
}
</style>
<link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.2/css/all.css" integrity="sha384-oS3vJWv+0UjzBfQzYUhtDYW+Pj2yciDJxpsK1OYPAYjqT085Qq/1cq5FLXAZQ7Ay" crossorigin="anonymous">

![Legenda](../imagens/capitulo.png)




<div style="text-align: right"> 
<p><em>Leandro Sodre Barreto</em></p>
<p><em>Genilson Ribeiro de Melo</em></p> 
<p><em>Ariston de Lima Cardoso</em></p> 
 </div>

A área de ensino de ciências e engenharias tem ampliado suas
preocupações com a relação ensino aprendizagem em seus espaços de sala
de aula nos últimos tempos, especialmente com expansão dos recursos
tecnológicos e computacionais que se desenvolvem em toda a sociedade
contemporânea. O avanço imprimido por estes recursos mudam, alteram e
influenciam diretamente no nosso modo de vida, principalmente na
educação, com sua complexa relação de ensinar e aprender [1] e
[2]. Contudo, esta sociedade, imersa em um grande volume de
informação, muitas vezes não consegue produzir conhecimento, que
consequentemente não produz aprendizagem. Assim, a constante interação
de pessoas com computadores, dispositivos móveis e laboratórios
experimentais de ciências acoplados a computadores, estão cada vez mais
presentes ao indivíduo que possui uma realidade de mobilidade, que
quando superam a barreira da informação e do conhecimento, podem
construir uma aprendizagem significativa, classificando muitas vezes em
uma aprendizagem significativa [3], que poderão a partir de novas
metodologias de uso e aprendizagens móveis dentro dos conceitos da
aprendizagem móvel (m-learning) e ubíqua (u-learning) tornarem
ferramentas essenciais para o futuro dos laboratórios experimentais das
ciências e engenharias, que constitui-se em um dos principais entraves
na oferta de cursos públicos do ensino superior na modalidade a
distância do Brasil.

O Sistema da Universidade Aberta do Brasil (UAB), atualmente com 103
Instituições de Ensino Superior aderidas, possui em sua proposta
pedagógica a estrutura de polos de apoio presencial como local onde são
realizados encontros e avaliações presenciais (obrigatoriedade da
legislação brasileira) e aulas experimentais em alguns cursos. Dada as
dimensões continentais do país e analisando criticamente o atual modelo
de aulas experimentais nos cursos presenciais de ciências e engenharias,
faz-se necessário a reflexão: os laboratórios experimentais conseguem
produzir aprendizagem significativa aos discentes? Como reproduzir este
modelo pedagógico nos diferentes e distantes pólos de apoio presencial
do sistema UAB? Estas questões, vitais na formação de cientistas e
engenheiros, unidas às imensas possibilidades dos tablets e smartphones,
com seus sensores diversos embarcados e de outros que podem ser
integrados a estes dispositivos, permitem uma ampliação do espaço e do
tempo da aprendizagem no contexto do mobile learning (m-learning) e
ubíqua learning (u-learning). Estes sensores possibilitarão ricas
estratégias de aprendizagens experimentais ativas, interativas,
colaborativas e o seu uso adequado poderá promover à aprendizagem
significativa e mudanças necessárias a experimentação no contexto
educacional atual.

Neste trabalho, apresentamos um aplicativo voltado ao entendimento das
medidas de força através da construção de um circuito integrado com um
transdutor que mede indiretamente tensões, definido como célula de
carga. Este por sua vez é acoplado aos dispositivos móveis,
possibilitando ao experimentador realizar medidas de tensões, forças,
empuxos, flambagens e quaisquer grandezas relacionadas à segunda lei de
Newton nos principais meios materiais. Este aplicativo faz parte de um
projeto maior do Grupo de Tecnologias Educacionais, Robótica e Física
(G-TERF) da Universidade Federal do Recôncavo da Bahia, definido como
laboratórios de bolso, que visa introduzir diversos sensores internos e
externos (integrados aos tablets e smartphones) para medidas
experimentais nas ciências e engenharias, que será constantemente
atualizado após desenvolvimentos e novas proposições no Google Play.
Estes laboratórios de bolso são pensados dentro de uma proposta
pedagógica que engloba a fundamentação teórica, a produção de roteiros
de medidas experimentais para iniciar e motivar o estudante na
realização de medidas, jogos interativos, vídeo de utilização no
processo de medida. E, são elencadas futuras medidas que o
experimentador pode fazer em qualquer lugar ou contexto que esteja
inserido. Apresentaremos algumas medidas experimentais realizadas com o
protótipo, seus desvios, erros e gráficos dos principais resultados.

## Aprendizagem Significativa, m-learning e u-learning 


As experimentações no campo das ciências exatas e tecnológicas devem
englobar os meios multimídias e a interatividade, presentes nas
tecnologias móveis, no contexto social dos discentes e sociedade,
ensejando sempre uma Aprendizagem Significativa (AS), construindo pontes
dimensionais geográficas e motivacionais. Este conceito de AS está
baseada na Psicologia Cognitiva de Ausubel [3], o qual estabelece
que aprendizagem ocorra por assimilação de novos conceitos e proposições
na estrutura cognitiva do aprendiz. Assim, novos conceitos e ideias são
aprendidos, quando o conhecimento prévio do sujeito e as novas
informações formam pontos de estabilidade na sua estrutura cognitiva. De
maneira contrária, existe a Aprendizagem Mecânica (AM) que corresponde à
aprendizagem de novas informações com pouco ou nenhuma associação a
conceitos da estrutura cognitiva, ocorrendo de forma aleatória. Como
exemplo da AM, podemos observar o atual modelo de experimentação dos
cursos de ciências físicas e engenharias, geralmente iniciados com um
roteiro prévio que descreve o procedimento experimental, em que os
estudantes o repetem de maneira mecânica, obtendo os valores e aferindo
as grandezas, muitas vezes sem nenhuma transposição ao conceito físico
observado, não se tornando co-autor do fenômeno experimental
reproduzido. Este fato deve-se muitas vezes a falta de compreensão
fenomenológica, pois a pouca interatividade, baixo estímulo a reflexão e
senso crítico, no momento da aula experimental, não produzem a liberdade
de medir objetos, forças e grandezas de maneira livre, vivendo novas
experiências no processo experimental, vital para a construção de uma
aprendizagem significativa.

A aprendizagem móvel, definida como mobile learning (m-learning), em
fase de iniciação nos espaços acadêmicos, com uma grande gama de
conceitos imbuídos, na definição de Attewell (2005)[4] indicam que a
aprendizagem móvel permite uma aprendizagem personalizada, em qualquer
hora e lugar. Assim, conectados à grande rede, os usuários não
necessitam de um espaço fixo ou formal de aprendizagem [5] e
[6], apenas conectado, de maneira síncrona ou assíncrona as pessoas
recebem comunicações e informações instantâneas, que são processadas em
curtos intervalos de tempo, cada vez mais otimizados, gerando múltiplos
contextos entre as pessoas e seus dispositivos móveis, amplamente
interativos e pessoais, possibilitando aprendizagens extremamente ricas
e complexas, ou simplesmente descarte.

Para a UNESCO a integração do celular à educação tem o potencial de
romper paradigmas pedagógicos tradicionais [7]. Os telefones móveis
são diferentes das ferramentas tradicionais de educação, como livro, giz
e lápis, porque permitem acesso simultâneo, tem espaço de armazenamento
de dados, são informativos e compartilham o conhecimento entre
indivíduos e grupos independentemente de tempo e da localização física.
Por estas razões, aquele órgão está interessado no seu potencial para
apoiar o ensino, aprendizagem e assim melhorar a educação com um todo.

## Tablets e Smartphones como ferramentas de laboratórios

A experimentação nas aulas das ciências físicas e tecnológicas é vital
ao entendimento da fenomenologia. O discente, através do empirismo
consegue expandir suas aptidões e capacidade de inovar em outros
aparatos, produtos, materiais e análises de construtos científicos e
tecnológicos. Todavia, as aulas dos laboratórios de ciência e
tecnologia, geralmente o tempo em que os estudantes estão interagindo
com o aparato experimental, normalmente ele gasta mais da metade do
tempo na montagem e construção dos passos para realização da medição
[8], não permitindo uma maior utilização deste para o esgotamento
das hipóteses de possibilidades e da exploração de outras metodologias
e/ou medidas que podem ser obtidas e construídas.


Como ferramenta de auxílio aos entraves dos laboratórios didáticos
experimentais, introduziu-se o uso de computadores no ensino de ciências
e tecnologias. Nestes, a tomada de apresentação dos dados, tornaram-se
muito rápidas, reduzindo o tempo de montagem e aumentando
significativamente a aprendizagem e o desenvolvimento cognitivo das
aulas experimentais. O uso de computadores, geralmente laptops, requer
que interfaces e sensores de alta complexidade sejam introduzidos
[9], além da instalação de softwares especializados para captação
dos valores experimentais que estão distante da realidade dos pólos de
apoio presenciais do sistema da Universidade Aberta do Brasil. Pois, os
cursos da área de ciência e tecnologia, geralmente possuem uma média
superior a trezentos estudantes distribuídos em regiões afastadas
geograficamente uma das outras, o que inviabiliza estas aulas
experimentais na sede das universidades, bem como torna complexo o envio
destes materiais aos pólos, mesmo sabendo que a solução encontrada por
algumas universidades foi a montagem de veículos itinerantes que visitam
os pólos e realizam os procedimentos experimentais. Em ambos os casos, o
contato dos estudantes com os aparatos experimentais ocorre de maneira
pontual e por muito tempo não reincidente, necessitando assim, de
ferramentas mais próximas de suas utilizações e que estejam no seu
convívio para realização de experimentos na hora e desejo de
aprendizagem.

Os tablets e smartphones resolvem tanto o problema da mobilidade, da
praticidade e do encurtamento das distâncias geográficas. A alta
portabilidade é característica desses aparelhos, além disso estes
computadores portáteis, com processadores altamente eficientes,
manuseios interativos, geometrias ergonômicas e de grande acesso à
sociedade, dada a expansão de fabricantes e seu baixo custo de
aquisição, tornam-se ferramentas ainda mais poderosas, quando são
conhecidos seus sensores internos que empoderam enormemente os
experimentadores de ciência e tecnologia. A exemplo, podemos citar mais
de dez sensores altamente complexos e caros de introduzir em
computadores laptops que existem nos tablets e smartphones que realizam
medidas físicas, como: acelerômetro, magnetômetro, câmeras de alta
resolução, microfones, giroscópios, luxímetros, sensores de proximidade
e outros que podemos acoplar através das entradas físicas e digitais
(wi-fi, e bluetooth). A utilidade dos tablets e smartphones para o
ensino de ciências e de tecnologia vem sendo gradativamente reconhecido,
existem diversos relatos descrevendo atividades práticas bem sucedidas
com esses aparelhos [9-19]. Porém, muito precisa ser investigado a
transformar estes equipamentos em laboratórios de bolso completos e
capazes de medir fenômenos experimentais em qualquer lugar e momento em
que o experimentador necessite e que seja capaz de transformar sua
realidade. Neste sentido, este trabalho contribui com seu primeiro
estudo de outros que estão sendo elaborados com temas, sensores e
medidas diferentes.

## Metodologia pocket labs

Neste trabalho, foi proposta a realização do estudo da mecânica dos
fluidos, especificamente, medir o empuxo aplicado a um corpo imerso
parcial ou totalmente em água. O princípio de Arquimedes estabelece que,
para um corpo imerso em um fluido, existe a atuação de uma força
ascendente, denominado empuxo. Em um laboratório tradicional de
ciências, a medida do empuxo é realizada através de instrumentos
analógicos. O instrumento utilizado para medir forças é o dinamômetro.
Uma das montagens possíveis é ilustrado na próxima página.


O empuxo é obtido a partir da análise das forças que atuam no corpo em
equilíbrio. O primeiro procedimento consiste em medir o peso do objeto.
Para isto, procedemos de acordo com a Figura 1a, analisando as forças
que atuam no corpo quando ainda não está submerso em água de acordo com
a Figura 2.  

<center>
  <p><small>Figura 1:  Aparato para aferir empuxo, neste molas são calibradas através
		de pontos de equilíbrio e a partir desta origem são adicionados objetos
		com pesos para observar a elongação de molas(1a), quando adicionados a
		meios fluidos, no caso a água, nota-se uma redução na elongação da mola
		devido ao fenômeno físico do empuxo, que por sua vez pode ser aferido
		através da densidade do fluido introduzido. </small></p><br>
    <img src="../imagens/image_37_38.png" style="width: 70%; height: auto;"/>
  </small>
</center>




<center>
  <p><small>Figura 2:  Diagrama de análise de forças em corpos com dinamômetros e
		objetos massivos fixados nas pontas (2a), quando submersos em meios
		fluidos surge uma força de oposição à força que atrai os objetos ao chão
		(2b). </small></p><br>
    <img src="../imagens/image_39_40.png" style="width: 70%; height: auto;"/>
  </small>
</center>

Utilizando a segunda lei de Newton teremos que

$$F_{R} = F - P = 0$$

\noindent
onde \emph{F} é a leitura no dinamômetro. Obtemos então o peso, $P=F$.

O segundo passo é realizar a imersão, analisar as forças atuantes e
empregar novamente a segunda lei de Newton. De acordo com a Figura 2b,
temos

$$F_{R} = F' + E - P = 0 $$ 

\noindent
o que dá $E= F'-P$.

A nossa proposta utiliza os smartphones e tablets para conduzir o
processo de medida de modo que o estudante tenha muitos instrumentos de
medida em um único dispositivo. Isto tornaria a experimentação um
processo dinâmico e passível de realização não só na sala de aula.

Sabemos que em um laboratório de física é imperativo um instrumento que
seja capaz de medir forças e apesar da maioria dos aparelhos possuírem
um acelerômetro integrado, a medida de uma força aplicada no aparelho
nem sempre é possível, já que em uma situação de equilíbrio não temos
aceleração. Ainda que fosse possível a medida em forças num sistema em
equilíbrio, encontra-se outra dificuldade em realizar a medida do empuxo
aplicado no corpo. Isso ocorreria pelo fato de que a maioria dos tablets
e smartphones não podem ser submetidos à imersão. Assim a realização
dessa medida, por imersão, seria inviável. Desta forma, é necessária a
construção de um dispositivo que seja capaz de realizar a medida de
força, como um dinamômetro. Como a nossa proposta é a construção de um
laboratório a partir de um telefone celular, logo precisamos de um
dispositivo digital para fazer a leitura das forças aplicadas e
transmiti-las ao dispositivo mobile através de um dos seus sensores
embarcados.

Outro ponto a ser desenvolvido foi uma interface para o usuário. Esta
interface assume a forma de um aplicativo e deve ser capaz de orientar o
usuário através de um processo de medida padrão para que o usuário
entenda os princípios de funcionamento do dispositivo para depois
realizar a medida desejada. Deve também contemplar também uma
fundamentação teórica que seja capaz de instruir de maneira simples e
objetiva o usuário. Outra característica do aplicativo é permitir a
experimentação livre e desapegada do ambiente de sala de aula, o que
potencializa o aprendizado nas situações cotidianas. Dessa forma, o
projeto Pocket Labs para a medida de empuxo tem a estrutura sugerida na
Figura 3.

<center>
  <p><small>Figura 3:   A célula de carga é acoplada via dispositivo microcontrolador
		que comunica-se com o tablet ou smartphone com sua interface construída
		para melhor interface com o usuário, após penduradas as massas e o meio
		fluido desejado pelo experimentador. </small></p><br>
    <img src="../imagens/image45.jpg" style="width: 70%; height: auto;"/>
  </small>
</center>

A ferramenta utilizada para desenvolvimento do aplicativo foi uma
plataforma de desenvolvimento online, MIT app inventor. Esta plataforma
disponibiliza a elaboração de um aplicativo com as telas formadas a
partir de imagens e a programação na forma de diagrama de blocos, o que
torna a programação descomplicada e dinâmica. A montagem das telas segue
a estrutura mostrada na Figura 3.

## Aplicativo Pocket Labs

O aplicativo construído para ampliar a interface dos discentes dos
cursos de ciência e tecnologia, denominado Pocket Labs pode ser obtido
gratuitamente no Google Play. Neste, o usuário encontra uma tela de
apresentação, e a partir de sua escolha direciona-o para o campo
experimental proposto, neste caso Empuxo. Após esta etapa, o
experimentador encontra um vídeo com um apresentador virtual que indica
quais são os principais botões e sua utilização inicial, os botões são
cinco: (a) conceitos teóricos, (b) vídeo zero, (c) conectar, (d) medir e
(e) análises; (a) na ordem, o primeiro está associado a fundamentação
teórica, caso o experimentador não tenha obtido contato com o processo
de medida que ora está por iniciar; (b) vídeo zero consiste em
introduzir um pequeno vídeo em que carrega as potencialidades do
experimento e como fazer o processo de medida zero; (c) conectar está
associado ao acoplamento e pareamento do circuito de medida com o
smartphone ou tablet, notando claro que o módulo bluetooth deste
equipamento deverá estar ligado; (d) o processo de medição levantará uma
série de dados, que podem ser exportados ou analisados no próprio
equipamento, para isso introduziu-se um botão de análises (e), que
realiza as análises gráficas através de pacotes específicos da
GoogleLabs, podendo ser alterados ou levados para outras plataformas
para outras interpretações.

## Considerações finais

Neste artigo, consideramos os benefícios e possibilidades de
experimentação nas ciências físicas e tecnológicas utilizando tablets e
smartphones dentro das teorias de aprendizagem m-learning e u-learning.
A experimentação tem papel vital no processo de ensino aprendizagem das
ciências, sendo que sua importância transcende a repetição de práticas
experimentais ou de aprendizagens mecânicas. Sobretudo, em laboratórios
que os estudantes gastam maior parte do tempo na montagem e na
reprodução de procedimentos experimentais, sem muita reflexão e
possibilidade ampla de utilização, caracterizando em um empirismo
ingênuo e pontual. Assim, a transposição didática entre os conceitos e
as medidas reais, objetivo principal dos experimentos nas ciências e
tecnologias, centrados na coleta de dados, na interface e praticidade de
utilização de equipamentos de medidas e na portabilidade destes
instrumentos é caracterizado na construção do aplicativo Pocket Labs.

Com os Pocket Labs, vimos que é possível desenvolver experimentos
didáticos e de aprendizagem livre na área da mecânica dos fluidos,
especialmente nos conceitos hidrostáticos de empuxo. A versatilidade dos
smartphones e do tablet unidos a circuitos simples e de fácil
manipulação abre muitas portas aos estudantes, que de posse dos seus
aparelhos pessoais podem realizar medidas, coletas e análises em
quaisquer espaços de aprendizagem e disseminar junto aos seus pares
metodologias adotadas e medidas realizadas.

A utilização de aplicativos e células de interface potencializa os
objetos virtuais de aprendizagem nas aulas experimentais dos diversos
cursos de educação, em particular educação a distância da Universidade
Aberta do Brasil. Em posse de um conjunto de experimentos desta
natureza, poderão integrar e co-participar como construtores de diversas
metodologias e aplicações dos Pocket Labs em seus contextos de cursos,
podendo ser da física, matemática, química, biologia e das engenharias,
ou de qualquer demanda de formação nestas áreas científicas. Contudo,
tão importante quanto a construção, a segunda etapa que está por vir, é
a adequação deste aplicativo e de outros objetos. também serão as
escolhas dos ambientes a serem utilizados e a forma de apoio dada aos
estudantes que serão iniciados a esta utilização.

A expansão de outros aplicativos dentro do Pocket Labs é fundamental
para avançarmos neste contexto de ensino experimental através do
m-learning, saindo dos laboratórios de repetição sem muito tempo para a
interpretação e reflexão de dados para situações complexas e ricas, em
que o estudante estará construindo suas situações problemas e junto aos
seus dispositivos móveis buscar traçar qual conclusão, quais desafios a
serem pensados e os erros cometidos. Assim, os Pocket Labs estarão
alcançando seu clímax maior de propor uma aprendizagem significativa aos
seus usuários.

## Referências 

[1] Castells, M. A. (2009) sociedade em rede. São Paulo: Paz e Terra,
	1999. KADIRIRE, J. Mobile learning demystified. In: GUY, R. The
	evolution of mobile teaching and learning. Santa Rosa: Informing
	Science Press, v. 1. p. 103-118.

[2] Maturana, H. (1993). Uma nova concepção de aprendizagem. Dois Pontos,
	v. 2, n. 15, p. 28-35.

[3] Ronca, A.C.C. (1980) O modelo de ensino de David Ausubel. In:
	Penteado, W.M. A. (Org.) Psicologia e ensino. São Paulo: Papelivros,
	1980.p.59-83.

[4] Attewell, J.(2005). J. From research and development to mobile
	learning: tools for education and training providers and their
	learners. Disponible
	in: [http://www.mlearn.org.za/CD/papers/Attewell.pdf](http://www.mlearn.org.za/CD/papers/Attewell.pdf).
	Acess in 12 may 2015.

[5] Freysen, J. (2004) M-Learning: an educational perspective. Moblie
	Learing any time everywhere. Org. Atewell, J. E Savill-Smith, C.
	Mlearn2004. London, UK., 232p, 2004.

[6] David Paul Ausubel. Disponible in: [http://davidausubel.org](http://davidausubel.org).
	Acess in 12 may 2015.

[7]  Dias, E.J., Araujo JR., C.F. (2012) Mobile learning no ensino de
matemática: um _framework_ conceitual para uso dos _tablets_
na educação básica. Anais do Encontro de Produção Discente
PUCSP/Cruzeiro do Sul. São Paulo. P.1-13.
	
[8]  Laburu, C.E. (2006).Fundamentos para um experimento cativante. Caderno
	Brasileiro de Ensino de Física, v.23, n.3: p. 382-404.

[9]  Mishra, P., Koehler, M. J. (2006).Technological pedagogical content
	knowledge: a framework for teacher knowledge. Teachers College Record,
	108(6), 1017--1054. OLT2006_paper.pdf.
	
[10]  Sharma, S., Kitchens, F.(2004). Web services architecture for
	m-learning. Electronic Journal of e-Learning (2), 203--216.
	
[11]  J. Kuhn and P. Vogt, Difraction experiments with infrared remote
	con-trols, The Physics Teacher, v. 50, n. 2, p. 118-119, 2012.

[12]  P. Vogt, J. Kuhn, Analyzing free fall with a smartphone acceleration
	sensor, The Physics Teacher, v. 50, n. 3, p. 182-183, 2012.

[13] K. Forinash, R. F. Wisman, Smartphones as portable oscilloscopes for
	physics labs, The Physics Teacher, v. 50, n. 4, p. 242-243, 2012.
	
[14] P. Vogt, J. Kuhn, Determining the speed of sound with stereo
	headpho-nes, The Physics Teacher, v. 50, n. 5, p. 308-309, 2012.
	
[15] N. Silva, Magnetic eld sensor, The Physics Teacher, v. 50, n. 6, p.
	372,2012.

[16] P. Vogt, J. Kuhn, Analyzing simple pendulum phenomena with a
	smartphone acceleration sensor, The Physics Teacher, v. 50, n. 7, p.
	439-440, 2012.
	
[17] Leonardo P. Vieira, Vitor O. M. Lara, Macrofotograa com um tablet:
	aplicações ao ensino de ciências, Revista Brasileira de Ensino de
	Física, v. 35, n. 3, art. 3503, 2013.

[18] Leonardo P. Vieira, Vitor O. M. Lara, Física em tablets: a segunda lei
	de Newton, Anais do XX Simpósio Nacional de Ensino de Física, 2013,
	São Paulo.

[19] Leonardo P. Vieira, Vitor O. M. Lara, (2013). Física em tablets:
	obtendo fo-tograas macro com a técnica da gota d'água, Anais do XX
	Simpósio Nacional de Ensino de Física, 2013, São Paulo.

[20] Alexandre C. Azevedo, Leonardo P. Vieira, Carlos E. Aguiar, Antonio
	Carlos F. Santos, (2013).Experimentos de ótica com laser para alunos
	com deciência visual, Anais do XX Simpósio Nacional de Ensino de
	Física, São Paulo.

