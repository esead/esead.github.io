
![Legenda](../imagens/capitulo.png)


# **MAPEAMENTO PRELIMINAR DOS SOLOS DE SANTO AMARO -- BA, USO DE CONHECIMENTO ESPECIALISTA E ÁLGEBRA DE MAPAS**

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

<center><h3><em>Ícaro Barreto Souza</em>[^1]</h3></center>

<center><h3><em> Oldair Del'Arco Vinhas Costa</em>[^2]</h3></center>

<center><h3><em> Everton Luís Poelking</em>[^3]</h3></center>



[^1]: Estudante de Graduação UFRB, icaro@ufrb.edu.br. 

[^2]: Professor da UFRB, oldair@ufrb.edu.br.

[^3]: Professor da UFRB, everton@ufrb.edu.br.

\section*{Resumo}

\noindent
 O recurso natural solo encontra-se no ambiente em uma
zona de interseção entre diversos outros recursos, apresenta-se como
fator crucial para a manutenção da homeostase do meio físico.
Sistematizar informações sobre solos é uma tarefa complexa devido à
enorme variação dos seus atributos e da distribuição espacial. Diante
disso o presente trabalho teve por objetivo unir a aplicação de técnicas
computacionais com métodos tradicionais de levantamento de solos para
gerar um mapa da distribuição espacial da cobertura pedológica em Santo
Amaro/BA. Foram identificadas no município 17 unidades de mapeamento
compostas por associações ou unidades simples, e 19 diferentes classes
de solos, onde predominam: ARGISSOLOS, LATOSSOLOS, VERTISSOLOS e
GLEISSOLOS.


\noindent
\textbf{Palavras-chave}: Solos, Álgebra de mapas, Sig.


\vspace{-0.7cm}
\section*{1. Introdução}


Sistematizar informações sobre os solos é uma tarefa complexa, visto que
o recurso apresenta uma enorme variação de atributos e de distribuição
espacial. Diante disso, faz-se necessário o uso de técnicas que permitam
a obtenção e validação de dados dos solos de forma eficaz e precisa. A
aplicação de ferramentas computacionais aliadas à Ciência do Solos
possibilita que umas vastas gamas de técnicas sejam empregadas às
informações do solo, gerando produtos cada vez mais especializados e com
alta precisão. Neste contexto, o presente trabalho aplicou técnicas de
modelagem matemática e de sintaxe computacional, unindo dados legados de
solos e bases cartográficas digitais, sob a supervisão de um Pedólogo
especialista, para gerar um mapa preliminar de solos do município de
Santo Amaro em escala 1:50.000, equivalente à um levantamento de
reconhecimento de alta intensidade.

\section*{2. Materiais e Métodos}

O material básico utilizado consistiu em: levantamento exploratório de
solos (BRASIL,1981); dados do conjunto de \emph{pedons} (CARVALHO,2001;
SILVA,2004; BONFIM, 2015; SOUZA,2014); modelo digital de elevação (INPE,
2011); imagem de satélite (ESRI); mapa geológico do estado da Bahia
(CPRM,2003); mapa geológico da região metropolitana de Salvador
(CPRM,2008); mapa divisão político administrativa da Bahia
(SEI-BA,2018).

O método utilizado para execução do presente trabalho consistiu, na
aplicação da álgebra de mapas em dados matriciais de variáveis do modelo
s.c.o.r.p.a.n, relacionadas ao material de origem e relevo, para
predição da distribuição espacial das classes de solo em Santo Amaro/BA.
Foi executada uma função condicional em que as regras operacionais foram
definidas por um Pedólogo a partir do conhecimento prévio da área de
estudo, e uso de dados de perfis pedológicos.

Através de uma revisão bibliográfica foram selecionados um conjunto de
dados de perfis pedológicos que já haviam sido levantados por outros
autores na área de estudo FIGURA \eqref{img34}.

%Figura 1: Conjunto de \emph{pedons}





\begin{figure}[!htb]
	\centering
	\includegraphics[scale=0.65]{Imagens/min_38_img.png}
	\caption{ Conjunto de \emph{pedons}.}\label{img38}
	%fig_08 no trabalho original
	%\small{Fonte: \textcolor{red}{Não identificamos fonte da imagem}.}
\end{figure}




Os dados de relevo foram gerados através do modelo digital de terreno
TOPODATA (INPE,2011), do qual extraiu-se as camadas de declividade e
altitude.




Para geração da camada correspondente ao material de origem foram
utilizados os vetores dos mapas de geologia (CPRM 2003, 2008). Foi
realizado um ajuste entre as bases cartográficas, com objetivo de
preencher vazios de informação, e padronizar as escalas. Os mapas foram
fundidos, e através da vetorização manual com suporte de informações de
campo, imagens de satélite e modelo numérico do terreno, foi feito novo
delineamento das unidades.

\newpage 

Um conjunto de regras foi construído para descrever a distribuição
espacial da cobertura pedológica no município. Esse modelo sintetiza o
conhecimento de campo do Pedólogo, estruturado com base em estudos,
observações de campo e coleta de dados, executados pelo profissional em
diversos trabalhos realizados na área. Grande parte dessas informações
advém de análises pontuais realizadas ao longo de toda área do
município, descrições da morfologia de perfis pedológicos e estudos de
topossequências.

As regras preditoras foram aplicadas às camadas de covariáveis através
da função condicional na calculadora raster do módulo \emph{Spatial
	Analyst} do ArcGIS 10.2, utilizando operadores relacionais
(\textless{};=;\textgreater{}) e de lógica booleana (\&) estruturados
uma sintaxe computacional que correlacionava o material de origem e sua
posição no relevo através dos dados de elevação e declividade. A partir
da aplicação do algoritmo foi gerado o arquivo matricial com o
delineamento das diferentes unidades de mapeamento dos solos.

%Figura 2. Aplicação da álgebra de mapas.


\begin{figure}[!htb]
	\centering
	\includegraphics[scale=0.35]{Imagens/min_39_img.png}
	\caption{Aplicação da álgebra de mapas.}\label{img39}
	%fig_08 no trabalho original
	%\small{Fonte: \textcolor{red}{Não identificamos fonte da imagem}.}
\end{figure}




\section*{3. Resultados e Discussão}

Foram identificadas 17 unidades de mapeamento e 19 diferentes classes
identificadas a partir do método utilizado. Predominam no município as
ordens dos: ARGISSOLOS, VERTISSOLOS, LATOSSOLOS e GLEISSOLOS. Outras
ordens que ocorrem em manchas menores são: CAMBISSOLOS, NEOSSOLOS e
PLANOSSOLOS. O Mapa de Solos gerado está representado na FIGURA \eqref{img40}.

%Figura 3. Mapa preliminar de solos Santo Amaro - BA



\begin{figure}[!htb]
	\centering
	\includegraphics[scale=0.45]{Imagens/min_40_img.png}
	\caption{Mapa preliminar de solos Santo Amaro - BA.}\label{img40}
	%fig_08 no trabalho original
	%\small{Fonte: \textcolor{red}{Não identificamos fonte da imagem}.}
\end{figure}







\section*{4. Conclusão}

A aplicação da função condicional através da álgebra de mapas mostrou-se
um método preditor eficiente e de fácil execução.

Foram identificadas no município 17 unidades de mapeamento compostas por
associações ou unidades simples, e 19 diferentes classes de solos.

ARGISSOLOS, LATOSSOLOS, VERTISSOLOS e GLEISSOLOS são as ordens que
ocupam as maiores áreas no município.

\section*{Referências Bibliográficas}

\retirarecuo
BOMFIM, M.R. \textbf{Características de ecossistemas manguezais
contaminados por metais traços. Salvador}, UFBA, Instituto de
Geociências, 2014. 107p. (Tese Doutorado).

\retirarecuo
BRASIL. Ministério das Minas e Energia. Secretaria Geral.
\textbf{Projeto RADAMBRASIL} Folha SD. 24 Salvador: Geologia,
geomorfologia, pedologia, vegetação e uso potencial da terra.
MME/SG/Projeto RADAM BRASIL, Rio de Janeiro, 1981.

\retirarecuo
CARVALHO, C.C.N. de. \textbf{Gênese e transformação de solos em um
tabuleiro do Recôncavo Baiano.} Salvador, UFBA, Instituto de
Geociências, 2001. 116p. (Dissertação Mestrado).

\retirarecuo
CPRM -- Companhia de Pesquisa de Recursos Minerais. \textbf{Materiais de
construção civil na região metropolitana de Salvador.} Gonçalves, J. C.
V; Moreira, M.D; Borges, V. P. Salvador: CPRM, 2008. 53p. (Informe de
Recursos Minerais. Série Rochas e Minerais Industriais, 2). Programa
Geologia do Brasil - PGB.

\retirarecuo
CPRM -- Companhia de Pesquisa de Recursos Minerais. \textbf{Mapa
geológico do estado da Bahia.} Versão 1.1. Souza, J. D. de; Melo, R. C.
de; Kosin, M. (Coords.). Salvador: CPRM, 2003. Escala 1:1.000.000.

\retirarecuo
INPE -- INSTITUTO NACIONAL DE PESQUISAS ESPACIAIS. \textbf{Banco de
Dados Geomorfométricos do Brasil.} Topodata. s.d. Disponível em:
\textless{} http://www.dsr.inpe.br/topodata/dados.php\textgreater{}.
Acesso em: 10 de ago. 2014.

\retirarecuo
SEI. Superintendência de Estudos Econômicos e Sociais da Bahia.
\textbf{Divisão Político-Administrativa do Estado da Bahia-Vetor}.
Versão1.Salvador: SEI-BA, 2018.Escala: 1:100.000.

\retirarecuo
SILVA, D.B. \textbf{Estratificação e diagnóstico de ambientes do
assentamento rural Nova Suissa, Santo Amaro/Bahia -- com ênfase na
análise dos solos.} Salvador, UFBA, Instituto de Geociências, 2004.
153p. (Dissertação Mestrado).

\noindent
SOUZA, J. P. de. \textbf{Caracterização de solos de uma topossequência,
em área contaminada por rejeitos de mineração de chumbo}. Cruz das
Almas, UFRB, Solos e Qualidade de Ecossistemas, 2014. 38p. (Dissertação
Mestrado).





