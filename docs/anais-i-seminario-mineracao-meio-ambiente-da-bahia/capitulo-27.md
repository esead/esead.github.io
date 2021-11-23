
![Legenda](../imagens/capitulo.png)


# **CADASTRO ESTADUAL FLORESTAL DE IMÓVEIS RURAIS: PROCEDIMENTO SEMIAUTOMÁTICO DE COLETA E PROCESSAMENTO DE DADOS**

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

<center><h3><em>Marcos Roberto Santos Correia</em>[^1]</h3></center>

<center><h3><em>Danívio Batista Carvalho de
Vasconcellos</em>[^2]</h3></center>

[^1]: CCAAB, UFRB, marcos_roberto9974@hotmail.com.

[^2]: CETEC, UFRB, danivio@ufrb.edu.br.

RESUMO:} O Código Florestal (CF) Lei 12.651/12 que rege as ações
de regularização ambiental, o qual criou, no âmbito do Sistema Nacional
de Informação sobre Meio Ambiente (SINIMA), o Cadastro Ambiental Rural
(CAR), registro eletrônico obrigatório a todos os imóveis rurais, tem
por finalidade unificar informações ambientais das propriedades e posses
rurais do país. Na Bahia, o CAR vem sendo implementado desde 2012,
denominado Cadastro Estadual Florestal de Imóveis Rurais (CEFIR),
previsto na Lei Estadual nº 10.431, de 20 de dezembro de 2006. O CAR
atende aos requisitos preconizados pelo código florestal, nesse estado
inclui a solicitação de autorizações referentes ao licenciamento
ambiental e à outorga de uso dos recursos hídricos. O CEFIR é um Sistema
de Informações Geográficas operado por meio da internet (WEBGIS),
chamado Sistema Estadual de Informações Ambientais e de Recursos
Hídricos (SEIA), para realizar o cadastro dos imóveis rurais no sistema
é necessário ter conhecimento da legislação ambiental, geoprocessamento,
cartografia, uso da terra, e de softwares de geoprocessamento, para
gerar peças técnicas exigidas. O objetivo do trabalho é apresentar uma
metodologia de geração das peças técnicas para o CEFIR, por intermédio
da estruturação de um procedimento semiautomático integrado a um Sistema
de Informações Geográficas (SIG). Os procedimentos desenvolvidos foram
implementados e validados em mais de 500 imóveis rurais localizados nos
municípios de Valença, Jaguaripe e Taperoá. Na coleta dos dados
georreferenciados são utilizados equipamentos receptores GNSS de alta
sensibilidade para representar o perímetro do imóvel, uso da terra e das
restrições legais por meio de atributos relacionados a cada ponto e
identificados por siglas para agilizar o processo de aquisição. Na fase
de processamento de dados foi utilizado o software QGIS, versão 2.18. Um
banco de dados padronizado é criado para receber as informações
espaciais e de atributos dos limites e de informações ambientais de cada
imóvel rural, representados em duas camadas. Os limites são traçados
utilizando apenas os pontos que contém a informação de limite e
aplicando um procedimento de vetorização automática a partir do
_plugin Points2One_. São filtrados os pontos de cada tipo de uso
para realizar os recortes dos polígonos dos diferentes usos da terra, o
que evidencia um processo de vetorização semiautomática, as restrições
de uso são elaboradas utilizando ferramentas de geoprocessamento,
especialmente o _Buffer_, que cria faixas marginais para as feições
que apresentam algum tipo de restrição prevista no CF e são utilizadas
como referência para o recorte na camada de uso da terra. Posteriormente
é feito o preenchimento das informações de atributos, adaptados ao que é
solicitado no CEFIR. Ao fim do processo, são geradas as peças técnicas
(shapefile) conforme são solicitados no SEIA, a exemplo do Limite do
Imóvel, APP, RL, Áreas de Vegetação Natural e Produtiva. Destaca-se que
o procedimento aplicado, além de ser uma solução prática e operacional
de atendimento à legislação ambiental, permite a geração e informações
de alta qualidade e estrutura um banco de dados georreferenciados com
potencial de contribuir com o planejamento agroambiental das regiões
onde é implementado.

**Palavras-chave**: Cadastro Ambiental Rural, Sistema de
Informações Geográficas, Mapeamento.