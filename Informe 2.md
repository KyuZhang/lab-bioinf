# Laboratorio nº2: Alineamiento de secuencias #
Marcelo Araya Yáñez

----------
### Parte 1: Colectar secuencias homólogas ###
El gen **SRY** codifica para la proteína TDF (testis-determining factor), la cual da comienzo a la determinación sexual primaria masculina.  
En la base de datos de NCBI se tiene registro de **25 genes ortólogos** con el gen SRY de humano.  
Se compilaron las 26 secuencias en un archivo de texto que puede encontrarse [**aquí**](https://github.com/KyuZhang/lab-bioinf/blob/master/Lab%2002/Secuencias%20SRY.txt).

----------
### Parte 2: Alineamiento de secuencias ###
El EMBL-EBI es el Instituto de Bioinformática Europeo. En este ofrece una variedad de herramientas, entre las cuales se pueden encontrar herramientas para busqueda de secuencias similares para secuencias de nucleótidos y proteínas, análisis funcional de proteínas, reconocimiento de motivos de secuencia y herramientas para alineamiento de secuencias.  
En EMBL-EBI se pueden realizar alineamientos de secuencias en pares y alineamientos múltiples.  
El sitio de EMBL-EBI ofrece **MUSCLE** como una herramienta de alineamiento de secuencias especialmente buena para proteínas.  

En **MAFFT** el costo de abrir un gap es de **1.53**, mientras que el costo de extender un gap es de **0.123**.  
EL alineamiento obtenido en MAFFT tiene una longitud de 1900 nucleótidos.

En el árbol filogenético se puede observar que el gen SRY más cercano al humano es el de *Chlorocebus sabaeus* (mono verde), mientras que el más alejado es el de *Equus przewalskii* (caballo de Przewalskii), que a su vez es el más cercano al gen SRY de burro.

![Filogenia](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2002/Filogenia.JPG)

Al aumentar el costo de abrir un gap, se espera que haya una disminución en la cantidad de gaps, pero un aumento en la longitud de estos. De forma contraria, si se disminuye el costo de abrir un gap, habrá un aumento en la cantidad de gaps, pero una disminucion en la longitud de estos.  
El cambio en el costo de extender un gap tiene un efecto contrario al mismo cambio en el costo de abrir un gap. Es decir, si se aumenta el costo de extender un gap, se espera ver un aumento en la cantidad de gaps y una disminución en el largo de estos. Mientras que si se disminuye el costo de extender un gap, se espera una disminución en la cantidad de gaps, pero un aumento en su longitud.

Al aumentar el costo de abrir un gap de 1.53 a 2.0, se obtuvo un alineamiento con una longitud de 1922 nucleótidos, lo que corresponde a un aumento de 22 nucleótidos con respecto al alineamiento anterior.  
Al disminuir el costo de extender un gap de 0.123 a 0, se obtuvo un alineamiento con una longitud de 1977 nucleótidos, donde secciones pequeñas de las secuencias de nucleótidos se encuentran separadas por gaps considerables como en la siguiente imagen:

![Alineamiento](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2002/Alineamiento.JPG)

----------
### Parte 3: Diseño de partidores ###
Los partidores encontrados para la amplificación de la región codificante de SRY en las cuatro especies seleccionadas son:

>**CCGCCGTTCAACAAaayathccngc**

>**GGGTAGGTGGCCTAGTtgrtgytscat**