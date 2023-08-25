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

<p style="text-align:center"><span style="font-size:18px">La cantidad de accesos de internet fijo por rango de velocidad</span></p>

<p style="text-align:center"><span style="font-size:16px">***************</span></p>

<p style="text-align:center"><span style="font-size:16px">Se observa que a nivel nacional la cantidad de accesos a velocidades mayores a 30Mb crece mientras que en el caso de velocidades menores la tendencia es bajista, esta tendencia se corresponde con la evolucion de las tecnologias de conexion a internet ya que con la implementacion de nuevas tecnologias las velocidades crecen y al mismo tiempo la demanda aumenta segun los precios por el servicio disminuyen.</span></p>

<p style="text-align:center">&nbsp;</p>

<p style="text-align:center"><span style="font-size:18px">La cantidad de accesos por tecnologia de internet fijo&nbsp;</span></p>

<p style="text-align:center"><span style="font-size:18px">***************</span></p>

<p style="text-align:center">&nbsp;</p>

<p>&nbsp;</p>

<p style="text-align:center">&nbsp;</p>

<p>&nbsp;</p>

<p>&nbsp;</p>

<p style="text-align:center">&nbsp;</p>

<p style="text-align:center">&nbsp;</p>