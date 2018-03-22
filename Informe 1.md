Marcelo Araya Yáñez  
BIOL311

# Laboratorio nº1: Bases de datos biológicas. #

---

### Parte 1: Enfermedades genéticas y genes. ###

#### Ataxia-Telangiectasia (Síndrome de Louis-Barr) ####
El **síndrome de Louis-Barr** es causado por la ausencia de la enzima **ATM serina/treonina quinasa**. Los principales síntomas de esta enfermedad son **ataxia** (disminución en la coordinación de los movimientos) y **telangiectasia** (dilatación de vasos sanguíneos) sobre la esclerótica (también puede aparecer en áreas de la piel expuestas al sol). Otros síntomas incluyen disminución del ritmo de crecimiento y desarrollo incompleto de la pubertad.

Esta enfermedad se relaciona con el gen ATM, también conocido como gen ataxia-telangiectasia mutado.

Segun la [base de datos de NCBI](https://www.ncbi.nlm.nih.gov/gene/472) el gen ATM tiene los siguientes nombres alternativos: AT1; ATA; ATC; ATD; ATE; ATDC; TEL1; TELO1.

El gen ATM se encuentra en el brazo largo del cromosoma 11 (11q22.3) y tiene 69 exones.  
Río arriba del gen ATM se encuentra el gen NPAT, y río abajo del gen ATM se encuentra el gen C11orf65 (parte de este se encuentra solapado con el extremo 3' del gen ATM).  
![contexto genético del gen 472](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%20%2001/Contexto%20gen%C3%B3mico%20ATM.PNG)  
El gen ATM presenta **14 isoformas transcripcionales**.  
![isoformas transcripcionales](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%20%2001/Isoformas%20de%20transcritos%20ATM.PNG)  
El gen ATM codifica para la ATM serina/treonina quinasa, una **proteína serina/treonina quinasa no específica**, la cual posee un EC 	**2.7.11.1**.

La longitud del gen ATM es de **146,619** pares de bases.  
En [ClinVar](https://www.ncbi.nlm.nih.gov/clinvar/?term=ATM[gene]) se encuentran **4947** variantes diferentes del gen, las cuales se dividen en:

* 480 Deleciones
* 141 Duplicaciones
* 58 Indels
* 228 Inserciones 
* 4263 **Sustituciones**

Se describen sustituciones sinónimas como [**c.162T>C**](https://www.ncbi.nlm.nih.gov/clinvar/variation/132757/) y [**c.198A>G**](https://www.ncbi.nlm.nih.gov/clinvar/variation/135741/).  
Segun la [base de datos de NCBI](https://www.ncbi.nlm.nih.gov/gene/?Term=ortholog_gene_472[group]) existen **212** ortólogos con el gen ATM humano, algunas de las especies que presentan ortólogos con este gen son:

* *Pan troglodytes* (chimpancé)
* *Mus musculus* (ratón doméstico)
* *Canis lupus familiaris* (perro)
* *Pterus alecto* (zorro volador negro)
* *Danio rerio* (pez cebra)

No se describen genes parálogos ni pseudogenes para el gen ATM.
***
### Parte 2: Rutas y procesos metabólicos. ###

En [KEGG](http://www.kegg.jp/dbget-bin/www_bget?hsa:atm) se reportan los mismos nombres alternativos para el gen ATM que en [NCBI](https://www.ncbi.nlm.nih.gov/gene/472).  
La proteina codificada por el gen ATM participa en las siguientes vías metabólicas:  
![Rutas metabólicas](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%20%2001/Rutas%20metab%C3%B3licas%20ATM.PNG)  
EL número de identificación (Entry Number) del gen ATM es 472   
Los códigos de identificación para el gen ATM en distintas bases de datos son los siguientes:

* **NCBI**: 472
* **KEGG Orthology**: K04728
* **OMIM**: 607585
* **HGNC**: 795
* **Ensembl**: ENSG00000149311
* **Vega**: OTTHUMG00000166480
* **Pharos**: Q13315

Una de las rutas metabólicas en las que participa la proteína codificada por el gen ATM es el ciclo celular.  
![Ciclo celular](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%20%2001/Ciclo%20celular.PNG)  
En este diagrama, los cuadros verdes significan que el gen que codifica para la proteína que participa en ese proceso se encuentra en la base de datos.  
La ruta metabólica del diagrama se cruza con las rutas de:

* Apoptósis
* MAP quinasas
* Proteólisis mediada por ubiquitina

Las anotaciones de GO (Gene Onthology) se dividen en 4 tipos:

* Anotaciones apoyadas por experimentos
* Anotaciones inferidas filogenéticamente
* Anotaciones inferidas computacionalmente
* Extensión de anotaciones

El termino GO:0006096 corresponde a la categoría de proceso glicólitico. La página provee información sobre la ontología del proceso, sinónimos, definición e IDs alternativas.

Siguiendo el gráfico de [QuickGO](https://www.ebi.ac.uk/QuickGO/GTerm?id=GO:0006096) podemos observar que el proceso glicolítico pertenece a las siguientes sub-categorías:

1. Proceso biosintético de ATP
2. Generación de ATP a partir de ADP
3. Proceso biosintético de piruvato
4. Proceso catabólico de nucleótidos
5. Proceso metabólico de nucleótidos
6. Proceso catabólico de carbohidratos
7. Fosforilación de nucleósidos bifosfato
8. Fosforilación de nucleótidos
9. Proceso catabólico de nucleósidos fosfato
10. Proceso biosintético de ácido carboxílico

---

### Parte 3: Descargando secuencias, convirtiendo formatos. ###

Al buscar GAPDH en la base de datos de nucleótidos de NCBI se encuentran **70748** items, de los cuales **13419** se encuentran en animales.  
El mRNA de GAPDH de gallina tiene un largo de 1288 pares de bases.  
La referencia bibliográfica más reciente corresponde a una cita al articulo "**Binding chicken Anx2 is beneficial for infection with infectious bursal disease virus**", publicado el año 2015.  
El número de acceso de esta secuencia es NM_204305.

**Secuencia en formato FASTA:**  
![secuencia.fasta](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%20%2001/secuencia.fasta.PNG)

**Secuencia en formato NEXUS:**  
![secuencia.nexus](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%20%2001/secuencia.nexus.PNG)

---

### Parte 4: Buscando artículos científicos en línea ###

**Alerta de busqueda de PubMed:**

![alerta pubmed](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%20%2001/PubMed%20search%20alert.PNG)

**Correo de confirmación a la suscripción a Nature Genetics:**
 
![correo suscripción](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%20%2001/Suscrpci%C3%B3n.PNG)

Al buscar en Google Scholar **Huntington's Chorea** se obtienen los siguientes resultados:  
![google huntington](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%20%2001/google.PNG)

Al escribir la busqueda entre comillas, mostrando sólo los resultados donde aparezca "Huntington's Chorea" como una frase exacta, los resultados de la búsqueda son idénticos. Sin embargo, al usar un asterico para representar que falta una palabra entre "Huntington's" y "Chorea"	aparecen los siguientes resultados:

![google huntington 2](https://raw.githubusercontent.com/KyuZhang/lab-bioinf/master/Lab%20%2001/google%202.PNG)

Al buscar **"Huntington's Chorea" filetype:pdf** sólo aparecen artículos en pdf o citas a estos artículos.

Al buscar **"PCR amplification" +temperature** los resultados muestran artículos donde aparezca la frase "PCR amplification" y que además contengan la palabra temperature, haciendo que aparezcan incluso resultados que no tienen "PCR amplification" en el título.  
Mientras que al buscar **"PCR amplification" -temperature** los resutados muestran artículos que contengan la frase "PCR amplification" y que no contengan la palabra temperature.

Al buscar **Soil OR Human pathogens** aparecen resultados que contienen alguna combinación de las tres palabras ingresadas, siendo principalmente resultados que contienen la frase **human pathogens**, existiendo resultados con la palabra **soil** y la frase **human pathogens**, y resultados con la frase **soil pathogens**.  
En cambio al buscar **Soil AND Human pathogens** se obtienen resultados parecidos a cuando se utiliza el simbolo **+** para una búsqueda, con resultados que contienen la frase **Human pathogens** y además contienen la palabra **soil**.
