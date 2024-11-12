Prácticas de aula 9 (PA09): Teoría de la biogeografía insular en la
bibliografía, herramientas precursoras de la TBI<small><br>Biogeografía
(GEO-131)<br>Universidad Autónoma de Santo Domingo (UASD)<br>Semestre
2024-02</small>
================
El Tali
2024-11-12

Versión HTML (quizá más legible),
[aquí](https://biogeografia-master.github.io/biogeografia-insular-en-bibliografia/README.html)

# **Fecha/hora de entrega**

**18 de noviembre de 2024, 23:59 pm.**

# Introducción

Diseñé esta asignación para que explores el tema de **“teoría de la
biogeografía insular” o “teoría de la biogeografía de islas”** (TBI)
abordado en clase por medio revisión de publicaciones. La idea es
revisar trabajos científicos sobre cómo, aplicando metodologías
específicas, se ha podido comprobar o refutar la teoría de la
biogeografía de islas y/o sus bases en investigaciones recientes. Son
válidas las publicaciones donde se usen técnicas estadísticas,
cartográficas o de muestreo, así como filogenias y genómica, para
someter a escrutinio la TBI. Por otro lado, te incluí también un
ejercicio sobre modelos de relación especies-área y especies-abundancia,
que fueron algunos de las herramientas ecológicas usadas para formular
la TBI.

# Objetivos

1.  Analizar la aplicación de la TBI mediante la búsqueda y síntesis de
    un artículo científico en la bibliografía disponible y abierta,
    aplicando habilidades de lectura crítica y capacidad de síntesis
    para identificar resultados que comprueben o refuten la teoría.

2.  Analizar datos de incidencia o abundancia para aplicar técnicas de
    asociación entre área-especies o abundancia-especies, como
    herramientas precursoras de la TBI.

# Ejercicio 1. TBI en la bibliografía. Busca y resume artículo

Este ejercicio se puede hacer en el aula sin mayores complicaciones
dentro del aula.

## Instrucciones

1.  **Encuentra un artículo científico** sobre la aplicación de la TBI,
    que implique el uso de una (o varias) metodología expresamente
    declarada y especificada, que pueden incluir técnicas estadísticas,
    técnicas cartográficas, técnicas de muestreo, filogenias o genómica.
    Otras características deseables del artículo a elegir:

    - Referido a RD o la isla; si no es posible, entonces que sea de
      ámbito Caribeño (insular o continental).
    - Puede estar escrito en inglés o español.

2.  **Realiza un resumen escrito:** escribe un resumen en tus propias
    palabras de no más de 250 palabras sobre el trabajo encontrado.
    Deberás presentarlo oralmente en clase, con un tiempo de 5 minutos.

3.  **Citación:** cita el artículo de manera adecuada utilizando el
    formato APA.

# Ejercicio 2. Asociación entre área-especies o abundancia-especies, como herramientas precursoras de la TBI

Busca datos y evalúa la distribución de Preston o la relación
especies-área (Arrhenius, Gleason, Gitay, Lomolino, etc.)

Este ejercicio, si bien se puede hacer en el aula, es más idóneo hacerlo
en una pantalla más grande que la de un celular. Por tal razón, esta
práctica de aula tiene un plazo de entrega mayor que el habitual.

## Instrucciones

1.  Busca registros de incidencia de GBIF (si eliges la relación
    especies-área), o datos de abundancia (si eliges la relación
    especies-abundancia). Los registros de incidencia (presencia de
    especies) de GBIF son muy accesibles, aunque no son exhaustivos. Por
    otra parte, los datos de abundancia son escasos. Si conoces algún
    *dataset* en el cual se contabilice, por sitios, el número de
    individuos por cada especie, entonces úsalo. De lo contrario, si no
    conoces ninguno, dispones de [esta
    opción](https://github.com/biogeografia-master/scripts-de-analisis-BCI/tree/master/biodata),
    donde cada archivo `.Rdata` es una matriz de comunidad basada en
    datos de abundancia (es decir, conteo de individuos).

2.  Sube el *dataset* al servidor de RStudio, usa las funciones del
    paquete `vegan` correspondientes (`prestondistr`, `prestonfit`,
    `veiledspec` `SSarrhenius`, `SSgleason`, `SSgitay`, `SSlomolino`,
    `SSmicmen`) para obtener los parámetros de las funciones de ajuste
    y, en el caso de Preston, el número de especies veladas. Necesitarás
    usar la ayuda de estas funciones para aplicarlo a tu caso.

3.  Extrae tus conclusiones en un párrafo que sintetice tu objetivo, la
    técnica y datos empleados (citar la fuente y la ruta desde donde los
    descargaste), el pequeño código que hayas usado, los resultados
    obtenidos, la interpretación del resultado obtenido y las
    conclusiones/implicaciones.

> Nota sobre los modelos de relación especies-área, en concreto, el caso
> de Arrhenius.

> En el caso del modelo de Arrhenius para la relación especie-área,
> obtener los parámetros y aplicar el método permite comprender y
> cuantificar cómo cambia la riqueza de especies (número de especies) en
> función del área de estudio. Esto es útil porque:

> Interpretación ecológica: Los parámetros ajustados, como la constante
> y el exponente, reflejan la tasa de cambio en la riqueza de especies a
> medida que se incrementa el área, lo que proporciona información sobre
> la estructura y la diversidad del ecosistema. Por ejemplo, un
> exponente alto sugiere que la riqueza de especies aumenta rápidamente
> con el área, lo que puede indicar alta diversidad o un ecosistema
> heterogéneo.

> Predicciones y extrapolaciones: Con los parámetros del modelo, puedes
> predecir cuántas especies esperarías encontrar en áreas no
> muestreadas, lo que es útil en conservación y gestión de la
> biodiversidad.

> Comparaciones entre hábitats: Al comparar los parámetros de diferentes
> áreas o ecosistemas, puedes identificar patrones y comparar la
> biodiversidad entre regiones o tipos de hábitats. Esto es clave para
> estudios de biogeografía y ecología comparada.

> Ajuste y validación de teorías: El modelo de Arrhenius también sirve
> para probar la teoría de la biogeografía de islas, que sugiere que la
> relación especie-área es una función generalizable en muchos sistemas.
> Ajustar el modelo permite ver si tus datos se alinean con esta teoría.

> Aplicación en conservación: Los parámetros obtenidos ayudan a estimar
> los efectos de la fragmentación del hábitat en la pérdida de
> biodiversidad, ya que el modelo puede predecir cuántas especies
> podrían perderse si se reduce el área disponible.

# Materiales

Para esta práctica, en principio, solo necesitarías papel y lápiz, así
como algún dispositivo con conexión a Internet, que te permita tanto
acceder al servidor de RStudio (e.g. una tableta, una PC, tu teléfono
móvil) como consultar recursos bibliográficos, buscar artículos y datos
fuente.

También dispones del libro de la asignatura (citado al final), y de la
[presentación de
diapositivas](https://biogeografia-master.github.io/tema-9-biogeografia-insular/index.html)
del tema “Biogeografía insular”.

# Entregable

- Documento, que puede ser escrito a mano, o electrónico, en formato PDF
  o en tu procesador de texto favorito. IMPORTANTE: no es obligatorio,
  en esta práctica, generar un cuaderno reproducible RMarkdown.

# Referencias

Lomolino, M.V., Riddle, B.R, Whittaker, R., Brown, J.H. (2010).
Biogeography. Fourth Edition. Sinauer Associates, Inc.
