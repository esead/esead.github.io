
# **Aplicativo Quick voice: uma ferramenta de acessibilidade para deficientes visuais**

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
</style>
<link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.2/css/all.css" integrity="sha384-oS3vJWv+0UjzBfQzYUhtDYW+Pj2yciDJxpsK1OYPAYjqT085Qq/1cq5FLXAZQ7Ay" crossorigin="anonymous">

![Legenda](../imagens/capitulo.png)

<div style="text-align: right"> 
    <p><em>Adilson Gomes dos Santos</em></p> 
    <p><em>Ariston de Lima Cardoso</em></p> 
    <p><em>Eniel do Espírito Santo</em></p> 
 </div>

A condição humana, na perspectiva de Hannah Arendt, está para além do
conceito de natureza humana, neste sentido as ciências humanas envolvem
a tecnologia e a educação para atender as necessidades do ser humano
como um todo em uma ''sociedade em rede'' [1], [2].

Dessa forma, a inclusão se apresenta como um estruturante da sociedade
contemporânea, um direito de acesso. Conforme o Relatório Mundial sobre
a Pessoa com Deficiência [3], pessoas com deficiência apresentam
taxas mais baixas de uso de tecnologias digitais da informação e
comunicação (tecnologia móvel: telefones celulares, smartphones,
tablets, notebooks) em relação às pessoas sem deficiência, apesar do
avançado desenvolvimento das tecnologias à acessibilidade com uma
interação segura e eficiente, ainda que limitada em um produto com
desenho universal.

O potencial dos dispositivos móveis e sem fio de oferecer informação em
qualquer tempo e espaço, abre um leque de possibilidades para a
aprendizagem, e o mobile learning _(m-learning)_
apresenta-se como um importante ambiente de aprendizagem.

A partir do cenário apresentado, o Grupo de Tecnologia, Engenharia,
Robótica e Física (G-TERF) e o Grupo de Estudos sobre Educação
Diversidade e Inclusão (GEEDI) da Universidade Federal do Recôncavo da
Bahia (UFRB) idealizou o projeto de pesquisa com o desafio de construir
um aplicativo para converter código de barras bidimensional (QR Code) em
arquivo de texto, seja por escrito ou em áudio. Com o advento da
convergência de mídias para os dispositivos móveis, que possibilitou a
realização de tarefas de outros dispositivos (computadores, televisores,
etc), transformou uma grande parcela da população em usuários das
tecnologias móveis com novas possibilidades de aprendizagem apresentadas
pelas tecnológicas digitais.

A inclusão das pessoas com deficiência visual que, cada vez mais, passam
a utilizar os dispositivos móveis no seu cotidiano para ampliar sua
comunicação e acessar informações. O ''Quick Voice'', aplicativo de
tecnologia assistiva, promove à autonomia e independência de acesso à
informação para usuários como limitações visuais. Nesse processo de
inclusão, a utilização do App ''Quick Voice'' na mediação da
aprendizagem das pessoas com deficiência visual, na abordagem da
Tecnologia Educacional, apresenta potencialidades de utilização dos
dispositivos móveis, o mobile learning _(m-learning)_ como ambiente
de aprendizagem, cada vez mais presentes na forma de vida imposta pela
'sociedade em rede'.

Neste sentido, o conjunto de técnicas que promova à mediação da
aprendizagem utilizando meios tecnológicos, entendida como tecnologia
educacional, utiliza os recursos tecnológicos de acordo com o momento
histórico, contudo, a educação no sentido formal ainda resiste às
mudanças. Assim, o desenvolvimento tecnológico aumentou a complexidade,
todavia as potencialidades de uso ainda não estão exploradas na sua
totalidade.

Segundo Vygotsky [4], a aprendizagem é um processo
sociointeracionista, o aprendiz constrói conhecimentos da mesma forma
que internaliza padrões de comportamento, que o transforma ao mesmo
tempo em que está a transformar o objeto. Desta forma, o ''Quick Voice''
oportuniza a inclusão, respeitando as individualidades com a utilização
dos dispositivos móveis pelos deficientes visuais.

Este trabalho propõe o desenvolvimento de um aplicativo para
dispositivos móveis capaz de converter código de barras bidimensional
(QR Code) em arquivo de texto, seja por escrito ou em áudio, com o
objetivo de facilitar o acesso das pessoas deficiência visual ao
conteúdo do código, que pode ser ouvido em qualquer lugar, respeitando
os princípios de acessibilidade e de usabilidade. Aborda a inclusão das
pessoas com deficiência visual no processo de aprendizagem a partir do
entendimento que inclusão só se efetiva com a mudança de comportamento
da sociedade. O ''Quick Voice'' está disponível online, sem custo, no
Google Play.

## Tecnologias Assistivas

A Tecnologia Assistiva (TA) tem avançado constantemente, devido a
demanda advinda do processo de inclusão sócio-educa-
cional de pessoas com
deficiência. Segundo o Comitê de Ajudas Técnicas da Coordenadoria
Nacional para Integração da Pessoa Portadora de Deficiência (Corde), a
Tecnologia Assistiva

> (...) é uma área do conhecimento, de característica interdisciplinar,
que engloba produtos, recursos, metodologias, estratégias, práticas e
serviços que objetivam promover a funcionalidade, relacionada à
atividade e participação, de pessoas com deficiência, incapacidades ou
mobilidade reduzida, visando sua autonomia, independência, qualidade de
vida e inclusão social [5].

Compreende-se dessa forma, que a Tecnologia Assistiva engloba recursos e
serviços que objetivam favorecer autonomia no desenvolvimento de ações
em áreas diversas, como: educação, trabalho, mobilidade, lazer,
comunicação, dentre outras fundamentais para a garantia da qualidade de
vida e inclusão em variados ambientes sociais, facilitando a vida dos
usuários em relação ao desenvolvimento da rotina diária, da comunicação,
da locomoção, da aprendizagem, assim como do uso do computador.

Têm sido adotadas referências com diferentes apresentações de aplicação
e focos de organização, para a classificação da Tecnologia Assistiva,
tais como: ISO 9999; Classificação Horizontal EuropeanActivities in
Rehabilitation Technology -- HEART; e Classificação Nacional de
Tecnologia Assistiva, do Instituto Nacional de Pesquisas em Deficiência
e Reabilitação, dos Programas da Secretaria de Educação Especial,
Departamento de Educação dos Estados Unidos [6].

No processo de classificação de Tecnologia Assistiva, são consideradas
algumas categorias, as quais podem ser: Auxílios de mobilidade; Auxílios
para a vida diária e vida prática; Comunicação Aumentativa e
Alternativa; Recursos de acessibilidade ao computador; Auxílios para
cegos ou para pessoas com visão subnormal; Auxílios para pessoas com
surdez ou com déficit auditivo; Adaptações em veículos [7].

A TA pode ser de baixo ou alto custo. Mendes & Lourenço (8) destacam
que na literatura os diferentes tipos de TA são classificados em três
categorias, sendo estas:

> a) recursos de baixa-tecnologia: recursos simples, não elétricos, cuja
vantagem seria o baixo custo e que requerem menos treinamento para uso;
b) recursos de média-tecnologia: geralmente elétricos, porém sem um
sistema computacional; e c) recursos de alta-tecnolo-
gia: que geralmente requerem sistemas computadorizados, operados através de programas de
softwares especiais, que são mais complexos e às vezes multifuncionais e
requerem treino para uso (p. 425).

Galvão Filho (9), ao exemplificar recursos de TA de baixo custo
demonstra que muitos podem ser feitos artesanalmente, tais como:

> (...) suportes para visualização de textos ou livros (foto abaixo);
fixação do papel ou caderno na mesa com fitas adesivas; engrossadores de
lápis ou caneta confeccionados com esponjas enroladas e amarradas, ou
com punho de bicicleta ou tubos de PVC ''recheados'' com epóxi;
substituição da mesa por pranchas de madeira ou acrílico fixadas na
cadeira de rodas; órteses diversas, e inúmeras outras possibilidades
(p.208).

Os recursos de Tecnologia Assistiva podem assim proporcionar novas
possibilidades para a participação das pessoas com deficiência nos
espaços sociais, e ainda potencializar as já existentes. Ressalta-se
ainda, a possibilidade de utilização das TIC como recursos de Tecnologia
Assistiva, tornando possível ou facilitando o uso de equipamentos e o
desenvolvimento de atividades por pessoas com deficiência. Segundo
Galvão Filho (9),

> (...) as TIC podem ser utilizadas ou como Tecnologia Assistiva, ou por
meio de Tecnologia Assistiva. Utiliza-se as TIC como Tecnologia
Assistiva quando o próprio computador é a ajuda técnica para atingir um
determinado objetivo. Por exemplo, o computador utilizado como caderno
eletrônico, para o indivíduo que não consegue escrever no caderno comum
de papel. Por outro lado, as TIC são utilizadas por meio de Tecnologia
Assistiva, quando o objetivo final desejado é a utilização do próprio
computador, para o que são necessários determinadas ajudas técnicas que
permitam ou facilitem esta tarefa. Por exemplo, adaptações de teclado,
de mouse, software especiais etc (p.191).

Os softwares especiais de acessibilidade são programas especiais de computador que possibilitam ou
facilitam a interação da pessoa com deficiência com o programa. Através
dos softwares especiais de acessibilidade, diversas adaptações podem ser
realizadas para favorecer a acessibilidade ao usuário. São exemplos de
softwares especiais de acessibilidade: softwares leitores de textos;
leitores de tela; simuladores de teclado e mouse; sistemas
computacionais de comunicação alternativa, entre outros.

A utilização de softwares de acessibilidade, possibilita o atendimento
às necessidades do usuário, facilitando o seu acesso e utilização ao
computador, e consequentemente às atividades desenvolvidas através deste
equipamento.

Além dos recursos de TA, destaca-se também os seus serviços sendo que
estes favorecem a inclusão da pessoa com deficiência mediante o
fornecimento de orientações para que ela possa utilizar equipamentos,
auxiliando assim a autonomia do sujeito. Também denominado Sistema de
Prestação de Serviços, o Serviço de Tecnologia Assistiva é conceituado
pela Eustat Consortium (10) como,

> (...) o conjunto de facilidades, procedimentos e processos que actuam
como intermediários entre estruturas do mercado de TA e os utilizadores
finais, de modo a facilitar o acesso das pessoas com deficiência a estas
tecnologias, através de ajuda financeira, competência profissional,
informação, formação etc (p. 17).

Assim, por meio da utilização dos recursos ou serviços de TA, a pessoa
com deficiência pode ter uma maior facilidade no uso de equipamentos,
assim como no desenvolvimento de ações que sem estes seriam mais
difíceis de realizar.

## Aprendizagem com Mobilidade (M-Learning, U-Learging)

O Brasil terminou o primeiro trimestre de 2015 com 283,4 milhões de
telefones celulares e densidade de 138,98 cel/100 hab segundo a empresa
de consultoria Teleco, sendo que desse total 75,48% são de assinantes
na modalidade pré-pago. Em relação aos assinantes móveis no mundo
inteiro, a consultoria MobiThinking apontou em maio de 2014 já existirem
quase 7 bilhões de assinaturas de telefones celulares, o que representa
um número de celulares equivalente 95,5% da população mundial. Sem
analisar a possibilidade de que algumas pessoas possam possuir mais de
uma assinatura, a verdade é que uma parcela significativa da população
hoje possui acesso a esses serviços, cenário promissor para a prática
educativa. Nesse contexto, o _m-learning_ se apresenta como uma
nova possibilidade de aprendizagem, como mediador no processo de
construção do conhecimento de forma ubíqua.

As possibilidades que os dispositivos móveis e sem fio apresentam no
processo de aprendizagem na modalidade educacional a distância apoiada
nos conceitos de aprendizagem móvel _(m-learning)_ e aprendizagem
ubíqua _(u-learning)_ na sociedade em rede, segundo Castells
[2], está estruturada nas tecnologias, que ressignificou a forma de
viver em sociedade. Nesse contexto, o desafio da educação na
contemporaneidade está no ressignificar os processos de ensino e de
aprendizagem influenciada pela ''tecnologização'' da sociedade que
modificou a forma de fazer educação, as relações sociais e o mundo do
trabalho, impondo a necessidade da aprendizagem permanente.

A tecnologia educacional, nesse cenário, busca novas possibilidades
educacionais para as práticas docentes, através das tecnologias móveis e
sem fio que ultrapassam as paredes dos espaços físicos das escolas.
Desta forma, a modalidade de ensino tanto presencial quanto as
distâncias começam aos poucos a modificar o paradigma educacional com a
aprendizagem mediada por redes de computadores
_(e-learning)_, a aprendizagem por dispositivos móveis sem
fio _(m-learning)_ e a aprendizagem ubíqua, que integra as
anteriores tornando-se ainda mais imersiva _(m-learning)_,
como alternativa para otimizar e administrar o tempo na sociedade em
rede. Entretanto, a fragilidade dessas modalidades está no processo de
ensinar e aprender, pois ter apenas o acesso aos dispositivos móveis e
consequentemente a informação não é suficiente, é preciso saber
utilizá-la na perspectiva metodológica da mediação pedagógica do ensino
e aprendizagem.

Nos dispositivos móveis e sem fio, a informação está acessível em
qualquer tempo e espaço, oferecendo maior autonomia ao aprendiz. Mas,
ter acesso à informação não significa, necessariamente, acesso a um
processo de aprendizagem, ou seja, às possibilidades de passar de um
conhecimento pouco organizado para um mais organizado. Nesse sentido,
quando a mediação pedagógica consegue intervir na ZDP são estimulados
processos internos ainda não amadurecidos nos aprendizes, tornando-se um
instrumento significativo para a orientação da forma de trabalhar
educação [4].

As implicações desse conceito no processo de ensinar e aprender tem
importante relevância nas pesquisas sobre a aprendizagem escolar. Nessa
perspectiva, ressaltam-se as ligações existentes entre fala e
pensamento, entre sentido e significado. No processo de aprendizagem, os
mecanismos mentais do aprendiz, presentes na relação com o objeto exerce
uma atividade mediada por instrumentos e signos, ocorrendo o processo de
internalização a partir da mediação externa com o objeto em interação
[4].

Essas observações demonstram que a utilização do aplicativo para
dispositivos móveis, ''Quick Voice'', com o conceito da ZDP tem o
caráter social de inclusão dos deficientes visuais no processo de
aprendizagem formal e não-formal, considerando-se as mediações
histórico-culturais possíveis nesse cenário. Par-
tindo-se do pressuposto
que o aprendiz é capaz de construir mais com o auxílio de um mediador do
que faria sozinho, o desenvolvimento do aplicativo foi orientado para
exploração da ZDP, por meio da qual são desenvolvidas as capacidades e
habilidades potenciais. E, a partir do momento, que são internalizadas,
passam a fazer parte das conquistas independentes da pessoa com
deficiência visual. Vale ressaltar, que em todo o processo de
desenvolvimento, não se perdeu a atenção para a complexidade do processo
de aprendizagem pelo deficiente visual, que não é estritamente homogênea
e harmoniosa [4].

## Quick Voice: Construção e Aplicações

O acelerado desenvolvimento dos dispositivos móveis e sem fio abre novos
caminhos para a inclusão da pessoa com deficiência. Esta realidade tem
estimulado novas pesquisas com as tecnologias móveis que apontam para
novas concepções e possibilidades pedagógicas que surgem na sociedade
contemporânea. A Organização Mundial de Saúde (OMS) estima que 10% da
população global são de pessoas com deficiência, mais de 700 milhões de
pessoas. No Brasil, de acordo com o Censo 2000 (IBGE), 24,6 milhões de
pessoas têm algum tipo de deficiência. Esses dados demonstram o grande
do desafio a ser enfrentado na construção de uma sociedade inclusiva,
que respeite às diferenças e garanta o acesso universal aos direitos
[5].

Apesar do inegável avanço e inovação dos dispositivos móveis sem fio com
a crescente convergência de mídias, que transformou a forma de comunicar
e empoderar o usuário para interagir, participar e de influenciar na
sociedade em rede. Todavia, uma parcela significativa de usuários foi
esquecida por essas inovações, as pessoas com deficiência visual. A
maioria são usuários de telefones celulares com teclado tradicional, com
a função de receber chamadas e ligar para números memorizados.

Com o objetivo de oportunizar a inclusão desse grupo de usuários com
deficiência visual, de aproximadamente 6,5 milhões de pessoas com
deficiência visual no Brasil (IBGE), aos dispositivos móveis e sem fio,
o Grupo de Tecnologia, Engenharia, Robótica e Física (G-TERF) e o Grupo
de Estudos sobre Educação Diversidade e Inclusão (GEEDI) da Universidade
Federal do Recôncavo da Bahia (UFRB) criaram o aplicativo chamado
''Quick Voice'', para cegos e deficientes visuais, para converter código
de barras bidimensional (QR Code) em arquivo de texto, seja por escrito
ou em áudio, auxiliando principalmente pessoas com deficiência visual.
Sem a necessidade de equipamentos de custo elevado e difícil
usabilidade, qualquer pessoa pode acessar um site ou software de criação
de etiquetas em QR Code e transformar um texto numa etiqueta, podendo
imprimir em sua impressora comum. A partir desse material, outra pessoa
tem a possibilidade de transcrever essa etiqueta em áudio, o que
possibilitaria a leitura do texto completo.

O "Quick Voice" foi desenvolvido em dispositivos ANDROID 4.3 e os
dispositivos anteriores precisam ter conexão com a internet para
realizar a conversão. A partir da versão ANDROID 4.3, é possível baixar
o módulo offline de vozes do ANDROID e realizar a conversão mesmo
estando desconectados. Para utilizar o ''Quick Voice'' como um recurso
para a Tecnologia Assistiva, aplicativo desenvolvido em pelo GTERF/UFRB
com intuito dar acessibilidade as pessoas com deficiência visual.

O Código QR (sigla do inglês Quick Response) é um código de barras
bidimensional que pode ser facilmente digitalizado usando a maioria dos
telefones celulares equipados com câmera. Esse código é convertido em
texto (interativo), um endereço URL, um número de telefone, uma
localização georreferenciada, um e-mail, um contato ou um SMS.

Por se tratar de um item de baixa complexidade, o QR Code pode ser
empregado em diversos ambientes e com diversas funcionalidades. Em
geral, o propósito do QuickVoice -- Leitura QR Code é tornar possível o
entendimento do conteúdo associado ao código QR, por meio de áudio. Com
isso, temos a possibilidade de empregá-lo em ambientes e elementos que
se tornam chave para a tecnologia assistiva. Além de ser facilmente
encontrado, o código QR também pode ser facilmente gerado, como pode ser
visto no site [http://qrcode.kaywa.com/](http://qrcode.kaywa.com/) A partir dele ou de outros
softwares semelhantes é possível inserir o texto desejado ou a URL e
criar o QR code desejado. Veja Figura 1.


<center>
  <p><small>Figura 1: Código QR Code. </small></p><br>
    <img src="../imagens/image34.jpg" style="width: 70%; height: auto;"/>
  </small>
</center>

Na concepção do aplicativo ''Quick Voice'' foi empregado um botão de
acionamento rápido para a leitura do QR Code, que também pode ser feita
agitando o aparelho. Constam dois botões auxiliares, `Apagar' e
`Repetir', utilizados respectivamente para apagar o texto recém
transcrito para repeti-lo. Ao pressionar qualquer um dos botões por um
dado instante, é possível ouvir qual sua funcionalidade, para só depois
acioná-lo, conforme Figura \ref{image35}.

<center>
  <p><small>Figura 2: Aplicativo Quick Voice. </small></p><br>
    <img src="../imagens/image35.jpg" style="width: 70%; height: auto;"/>
  </small>
</center>

A utilização do ''Quick Voice'' é relativamente simples, pois utilizando
a câmera do dispositivo para capturar as imagens do QR e um
decodificador que transforma as imagens geradas em strings de texto em
que é lida e convertido em áudio, podendo ser utilizado em muitos
seguimentos desde revista, livros, panfletos, identificação de lugares e
objetos que estes estejam codificados, conforme a Figura 3.

O Quick Voice está disponível para Android, foi desenvolvido no APP
Inventor uma plataforma do Massachusetts Institute of Technology - MIT
na plataforma é possível desenvolver aplicativos para dispositivos
móveis utilizando blocos de comando.


<center>
  <p><small>Figura 3: Utilização do Quick Voice. </small></p><br>
    <img src="../imagens/image36.jpg" style="width: 70%; height: auto;"/>
  </small>
</center>

A codificação do livro ''Linguagem e suas Tecnologias'' do curso de
Graduação em Matemática utilizado na Superintendência de Educação Aberta
e a Distância (SEAD) da UFRB, o conteúdo de cada página foi disposto em
dois Códigos QR Code com $45mm \times 45mm$ posicionados de forma padrão nos
cantos superior e inferior direito. Para isso, foi utilizado o site QR
Creator, um programa que pode ser instalado gratuitamente no computador
e que permite codificar sem que esteja conectado à internet para criar o
QR Code.

## Considerações finais

A partir da revisão de literatura sobre a aprendizagem com moblidade
(m-learning) e dos conceitos de tecnologia assistiva avaliados, este
trabalho oferece uma análise sobre o ''Quick Voice'', um aplicativo
abrangente que promove à acessibilidade das pessoas com deficiência
visual.

Dessa forma, contribuir para disseminar a aprendizagem (m-learning),
oferecendo um aplicativo com o intuito da inclusão social e do ambiente
educacional brasileiro em que o usuário de tecnologias móveis ganha um
novo papel -- o de aprendiz.

Contudo, apenas a familiarização e o acesso dos deficientes visuais às
tecnologias móveis, por si só, não garante a adesão ao m-learning. Para
garantir o uso contínuo e eficaz dos usuários, que são responsáveis por
suas aprendizagens, é necessário internalizar que o m-learning está
presente em qualquer tempo e espaço no que diz respeito ao processo de
aprendizagem.

## Referências 

[1] Arendt, H. (2009). _A Condição Humana_. (10 ed.). Rio de Janeiro:
Forense Universitária.

[2] Castells, M. (2006). _A sociedade em rede._ (9 ed.). São Paulo:
Paz e Terra.

[3] OMS. (2012). _Relatório mundial sobre a pessoa com deficiência. Tradução de: World Report on Disability (World Health Organization)._
Governo do Estado de São Paulo, Secretaria dos Direitos da Pessoa com
Deficiência. São Paulo: Governo do Estado de São Paulo.

[4] Vygotsky, L. (1998). _A formação social da mente_ (6 ed.). S.P.:
Martim Fontes.

[5] BRASIL. (2007). _Ata da 7ª Reunião do Comitê de Ajudas Técnicas._
Acesso em 13 de Mai de 2014, disponível em Secretaria Especial dos
Direitos Humanos. Coordenadoria Nacional para Integração da Pessoa
Portadora de Deficiência.: Integração da Pessoa Portadora de
Deficiência. Ata da 7ª Reunião do Comitê de Ajudas.
[http://www.infoesp.net/CAT_Reuniao_VII.pdf](http://www.infoesp.net/CAT_Reuniao_VII.pdf).

[6] BRASIL. (2009). _Tecnologia Assistiva. Subsecretaria Nacional de Promoção dos Direitos da Pessoa com Deficiência._ Brasília: Comitê de
Ajudas Técnicas. Fonte: Comitê de Ajudas Técnicas. Tecnologia
Assistiva. Brasília: CORDE, 2009.

[7] BERSCH, R. (2008). _Introdução à Tecnologia Assistiva. CEDI -- Centro Especializado em Desenvolvimento Infantil._ Porto Alegre:
CEDI.

[8] MENDES, E., & LOURENÇO, G. (2012). Recursos computadorizados de
Tecnologia Assistiva  para  estudantes com 
paralisia cerebral em
múltiplos contextos. IN: 2012, _Dimensões pedagógicas nas práticas de inclusão escolar._ Marília: ABPEE.

[9] GALVÃO FILHO, T. A. (2009). _Tecnologia Assistiva para uma escola inclusiva: apropriação, demanda e perspectivas._ Salvador:
Universidade Federal da Bahia.

[10] CONSORTIUM., E. (1999). _Educação em tecnologias de apoio para utilizadores finais: linhas de orientações para formadores._ Acesso em
31 de mar de 2013, disponível em EUSTAT CONSORTIUM.:
[http://portale.siva.it/files/EUSTAT_Tec_Pt.pdf](http://portale.siva.it/files/EUSTAT_Tec_Pt.pdf).