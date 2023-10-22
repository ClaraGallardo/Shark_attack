![Imagen local](https://www.tonica.la/__export/1671505182718/sites/debate/img/2022/12/19/jaws.jpg_463833556.jpg)


##SHARK ATTACK:##

Dividiremos el proyecto en tres partes principales:

	1.ANALISIS PREVIO
	2.LIMPIEZA
	3.RESULTADOS Y CONCLUSIONES	

#OBJETIVOS.

Conocer los lugares donde mas ataques hay, actividades que pueden influir y mortalidad.
La mortalidad esta relacionada con la especie o actividad? y con el sexo, hay mayor supervivenvia?
Los ataques tienen relación según el momento del día?
Dependiendo del lugar, hay mas ataques?



1. ANALISIS PREVIO:

-Dimensiones
-Indices
-Tipo de dato

**Observaciones:

- 3 columnas con archivos y enlaces:

    - ¿Hay que tener en cuenta? 'pdf', 'href formula', 'href'. Como no se pueden borrar las dejare por si me hacen falta

- 'original order' información:
    - revisar si es necesaria la información aportada por la columna. Revisar si debe convertirse en el índice del df.

-Quitamos los espacios finales de 'Sex y Species para poder buscarlo mas comodamente. Fatal (Y/N) lo ponemos solo como Fatality.

-Convertimos Year de float a int

2.LIMPIEZA:

-Valores nulos: 

Las columnas Unnamed: 22 y Unnamed: 23 las paso a 0 directamente porque son casi totalmente nulas.

-Valores duplicados:

Ninguno

-Valores constantes:

No hay😒 pero tiene sentido, hay poco dato numerico

Vamos a chequear que verdaderamente no haya y no sea porque el dato tenga alguna


-Outliner. No tiene sentido buscarlos ya que cada dato es de su padre y su madre 🤦‍♀️

-Limpieza e valores de colmnas, le damos caña al regex 🥊🥊🥊.

Usando value-counts.head() o .tail() o unique() podemos apreciar por columnas cuales valores se han repetido mas y podemos darlos por válidos o corregirlos.
Nos fijamos en los que aparecen una vez ya que tienen mas papeletas para que sean errores o estén mal escritos y haya que arreglarlos.

Principlalmente nos fijaremos en las columnas que nos interesen para lograr nuestos objetivo.

Para Sex , insertamos en M y F los valores que tienen pinta de pertenecer al mismo sexo unasdo el condicional 'where'
Hacemos lo mismo con Fatality.

Para Activity, hay que currarselo mas porque tienen muchas discrepancia pero hayq eu tener en cuenta que la misma actividad de expresa de diferentes maneras asi que las filtramos con una funcion usando regex para hayar los patrones y añadirlos a un diccionario que luego aplicaremos dentro de la columna . Currao currao 💪💪💪

Para Country, voy a quitar las NORTH, SOUTH, EAST, WEST así lo generalizo un poco. Con .unique() veo que hay espacios al principio de los paises,los quito. Pongo todo en mayúsculas y quito ? por aprox.

Para Type, voy a corregir un poco pero como es mas general para el objetivo mejor usar la colunad de Activity,es mas específico.

Para Year, quito los número raros (0,555,7,...) y lo dejo todo como 0000. 

Area y Location no los voy a corregir, hay muchisimas variaciones y poco tiempo 😭.


Una vez terminada la limpieza se han optimizado los tipos de datos y guardado el fichero en un csv nuevo.

![Imagen local](https://scontent.fmad6-1.fna.fbcdn.net/v/t31.18172-8/17834913_1060299644104591_6076313270153662717_o.jpg?_nc_cat=106&ccb=1-7&_nc_sid=9b3078&_nc_ohc=QV2e9p7K84IAX9IZL01&_nc_ht=scontent.fmad6-1.fna&oh=00_AfClLiIJqJArq0Rhe6s_2u24LMXs1KXD1D3_ZW5Bp_wEEA&oe=655CF1E8)


# ANALISIS Y CONLCUISONES










