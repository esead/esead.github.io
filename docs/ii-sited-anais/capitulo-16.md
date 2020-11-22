
![Legenda](../img/nova_capitulo.png)

# **_GAME_ COMO FACILITADOR NO ESTUDO DA LINHA DO TEMPO HISTÓRICA**

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


<center><h3><em>Brigitte Bedin</em>[^1]</h3></center>


<center><h3><em>Marilúcia Campos dos Santos</em>[^2]</h3></center>

[^1]: UFRB -- bbedin@gmail.com

[^2]: UFRB -- marilucampos@gmail.com



## **Resumo** 

O trabalho tem como objetivo apresentar a possibilidade de um game com
propósito educativo. Partindo da premissa de que se pode aprender por
meio desse tipo de objeto, o game entra em cena como facilitador no
processo de aprendizagem, sem que se perca o foco educativo. Interação,
prazer por meio do jogo, sendo a tecnologia e o espaço virtual
responsáveis por essa possibilidade. Os serious games fazem parte do
mundo corporativo e ganham espaço no contexto educativo. No Brasil essa
realidade ainda não tomou corpo, pois existe ainda uma certa resistência
por parte dos usuários que preferem games estrangeiros, no tocante aos
serious games isso também se aplica, o que existe na verdade são
encomendas pontuais para esse tipo de demanda. Na educação a utilização
do jogo deve ser cautelosa, lembrando que não existe a possibilidade de
transferir responsabilidades educacionais para o mesmo, mas sim,
utilizá-lo com parcimônia e como facilitador nesse processo. O jogo
proposto nesse artigo busca facilitar o aprendizado histórico da linha
do tempo e suas divisões, uma vez que, existe dificuldade por parte dos
alunos nesse tipo de estudo, assim sendo, o trabalho apresenta as fases
e possibilidades do game em questão. Ressalta a ludicidade e o fluxo que
envolve o jogador no universo histórico.

**Palavras-chave**: Game, facilitador, educação, lúdico, virtual.


## **1. Introdução**

Aprender brincando é um sonho partilhado por muitos e os jogos digitais
estão cada vez mais populares, envolvem e seduzem. A possibilidade de um
recurso lúdico que facilite o aprendizado é instigante e desafiador.

Ao produzir um jogo digital didático, é essencial o foco educativo. A
ludicidade é importante, mas o aprendizado é fundamental, por isso
torna-se necessário unir esses dois elementos. Nesse contexto, essa
ferramenta deve ser elaborada por especialistas em _games_ sem
esquecer do viés pedagógico.

De acordo com Oliveira (2013), o conceito de diversão está ''relacionado
ao aprendizado do jogador durante a interação com o jogo''. Por isso, o
jogador, por meio do jogo, consegue aprender pela experiência, prevê as
possibilidades possíveis nas próximas jogadas, tudo isso tendo como pano
de fundo o divertimento. Essa situação gera envolvimento e imersão. Para
Csikszentmihalyi (2010), o jogo se traduz em diversão enquanto tarefas
cotidianas são cansativas. A estrutura dos jogos propicia o prazer por
causa de sua composição: regras, objetivos, pronta resposta e
possibilidade de controle e concentração, tudo muito diferente do dia a
dia.

Porém, esse contexto de jogo é enriquecido pelo uso das tecnologias e
tudo que elas englobam. Barros (2009) aponta que as tecnologias visam ao
atendimento da diversidade de informações disponíveis atualmente para o
desenvolvimento dos conteúdos, ou seja, uma possibilidade a mais do
ponto de vista didático-pedagógico. A autora destaca, citando Levy
(1996) e Horrocks (2004), que o espaço virtual é caracterizado, entre
outros elementos, pela informação e que ele é agente de mudanças
globais, estimulador dos sentidos e responsável pelo montante de dados
que chegam a nós. Barros (2009) discorre também sobre a transformação da
percepção e da interatividade oferecida por este espaço, tornando a
tecnologia um estímulo para o pensamento. Ainda sobre o espaço virtual,
a autora destaca que a linguagem da web faz uma junção entre linguagens,
línguas, símbolos e imagens, os quais converteram-se em elementos de
aprendizagem indutiva pela lógica e pela experiência do dia a dia.

Barros (2009) conclui, portanto, que há grande possibilidade de aprender
no ambiente virtual, espaço no qual isso ocorre amplamente, de forma
detalhista e com múltiplas percepções. No ambiente virtual a motivação e
os interesses do indivíduo são o ponto principal a ser considerado e não
a lógica de facilidades ou dificuldades com esse ambiente. Além disso,
idade, linguagem, formação e diferenças institucionais não
impossibilitam o desenvolvimento neste espaço, pois ele é aberto e
acessível.

No tocante ao Brasil, Alves e Hetkowski (2007) traçaram o perfil do
_gamer_ brasileiro, por meio de entrevistas realizadas com 220
indivíduos de todo o país, entre 9 e 59 anos. Na pesquisa constatou-se
que, mesmo sem acesso a algum tipo de jogo, no geral os entrevistados
desvendaram os símbolos envolvendo os _games_. A educação no século
XXI conta com avanços digitais estruturados na aprendizagem informal,
educação a distância, aprendizagem colaborativa, e o _game_ faz
parte deste universo, portanto será o objeto por nós analisado.

Fagundes e Garcia (2014), em pesquisa, observaram que alunos de séries
iniciais têm pouco ou nenhum conhecimento prévio de História e quando
chegam ao 6º ano, essa ausência fica evidente. Os autores argumentam que
isso ocorre em função dos professores dessas séries abordarem os mais
diversos temas, mas, por falta de formação específica, não abordar os
conteúdos históricos. Esse ensino fica limitado aos livros didáticos e
memorização de fatos e datas, tendo como objetivo apenas a aprovação na
disciplina. Não existe uma preocupação com o tempo e o espaço, a
importância da História na formação do indivíduo fica aquém e, para o
aluno, o entendimento aprofundado e o significado histórico se tornam
difíceis de entender, pois não exercitam o pensamento nessa direção.

Portanto, os professores Fagundes e Garcia (2014), diante do quadro
apresentado, propuseram um estudo com o intuito de facilitar o
entendimento de História, sob a perspectiva **glocal** -- global e
local -- que envolve: Antropologia, História, Sociologia e práticas
culturais (RODRIGUES, 2017) -- a qual foi aplicada em alunos do 6º ano,
cujo viés envolvia a realidade deles. Nesse contexto, buscaram
relacionar o que acontecia no local com acontecimentos do mundo,
envolvendo educação, economia e ambiente. Essa foi uma forma de mostrar
que tudo está interligado, que existe um entrelaçamento entre o local e
o global. Para isso, se reportaram às memórias envolvendo a sala de
aula, tendo como objetivo criar a identidade do aluno, uma construção
com cunho social.

Assim sendo, inspirada na pesquisa de Fagundes e Garcia (2014), no
presente trabalho, a linha do tempo histórica foi escolhida para a
elaboração de um _game_. A escolha justifica-se por ser um assunto
que embora possa parecer simples e de fácil aprendizagem, representa
dificuldade para alunos de diversas idades, pois eles não conseguem
estabelecer a linha do tempo e seus respectivos períodos.

O _game_ proposto será dividido em: Pré-história; História Antiga;
História Medieval; História Moderna; História Contemporânea; e
Pós-modernidade. No total serão sete (7) fases, sendo a primeira uma
sala de aula e as demais os níveis, cada qual representado por um
período histórico.

A dinâmica do jogo consistirá em apresentar desafios para que o aluno
passe para a fase seguinte, ou seja, num primeiro momento, ele se
encontra na sala de aula e, para dar início à aventura, terá que passar
por um portal do tempo localizado na lousa. Para tanto, deverá resolver
alguns enigmas e obstáculos até que chegue no portal. Fase por fase,
deverá transpor os obstáculos e conquistar o ''passe'' para a próxima
etapa.

Diante do exposto, o presente trabalho pretende demonstrar que é
possível ensinar por meio do jogo, sendo este um facilitador do
aprendizado.

## **2. _Serious games_: mercado e responsabilidades**

Silva (2014) aponta que embora existam diversas denominações para jogos
voltados para outros fins que não a educação, o termo mais usual é
_serious games_. Esses jogos foram usados em diversas áreas:
militar, governamental, na área da saúde, em marketing, empresas e na
educação. Destaca que entre os benefícios dos _serious games_ na
educação estão a ludicidade, a competição e o ato de compartilhar, além
da possibilidade de aprimorar competências e habilidades. O jogo vem
como um elemento a mais e uma forma de atrair e motivar.

A produção de um _game_ envolve diversos profissionais, como o
_designer_ de _games_, músicos, artistas visuais, modelador,
entre outros. Todos devem entender com clareza a dinâmica e preceitos do
_game_ que será desenvolvido, no entanto, o _game designer_
responsável fará o arremate de todas as áreas envolvidas. Além disso, o
_game_ nos remete ao entretenimento, não existe um mercado forte de
_serious_ _games_, jogos voltados para treinamentos e educação
(SANTAELA; FEITOZA, 2009).

Os _serious_ _games_ servem de apoio na aprendizagem quando
atrelados às teorias da ciência cognitiva. Entre as diversas teorias,
destacamos:

+ Teoria cognitivista, na qual, segundo Bruner, o aluno é ativo e
	responsável pelo seu aprendizado, levando-se em conta suas
	experiências enquanto indivíduo;

+ Teoria sociocultural de Vygotsky, em que o meio social no qual estamos
	inseridos é responsável pelo conhecimento adquirido inicialmente,
	sendo interiorizado a partir do desenvolvimento de habilidades
	específicas;

+ Teoria da inclusão produzida por David Paul Ausubel, que não descarta
	a importância do meio social, mas dá crédito maior ao que se
	desenvolve em sala de aula, levando em conta os conhecimentos prévios
	do aluno com o intuito de adequar os materiais didáticos;

+ Aprendizagem baseada em problemas de Bransford, que propicia situações
	de análise e resolução de problemas, residindo aí uma forma de
	aprender.


A aplicação destas teorias nos _serious games_  possibilita
um ganho maior, pois entram em cena aspectos fundamentais no
ensino-aprendizagem, são eles: a motivação por promover a descoberta do
que é proposto no jogo; reflexão; planejamento e busca por estratégias
que levem ao sucesso no jogo; escolhas que irão impactar no resultado
final; entendimento dos processos concorrentes e de avaliação (DANTAS;
BUBLITZ; QUEIROZ, 2011).

O Relatório do Mapeamento da Indústria Brasileira e Global de Jogos
Digitais, desenvolvido pelo Núcleo de Política e Gestão Tecnológica --
PGT, aponta que no Brasil o mercado consumidor prefere os jogos
importados, cujo investimento é altíssimo e consideram sua qualidade
superior. Se já não é fácil para os _games_ populares, no que se
refere aos jogos educativos, então, essa realidade é mais custosa e
depende de encomendas feitas por empresas ou escolas.

Vamos tentar justificar isso de forma mais consistente? Por que não é
sensato? A proposta consiste em ter um jogo digital com boas
possibilidades, para então o profissional do ensino elencar os conteúdos
e as respectivas competências que podem ser desenvolvidas, tendo como
suporte o jogo digital. Um bom exemplo é o War®. Embora não pretenda
ensinar geografia, o faz com sucesso (SANTAELA; FEITOZA, 2009).

## **3. Os jogos digitais na educação**

Ao pensar no jogo como possibilidade educativa, precisamos tomar alguns
cuidados, pois essa proposta não pode representar uma solução para os
problemas enfrentados na educação, o jogo é mais um objeto de
aprendizagem que pode ser explorado se usado com parcimônia. Alves
(2008) discute essa questão quando reitera que não podemos pensar no
jogo digital enquanto desenvolvedor de conceitos, cognição e por último
diversão. Lembrando que esta ferramenta é simplista, contrapondo as
teorias clássicas da educação.

A visão conteudista em jogos deve ser descartada. Deve-se sim buscar um
jogo que seja envolvente e que possibilite desenvolver os conteúdos e
competências necessárias sob responsabilidade do docente, sendo o jogo
um suporte (SANTAELA; FEITOZA, 2009).

Outra questão interessante é a narrativa propiciada pelos _games_
com interação lúdica narrativa. São inúmeros os exemplos que indicam
esta possibilidade: o jogo War com suas batalhas épicas; ou o Super
Breakout que narra uma história fantástica; no Monopoly com a disputa
entre barões. São infinitas possibilidades e experiências que envolvem
narrativas. O desafio consiste em usar essa possibilidade de diversas
formas. Um único jogo pode ter inúmeras perspectivas. Dessa narrativa
fazem parte: personagens, cenários e o próprio enredo (SALEN; ZIMMERMAN,
2012).

Pensando nos jogos para a educação, um jogo voltado para a História,
além de viável, é também fascinante. Podemos jogar tendo como enredo a
própria História, o mundo não ficcional, tornando esse tema interessante
e sedutor.

## **4. Pensando um jogo**

O jogo proposto possui sete fases. A primeira fase tem como cenário uma
sala de aula. O desafio consiste em chegar até a lousa, a qual é um
portal que leva à próxima fase. A Figura 1, sala de aula, apresenta uma
sala comum em perspectiva:

 <center>
  <p><small>Figura 1: Sala de aula.</small></p><br>
    <img src="../imagens/imagem7.jpg" style="width: 70%; height: auto;"/>
  <small>
     <p>Fonte: A autora.</p>
  </small>
</center>

Ao dar início ao jogo, o jogador vê a planta baixa da sala (Figura 2), a
qual apresenta desafios/obstáculos e prêmios, levando-o a se aproximar
do portal.

 <center>
  <p><small>Figura 2: Planta baixa da primeira fase.</small></p><br>
    <img src="../imagens/imagem8.jpg" style="width: 70%; height: auto;"/>
  <small>
     <p>Fonte: A autora.</p>
  </small>
</center>

O jogo deve ser intuitivo, as setas vão piscar conforme o jogador for
avançando. Os obstáculos surgem e a cada etapa vencida abra-se a
passagem para a próxima etapa na fase correspondente. No final da
primeira fase o jogador deverá responder as seguintes perguntas:


+ Seu nome;

+ Sua idade;

+ E a última pergunta instigando o jogador: Quer viajar no tempo?

As próximas fases seguem a mesma abordagem, passo a passo o jogador vai
seguindo no tempo, vencendo os desafios e obstáculos.


 <center>
  <p><small>Figura 3: As fases seguintes.</small></p><br>
    <img src="../imagens/imagem9.jpg" style="width: 70%; height: auto;"/>
  <small>
     <p>Fonte: A autora.</p>
  </small>
</center>

As fases obedecem a sequência lógica e progressão do mais antigo para o
mais novo. Ao final de cada fase o jogador deve atingir o prêmio máximo,
só assim terá condições de avançar. Os prêmios estão atrelados a um fato
histórico relevante da época. Exemplo: Na História Antiga o desafio
consiste em tirar a Espada de Lancelot da pedra fundamental.

 <center>
  <p><small>Figura 4: Espada de Lancelot.</small></p><br>
    <img src="../imagens/imagem10.jpg" style="width: 70%; height: auto;"/>
  <small>
     <p>Fonte: A autora.</p>
  </small>
</center>

O jogo é finalizado quando o jogador chega à Pós-modernidade. Nessa fase
são abarcados assuntos e imagens da atualidade e o prêmio final é o
Troféu Master. No seu desenrolar fatos e imagens vão surgindo, dessa
forma o jogador vai relacionando e associando tais informações. A
narrativa é importante e pequenas histórias vão sendo contadas no
decorrer da empreitada, além de motivar e envolver, a história contada
dá sentido à brincadeira.

O personagem deve ter relação com o jogador -- segundo Almeida (2019)
Professor da SAGA: School of Arts, Games -- o flow ocorre conforme
propiciamos um reporte ao dia-a-dia do aluno, isso envolve cores,
lugares, particularidades do quotidiano e pessoas próximas às imagens
conhecidas pelo jogador. O personagem escolhido é um adolescente com
características do \emph{cartoon}.

 <center>
  <p><small>Figura 5: Personagem.</small></p><br>
    <img src="../imagens/imagem11.jpg" style="width: 70%; height: auto;"/>
  <small>
     <p>Fonte: A autora.</p>
  </small>
</center>

Todo o ambiente é cuidadosamente planejado, tendo como premissa envolver
o jogador, ou seja, ao elaborar um jogo a multidisciplinaridade está
presente em todos os momentos da execução, temos a arte, a modelagem das
imagens, o trabalho de programação em 3D e acima de tudo, se falamos em
jogo educativo não podemos deixar de lado a construção pedagógica.

Espera-se que ao final do jogo, as divisões básicas das fases
históricas, tenham sido assimiladas e interiorizadas pelo jogador. Que
essas informações passem a fazer parte dos conhecimentos do jogador e
que seja simples e clara essa interpretação.


## **5. Considerações finais**

Com a tecnologia avançando cada vez mais, torna-se primaz que a educação
também acompanhe esses avanços. Os alunos mudaram e os educadores também
precisam acompanhar essas mudanças. Nesse contexto hoje temos inúmeras
possibilidades, entre elas os games. Os alunos não mais se enquadram nas
metodologias antigas e ultrapassadas, a linguagem mudou e o ensino
tradicional perdeu seu lugar para um ensino envolvente e interativo.

Jogos estruturados e direcionados ao aprendizado tendem a se tornar algo
comum com o tempo, cabe aos educadores buscar soluções viáveis e
envolventes, que possibilitem ensinar de forma prazerosa e eficaz.

## **Referências**


ALVES, Lynn. Relações entre os jogos digitais e aprendizagem: delineando
percurso. **Educação, Formação & Tecnologias**, v.1, n. 2, p.
3-10, nov. 2008. Disponível em: https://eft.educom.pt/index.php/eft/article/view/58/38\.
Acesso em: 28 maio 2019.


_______________ ; HETKOWSKI, Tânia Maria. _Gamers_ brasileiros:
definindo o perfil. In: DIAS, Antonio; FIALHO, Nádia Hage; HETKOWSKI,
Tânia M. (orgs.). **Desenvolvimento sustentável e tecnologias da informação e comunicação.** Salvador: Edufba, 2007, v.1, p. 161-174.


BARROS, Daniela Melaré Vieira Barros. Estilos de uso do espaço virtual:
como se aprende e se ensina no virtual? **Inter-Ação**: Rev. Fac.
Educ. UFG, v. 34, n. 1, jan./jun. 2009, p. 51-74. Disponível em:
https://bit.ly/2Wsz4hz. Acesso em: 5 maio 2019.


CSIKSZENTMIHALYI, Mihaly. **Fluir (Flow):** una psicologia de la
felicidad. Canadá: Editora Kairus, 2010.


DANTAS, Wannyemberg K. da S.; BUBLITZ, Frederico M.; QUEIROZ, José E. R.
de. **Desenvolvimento de _serious games_** centrado nos
usuários}. In: X Simpósio Brasileiro de Games e Entretenimento Digital,
2011, Salvador - Bahia. SBC - Proceedings of SBGames 2011, 2011. p. 1-8.
Disponível em: https://bit.ly/2EDmHVK. Acesso
em: 24 maio 2019.


FAGUNDES, Bruno Flávio Lontra; GARCIA, Maria de Lourdes
Decósimo. Memórias da história local em sala de aula. In:
**Os desafios da escola pública paranaense na perspectiva do professor PDE**: artigos. Paraná: Governo do Estado, Secretaria da
Educação, 2014. Cadernos PDE vol. 1. Disponível em:
https://bit.ly/2Qy4opN. Acesso em: 18 maio
2019.


NÚCLEO DE POLÍTICA E GESTÃO TECNOLÓGICA -- USP. **Relatório final**: Mapeamento da Indústria Brasileira e Global de Jogos Digitais.
São Paulo, Gedigames, 2014. Disponível em:
https://bit.ly/2zpyJjY. Acesso em: 5 maio 2019.


OLIVEIRA, Fabiano Naspolini de. **Entendendo a diversão nos jogos digitais**. Fábrica de jogos, 19 nov. 2013. Disponível em: https://bit.ly/2G9FtUS. Acesso em: 13 abr.
2019.


RODRIGUES, Donizete. Patrimônio cultural, memória social e identidade:
interconexões entre os conceitos. **Letras Escreve**, Macapá, v. 7,
n. 4, p. 337-361, 2º semestre, 2017. Disponível em:
https://bit.ly/2Xc9yKN. Acesso em: 12 maio
2019.


SALEN, Katie; ZIMMERMAN, Eric. **Regras do jogo**: fundamentos do
_design_ de jogos. Volume 3: Interação lúdica. São Paulo: Editora
Edgard Blücher Ltda, 2012.


SANTAELLA, Lucia; FEITOZA, Mirna (orgs.). **Mapa do jogo**: uma diversidade cultural dos jogos. São Paulo: Cengage Learning, 2009.


SILVA, Giancarlo Lima da .**EduQuest**: uma proposta para o uso de
_serious games_ na educação e na capacitação profissional. Rio
Grande do Norte: Instituto Federal de Educação, Ciência e Tecnologia do
Rio Grande do Norte, 2014. Disponível em: https://www.academia.edu/11690740/EduQuest_Uma_proposta_para_o_uso_de_Serious_Games_na_educa\%C3\%A7\%C3\%A3o_e_na_capacita\%C3\%A7\%C3\%A3o_profissional. Acesso em: 13 maio 2019.