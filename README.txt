## PROYECTO ##

SHARK ATTACK:

Dividiremos el proyecto en tres partes principales:

	1.ANALISIS PREVIO
	2.LIMPIEZA
	3.RESULTADOS Y CONCLUSIONES	

#OBJETIVOS.

Conocer los lugares donde mas ataques hay, actividades que pueden influir y mortalidad
La mortalidad esta relacionada con la especie o actividad? y con el sexo, hay mayor supervivenvia?
Los ataques tienen relación según el momento del día?
Dependiendo del lugar, hay mas ataques?



1. ANALISIS PREVIO:

-Dimensiones
-Indices
-Tipo de dato

**Observaciones:

- columnas con más valores nulos:



- 3 columnas con archivos y enlaces:

    - ¿Hay que tener en cuenta? 'pdf', 'href formula', 'href'

- 'original order' información:
    - revisar si es necesaria la información aportada por la columna. Revisar si debe convertirse en el índice del df.



2.LIMPIEZA:

-Valores nulos: 

Las columnas Unnamed: 22 y Unnamed: 23 las borro directamente porque son casi totalmente nulas.

-Valores duplicados
-Valores constantes:

No hay😒 pero tiene sentido, hay poco dato numerico

Vamos a chequear que verdaderamente no haya y no sea porque el dato tenga alguna


-Outliner. No tiene sentido buscarlos ya que cada dato es de su padre y su madre 🤦‍♀️

-Limpieza e valores de colmnas, le damos caña al regex 🥊🥊🥊.

Usando value-counts.head() o .tail() podemos apreciar por columnas cuales valores se han repetido mas y podemos darlos por válidos.
Nos fijamos en los que aparecen una vez ya que tienen mas papeletas para que sean errores o estén mal escritos y haya que arreglarlos.








