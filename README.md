# Proyecto-Individual-2

# <h1 align="center">**`Informe sobre el Comportamiento de las Telecomunicaciones a Nivel Nacional`**</h1>
Análisis Estratégico Claro

# Descripción del proyecto
Este repositorio contiene el Dashboard desarrollado en Power BI Desktop para el análisis estratégico de las telecomunicaciones en Argentina, con foco en los accesos a internet. El informe visualiza tendencias históricas, participación por tecnologías, objetivos de crecimiento y cobertura geográfica, usando los últimos datos abiertos de ENACOM del 2do trimestre de 2024.

# Objetivos principales:

- Analizar la evolución de los accesos por tecnología (ADSL, Cablemodem, Fibra Óptica) a través del tiempo.

- Medir el KPI obligatorio: crecimiento mínimo de 2% de accesos por cada 100 hogares por provincia en el próximo trimestre.

- Proponer y visualizar tres KPIs adicionales: participación de Fibra Óptica en el AMBA, cuota de mercado de Fibra óptica y cuota de mercado de Cablemodem por provincia.

- Identificar oportunidades de despliegue y mejora en provincias menos saturadas.

🗂️ Estructura del repositorio
**`EDA:`**
Importe las librerías Pandas, Matplotlib y Seaborn. Del Excel importé las hojas elegidas, use la función .head() para verificar que todo ande bien, y la función .info() para traer información general. Revisé valores Nulos y los encontré en la tabla de Dial Up en la columna homónima, sin embargo no fue necesario tratarlos ya que eran datos que no iban a complicar el análisis ni el dashboard. En Accesos por Tecnología se marcaban como nulos unos valores que correspoden a una nota dejada en el Excel la cuál no tiene valor por lo cuál eliminé esas últimas dos filas. Use la función .describe() para obtener más información de las tablas. Usé un Boxplot para verificar si hay outliers en la tabla de Totales Accesos por Tecnología. Para las demás tablas, los datos traídos del AMBA resaltaban demasiado, por lo cuál decidi no buscar outliers ahí ya que la disparidad entre el Capital y Provinica de Buenos Aires, y las demás provincias es demasiada. Lo que sí, revise que porcentaje del total de Accesos de Banda Ancha y Dial Up provenían del AMBA, donde pudimos ver que la mitad se concentran en esta zona. Luego, verifique la distribución del uso de las diferentes tecnologías analizando la tabla "Totales Accesos por Tecnología" con la información del último trimestre. Luego, hicimos un gráfico de lineas que nos permitia ver la evolución del uso de las diferentes tecnologías a traves del tiempo. Y por último otro gráfico de lineas que nos permitio ver la evolución de la penetración cada 100 hogares por Provincia a traves del tiempo. Y la conclusión.

**`Dashboard:`**
En nuestro Dashboard se puede ver en la primera página la presentación, donde abajo se puede acceder a un navegador de páginas que nos llevara a las páginas que desiemos, por otro lado también aparece la fuente de la información, en el pie de página. En la página "Accesos por Tecnología" podremos ver distintos graficos, el primero nos mostrara la evolución de las diferentes tecnologías a traves del tiempo a nivel nacional, el segundo, un KPI que nos muestra el porcentaje de Accesos a Fibra óptica que pertenecen al AMBA. Y por otro lado, el tercero y cuarto son el porcentaje de participación de la fibra óptica y cablemodem (respectivamente) por provincia sobre el total de las tecnologías. En la página de Accesos cada 100 Hogares, en la derecha superior tenemos un segmentador de botones con el cuál podemos elegir que Provincia revisar, a la izquierda superior hay un grafico que muestra la evolución de la penetración por hogares a través del tiempo. A la derecha inferior hay dos etiquetas donde se muestra el acceso actual y el acceso objetivo. Y a la izquierda inferior un grafico comparativo entre el acceso actual y el acceso objetivo.
