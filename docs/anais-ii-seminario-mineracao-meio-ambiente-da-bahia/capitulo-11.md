
![Legenda](../imagens/capitulo.png)


# **DETECÇÃO DE SÓLIDOS SUSPENSOS A PARTIR DE DADOS ORBITAIS OLI NO ESTUÁRIO DO RIO SUBAÉ, BAÍA DE TODOS OS SANTOS, BAHIA.**

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

<center><h3><em>Cezar Augusto Teixeira Falcão Filho</em>[^1]</h3></center>


[^1]: Universidade Federal da Bahia - cezarfalcaof@gmail.com.

## **Resumo**


O presente trabalho descreve o procedimento
metodológico para detectar e estimar a concentração do Total de Sólidos
Suspensos (TSS) com uso da banda $\lambda_{4}$ (0.63 - 0.69 μm) do sensor OLI a
bordo do satélite Landsat 8. A estimativa dos valores de TSS se deu com
a aplicação de um modelo linear empírico e técnicas de sensoriamento
remoto da cor da água. A análise de resíduos revelou uma baixa variação
para as concentrações estimadas pelo modelo para todos os pontos. Os
resultados indicaram que o procedimento é uma opção viável e de baixo
custo para o monitoramento da qualidade da água do Rio Subaé e da Baía
de Todos os
Santos.


**Palavras-chave**:  Sensoriamento Remoto; Cor da água; TSS.

## **1. Introdução**


O Rio Subaé é um dos três principais afluentes da Baía de Todos os
Santos (BTS) e, apesar de descargas modestas ($4,5 m^{3}/s$), é a segunda fonte mais importante de água doce
e material em suspensão desta baía (CRA, 2004).

Durantes as décadas de 60 até os 3 primeiros anos da década de 90,
funcionou uma fábrica de fundição de chumbo primária na bacia
hidrográfica do Subaé, em Santo Amaro, a qual liberou grandes
quantidades de metais, especialmente Pb e Cd.

Reis (1975) mostrou que as concentrações de Cd e Pb nas águas de Subaé
excederam os limites de tolerância da Organização Mundial de Saúde.
Também foram relatadas altas concentrações de metais traços em
sedimentos e moluscos coletados no estuário de Subaé (Tavares, 1996;
CRA, 2004).

Porém mesmo diante de um problema desta magnitude, os estudos sobre o
material particulado em suspensão na BTS (Moura, 1979; Wolgemuth et al.,
1981; Santos, 2005; Oliveira, 2014) e no Rio Subaé (Hatje et al., 2006)
foram pontuais.

Dessa forma, considerando que a cor das águas costeiras está diretamente
ligada às suas propriedades ópticas inerentes (absorção e espalhamento)
e que estas propriedades variam conforme a concentração, natureza e
tipos de Componentes Opticamente Ativos (COA) (KIRK, 1983), o presente
estudo apresenta a aplicação de um modelo linear para detectar e
quantificar a carga de material sólido suspenso com o uso de dados
orbitais do sensor OLI a bordo do satélite LANDSAT-8.

## **2. Materiais e Métodos**

### 2.1. Seleção e aquisição da imagem de satélite

Foi adquirida gratuitamente 1 imagem Landsat 8 do sensor OLI
(_Operational Land Imager_) através do portal _on line} do
serviço geológico americano - USGS (_U.S. Geological Survey_),
disponível na página: https://earthexplorer.usgs.gov. A imagem escolhida
foi do dia 10/12/2013 por ser a mais próxima dos dados de TSS coletados
_in situ_ no dia 11/12/2013 a fim de validar o modelo.

### 2.2. Processamento Digital


Todo o processamento digital foi realizado através do _software_
Terrset\textsuperscript{@} versão 18.31.

#### 2.2.1. Correção atmosférica

Os valores físicos de reflectância da superfície da água foram obtidos
através do modelo de correção atmosférica denominado de Cos (t) (Chavez,
1996). Esse modelo incorpora todos os elementos do DOS - Dark Objection
Subtraction (para remoção de neblina), porém estima os efeitos da
absorção por gases atmosféricos e espalhamento Rayleigh.


#### 2.2.2. Máscara Booleana

A máscara foi elaborada através do coeficiente normalizado entre as
bandas OLI $\lambda_{3}$ e $\lambda_{5}$. O coeficiente foi proposto por McFeeters (1996) que
o denominou de Normalized Difference Water Index (NDWI) (Equação 1). Seu
resultado é uma imagem cujos pixels oscilam entre -1 a 1 (-1 a 0 para a
terra e de 0 a 1 para a água). Isso permite que a imagem seja
reclassificada gerando uma nova imagem na qual os valores negativos são
transformados em 0 e valores positivos em 1.

$$
\begin{equation} \label{eq_1} 
NDWI = (\lambda_3 -- \lambda_5) / (\lambda_3 + \lambda_5) 
\end{equation}  
$$ 

Onde $\lambda_3$ e $\lambda_5$ representam as bandas 3 e 5 do sensor OLI.**~}

#### 2.2.3. Comprimento de onda $\lambda$  aplicado ao modelo

A banda $lambda_4$ é sensível à reflectância na região do espectro
eletromagnético compreendido entre 0,63 - 0,69 μm. Este intervalo capta
a luz refletida por pigmentos vermelhos, característicos das partículas
inorgânicas em suspensão típicas de águas do Caso 2 (Nichol, 1993). Além
de apresentar uma menor penetração na coluna d'água, até 5m (Green et
al., 2000) em águas oligotróficas, com pouca concentração de COA.

#### 2.2.4. Eliminação de Ruídos nos valores de reflectância}

O filtro mediano 3x3 foi aplicado para remoção de ruído aleatória.

#### 2.2.5. Escalonamento dos dados de reflectância

O arquivo de saída das imagens possuem valores de reflectância, expressa
em formato de número real, com variação de 0 a 1. O modelo linear
aplicado foi calibrado a partir de valores que variavam de 0 a 100. Com
isso foi necessário multiplicar a banda $\lambda_4$ por 10.

#### 2.2.6. Aplicação do Modelo

O modelo aplicado foi desenvolvido através do método da calibração
direta (Acker et al., 2005), por Falcão Filho et al., (2016):

$$
\begin{equation}
Ln(TSS) = 1.258760 + 1.980676 \cdot (L_n (Banda 4) +1)
\end{equation}
$$ 

Onde Ln(TSS) é a concentração de Total de Sólidos Suspenso (mg/l) em
Logaritmo natural na base (e); 1.258760 é o intercepto em $y$; 1.980676 é
o coeficiente angular (ambos constantes numéricas); $\lambda$ é o comprimento de
onda centralizado específico do sensor (Falcão Filho et. al, 2016)

#### 2.2.7. Determinação das concentrações de TSS na imagem

Cada píxel da imagem possui um valor que precisa ser transformado em
valores físicos de concentração de TSS (mg/L). Para isso foi calculado o
_antilog_ natural através do módulo _Transform_. De forma
automática, o módulo calcula o _antilog_ natural de um píxel onde o
mesmo é elevado a uma potência igual àquele número.

$$
\begin{equation}  
_anti}log\textsubscript{b} \cdot  a = x b\textsuperscript{a} = x
\end{equation}
$$ 

### 2.3. Análise de Resíduos

A eficácia da aplicação do modelo foi avaliada usando a análise dos
resíduos. Foi empregada a Equação 4 para calcular os resíduos em cada
ponto (MATOS, 1995).

$$ 
\begin{equation}  
**r} = **a} **â}
\end{equation}
$$ 



Os Resíduos representam a diferença entre o valor observado e o que foi
predito pelo modelo de regressão (MATOS, 1995). Sendo assim **a}
corresponde aos valores reais de TSS e **â** corresponde aos
valores gerados pelo modelo. Os dados de TSS coletados in situ e
utilizados para a análise de resíduos foram disponibilizados pelo
projeto COPPEUFRJ, uma cooperação do grupo de Oceanografia física da
UFBA e UFRJ.

## **3. Resultados e discussões** 

A análise de resíduos revelou que, em todos os pontos, o modelo
superestimou as concentrações de TSS. Todas as diferenças nas
estimativas foram abaixo de 1 mg/L, exceto para os pontos 5 e 9, onde o
modelo apresentou concentrações de 2,32 e 2,84 mg/L. A menor diferença
foi no ponto 7, onde o modelo superestimou em apenas 0,11mg/L. As
maiores diferenças nas concentrações de TSS podem ser explicadas pela
localização do ponto 5 na saída do canal de Itaparica, e do ponto 9 no
canal do Rio Paraguaçu (Figura 1).

O Rio Subaé apresentou valores com uma variação de 0,3 a 18,4mg/L. O
valor máximo foi localizado na desembocadura do estuário na BTS. O valor
mínimo foi localizado no canal fluvial onde ainda foi observado uma
concentração máxima de 9,9mg/L.

Apesar da diferença de um dia entre os dados de TSS e os dados de
reflectância, e considerando ainda a rápida dinâmica comum a ambientes
estuarinos, ambos os conjuntos de dados foram obtidos no mesmo horário e
correspondem a maré de quadratura na preamar.



<center>
<p>Tabela 1: Análise de resíduos entre as concetrações de TSS _in situ_ e do modelo linear.</p> <br> 
<img src="../imagens/capitulo_11_tabela_1.png" style="width: 80%; height: auto;"/><br> 
 
</center> 




<center>
<p>Figura 1: A: modelo da distribuição de TSS na BTS do dia
10/12/2013 com a distribuição dos pontos amostrais de TSS coletados no
dia 11/12/2013 utilizaddos na análise de resíduos. B: Distribuição do
TSS na região da BTS adjacente a desembocadura do Rio Subaé. Valores dos
píxels em mg/L.</p> <br> 
<img src="../imagens/min_29_img.png" style="width: 80%; height: auto;"/><br> 
 
</center> 



## **4. Considerações finais**

As concentrações de TSS estimadas corroboraram com estudos anteriores
que mostraram que a turbidez na BTS é considerada baixa com o aumento
dos valores em direção ao interior, próximo a desembocadura dos Rios, a
exemplo do Subaé. Apesar da baixa superestimativa apresentada pela
análise de resíduos é possível tornar o modelo ainda mais próximo do
real calibrando-o através da aquisição de dados _in situ_
coincidentes com dados orbitais. Esse estudo é inovador para a região e
apresenta baixo custo para o monitoramento da qualidade da água, além de
possibilitar estimavas de TSS até 45 anos no passado.

## **Referências Bibliográficas**


 
ACKER, J.; OUILLON, S.; GOULD, R.; ARNONE, R. Measuring marine suspended
sediment concentrations from space: History and Potential. In:
**8th International Conference on Remote Sensing for Marine and Coastal Environments**, Halifax, NS, Canada, May 17-19, 2005.

 
CHAVEZ, P. S. Image-Based Atmospheric Corrections -- Revisited and
Improved, **Photogrammetric Engineering and Remote Sensing**, 1996.
62, 9, 1025-1036.

 
CRA. **Diagnóstico ambiental do grau de contaminação da baía de todos os santos por metais pesados e hidrocarbonetos**. CRA, Salvador,
2004.


GREEN, E.P.; MUMBY, P.J.; EDWARDS, A.J.; CLARK, C.D. Remote Sensing
Handbook for Tropical Coastal Management. **Coastal Management Sourcebooks**. Paris: UNESCO, p.316, 2000.


 
HATJE, V; BARROS, F.C. R. de ; FIGUEIREDO, D.G.; SANTOS, V.L. C. S.
Trace metal contamination and benthic assemblages in Subaé estuarine
system, Brazil. **Marine Pollution Bulletin**, publicado na web em
2006, v. 52, p. 969-977, 2006.

 
KIRK, J.T.O. Light and photosynthesis in aquatic ecosystems. Cambrige:
**Cambrige Universety Press**, p. 436, 1983.

 
MATOS, M.A. **Manual Operacional para a Regressão Linear**. FEUP.
1995. p 0- 26.

 
McFEETERS, S.K. The use of the Normalized Difference Water Index (NDWI)
in the delineation of open water features. **International Journal of Remote Sensing**, v.17, n.7, p.1425-1432, 1996.

 
MOURA, P. L. **Material em suspensão na Baía de Todos os Santos**.
Dissertação (Mestrado em Geologia). Instituto de Geociências.
Universidade Federal da Bahia, 1979. 49p.

 
NICHOL, J.E. Remote Sensing of Water Quality in the Singapore-Johor-Riau
Growth Triangle. **Remote Sensing of Environment**. v.43,
p.139-148, 1993.

 
OLIVEIRA, W. P. **Dinâmica do material particulado em suspensão no eixo principal da Baía de Todos os Santos**. Trabalho de conclusão de
curso (Graduação em Oceanografia). Instituto de Geociências,
Universidade Federal da Bahia, 2014. 52p.

 
REIS, J.O.N. **Determinação polarográfica de Pb2+ and Cd2+ em a´guas do Rio Subaé, Santo Amaro, Bahia**. Master thesis, Universidade
Federal da Bahia, Brazil, 1975. p. 81.

 
SANTOS, C. B. **Contribuição aos estudos da carga sedimentar em suspensão na Baía de Todos os Santos**. Trabalho de conclusão de curso
(Graduação em Oceanografia). Instituto de Geociências, Universidade
Federal da Bahia, 2005. 47p.

 
TAVARES, T.M. **Programa de monitoramento dos ecossistemas ao norte da Baía de Todos os Santos**, 1996 Relatório Final, Universidade
Federal da Bahia Salvador.

 
WOLGEMUTH, K.; BURNETT, W. e MOURA, P. L. (1981) Oceanography and
suspended materials in Todos os Santos Bay. **Revista Brasileira de Geociências**, 11:172-178.



