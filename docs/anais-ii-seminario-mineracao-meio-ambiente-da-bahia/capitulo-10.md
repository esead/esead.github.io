
![Legenda](../imagens/capitulo.png)


# **DELIMITAÇÃO E AVALIAÇÃO DE IMPACTOS AMBIENTAIS EM ÁREA DE EXTRAÇÃO MINERÁRIA NO MUNICÍPIO DE ITAGIBÁ-BA**

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
<center><h3><em>Bruno Meira Gomes</em>[^1]</h3></center>

<center><h3><em>Juraci Jesus de Santana Junior</em>[^1]</h3></center>

<center><h3><em>Joaquim Custódio Coutinho</em>[^2]</h3></center>

<center><h3><em>Everton Luís Poelking</em>[^1]</h3></center>

<center><h3><em>Diego Sousa Dias dos Santos</em>[^1]</h3></center>


[^1]: Universidade Federal do Recôncavo da Bahia - UFRB, Cruz das Almas,
	BA, E-mail: meira_20bruno@hotmail.com. juraci.sjr@gmail.com. everton@ufrb.edu.br. diegosousa_ds@hotmail.com

[^2]: Universidade Federal do Rio Grande do Norte - UFRN, Macaíba, RN,
	E-mail: joaquimcustodiocoutinho@gmail.com. 


## **Resumo**


A mineração atua de forma direta no crescimento
econômico do Brasil. A Bahia é um dos estados destaque no setor, por sua
diversidade geológica, como do ouro, cobre, níquel, etc. No município de
Itagibá-BA, a Mina de Santa Rita, é a maior descoberta de níquel
sulfetado dos últimos anos, trazendo desenvolvimento para a região.
Entretanto, surgem os impactos socioambientais inerentes a atividade
minerária que necessitam de monitoramento. O trabalho objetivou avaliar
as áreas de extração minerária no município de Itagibá-BA, identificando
as áreas impactadas, através de mapas temáticos, de forma temporal.
Fez-se a análise da área anterior ao início das instalações e após a
exploração via imagens de satélite. As áreas foram quantificadas, e
comparadas quanto a expansão, ao logo dos anos, além de visita in loco.
Houve aumento de 57% na área de exploração da Mina no período de 7
anos.



**Palavras-chave**: Mineração; Extração de Níquel;
Geoprocessamento.


## **Introdução**
	
A mineração funciona como um fator de desenvolvimento econômico
regional. Faz-se necessário que o município com essa atividade adote em
seu Plano Diretor, instrumentos e diretrizes para a gestão e o seu
monitoramento. Apesar da responsabilidade do órgão federal
fiscalizá-las, o município deve se preocupar com o aproveitamento de
seus recursos minerais, com a relação destas atividades com as outras
formas de uso e ocupação do solo, e com a conservação ambiental
(DENÚBIA, 2013).
	
A diversidade geológica do território da Bahia permite a exploração de
aproximadamente quarenta substâncias minerais, com destaque para o
ferro, ouro e cobre, caracterizando o subsolo do estado como um dos
maiores potenciais ainda não explorados pela indústria extrativa
mineral. A produção ocorre no semiárido, nos municípios de Andorinha,
Brumado, Caetité, Campo Formoso, Jaguarari, Jacobina, Santa Luz e
Vitória da Conquista, cuja atividade destes, representa 75% da produção
mineral baiana comercializada no estado (CBPM, 2014).
	
Em Itagibá (Ba), o depósito da Mina Santa Rita constitui a principal
descoberta mundial de níquel sulfetado nos últimos anos. A empresa
Mirabela Mineração iniciou suas operações em 2009 nesta Mina, produzindo
sulfeto de níquel para exportação (50%) e comercializando o restante
para produção metálica no Brasil (TEIXEIRA, 2015).
	
Atrelado a toda essa ascensão é necessário o monitoramento dessa
atividade de extração mineral, das áreas que serão exploradas, sujeitas
a licenciamentos, e as degradadas através do uso do zoneamento
ambiental. Para o monitoramento e caracterização da mina de extração
utiliza-se Sistemas de Informações Geográficas (SIG), efetuando a
delimitação da área da cava de extração e das regiões de depósito de
rejeitos, as vias de acesso e pontos de interesse na área em questão
(Torchetto et al., 2014). Este trabalho tem como objetivo avaliar
impactos ambientais em área de extração minerária no município de
Itagibá-BA, identificando as áreas de cava, exposição do solo e
rejeitos, fornecendo informações geográficas sob a forma de mapas
temáticos das áreas impactadas, de forma temporal.

	
## **2. Material e Métodos**

A mina de Santa Rita da Mirabela Mineração do Brasil trata-se de uma
mineradora localizada a 15 km da zona urbana do município de Itagibá-BA,
no sudeste do Estado da Bahia, a 14° 16' 57'' Sul, 39° 50' 46'' Oeste
(Figura 1). Com população estimada em 15.193 habitantes, e área de 788,8
km². Fisiograficamente inserido no domínio do bioma Mata Atlântica, e na
bacia hidrográfica do Rio de Contas, de relevos planos a suavemente
ondulados, altitudes de aproximadamente 150m e elevações topográficas
arredondadas de 350 a 400m (Lazarin, 2011). A economia do município
baseia-se na mineração de níquel e atividade agropecuárias, tendo o
cacau e a pecuária (leite e corte) como as de grande importância.

%Figura 1 -- Localização da Mina de Santa Rita, Fazenda Mirabela,
%Itagibá-BA




<center>
<p>Figura 1: Localização da Mina de Santa Rita, Fazenda Mirabela, Itagibá-BA.</p> <br> 
<img src="../imagens/min_26_img.png" style="width: 80%; height: auto;"/><br> 
<small>Fonte: LAZARIN, 2011.</small> 
</center> 



O minério explorado é o níquel, explorado em cava a céu aberto com
início de operação em 2009, obtendo ao município a maior arrecadação do
CFEM na Bahia. A estrutura compreende também uma usina de concentração
via flotação (britagem - moagem - flotação - espessamento - filtragem)
para o processamento do minério que é lavrado na mina, utilizado nas
operações da Planta de Beneficiamento, e estocado nas áreas destinadas
às pilhas de~_Run of Mine_ -- ROM (MATTA, 2016).

### 2. 1 Processamento digital de imagens

Fazendo uso das imagens implemetadas no programa _Google Earth_,
foi selecionada a área de estudo, com a imagem do ano de 2007
identificando o periodo anterior ao início das explorações da mina
(2009). Através da imagem do satélite _RapidEye_ de 2011,
observou-se o avanço no uso e ocupação do solo. Para a criação do mapa
de divisão de áreas para análise ambiental, foram utilizadas imagens do
satélite _PlanetScope_ atualizadas (2018) com resolução espacial de
3 m, e processadas no _software_ _ArcGis_ 10.3, identificando
as áreas de influência a serem trabalhadas, quantificando o tamanho da
área submetida a exploração através da delimitação de polígono no fomato
_shapefile_, bem como, a divisão das áreas distintas.

## **3. Resultados e Discussão**

A barragem de rejeitos da Santa Rita, localiza-se na entrada da mina
(Figura 2), a uma distância aproximada de 1km do Rio de Contas e à sua
margem direita (montante-jusante). A curta proximidade entre ambos,
aumenta a apreensão da população local e a responsabilidade da empresa
no que diz respeito a segurança da barragem, sendo importante ressaltar
que qualquer vazamento ou rompimento pode pôr em risco ambiental não só
pontualmente a região, mas todo o litoral sul baiano.

%Figura 2 -- Área total impactada pelas instalações e pelas cavas de
%exploração no ano de 2011 e 2018 respectivamente.





<center>
<p>Figura 2: Área total impactada pelas instalações e pelas cavas de exploração no ano de 2011 e 2018 respectivamente.</p> <br> 
<img src="../imagens/min_27_img.png" style="width: 80%; height: auto;"/><br> 
<small>Fonte: LAZARIN, 2011.</small> 
</center> 




É identificado o aumento significativo das cavas, perante o avanço das
explorações minerárias, consequentemente dos depósitos de estéril e
barragem de rejeito (Tabela 1).



<center>
<p>Tabela 1: Área total impactada dos anos 2011 e 2018.</p> <br> 
<img src="../imagens/capitulo_10_tabela_1.png" style="width: 80%; height: auto;"/><br> 
 
</center> 


Foi identificado através do uso do solo na área da exploração, 8 (oito)
classes distintas, descritas conforme seu uso e estado atual analisadas
pelas imagens de satélite, e, mediante visita a mineradora (Figura 3). O
fato de não possuir os limites da Mirabela Mineração, a vegetação não
foi mensurada, sendo executada apenas a sua classificação, como também
uma abordagem das diretrizes ambientais que a empresa desenvolve.



<center>
<p>Figura 3: Zoneamento das áreas para análise ambiental (2018).</p> <br> 
<img src="../imagens/min_28_img.jpg" style="width: 80%; height: auto;"/><br> 
<small>Fonte: LAZARIN, 2011.</small> 
</center> 




Na Tabela 2, estão descritas as áreas, os tamanhos em hectares (ha) de cada classe e a porcentagem (%), respectivamente.



<center>
<p>Tabela 2: Áreas impactadas pelas instalações e pelas cavas de exploração no ano 2018.</p> <br> 
<img src="../imagens/capitulo_10_tabela_2.png" style="width: 80%; height: auto;"/><br> 
 
</center> 



O aumento das cavas são característicos, estando diretamente
relacionados ao volume do depósito e barragem de rejeito. A Mirabela
realiza a recomposição de áreas de empréstimos e construções, de forma a
evitar focos erosivos e de assoreamento, atuando na recuperação,
simultaneamente ao desenvolvimento da mineração, das áreas inertes das
pilhas de estéril, das cavas e recomposição, onde possível, da cobertura
vegetal.


## **4. Considerações finais**

- Durante o período de 2011 a 2018, houve o aumento de 57% na área de
exploração da Mina de Santa Rita;

- A mineração é uma atividade determinante para o desenvolvimento
econômico, no entanto, as consequências socioambientais inerentes a ela
carecem de atenção e monitoramento;

- Nesse aspecto, a promoção de programas que mitiguem seus impactos
negativos é o caminho para o desenvolvimento sustentável.

- A empresa cumpre mediante a legislação as condicionantes
estabelecidas.

## **5. Referências Bibliográficas**


CBPM. COMPANHIA BAIANA DE PESQUISA MINERAL. 2014. **Oportunidades em Negócios Minerais da CBPM**. Coord. Hélio C. Azevedo. Salvador: CBPM.


DENÚBIA, L. A. **Alterações ambientais associadas à mineração no município de São Carlos (SP), utilizando AHP e SIG**. 2013. (Dissertação
de Mestrado) -- Escola de Engenharia de São Carlos da Universidade de
São Paulo, 2013.


LAZARIN, F. A. **Geologia, Petrologia e Estudos Isotópicos dos Depósitos de Níquel-Cobre Sulfetados Santa Rita e Peri-Peri, Nordeste do Brasil**. 2011. (Dissertação de Mestrado). -- Instituto de Geociências,
universidade de Brasília -- UNB, 2011.


MATTA, G. N. **Extração de níquel contido em rochas ultramáficas do depósito de Santa Rita (Bahia)**. 2016. (Dissertação de Mestrado --
Programa de pós-graduação em engenharia industrial) -- Universidade
Federal da Bahia, Escola Politécnica, 2016.


TEIXEIRA, J. B. G. **Minério de Níquel Sulfetado no Brasil. Recursos Minerais no Brasil: problemas e desafios**. Capítulo I:
Potencial Mineral do Brasil. 116 p. 2014.


TORCHETTO, N. L.; QUEIROZ, R.; PEYROT, C.; PATATT, E. R.; LANGNER, C.
H.; OCHOA, L; KOPPE, E. O uso do Quantum Gis (QGIS) para caracterização
e delimitação de área degrada por atividade de mineração de basalto no
município de Tentente Portela (RS). **Revista do Centro do Ciências Naturais e Exatas -- UFSM**. Santa Maria-RS. 2236 1170 - V. 18
n. 2, p.719-726, Mai-Ago 2014.