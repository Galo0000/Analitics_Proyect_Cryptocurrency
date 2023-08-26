<h1 style="text-align:center"><strong>Analisis exploratorio de datos de criptomonedas</strong></h1>

<p><span style="font-size:18px">En este informe se analizaran las criptomonedas mas rentables a pedido de la empresa x la cual a solicitado un an&aacute;lisis exhaustivo utilizando datos de la API CoinGecko para entender mejor el mercado de criptomonedas y presentar tus hallazgos y recomendaciones en un informe detallado.</span></p>

<h2><strong><span style="font-size:26px">Herramientas:</span></strong></h2>

<p><span style="font-size:20px">Python 3.8.13:&nbsp;Es un lenguaje de programaci&oacute;n vers&aacute;til y de alto nivel, con caracteristicas esenciales para el analisis de datos.</span></p>

<p><span style="font-size:20px">Librerias: </span></p>

<ul>
	<li><span style="font-size:18px">Pandas: Una libreria para an&aacute;lisis y manipulaci&oacute;n de datos en Python.</span></li>
	<li><span style="font-size:18px">NumPy: Una libreria para procesamiento num&eacute;rico en Python.</span></li>
	<li><span style="font-size:18px">Seaborn: Una libreria de visualizaci&oacute;n de datos en Python basada en Matplotlib.</span></li>
	<li><span style="font-size:18px">Power BI:&nbsp;Herramienta de visualizaci&oacute;n de datos de Microsoft.</span></li>
</ul>

<p><strong><span style="font-size:26px">Estructura de carpetas</span></strong></p>

<p><span style="font-size:20px">Data: Contiene los datasets en extencion csv que se utilizaran.</span></p>

<p><span style="font-size:20px">EDA: Archivo con extencion ipynb con el desarrollo de EDA.</span></p>

<p><span style="font-size:20px">Extrac_data:&nbsp;Archivo con extencion ipynb donde se extraen los datos de la api y se realizan el ETL.</span></p>

<p>&nbsp;</p>

<p><span style="font-size:26px"><strong>Descripci&oacute;n del Proyecto</strong></span></p>

<p style="text-align:center">&nbsp;</p>

<p style="text-align:center"><strong><span style="font-size:28px">EDA</span></strong></p>

<p style="text-align:center">&nbsp;</p>

<p style="text-align:center"><span style="font-size:18px">El EDA (An&aacute;lisis Exploratorio de Datos) es una t&eacute;cnica utilizada en ciencia de datos para explorar, analizar y comprender los datos antes de realizar an&aacute;lisis m&aacute;s avanzados. Ayuda a identificar patrones, detectar anomal&iacute;as y obtener informaci&oacute;n relevante para investigaciones posteriores.</span></p>

<p style="text-align:center"><span style="font-size:18px">Se seleccionaron varios datasets despues de un analisis de la informacion que muestra cada uno de ellos tratando de seleccionar los mas representativos a los objetivos del proyecto.</span></p>

<p><span style="font-size:18px">En primera instancia se utiliza la api de coingecko solicitada por el cliente, extrae la informacion que se considera importante para el analisis y se adecua la base de datos en un proceso de ETL. Como resultado se obtienen dos bases de datos:</span></p>

<p><span style="font-size:18px">all_coins: Contiene datos de 250 monedas ordenadas segun su capitalizacion en el mercado.</span></p>

<p><span style="font-size:18px">exhanges: Contiene datos de 250 echanges ordenados segun un rankin proporcionado por la api.</span></p>

<p><span style="font-size:18px">Se responderan preguntas basicas que serviran como guia para el analisis.</span></p>

<p>&nbsp;</p>

<p style="text-align:center"><span style="font-size:18px">Que monedas?</span></p>

<p style="text-align:center"><span style="font-size:16px">***************</span></p>

<p style="text-align:center"><span style="font-size:16px">Para responder esta pregunta se analizara la base de datos all_coins con los siguientes datos:</span></p>

<p style="text-align:center">&nbsp;</p>

<p><span style="font-size:16px">id: Identificacion de la moneda en la api.</span></p>

<p><span style="font-size:16px">symbol: Synbologia utilizada para identificar la moneda.</span></p>

<p><span style="font-size:16px">name: Nombre completo de la moneda.</span></p>

<p><span style="font-size:16px">current_price: Precio actual de la criptomoneda en dolares.</span></p>

<p><span style="font-size:16px">market_cap: Capitalizacion en el mercado representado en dolares.</span></p>

<p><span style="font-size:16px">market_cap_rank: Rankin de capitalizacion en el mercado segun la api.</span></p>

<p><span style="font-size:16px">fully_diluted_valuation: Valor total de mercado te&oacute;rico de una criptomoneda en circulaci&oacute;n.</span></p>

<p><span style="font-size:16px">total_volume: Cantidad total de la criptomoneda que ha sido intercambiada en todos los mercados.</span></p>

<p><span style="font-size:16px">circulating_supply: Cantidad total de esa criptomoneda que actualmente est&aacute; en manos de los inversores y el p&uacute;blico en general.</span></p>

<p><span style="font-size:16px">max_price: Precio maximo que alcanzo historicamente.</span></p>

<p><span style="font-size:16px">min_price: Precio minimo que alcanzo historicamente.</span></p>

<p><span style="font-size:16px">last_updated: Fecha de actualizacion de los datos.</span></p>

<p>&nbsp;</p>

<p><span style="font-size:16px">Se analizaran las 10 monedas con mas capitalizacion en el mercado ya que es un indicador de confianza en la criptomoneda. En este ranking no se tendran en cuenta aquellas criptomonedas que tengan pariedad con el dolar ya que no son utilizadas en el mercado para generar ganancias considerables.</span></p>

<p style="text-align:center"><img alt="" src="https://github.com/Galo0000/Analitics_Proyect_Cryptocurrency/blob/main/Images/top10crip.jpg" /></p>

<p style="text-align:center">&nbsp;</p>

<p style="text-align:center"><span style="font-size:18px">En que exchange?&nbsp;</span></p>

<p style="text-align:center"><span style="font-size:18px">***************</span></p>

<p style="text-align:center"><span style="font-size:18px">Que es un exchange?</span></p>

<p style="text-align:center"><span style="font-size:16px">Es una plataforma en l&iacute;nea que permite a los usuarios comprar, vender e intercambiar diferentes criptomonedas.</span></p>

<p style="text-align:center">&nbsp;</p>

<p style="text-align:center"><span style="font-size:16px">Se utilizara la base de datos del archivo&nbsp;exhanges.csv&nbsp;con los siguientes datos:</span></p>

<p><span style="font-size:16px">id: Nombre que utiliza la api de coingecko para identificar el exchange<br />
name: Nombre del exchange</span></p>

<p><span style="font-size:16px">year_established: A&ntilde;o en que se fundo el exchange.</span></p>

<p><span style="font-size:16px">country: Pais donde opera el exchange.</span></p>

<p><span style="font-size:16px">trust_score: Puntuacion del 1 al 10.</span></p>

<p><span style="font-size:16px">trust_score_rank: Rankin del exchange.</span></p>

<p><span style="font-size:16px">trade_volume_24h_btc: Volumen de operaciones de bitcoin que se hicieron en la ultimas 24hs.</span></p>

<p><span style="font-size:16px">trade_volume_24h_btc_normalized: Es similar al trade_volume_24h_btc que mencion&eacute; anteriormente, pero con la diferencia de que el volumen se normaliza en funci&oacute;n del precio actual de Bitcoin.<br />
<br />
Esta base de datos como en el caso anterior tambien cuenta con un rankin de exchange pero se analizaran otros aspeactos de las mismas.</span></p>

<p style="text-align:center"><span style="font-size:16px">Cantidad de exchange que se fundaron segun a&ntilde;o</span></p>

<p>&nbsp;</p>

<p style="text-align:center"><img alt="" src="https://github.com/Galo0000/Analitics_Proyect_Cryptocurrency/blob/main/Images/exhange_year.jpg" /></p>

<p>&nbsp;</p>

<p><br />
<span style="font-size:16px">En el a&ntilde;o 2018 se fundaron mas exchanges que en las demas fechas, esto podria tener explicacion por lo que paso con bitcoin que en ese mismo a&ntilde;o tuvo su primera gran gran correccion en el precio.</span></p>

<p style="text-align:center"><span style="font-size:16px">Cantidad de exchange que se albergan por pais</span></p>

<p>&nbsp;</p>

<p style="text-align:center"><img alt="" src="https://github.com/Galo0000/Analitics_Proyect_Cryptocurrency/blob/main/Images/echange_country.jpg" /></p>

<p>&nbsp;</p>

<p><span style="font-size:16px">En este grafico se puede ver la cantidad de exchanges que alberga cada pais, observando una gran cantidad en&nbsp;Seychelles que es un archipi&eacute;lago, frente a africa oriental. Este resultado puede estar condicionado por la libertades economicas y normativas</span></p>

<p>&nbsp;</p>

<p style="text-align:center"><span style="font-size:16px">Este cuadro agrupa por paises y suma el Volumen de operaciones de bitcoin normalizado de los exchanges.</span><br />
&nbsp;</p>

<p style="text-align:center"><img alt="" src="https://github.com/Galo0000/Analitics_Proyect_Cryptocurrency/blob/main/Images/sumcap_country.jpg" /></p>

<p>&nbsp;</p>

<p>&nbsp;</p>

<p>&nbsp;</p>

<p style="text-align:center"><span style="font-size:16px">En este apartado de explicaran los kpi utilizados:</span></p>

<p style="text-align:center"><span style="font-size:16px">KPI: es una medida cuantificable que se utiliza para evaluar el rendimiento</span></p>

<p><span style="font-size:16px">Porcentaje de crecimiento de Market_cap por a&ntilde;o: Es el porcentaje de crecimiento que a tenido una criptomoneda con respecto de un promedio anual de sus precios mensuales.</span></p>

<p><span style="font-size:16px">Promedios moviles: Es una t&eacute;cnica estad&iacute;stica utilizada para suavizar una serie de datos, lo que facilita la identificaci&oacute;n de tendencias y patrones a lo largo del tiempo.</span></p>

<p><span style="font-size:16px">Patrones de Volumen de Operaciones: Valida una tendencia teniendo en cuenta el volumen de transacciones.</span></p>

<p><span style="font-size:16px">tasa de crecimiento de la capitalizaci&oacute;n de mercado: Proporciona informaci&oacute;n sobre c&oacute;mo ha cambiado la capitalizaci&oacute;n de mercado de un activo</span></p>