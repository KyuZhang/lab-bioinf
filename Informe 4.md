Marcelo Araya

----------
# Laboratorio nº4: Filogenética molecular #
El portal Phylogeny.fr ofrece una plataforma que incluye programas relevantes para análisis filogenético. Esta web está diseñada para personas sin experiencia en filogenética, pero también es útil para usuarios más experimentados debido a que es personalizable.  
De acuerdo a la documentación del sitio, pueden realizarse los siguientes análisis:

+ Filogenia usando máxima semejanza
+ Filogenia usando parsimonia
+ Filogenia bayesiana
+ Filogenia usando distancias
+ Estimación de clados

El paso de curación de alineamiento consiste en eliminar posiciones pobremente alineadas y regiones divergentes en un alineamiento de secuencias.  
La diferencia entre BioNJ y Neighbor es su limitación en el número de taxones (<5000 para BioNJ y <500 para Neighbor).  

Se infirieron dos filogenias distintas usando distintos programas, y luego se infirieron otras dos filogenias con los mismos programas pero omitiendo el paso de curación del alineamiento.  

#### Filogenia I (ProbCons, Gblocks, MrBayes y TreeDyn): ####

![filogenia 1](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2004/filogenia%201.JPG)

#### Filogenia I (omitiendo curación de alineamiento): ####

![filogenia 3](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2004/Filogenia%203.JPG)

Al omitir el paso de curación del alineamiento se obtienen ligeras diferencias en el árbol filogenético. Por ejemplo: *Capra hircus* cambia de posición con *Odocoileus virginianus*, en el segundo árbol se omite un ancestro común entre *Pteropus alecto* y *Camelus ferus* y se añade un ancestro común entre *Marmota marmota* y *Fukomys damarensis*.

#### Filogenia II (ClustalW, Remove positions with gaps, TNT y TreeDyn): ####

![filogenia 2](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2004/filogenia%202.JPG)

#### Filogenia II (omitiendo curación de alineamiento): ####

![filogenia 4](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%2004/Filogenia%204.JPG)

Al omitir el paso de curación del alineamiento se pueden apreciar ligeras diferencias en el árbol filogenético. Por ejemplo: *Equ* y *Tupaia chinensis* dejan de estar relacionados directamente, y *Equus przewalskii* se relaciona más cercanamente a *Camelus ferus* en el segundo árbol.