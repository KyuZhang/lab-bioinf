Marcelo Araya Yáñez

----------
# Laboratorio nº3: Ensamblaje de genomas y predicción de genes #
### Parte 1: El artículo genoma ###
En la base de datos GOLD se encuentran un total de **128.853** genomas completamente secuenciados, de los cuales **35.280** son de organismos eucariontes y **93.573** de organismos procariontes.  
Estos genomas no son los mismos que se encuentran en GenBank, debido a que GenBank almacena secuencias de DNA en vez de genomas completos como GOLD.

El N50 es una estadística que indica el largo del contig más corto a la mitad de un ensamble. Esto es útil para comparar la calidad de ensambles de logitudes de tamaños similares.  
El L50 es la menor cantidad de contigs tal que la suma de sus longitudes corresponda al N50.  
El NG50 es una estadística definida de la misma que el N50, pero se toma en cuenta la mitad de la longitud estimada del genoma. Esto permite comparar de forma significativa dos ensambles de largos distintos.  
El genoma escogido fue el de ***Beta vulgaris* (betarraga)**. El artículo original puede encontrarse [**aquí**](https://www.nature.com/articles/nature12817).  
El N50 del genoma es de **2,01 Mb**. El valor del NG50 no se especifica, pero se puede asumir que será menor al N50 debido a que el genoma posee una longitud mayor a la del ensamble.  
El genoma fue secuenciado usando principalmente una plataforma illumina (secuenciación por síntesis). En el genoma hay **9 cromosomas distintos** (18 cromosomas en total) con un tamaño promedio de **53.3 Mb**.

----------
### Parte 2: Predicción de genes ###
Para la secuencia dada, ORFfinder encontró 7 ORF, de los cuales 3 pertenecen a la secuencia nucleotídica y 4 pertenecen a su hebra complementaria.

![Resultados ORF](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/ORFfinder.JPG)

GLIMMER encontró 10 ORF, de los cuales 4 se encuentran en la secuencia y 6 se encuentran en la hebra complementaria. GLIMMER es un programa de tipo Ab Initio.

![Resultados GLIMMER](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/GLIMMER.JPG)

Algunos de estos ORF coinciden parcialmente, estos son:

- **ORF4** con **G2**
- **ORF5** con **G3**
- **ORF7** con **G4**

Los resultados de BLAST para los ORF encontrados por ORFfinder son:

+ **ORF1**: Corresponde a una proteína homóloga de FdhE.  
![ORF1](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/ORF1.JPG)
+ **ORF2**: El alineamiento más significativo fue con una proteína de cápside VP2, aunque estadísticas como el query coverage y el E value indican que estos resultados no son fiables.  
![ORF2](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/ORF2.JPG)
+ **ORF3**: No se encontraron similitudes significantes.  
![ORF3](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/ORF3.JPG)
+ **ORF4**: Corresponde a la proteína Alanina-aciltransferasa.  
![ORF4](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/ORF4.JPG)
+ **ORF5**: Corresponde a la subunidad psi de la DNA polimerasa III.  
![ORF5](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/ORF5.JPG)
+ **ORF6**: El alineamiento más significativo fue con la proteína TY4A, aunque las estadísticas de este resultado indican que no es fiable.  
![ORF6](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/ORF6.JPG)
+ **ORF7**: No se encontraron similitudes significantes.  
![ORF7](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/ORF7.JPG)

Los resultados de BLAST para los ORF encontrados por GLIMMER son:

+ **G1**: Corresponde a una peptido n-aciltransferasa de *H. influenzueae*.  
![G1](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/G1.JPG)
+ **G2**: Corresponde a la misma peptido n-aciltransferasa que **G1**.  
![G2](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/G2.JPG)
+ **G3**: Corresponde a la subunidad psi de la DNA polimerasa III de *H. influenzae*.  
![G3](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/G3.JPG)
+ **G4**: Corresponde a una proteína FdhE de *H. influenzae*.  
![G4](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/G4.JPG)
+ **G5**: Corresponde a una proteína FdhE de *H. influenzae*.  
![G5](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/G5.JPG)
+ **G6**: Corresponde a una proteína FdhE de *H. influenzae*. El segundo resultado es el mismo que el de **G4**.  
![G6](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/G6.JPG)
+ **G7**: Corresponde a la misma subunidad de DNA pol III que **G3**.  
![G7](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/G7.JPG)
+ **G8**: Corresponde a la subunidad psi de la DNA polimerasa III de *H. influenzae*, el segundo resultado es el mismo que el de **G3** y **G7**.  
![G8](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/G8.JPG)
+ **G9**: Corresponde a una proteína FdhE de *H. influenzae*.  
![G9](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/G9.JPG)
+ **G10**: Los resultados más relevantes son los mismos que para **G8**.  
![G10](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2003/G10.JPG)