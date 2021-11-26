


<style>
p.combinado:first-letter { 
	color: #00587A; 
	font-size:xx-large; 
}
</style>

![Legenda](imagens/capitulo.svg)

# **Uso da tecnologia com placas de Arduino e ciberespaço para estudo do comportamento das marés**

??? "Ferramentas de acessibilidade"

    :material-cursor-default-click-outline: Clique no botão abaixo para alternar visualização:

    <div class="tx-switch">
       <button data-md-color-scheme="default"><code>Modo normal</code></button>
       <button data-md-color-scheme="slate"><code>Modo escuro</code></button>
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




??? info "Autores"
    === "João da Silva Melo"

        Mestre em Ensino de Física (UNEB). Especialista em Tecnologias e Educação Aberta e Digital (UFRB - UAb Portugal). Licenciado em Matemática. E-mail: joaomellomestr@gmail.com.

    === "Janaína dos Reis Rosado"

        Doutora em Educação e Contemporaneidade (UNEB). Mestra em Educação e Contemporaneidade (UNEB). Licenciada em Pedagogia (UNEB). Pesquisadora na Universidade do Estado da Bahia. sE-mail: janainarosado@yahoo.com.br.


**Resumo**: Este texto tem por objetivo discutir, a partir de pesquisa
bibliográfica, a aplicação da robótica através o uso da Tecnologia da
Informação e da Comunicação (TIC) nos espaços formais e informais de
ensino e aprendizagem e como esta pode contribuir para a difusão do
conhecimento em comunidades pesqueiras. É inegável que as tecnologias
tem se incorporado à cultura e alterado a concepção de espaço de
aprendizagem. Com essa premissa, a inserção das TICs (arduino^®^) e o
estudo da maré foram ancorados na teoria de aprendizagem significativa
de David Ausubel, propondo o estudo da astronomia no Ensino Fundamental,
séries finais, com inserção de tecnologia social. Como Instrumento
Pedagógico motivador, será levado em consideração o comportamento da
maré e a influência do campo gravitacional lunar e solar. Esses
fenômenos físicos fazem parte do dia a dia das comunidades litorâneas e
interfere diretamente na dinâmica das comunidades pesqueiras. Em
conformidade com as fontes bibliográficas, foi sugerido o uso de placa
de arduino^®^ e de sensores como instrumento tecnológico que possibilite
o registro de informações relacionadas às marés. Como resultados,
pode-se ressaltar que os saberes da comunidade de pescadores necessitam
de valorização e de socialização para que futuras gerações possam
ressignificar esse conhecimento.

**Palavras-chave**: Tecnologia. Difusão do conhecimento. Aprendizagem
significativa. Pescadores e marisqueiras.

## Introdução 

O diálogo entre os saberes e as práticas dos pescadores em relação às
marés têm se perpetuado através da difusão do conhecimento, que passa de
pai para filho, de mestre para aprendiz, de geração em geração, baseado
nas práticas e experiências pessoais.

Essa afluência de informações vem aumentando ano a ano e um dos fatores
que tem contribuído para esse aumento é a inserção de novas tecnologias
neste diálogo. Embora o conhecimento popular enfrente diversos
obstáculos epistemológicos (BACHELARD, 1996) -- diante do conhecimento
dito como acadêmico ou científico --, este tem sido responsável por
difundir as tradições, os costumes e em especial a cultura pesqueira.

Segundo Forquin, a difusão do conhecimento nas comunidades epistêmicas é
importantíssima para a preservação da identidade e dos valores
artísticos, religiosos, culturais, saberes e práticas: "Educar, ensinar
é colocar alguém na presença de certos elementos da cultura a fim de que
dele se nutra, que ele se incorpore à sua substância, que ele construa a
sua identidade intelectual e pessoal em função deles" (FORQUIN, 1993, p.
168 apud CANDAU, 2006, p.120).

O modelo de produção e transmissão de conhecimento está fundado sob a
ecologia do saber, em que um dos objetivos é a promoção do diálogo entre
os saberes, reforçar a luta pela identidade, assim como a inserção de
novas tecnologias sociais. Boaventura S. Santos (2005) considera que
esses elementos de luta visam restaurar os saberes e as práticas das
comunidades epistêmicas e ainda reforçar os laços de interesse.

Conforme Antonio Santos (2005), todo conhecimento é local e pode ter
caráter total, mas quando é questionado, emerge um novo paradigma (KUHN,
1987), uma nova tecnologia anexa a um conhecimento social já existente,
o que caracteriza a Epistemologia do Sul.

Vale ressaltar que nenhum conhecimento, seja ele popular ou acadêmico,
pode ser dado como acabado, assim como nenhum saber pode ser capaz de se
bastar, o saber por si só não sobrevive, precisará de outros saberes
para sua existência. A comparação entre os sabres é inevitável, contudo,
o importante são os seus limites e possibilidades.

Na atual sociedade, o conhecimento científico é considerado refutado,
testado e acabado (MOREIRA; MASSONI, 2016), com isso elevam o
conhecimento popular a uma marginalização e descrença, um saber dito
como desprestigiado (COSTA, 2008). Contudo, saberes populares, mesmo
sendo leigos (FEYERABEND, 2011), são tão importantes e confiáveis quanto
o conhecimento científico, pois é elaborado por seres humanos que
identificam uma problemática, estudam o caso e o resolvem (DAGNINO,
2014). Embora os saberes populares tenham sido construídos por
indivíduos não letrados, precisam ser validados pela academia:
"Conhecimentos esquecidos, abandonados, subjugado por um conhecimento
considerado superior e vivem à margem do que modernamente, chamamos de
ciências" (BASTO, 2013, p. 1).

Os saberes e as práticas populares podem até não seguir os métodos de
pesquisa sugeridos pela academia (MOREIRA; MASSONI, 2015), não possuir o
mesmo caráter de rigor, nem a mesma testabilidade ou até mesmo a
refutabilidade científica, mas revelam uma riqueza de conhecimento
cultural. Como diz Paulo Freire (1987, p. 68): "Não há saberes mais, nem
saberes menos, há saberes diferente".

A tecnologia social não visa apenas à construção de produto, processo ou
método que gere custo alto para seus membros, pelo contrário, são
produtos de baixo custo, mas de alto impacto social, aplicável e
inovador para o desenvolvimento social da comunidade.

Diante desse cenário, a presente pesquisa tem por interesse, a partir de
literaturas específicas, estudar o processo de construção de ações que
sejam capazes de estimular o diálogo entre pescadores e alunos em suas
comunidades, investigar saberes e práticas etnocitiológicas, a
influência da lua sobre as marés, assim como sugerir tecnologia social,
instrumentação midiática com placas de arduino^®^, para a medição de
fenômenos geofísicos em torno das marés e o impacto sociopedagógico que
essa tecnologia social poderá fornecer à comunidade.

Nesta pesquisa de cunho bibliográfico, propomos como objetivo geral:
Discutir a influência da lua sobre as marés, como instrumento de ensino
e aprendizagem; investigando as fases da lua e a sua correlação com as
marés, através do uso da tecnologia de arduino^®^. Para tal, serão
contemplados os seguintes objetivos específicos: i) Discutir o uso de
robótica a partir de placas de arduino para mensurar dados geofísicos
das marés; ii) Verificar a potencialidade dos ciberespaços para o estudo
os dados das marés; iii) Estudar as fases da lua e o efeito
gravitacional sobre as marés; iv) Estudar a utilização de softwares
específicos de astronomia (Stellarium e Celestia).

Adotou-se a perspectiva descritiva, visto ter por finalidade uma melhor
compreensão de uma realidade, considerando suas características e sua
relação com a sociedade. Para a coleta de dados, optou-se pela pesquisa
bibliográfica que, consiste no levantamento de bibliografia disponível,
com a finalidade de colocar o pesquisador em contato direto com aquilo
que foi escrito sobre determinado assunto (GIL, 2008). Em razão disso,
recorremos a obras de diferentes autores que abordam as temáticas
selecionadas.

## Trajetória do pescador artesanal: contexto brasileiro 

O pescador tem sido uma figura sempre presente na história humana desde
os primórdios até os dias atuais. Sua imagem é associada às navegações,
havendo grande influência no capitalismo mercantil nos séculos XV e XVI,
assim como teve participação importantíssima na formação histórica e
social do Brasil. Para Maldonado (1986), os pescadores são sujeitos
históricos que utilizam seus saberes para se relacionar com a natureza
através de suas embarcações e conseguem tecer valores sociais.

No Brasil pré-colonial, os saberes e as práticas de pesca foram uma
herança vinda dos índios que utilizavam jangadas e canoas rudimentares
para a pesca de subsistência. No período colonial, a pesca teve uma
emergente prática e a figura do pescador passa a ter uma articulação
importante nas relações sociais, embora sua produção naquele momento
fosse voltada para sustentação familiar ou até mesmo reprodução social,
sem preocupação com lucro; o objetivo não era viver da pesca, mas se
apropriar dos meios de produção e ter domínio dos saberes e práticas, na
captura de peixes, na variação lunar, das marés e das estações do ano;
esses conhecimentos, com passar do tempo, se tornaram segredos da
profissão (DIEGUES, 1983).

Com a instalação do poder português na Bahia, a pesca predatória de
baleias passou a ser um indicador econômico para o estado, aquecendo a
economia comercial por muito tempo. Apenas no século XIX, com a
proibição da pesca predatória de baleia, ocorreu a desativação de
fábricas de óleo e outros seguimentos que faturavam com essas
atividades.

O pescador, no período do Império, é citado em diversos grupos sociais
de resistência, tais como abolição dos escravos, revolta da cabanagem,
sabinada, farrapos e outros. Visto que as revoltas comprometiam os
interesses da elite política do Império, já que a defesa terrestre não
oferecia bons resultados e o comércio praticamente era realizado em via
marítima, o Império investia no reforço da Marinha, além de ser uma
ótima protetora para o comércio, para a fronteira e para o antitráfico.
Essa demanda levou o Império a criar a Capitania dos Portos e a
fortalecer a Reserva da Marinha com armas. Mesmo assim, foi necessária a
participação dos pescadores nessa nova conjuntura Naval (SILVA, 1993).

No período da República, houve a criação das Colônias de pescas que
ficavam no âmbito da Reserva Naval; na realidade, essas Colônias serviam
como base de apoio, era um "ponto" de aproveitamento dos melhores
pescadores (VILLAR, 1945). Todo pescador era obrigado a estar inscrito
na Marinha do Brasil, podendo ser convocado no caso de guerra. A Marinha
colocava nas Colônias de pescadores o lema "Pátria e Dever" (ABREU,
2012, p. 65), valorizando um pensamento positivista. No entanto, as
Colônias de pescadores não foram construídas para defender a classe,
pelo contrário, para atender aos interesses da elite capitalista (MARX,
1982).

No início do Estado Novo, foram criados vários códigos, órgãos e
departamentos ligados à pesca, com o intuito de manter as Colônias sobre
vigilância do Estado, estender o aparente poder da Marinha nas costas e
aumentar a fonte de renda em relação ao pescado. Nesse momento político,
o pescador é fragilizado e explorado por duas esferas hegemônicas: por
um lado, a Marinha, com um discurso positivista de "Dever a Pátria", por
outro, a Superintendência de Desenvolvimento da Pesca (Sudepe), tendo
como superintendente o Almirante Paulo Moreira, com uma ideologia de
domínio e exploração. Mediante isso, a figura do pescador se torna um
paradoxo, ora importante no contexto político como fonte de renda, porém
sem nenhuma autonomia, sem nenhuma identidade (DIEGUES, 1995).

Essa situação se alastrou por décadas. Durante o Período de Guerra (1939
a 1945), as Colônias serviam como pontos estratégicos de comunicação da
Marinha, principalmente no Rio de Janeiro, Pernambuco e Bahia, e eram
pintadas de azul e branco, com o símbolo da Marinha na entrada. O
gerenciamento paralelo durou até 1973. No governo ditatorial, foi criado
um projeto chamado PESCART, um programa assistencial aos pescadores e
Colônias de Pesca; o governo investiu na infraestrutura das Colônias e
em tecnologia no manejo da pesca, mas esses investimentos na realidade
dissimulavam uma tendência neoliberal, o objetivo era amparar o setor
empresarial e criar uma relação de paternidade com os pescadores; as
Colônias, sem autonomia e desprestigiadas, eram invadidas por capital
privado, com se fossem uma extensão da indústria pesqueira (CALLOU,
2007; RAMALHO, 1999).

Inserido na ideologia neoliberalista de privatizações, enfraquecimento
do Estado e quebra de leis trabalhistas, o setor sofre duro impacto,
inclusive com a extinção da Sudepe, em 1989, ficando o pescador
vinculado ao Instituto Brasileiro do Meio Ambiente e dos Recursos
Naturais Renováveis (IBAMA), um instituto ambientalista sem nenhuma
relação com o pescador; diante essa nova ideologia, o pescador artesanal
fica desamparado sem representação profissional, socialmente abandonado,
inserido em um contexto de desigualdade social.

Com a Constituição de 1988, os pescadores artesanais conquistaram
avanços no que tange aos direitos sociais e políticos, quando as
colônias de pescadores, através do artigo 8º, foram equiparadas aos
sindicatos de trabalhadores rurais e as Colônias passaram a ter caráter
sindical, e não mais militar e consensual. Segundo o inciso I deste
artigo, "\[...\] a lei não poderá exigir autorização do Estado para a
fundação de sindicato, ressalvado o registro no órgão competente,
vedadas ao Poder Público a interferência e a intervenção na organização
sindical" (BRASIL, 1988, n.p.).

Embora esta pesquisa tenha trazido recortes sócio-históricos, na
atualidade, a figura do pescador continua sem atenção do Estado. E, de
forma semelhante, as marisqueiras, pois suas atividades continuam
invisibilizadas, sua produção não entra nas estatísticas oficiais da
pesca regional ou nacional; o que se observa é a marginalização de uma
cultura essencial para sobrevivência de muitas comunidades litorâneas.
Segundo Diegues (1983), é fundamental a participação feminina na prática
de mariscagem, na organização produtiva de atividades de extração, no
manejo e na venda; isto porque o incrementando da renda nas comunidades
pesqueiras, assegura, aparentemente, uma igualdade de gênero na
conjuntura social. Contudo, ainda a política de pesca está voltada
apenas para os grandes empresários, membros da elite política do país,
enquanto os pescadores e as marisqueiras continuam refém do Estado ou
esquecidos nas suas comunidades.

## Fundamentação teórica 

O principal referencial teórico que embasa este trabalho é a Teoria de
Aprendizagem Significativa de David Ausubel na perspectiva de Marco A.
Moreira, por entender que os conhecimentos prévios dos estudantes filhos
de pescadores e marisqueiras devem ser valorizados e ancorados a novos
conhecimentos.

Na perspectiva de Ausubel (1968), para a construção da aprendizagem
significativa, são necessárias duas condições. Em primeiro lugar, o
estudante precisa ter o interesse em aprender. Em segundo, os conteúdos
trabalhados precisam ter ligação com o cotidiano do estudante, ou seja,
estes precisam ser potencialmente significativos, neste sentido, Moreira
e Masini (2006) afirmam:


> Para Ausubel, aprendizagem significativa é um processo pelo qual uma
nova informação se relaciona com um aspecto relevante da estrutura de
conhecimento do indivíduo. Ou seja, neste processo, a nova informação
interage com uma estrutura de conhecimento específica, a qual Ausubel
define como conceito subsunçor ou, simplesmente, subsunçor (subsumer),
existentes na estrutura cognitiva do indivíduo. A aprendizagem
significativa ocorre quando a nova informação ancora-se em subsunçores
relevantes e preexistentes na estrutura cognitiva de quem aprende.
Ausubel vê o armazenamento de informações na mente humana como sendo
altamente organizado. O uso de organizadores prévios é uma estratégia
proposta por Ausubel para, deliberadamente, manipular a estrutura
cognitiva a fim de facilitar a aprendizagem significativa. Organizadores
prévios são materiais introdutórios apresentados antes do próprio
material a ser aprendido. Segundo Ausubel, a principal função do
organizador prévio é a de servir de ponte entre o que o aprendiz já sabe
e o que ele deve saber, a fim de que o material possa ser aprendido de
forma significativa. Ou seja, os organizadores prévios são úteis para
facilitar a aprendizagem na medida em que funcionam como "pontes
cognitivas". (MOREIRA; MASINI, 2006, p. 19)


Dessa forma, a aprendizagem significativa é aprendizagem com
significado, compreensão, transferência de conhecimentos e capacidade de
aplicação a novas situações.

Presume-se ser necessário citar a importância dos Mapas Conceituais,
posto que, para Ausubel, no sentido de se tornarem evidentes as relações
hierárquicas existentes entre os diversos conceitos relativos a um
determinado conteúdo. Segundo Moreira e Buchweitz (1993), os mapas
conceituais são estratégias pedagógicas importantes no processo de
ensino e aprendizagem que também podem ser utilizadas como ferramentas
avaliativas, reflexivas e diagnósticas para promoção de experiências de
aprendizagem indicadas na Figura
1:

<center>
<p>Figura 1: Mapa Conceitual da Aprendizagem Significativa de David Paul
Ausubel.</p>
<img src="../imagens/imagem-cap-19-01.png" style="width: 75%; height: auto;"/>
<br><small>
Fonte: Moreira e Buchweitz (1993, p. 43).
</small>
</center>



Ressaltamos que o processo de aprendizagem significativa é um processo
cognitivo, na qual o conceito de intermediação vai dialogando com aquilo
que o estudante já sabe, com o que vai ser aprendido, seja um conceito,
uma situação, uma proposição ou um fenômeno (RONCA, 1994). Conforme
Celso Antunes (2001), a aprendizagem significativa se inicia com a
coleta do que o estudante sabe, não só sobre o ar, o tempo, a
temperatura, a chuva, o calor, o vento, o frio, mas também com esses
fenômenos interferem na vida e nas emoções; utilizando-se dos saberes
deles, encontrar um meio para explicar os desejos desejados, o que
Ausubel chama de organizadores prévios, que, no contexto da sala de
aula, são as noções iniciais, as informações introdutórias gerais
(AUSUBEL, apud SALVADOR, 2000).

Com relação a esta pesquisa, também foram utilizados alguns autores do
seguimento tecnologia, entre eles temos o sul africano Seymour Papert,
que é considerado um dos pais do campo da inteligência artificial
(I.A.), sendo reconhecido internacionalmente como um dos principais
pensadores sobre as formas pelas quais a tecnologia pode modificar a
aprendizagem, autor dos livros "Mindstorms: children computers and
powerful ideas" (1980) e "The children's machine: rethhing school in the
age of the computer" (1993), além disso, publicou diversos artigos sobre
aprendizagem e inteligência artificial. Outros pesquisadores são
Fernando José de Almeida e Fernando Moraes Fonseca Junior, autores de
"Prolnfo: Projetos e ambientes inovadores" (2000), uma literatura que
retrata o uso da informática como objeto potencializador de produtos
educacionais e a facilidade de cooperação interdisciplinar em ambientes
inovadores. E John Palfrey e Urs Gasser, autores de "Nascidos na Era
Digital" (2011), que tratam de vários assuntos midiáticos, tais como
identidade digital, bancos de dados e transposição de informações para
espaços digitais, assim como nativos digitais e imigrantes digitais;
temáticas que serão utilizadas no desenvolvimento desta pesquisa.

## Tecnologia midiática e ciberespaço no ensino-aprendizagem 

O mundo contemporâneo é significativamente diferente daquele de algumas
décadas atrás e muito distinto daquele do início do século passado, e
grande parte dessa mudança pode ser atribuída às transformações na
tríade do conhecimento, da ciência e da tecnologia. Essas mudanças
influenciam diretamente na educação básica e exigem novas formas de
ensinar os saberes necessários para a formação de cidadãos
contemporâneos capazes de intervir adequadamente na sociedade e
compreender com plenitude a realidade na qual estão imersos (RODRIGUES,
1998).

Segundo Santaella (2004), a atual sociedade encontra-se totalmente
envolvida na era midiática; seja nos supermercados, farmácias, bancos,
transportes coletivos e nos meios de telefonia, a sociedade
contemporânea utiliza-se no seu dia a dia de recursos midiáticos. E a
escola, enquanto agente de transformação, não pode ficar de fora dessa
mudança pragmática; os tabus que envolvem as mídias precisam ser
superados, os paradigmas devem ser trabalhados para emergir novos
conceitos.

Vale ressaltar que as mídias não podem surgir como instrumentos de
ameaça à docência, pelo contrário, estas podem ser mais um instrumento
de auxílio à prática docente, como também pode se estender como novos
espaços extraclasse e ao mesmo tempo pode ser gestada de maneira
virtual, coletiva ou individual (CARNEIRO, 2002). Nesse seguimento, Lévy
(2003) assevera que as Tecnologias da Informação e da Comunicação (TICs)
são as melhores e mais nova opção de ensino e aprendizagem sem
necessariamente estar preso a um espaço físico. Desterritorializar,
conforme Santaella (2007) é a palavra mais importante na inovação do
processo de ensino e aprendizagem, utilizando ferramentas virtuais para
potencializar o aprendizado.

Duas ferramentas midiáticas muito usadas no estudo da astronomia é o
Stellarium e a Celestia. Estes são softwares que os discentes poderão
usar para ressignificar seus conhecimentos em relação ao universo, assim
como observar os astros, fazer simulações, entender como se manifestam
os fenômenos celestes no espaço, as fases da lua, distância entre os
planetas, galáxias, e outros registros que a olho nu seria impossível.
Ressaltamos que esses softwares são livres, gratuitos e é possível fazer
downloads para qualquer sistema operacional.

Saviani (2011) defende que inovação é o que se opõe ao tradicional, é
utilizar outras formas, é utilizar a experiência educacional a serviço
de novos questionamentos, finalidades e experiências. Ou seja, a
inovação é vista por Saviani como mudança planejada com objetivo de
melhoria na qualidade do ensino e aprendizagem. De forma semelhante,
para Leite (1999), a inovação mobiliza uma diferente ação da usual. Já
para Ferreti (1989), inovar significa introduzir mudanças de forma
planejada, visando produzir uma melhora da ação educacional. Assim,
inovação parte de uma intenção deliberada de modificação a partir de uma
organização diferente da usual.

Os recursos tecnológicos, quando bem utilizados, oferecem todos os meios
possíveis para melhorar a qualidade de ensino e aprendizagem, através de
ações eficazes e bem planejadas. Como afirma Papert (1994):


> A mesma revolução tecnológica que foi responsável pela forte necessidade
de aprender melhor oferece também os meios para adotar ações eficazes.
As tecnologias de informação, desde a televisão até os computadores e
todas as suas combinações, abrem oportunidades sem precedentes para a
ação a fim de melhorar a qualidade do ambiente de aprendizagem \[...\].
(PAPERT, 1994, p. 6)


O termo tecnologia é uma palavra composta de origem grega, formada por
*techne* e *logos.* *Techne* significa arte, técnica ou ofício, e para
os gregos era conhecimento prático que objetivava um fim concreto;
*logos* significa corpo de conhecimento, conjunto de saberes. A
combinação dessas palavras diferenciava um simples fazer com um fazer
com raciocínio. A partir do século XIX, a tecnologia passou a
configurar-se como conhecimento e, atualmente, sua associação com o
conhecimento científico a tornou indissociável da ciência. Assim Lévy
(1995), define a tecnologia como sendo um conjunto de atividades
humanas, um processo de desenvolvimento, uma forma de vida vinculada ao
acervo cultural de um povo.

Durante a construção da pesquisa foi analisada as possibilidades que as
tecnologias dos arduinos^®^ e embarcados poderiam proporcionar através
da plataforma Google For Education^®^ em particular o Google Drive^®^,
por ser uma plataforma gratuita (até 15 G), que oferece vantagem em
aplicá-la não apenas no intuito de modernização da educação, mas
sobretudo conscientemente das possibilidades de novas estratégias
facilitadora para estudantes e professores.

A Google For Education^*®*^ surge como uma ferramenta disruptiva do
processo ensino e aprendizagem no contexto escolar. Segundo Mugnol
(2009) pesquisar e aplicá-la é uma tática de modernizar as antigas
metodologias, porém é necessário implementar novas estratégias
pedagógicas que melhor enfatize a necessidade de trabalhar com conteúdos
socialmente relevantes, ancorado a teoria mais significativa às
realidades dos estudantes.

Para o docente, essa é uma ferramenta que propõem uma inovação nas
práxis educacionais, com inúmeras vantagens evidenciadas no processo de
ensino e aprendizagem, conforme reforçado por Aruquipa, Chávez e Reyes
(2016) ao apontarem cinco principais vantagens: configuração fácil;
economia de tempo; melhora da organização; melhora para comunicação;
acessível e seguro. Nas palavras dos próprios autores:


> Google Apps tem todas as ferramentas que necessitam os centros
educacionais para serem produtivos, \[...\] todo o mundo pode trabalhar
de forma conjunta em qualquer dispositivo ou momento, é um pacote de
ferramentas de produtividade gratuito para auxiliar em sala de aula.
(ARUQUIPA; CHÁVEZ; REYES, 2016, p. 20-21)


Para Oliveira (2010) as tecnologias midiáticas assim como o Google For
Education*^®^* oferecem soluções inovadoras que podem contribuir com a
educação, atendendo às novas perspectivas da sociedade contemporânea
digital. Para Castells (2013) as tecnologias midiáticas podem contribuir
para dialogar os conhecimentos formais e os meios sociais, em especial
as comunidades endógenas; todavia, é válido ressaltar que os cenários
educacionais produtivos não requerem apenas implementação da tecnologia,
mas também a formação dos envolvidos e a mudança de postura da
comunidade escolar mediante a nova metodologia de ensino.

Com a inserção da tecnologia, espera-se que os professores possam
engajar os alunos no processo de traçar estratégias que os levem do
conhecimento prévio a novas criações. Durante essa construção, será
possível contribuir para ampliação do repertório de ciência e
movimentar-se pelas diferentes ferramentas midiáticas. As tecnologias
devem ser um objeto de ensino e não somente uma ferramenta de ensino.

É válido salientar que, no Brasil, há uma tendência em se utilizar
robótica nos ensinos médio e fundamental e, com a consolidação da Base
Nacional Comum Curricular - BNCC (BRASIL, 2018), ficou mais evidenciado
na atuação dos programas curriculares de Ciências Naturais. Na busca por
favorecer a implementação dessas inovações, é possível se valer de
diferentes estratégias, dentre elas destacam-se a utilização de novas
tecnológicas cada vez mais presentes em nosso cotidiano como, por
exemplo, o computador.

Algumas literaturas referem-se ao arduino^®^ na concepção de robótica,
embora o seu uso não se resuma apenas à construção do robô, mas também à
construção de instrumentos pedagógicos para estudar fenômenos naturais,
e essa construção é mais uma estratégia que o professor pode usar na
difusão de conhecimento, especialmente no âmbito escolar. Ou seja, "As
novas tecnologias podem reforçar a contribuição dos trabalhos
pedagógicos e didáticos contemporâneos, pois permitem que sejam criadas
situações de aprendizagens ricas, complexas, diversificadas" (PERRENOUD,
2002, p. 139).

Diante da necessidade de atender às novas demandas educacionais da
sociedade contemporânea, as tecnologias, aliadas às metodologias, estão
auxiliando o professor em suas práticas diárias dentro e fora do
ambiente escolar. Quando se trabalha robótica, as Metodologias Ativas
contribuem para a aprendizagem significativa e ampliam o conhecimento
dos estudantes; a partir de atividades programadas, os indivíduos
experienciam, compreendem e associam o que aprendem com a realidade na
qual vivem; para uma aprendizagem significativa, portanto, é fundamental
que o planejamento apresente uma sintonia entre os saberes escolares e
os conhecimentos prévios.

Vale ressaltar que as Metodologias Ativas servem como recurso didático,
como ferramenta que estimula o aluno a pesquisar, refletir e analisar, a
partir de sua vivência. Para Moran (2018), é importante que a
metodologia acompanhe os objetivos a serem alcançados. Assim como os
materiais devem ser relevantes para o contexto social do estudante, ao
professor cabe identificar elementos motivadores que provoquem o
envolvimento e o engajamento. Contudo, é imprescindível a elaboração de
"\[...\] atividades grupais e pessoais de aprendizagem, cooperativa e
competitiva de aprendizagem, tutorada e autônoma, com tecnologias
próximas da vida dos alunos" (MORAN, 2018, p. 3).

No contexto escolar, o uso da robótica (arduino^®^), considerando o
exposto por Moran, com base na Metodologia Ativa, estimula o
desenvolvimento do raciocínio lógico, torna o currículo escolar mais
atrativo, fortalece o trabalho em equipe, incentiva o protagonismo
estudantil, promove o aprendizado multidisciplinar e desenvolve a
criatividade.

As Metodologias Ativas são práticas de enfretamento ao modelo antigo e
tradicional consolidado por muito tempo no contexto escolar. Essa se
mostra de importância visto que a nova conjuntura social exige que o
aluno se torne protagonista no processo de construção de seu
conhecimento, sendo responsável pela sua trajetória e pelo alcance de
seus objetivos, no qual deve ser capaz de autogerenciar e autogovernar
seu processo de formação.

## Uso do arduíno^®^ no estudo das marés 

A proposta de estudar a influência da lua sobre as marés é indispensável
à compreensão da natureza cosmológica. Parece ser raro encontrar uma
pessoa que não se encante com algum conteúdo astronômico, seja olhando o
céu, seja com as perguntas mais comuns do dia-dia. Conforme Longhini
(2014), a astronomia foi, talvez, o primeiro estudo distinto a
incorporar a aplicação da matemática e de ciências. Além disso, é um
tema que oferece múltiplas abordagens interdisciplinares: história,
mitologia, literatura, ecologia, música e outros, e representa a busca
da humanidade pelo autoconhecimento (BARCELOS NETO, 2001).

Para o estudo dos fenômenos físicos da maré, o uso de espaços não
formais e as ferramentas midiáticas é uma estratégia para construção de
uma educação científica. Segundo Cunha (2009), a escola por si só não é
capaz de desenvolver uma educação científica e transmitir todo
conhecimento ao estudante, sendo assim, os espaços não formais e o uso
de tecnologia facilitaram o estudo, a observação e a problematização dos
fenômenos físicos de maneira mais sólida.

Para analisar os fenômenos geofísicos da maré, uma das alternativas
midiáticas é o uso do arduino^®;^ estes são micros programadores
responsáveis por converter (ou traduzir) informações coletadas do
ambiente em que estão inseridos em sinais elétricos. Assim, informações
como luminosidade, temperatura, pressão, distância, umidade relativa
atmosférica, entre outros, são convertidas em sinais elétricos que por
sua vez são interpretados e/ou armazenados em ciberespaços (OLIVEIRA,
2010).

O estudo da astronomia desperta nas pessoas vários questionamentos e com
isso nasce a curiosidade de como o universo foi formado e qual a nossa
participação nessa maravilhosa engrenagem celeste, por este motivo, ela
possui qualificação de alto nível no processo de ensino-aprendizagem.
Para Soler e Leite (2012), a astronomia se apresenta como oportunidade
que o docente tem em explorar várias áreas do conhecimento e extrapolar
sua disciplina, com isso levar o estudante ao universo de curiosidade,
inquietação e prazer.

Para compreensão da astronomia, é importante a inserção da tecnologia no
processo de construção do conhecimento; ela levará o estudante
compreender melhor, através de software, e aumenta sua capacidade
cognitiva (DIAS; RITA, 2008, p. 56). A implementação da Base Nacional
Comum Curricular e o ensino da astronomia em colaborativa com estudo das
marés nas séries finais do ensino fundamental, é uma proposta ousada e
inédita que favorece com louvor essa temática (BRASIL, 2018). Embora a
interação da tecnologia com o conhecimento em prol do desenvolvimento
social ainda não se constitua como uma prática pedagogia no ensino
fundamental, ela pode contribuir de forma inovadora para resolver
problemas epistemológicos e sociais. Para Antonio Santos (2005), essa
proposta de pesquisa promove um novo modelo de produção da ciência e da
aplicação da tecnologia em prol do desenvolvimento social.

### A interação entre o sol, a terra, a lua e a as marés 

O estudo das marés constitui um complexo campo de pesquisa na
astronomia, ela faz parte do cotidiano das pessoas, principalmente as
que residem nas proximidades do mar, embora, na sua maioria, sejam
moradores com pouca formação acadêmica (DIEGUES, 1983). Entretanto, eles
conseguem relacionar a maré ao movimento do sol e da lua, a partir do
comportamento cíclico dos astros, além de sincronizar os saberes com o
comportamento regular das marés. Esse conhecimento popular tem garantido
a sua sobrevivência (KULESZA, 1998).

As marés são alterações cíclicas do nível das águas do mar,
influenciadas pelos efeitos do movimento de rotação da terra, somado à
força gravitacional do sol e da lua. Embora o sol seja um corpo com
maior massa, sua força gravitacional é duas vezes menor em relação à
força gravitacional lunar devido à lua ter maior proximidade da terra.

A maré é um fenômeno periódico relacionado com os movimentos
sincronizados que envolvem sol, Terra e lua. O movimento que envolve os
três entes celestes possibilita a observação sistemática e,
consequentemente, aferir o comportamento das marés, como também concluir
algumas hipóteses com relação à interação gravitacional. Contudo, essa
analise é apenas o resultado final de uma complexa engrenagem
fenomenológica que ocorre em conjunto com peculiaridade geográfica de
cada *lócus* da pesquisa. As inferências, desde Aristóteles até os dias
atuais, são sinônimo de fascínio e nos conduzem a questionar a sua
influência no cotidiano das pessoas, plantas e seres aquáticos; embora
até mesmo exista uma ramificação da astronomia que cuida desta temática.

Para calcular as forças que atuam no mar, é necessário considerar apenas
o sistema Terra-lua, coberta uniformemente com água, razoavelmente sem
muita profundidade em relação ao raio do planeta.

Desde antiguidade, já se conhecia as fases da lua e a sua influência nas
marés, assim como o ciclo de pouco mais de vinte nove dias que muda a
sua posição. Em sua obra intitulada "Fases da lua", Aristóteles descreve
corretamente todas as fases. Segundo Horvath (2008), esses conhecimentos
foram herdados por Aristóteles e se devem a Anaxágoras, filósofo que
viveu séculos IV a.C; esses conhecimentos foram muito importante para os
gregos, isto porque a dinâmica da sociedade Grega estava baseada nas
fases da Lua. Conforme cita Horvath:


> Esta regularidade permitiu a confecção dos primeiros calendários,
baseados no mês lunar, e resultou de utilidade na contagem de tempos
importantes, por exemplo, das safras agrícolas. Tradicionalmente
reconhecem-se quatro fases denominadas Nova, Crescentes, Cheia e
Minguante, mas isso negligencia o fato de que a lua muda de aspecto
todos os dias assim a vemos, em geral, num aspecto intermediário entre
duas fases subseqüentes (HORVATH, 2008, p. 36).


Embora já se conhecesse as fases da lua, o interesse estava nas
previsões místicas, fortalecimento de grupos religiosos, agricultura,
navegação e deslocamento social, com isso a astronomia contribuiu além
da confecção de calendários e mapas, para a previsão de fenômenos; até
então, não havia um estudo que relacionasse as fases da lua com as
marés. Seleuco de Selêucia (190-150 a.C), filósofo e astrônomo grego,
seguidor da teoria heliocêntrica difundida por Aristarco de Samos,
considerava que seus argumentos em relação ao movimento da Terra-sol
estavam corretos, porém para ele atmosfera interferia nas marés através
dos movimentos da terra e da lua (HORVATH, 2008).

Enquanto que, para Posidônio (135-51 a.C), em seus relatos no texto
intitulado "Paradoxo", faz um questionamento entre os dois poços de sua
casa e o comportamento de subir e descer das marés. Embora sua obra
tenha observações regulares com relação ao comportamento das marés, ele
não faz referências aos entes celestes. Para ele, o fluxo e refluxo do
mar não tinham nenhuma relação com as fases da lua (HORVATH, 2008).

O mais conhecido dos astrônomos do século II, Cláudio Ptolomeu (90-168
d.C), sua magnífica obra "O almagesto", contribuiu muito para o estudo
da astronomia da época, embora sua teoria fosse geocêntrica; mas foi com
a obra Tetrabiblos que ele registra os fenômenos das marés e
correlaciona a influência das fases da lua e as marés (PINHEIRO;
MACHADO, 2015). Conforme Tetrabiblos:


> "A Lua, por ser o astro mais próximo, distribui sobre a Terra o máximo
de seu refluxo, pois a maioria das coisas animadas e inanimadas está em
sintonia com a Lua e se modifica de acordo com ela. Os rios aumentam e
reduzem seus fluxos devido à sua luminosidade; as marés são modificadas
conforme seus nascimentos e ocasos; as plantas e os animais tornam-se
maiores ou menores, totalmente ou em parte, em consonância com ela".
(PINHEIRO; MACHADO, 2015, p. 312).


Vale ressaltar que o estudo da astronomia, em especial o estudo do
comportamento das marés, é bem mais antigos que os relatos de
Aristóteles (385 a.C - 323 a.C). Segundo Oliveira Filho e Saraiva
(2004), na Ilha de Creta na Grécia foram escavadas lentes similares à
lente de lunetas que datam 2000 a.C. Ele ainda afirma que existem
registros históricos quanto ao uso de óculo desde 13500 a.C. Assim, é
possível considerar que a aferição da lua e de suas fases já acontecem
há mais de 3000 anos. Outro povo que reafirma essa ideia são os Caldeus;
povo semita de origem árabe que ocupou a Mesopotâmia no primeiro milênio
antes de Cristo, já adoravam em seus cultos a deusa lua, pelos atributos
ao fluxo e refluxo das águas, como também ao sucesso nas plantações.

No Brasil, os índios Tupinambás que moravam na Ilha de Itaparica e
outras ilhas já faziam relação das fases da lua com as marés, assim
afirma Ubaldo Osório (1974). Um monge francês chamado Claude
d'Abbeville, enviado pelo governo com um grupo de exploradores para
catequizar os índios, relata em seu livro "Capuchinhos na Ilha do
maranhão" lançado em 1614, em Paris na França, que os Tampinambás faziam
cultos relacionados ao fluxo e refluxo do mar às fases da lua, que esses
índios "conheciam" a influência das fases da lua sobre as marés como
fenômeno da natureza. Esse livro foi lançado dezoitos anos antes de
Galileu fazer sua publicação intitulada "Diálogo" (SOBEL, 2000, p. 147).

A lua é o único satélite natural da terra, e por enquanto o único ente
celeste visitado pelo homem, ela desenvolve três movimentos (Figura
1), translação solar, translação terrestre e
rotação. Uma característica importante é sua rotação ser igual à
translação terrestre, ou seja, completa uma volta em torno de si no
mesmo tempo que completa uma revolução em torno da terra. Com isso vemos
sempre a mesma face da lua, e a outra face ficará invisível para terra,
conhecida erroneamente como o lado escuro.


<center>
<p>Figura 2: Órbita da Terra e da Lua (fora de
escala).</p>
<img src="../imagens/imagem-cap-19-02.png" style="width: 75%; height: auto;"/>
<br><small>
Fonte: Autoria própria.
</small>
</center>


A lua é único satélite natural e visível aqui da terra, sabe-se desde a
antiguidade que o ciclo se repete em aproximadamente 29,5 dias.
Aristóteles conseguiu construir uma explicação correta para a fase da
lua. Esse conhecimento permitiu o calendário lunar e com isso contar o
tempo para safra agrícola; passados 2400 anos, as fases da lua continua
como referência para algumas comunidades, principalmente as litorâneas.

Durante o movimento de rotação e de translação executado pela lua em
torno de si e da terra, sua forma varia, podemos dizer que ela "muda" de
aspecto todo dia, assim vemos em aspecto intermediário entre duas fases
subsequentes. Contudo, a lua é considerada um corpo iluminado, sua face
depende da luz solar, a contagem do ciclo começa com lua nova, quarto
crescente, lua cheia e quarto minguante.

Vê-se que a relação entre as marés e as fases da lua tem sido
instrumentos de observações pelas antigas civilizações até os dias
atuais, seja ela formal, informal, colaborativa ou até mesmo "amadora",
fato que contribuiu e nas ultimas décadas tem contribuído para
construção da astronomia observacional. Atualmente poucos astrônomos
façam uso de telescópios, lunetas em suas pesquisas, pois com a
facilidade das tecnologias midiáticas, é muito comum o uso de câmaras ou
placas fotográficas acopladas em satélites. Mas vale ressaltar que a
astronomia não se resume apenas a observações, envolve também a análise
de dados.

## Considerações finais 

O presente trabalho teve como premissa pesquisar o uso de arduino^®^
como inserção de Tecnologias da Informação e da Comunicação (TICs) no
estudo dos efeitos gravitacionais sobre as marés em diferentes fases da
lua. Como referencial teórico da pesquisa optou-se pela teoria de
aprendizagem de David Ausubel. Durante a pesquisa, ficou evidenciado que
os pescadores e marisqueiras detêm certos sabres e eles são valores
epistemológicos, religiosos e sociais que garantem a sua identidade.

A integração das Tecnologias Digitais de Informação e Comunicação (TDIC)
nas escolas e comunidades litorâneas é uma necessidade urgente, em favor
de uma aprendizagem condizente com as transformações sociais das últimas
décadas. Nesse sentido, a criatividade e a inovação devem estar
presentes nos currículos das instituições de ensino e, portanto, na
prática dos professores; o efeito de tal integração é um "currículo
vivo", que possibilite a garantia de uma efetiva aquisição de
conhecimentos, com significados para os estudantes.

Ao mesmo tempo em que a emergência dessas tecnologias amplia espaços e
instâncias e abrem possibilidades para implementação de novas soluções e
formas de aquisição de conhecimentos, também suscita a necessidade de
novas abordagens metodológicas.

Entretanto, ainda são poucos os trabalhos de pesquisa acadêmica que
focam na utilização de outros materiais e ferramentas oferecidas pela
atual tecnologia, em especial os recursos inseridos no universo do
arduino^®^. Contudo, foi possível através de fontes bibliográficas,
verificar a possibilidade de dialogar tecnologia e comunidades
epistêmicas. Com isso, foi possível cumprir os objetivos propostos neste
trabalho, assim como ficou em evidencia a necessidade de mais pesquisas
acadêmicas neste potencial estudo da robótica de arduino^®^.

# Referências 

ANTUNES, Celso. **Como transformar informações em conhecimento**. 5 ed.
Petrópolis-RJ: Vozes, 2001.

ABREU, Berenice. **Jangadeiros**: uma corajosa jornada em busca de
direitos no Estado Novo. Rio de Janeiro: Civilização Brasileira, 2012.

ALMEIDA, Fernando José de; FONSECA JÚNIOR, Fernando Moraes. **PROINFO**:
Projetos e Ambiente Inovadores. Brasília: Secretaria de Educação a
Distância, 2000. Disponível em: http://www.dominiopublico.gov.br/download/texto/me002699.pdf. Acesso
em: 05 jun. 2020.

ARUQUIPA, Marcelo G.; CHÁVEZ, Bertha B.; REYES, Ruth. Mejoramiento del
Proceso Enseñanza Aprendizaje Aplicando Herramientas Google. **Revista Investigación y Tecnología**, v. 4, n. 1, p. 19-29, 2016. Disponível em:
http://www.revistasbolivianas.org.bo/pdf/rit/v4n1/v4n1_a05.pdf. Acesso
em: 10 dez. 2019.

AUSUBEL, D.P. **Educational psychology**: a cognitive view. New York,
Holt Rinehart and Winston, 1968.

BACHELARD, Gaston. **A formação do espírito científico**: contribuição
para uma psicanálise do conhecimento. Rio de Janeiro: Contraponto, 1996.

BARCELOS NETO, João. **Mecânica Newtoniana, Lagrangiana & Hamiltoniana**. São Paulo: Ed. Livraria da Física, 2013.

BASTO, Sandra Nazaré Dias. Etnociências na sala de aula: uma
possibilidade para aprendizagem significativa. CONGRESSO NACIONAL DE
EDUCAÇÃO, 2.; SEMINÁRIO INTERNACIONAL DE REPRESENTAÇÕES SOCIAIS,
SUBJETIVIDADE E EDUCAÇÃO, 2., 2013., Curitiba. **Anais** \[\...\].
Curitiba: PUC, 2013, p. 6192-6202. Disponível em:
https://educere.bruc.com.br/CD2013/pdf/10014_5318.pdf. Acesso em: 10
dez. 2019.

BRASIL. \[Constituição (1988)\]. Constituição da República Federativa do
Brasil.

Brasília-DF: Presidência da República, 1988. Disponível em:
<http://www.planalto.gov.br/ccivil_03/constituicao/constituicao.htm>.
Acesso em: 26 de jul. 2019.

BRASIL. **Base Nacional Comum Curricular (BNCC)**. Brasília: DF:
Ministério da Educação, 2018. Disponível em:
http://basenacionalcomum.mec.gov.br/abase/\#fundamental/lingua-portuguesa-no-ensino-fundamental-anos-finais-praticas-de-linguagem-objetos-de-conhecimento-e-habilidades.
Acesso em: 02 jun. 2019.

CALLOU, Ângelo Brás Fernandes. Extensão Rural no Brasil: da modernização
ao desenvolvimento local. **Revue uniRcoop**, v. 5, n. 1, p. 164-183,
2007.

CANDAU, Vera Maria Ferrão. **Educação intercultural e cotidiano
escolar**. Rio de Janeiro: 7 Letras, 2006.

CARNEIRO, Raquel. **Informática na educação**: representações sociais do
cotidiano. 2 ed. São Paulo: Cortez, 2002.

CASTELLS, Manuel. **Redes de Indignação e Esperança**: movimentos
sociais na era da Internet. Rio de Janeiro: Zahar, 2013.

COSTA, Ronaldo Gonçalves de Andrade. Os saberes populares da etnociência
no ensino das ciências naturais: uma proposta didática para aprendizagem
significativa. **Revista Didática Sistêmica**, v. 8, jul./ dez. 2008.

CUNHA, Ana Maria de Oliveira. Ensino de Ecologia em espaços não formais.
CLAE, 3.; CEB, 9., 2009, São Lourenço-MG. **Anais** \[\...\]. São
Lourenço-MG: CEB, 2009. Disponível em:
<http://www.seb-ecologia.org.br/revistas/indexar/anais/2009/resumos_professores/ana_cunha.pdf>.
Acesso em: 20 dez. 2019.

DAGNINO, Renato Peixoto. **Tecnologia Social**: Contribuições
conceituais e metodológicas. 1 ed. Florianópolis: Insular/EdUEPB, 2014.

DIAS, Claudio André C. M; RITA, Josué R. Santa. Inserção da astronomia
como disciplina curricular do ensino médio. **Revista Latino-Americana de Educação em Astronomia**, n. 6, p. 55-65, 2008.

DIEGUES, Antonio Carlos. **Pescadores, camponeses e trabalhadores do mar**. São Paulo: Ática, 1983.

DIEGUES, Antonio Carlos. **Povos e mares**. São Paulo: Nupaub-USP, 1995.

FEYERABEND, Paul. **Contra o Método**. São Paulo: Unesp, 2011.

FREIRE, Paulo. **Pedagogia do oprimido**. 17 ed. Rio de Janeiro: Paz e
Terra, 1987.

FERRETTI, Celso. A inovação na Perspectiva Pedagógica. *In*: GARCIA,
Walter E. **Inovação Educacional no Brasil**: problemas e perspectivas.
São Paulo: Cortez Editora. p. 55-82.

GIL, Antonio Carlos. **Como elaborar projetos de pesquisa**. 4 ed. São
Paulo: Ed. Atlas, 2008.

HORVATH, Jorge E. **O ABCD da Astronomia e Astrofísica**. São Paulo: Ed
Livraria da Física, 2008.

KUHN, Thomas Samuel. **Estrutura das revoluções científicas**.* *2 ed.
São Paulo: Perspectiva, 1987.

KULESZA, Wojciech Andrzej. Ciência e Educação Popular. *In*: COSTA,
Marisa Vorraber (Org.). **Educação popular hoje**. São Paulo, Loyola,
1998.

LEITE, Sérgio Celani. **Escola Rural**: urbanização e políticas
educacionais. São Paulo: Cortez, 1999.

LÉVY, Pierre. **As tecnologias da inteligência**. Rio de Janeiro:
Editora 34, 1995.

LÉVY, Pierre. **A inteligência coletiva**: por uma antropologia do
ciberespaço. 4 ed. São Paulo: Loyola, 2003.

LONGHINI, Marcos Daniel. A Astronomia e o Professor de Física -- Um
Estudo com Licenciandos em Física. Encontro de Pesquisa em Ensino de
Física, 13., 2014, Foz do Iguaçu. **Anais** \[\...\]. Foz do Iguaçu:
SEC, 2014.

MALDONADO, Simone Carneiro. **Pescadores do mar**. São Paulo: Editora
Ática, 1986.

MARX, Karl. **O capital**. 8 ed. São Paulo: Difel, 1982. Livro I, v. 1.

MORAN, José. Metodologias ativas para uma aprendizagem mais profunda.
*In*: BACICH, Lilian; MORAN, José (Org.). **Metodologias ativas para uma educação inovadora**: uma abordagem teórico-prática. Porto Alegre:
Penso, 2018. p. 2-25.

MOREIRA, Marco Antonio; MASINI, Elcie F. Salzano. **Aprendizagem significativa**: a teoria de David Ausubel. 2 ed. São Paulo: Centauro,
2006.

MOREIRA, Marco Antonio; BUCHWEITZ, Bernardo. **Novas estratégias de ensino e aprendizagem**: os mapas conceptuais e o Vê epistemológico.
Lisboa: Plátano, 1993.

MOREIRA, Marco Antnio; MASSONI, Neusa Teresinha, **Interfaces entre teoria de aprendizagem e Ensino de Ciências**. Porto Alegre: UFRGS:
2015.

MOREIRA, Marco Antonio; MASSONI, Neusa Teresinha. **Noções básicas de epistemologias e teorias de aprendizagem**. São Paulo: Livraria da
Física, 2016.

MUGNOL, Márcio. A educação a distância no Brasil: conceitos e
fundamentos. **Rev. Diálogo Educ**., Curitiba, 2009.

OLIVEIRA, Alice Virginia Brito de. O uso das mídias na sala de aula:
resistências e aprendizagens. EPEAL - Encontro de pesquisa em educação
em Alagoas, 2010, Alagoas. **Anais** \[\...\]. Alagoas: EPEAL, 2010.

OLIVEIRA FILHO, Kepler de Souza; SARAIVA, Maria de Fátima Oliveira.
**Astronomia e Astrofísica***.* 2 ed. São Paulo: Livraria da Física,
2004.

OSÓRIO, Ubaldo. **A ilha de Itaparica**. Salvador: Secção Gráfica da
Escola de Aprendizes de Artífices, 1928.

PALFREY, JONH. **Nascidos na era digital**: entendendo a primeira
geração de nativos digitais. Porto Alegre: Grupo A, 2011.

PAPERT, Seymour. **Mindstorms**: children computers and powerful ideas.
New York: Edit. Basic books, 1980.

PAPERT, Seymour. **The Children's Machine**: Rethinking School in the
Age of the Computer. New York: Edit. Basic books, 1993.

PAPERT, Seymour. **A máquina das crianças**: repensando a escola na era
da informática. Trad. Sandra Costa. Porto Alegre: Artes Médicas, 1994.

PERRENOUD, Phillippe. **Aprender a negociar a mudança em educação**:
novas estratégias de inovação. Porto: Edições ASA, 2002.

PINHEIRO, Marcus Reis; MACHADO, Cristina de Amorim. **Cad. Hist. Fil. Ci**., Campinas, Série 4, v. 1, n. 2, p. 301-332, jul.-dez. 2015.

RAMALHO, Cristiano Wellington Noberto. **Pescadores artesanais e o poder público: um estudo sobre a Colônia de Pesca de Itapissuma, PE**. 1999.
Monografia (Graduação em Ciências Sociais) -- Universidade Federal Rural
de Pernambuco, Recife, 1999.

RODRIGUES, Neidson. **Da mistificação da escola à escola necessária**. São Paulo, Ed. Cortez, 1998.

RONCA, Antonio Carlos Caruso. Teorias de ensino: a contribuição de David
Ausubel. **Temas em Psicologia**, n. 3, p. 91-95, 1994.

SALVADOR, Cesar Coll. **Psicologia do ensino**. Porto Alegre: Editora
Artes Médicas Sul, 2000.

SANTAELLA, Lucia. **Navegar no Ciberespaço**. O perfil cognitivo do
leitor imersivo. São Paulo: Paulus, 2004.

SANTAELLA, Lucia. **Linguagens líquidas na era da mobilidade**. São
Paulo: Paulus, 2007.

SANTOS, Antonio Raimundo. **Metodologia científica**: a construção do
conhecimento. Rio de Janeiro: DP&A, 2005.

SANTOS, Boaventura de Souza. **Reinventar a emancipação social**: para
novos manifestos. Rio de Janeiro: Civilização Brasileira, 2005.

SAVIANI, Demerval. **Pedagogia histórico-crítica**: primeiras
aproximações. 11 ed. Campinas: Autores Associados; 2011.

SILVA, Luís Geraldo da. **Os pescadores na história do Brasil**.
Campinas: Papirus, 1993.

SOBEL, Dava. **A filha de Galileu, um relato biográfico de ciência, fé e amor**. São Paulo: Companhia das Letras, 2000.

SOLER, Daniel Rutkowski; LEITE, Cristina. Importância e justificativas
para o ensino de Astronomia: Um olhar para as pesquisas da área.
SIMPÓSIO NACIONAL DE EDUCAÇÃO EM ASTRONOMIA, 2., 2012, São Paulo.
**Anais** \[\...\]. São Paulo, SNEA, 2012. Disponível em:
http://snea2012.vitis.uspnet.usp.br/sites/default/files/SNEA2012_TCO21.pdf.
Acesso em 01 jul. 2019.

VILLAR, Frederico. **A missão do Cruzador "José Bonifácio"** -- os
pescadores na defesa nacional -- a nacionalização da pesca e a
organização dos seus serviços (1919-1923). Rio de Janeiro: Gráfica
Laemmert Limitada, 1945.
