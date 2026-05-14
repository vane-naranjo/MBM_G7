# MBM_G7
GRUPO DE TRABAJO PROYECTO FINAL  
Integrantes:  
-Dylan Ron  
-Estefany German  
-Vanessa Terán  
-Vanesa Naranjo  
## Objetivo   
Determinar las diferencias significativas en el perfil de la microbiota intestinal entre individuos con obesidad y normopeso empleando secuenciación masiva 16S.  
## 1.Introducción  
La obesidad es una enfermedad multifactorial considerada uno de los principales problemas de salud pública a nivel mundial, debido a su relación con enfermedades metabólicas como diabetes tipo 2, hipertensión y trastornos cardiovasculares. En los últimos años, diversas investigaciones han demostrado que la microbiota intestinal desempeña un papel importante en el metabolismo energético, la digestión y la regulación del sistema inmunológico. La microbiota intestinal está compuesta por millones de microorganismos, principalmente bacterias, que habitan en el tracto gastrointestinal y mantienen una relación simbiótica con el organismo humano.
Diversos estudios han evidenciado que las personas con obesidad presentan alteraciones en la composición y diversidad de su microbiota intestinal en comparación con individuos con peso normal. Cambios en la abundancia relativa de ciertos grupos bacterianos, como los filos Firmicutes y Bacteroidetes, se han asociado con una mayor capacidad de extracción de energía de los alimentos y con procesos inflamatorios relacionados con el aumento de peso corporal. Por ello, el análisis de la microbiota intestinal se ha convertido en un área de gran interés dentro de la microbiología y la bioinformática.  

 
El gen 16S rRNA es un marcador molecular presente en todas las bacterias que contiene regiones conservadas y variables, lo que permite identificar y comparar comunidades bacterianas mediante secuenciación. La importancia del uso del gen 16S como marcador radica en que forma parte del ribosoma bacteriano, estructura encargada de la síntesis de proteínas. Algunas regiones de este gen son altamente conservadas entre distintas bacterias, mientras que otras presentan variaciones entre especies, característica que permite identificar géneros bacterianos y, en algunos casos, especies específicas (Janda & Abbott, 2007). Además, su estudio es fundamental para analizar la diversidad microbiana y la microbiota intestinal, como en el caso de este proyecto.  
La metagenómica basada en 16S permite estimar qué bacterias están presentes en una muestra, así como determinar su abundancia relativa, diversidad bacteriana y diferencias entre grupos. Estos análisis constituirán la base para comparar la microbiota intestinal de individuos normopeso y con obesidad. Esta ómica representa la principal herramienta utilizada en este proyecto, ya que permite analizar la comunidad bacteriana completa presente en muestras fecales y no únicamente microorganismos aislados. Aunque la metagenómica es el eje central del estudio, otras ciencias ómicas como la metabolómica, transcriptómica, proteómica y genómica también guardan relación, debido a su aporte en la comprensión integral de los procesos biológicos asociados a la microbiota y la obesidad (Janda & Abbott, 2007; Handelsman, 2004).  

Además del objetivo principal de comparar la microbiota intestinal entre individuos obesos y normopeso, el proyecto permitirá explorar la relación entre la microbiota y obesidad mediante la identificación de bacterias asociadas al metabolismo y el análisis de la diversidad bacteriana de cada individuo. De este modo, el uso de herramientas de metagenómica y bioinformática permitirá comprender cómo la microbiota intestinal se relaciona con la obesidad. La integración de la secuenciación 16S y el análisis computacional servirá como base para identificar diferencias microbianas entre ambos grupos, contribuyendo al estudio de enfermedades metabólicas, al desarrollo de habilidades bioinformáticas y, potencialmente, a la generación de futuras estrategias aplicadas al campo de la salud (Human Microbiome Project Consortium, 2012; Janda & Abbott, 2007).

## 2. Metodología  
### 1. Obtención de datos  
La datos se obtendrán a través de bases de datos públicas del NCBI de la secuenciación de la subunidad 16S de un individuo con normopeso y un individuo con sobrepeso. 
El número de identificaicón de las secuencias para un individuo sano (SRR37389193) e individuo con obesidad (SRR25916244)
### 2. Almacenamiento de la información y control de calidad 
Se utilizará la palataforma Galaxy para el procesamiento, análisis y visualización de los datos.
Las secuencias obtenidas serán evaluadas mediante FastQC para verificar parámetros de calidad como longitud de lecturas, contenido GC y presencia de adaptadores.   
### 3. Procesamiento de secuencias  
Las lecturas serán filtradas y limpiadas para eliminar secuencias de baja calidad y posibles contaminantes utilizando herramientas disponibles en Galaxy como Cutadapt o NanoFilt.
### 4. Comparación de microbiota  
Se comparará la composición bacteriana entre el individuo normopeso y el individuo con sobrepeso, evaluando diferencias en abundancia y diversidad microbiana.
### 5. Visualización e interpretación biológica  
Los resultados serán representados mediante gráficos y herramientas de visualización taxonómica. Finalmente, se realizará una interpretación biológica de las diferencias observadas en la microbiota intestinal.
Las lecturas serán filtradas y limpiadas para eliminar secuencias de baja calidad y posibles contaminantes utilizando herramientas disponibles en Galaxy como FASTQC, MULTIQC, FASTP.
## 3. Resultados




Individduo obeso:  

En la Figura 5 se presentan las estadísticas básicas FASTQC obtenidas para la secuencia 16s del individuo obeso.
<img width="486" height="276" alt="image" src="https://github.com/user-attachments/assets/ecc5cd59-f3b9-4267-ab91-05849183a8d9" />


## 4. Discusión
## 5. Conclusiones  

## 6. Link de tutorial 

https://training.galaxyproject.org/training-material/topics/microbiome/tutorials/nanopore-16S-metagenomics/tutorial.html  

## 7. Referencias bibliográficas  

Ley, R. E., Turnbaugh, P. J., Klein, S., & Gordon, J. I. (2006). Microbial ecology: Human gut microbes associated with obesity. Nature, 444(7122), 1022–1023. https://doi.org/10.1038/4441022a  

Qin, J., Li, R., Raes, J., Arumugam, M., Burgdorf, K. S., Manichanh, C., et al. (2010). A human gut microbial gene catalogue established by metagenomic sequencing. Nature, 464(7285), 59–65. https://doi.org/10.1038/nature08821  

Turnbaugh, P. J., Ley, R. E., Mahowald, M. A., Magrini, V., Mardis, E. R., & Gordon, J. I. (2006). An obesity-associated gut microbiome with increased capacity for energy harvest. Nature, 444(7122), 1027–1031. https://doi.org/10.1038/nature05414
World Health Organization. (2024). Obesity and overweight. https://www.who.int/news-room/fact-sheets/detail/obesity-and-overweight  

Handelsman, J. (2004). Metagenomics: Application of genomics to uncultured microorganisms. Microbiology and Molecular Biology Reviews, 68(4), 669–685. https://doi.org/10.1128/MMBR.68.4.669-685.2004  

Turnbaugh, P. J., Hamady, M., Yatsunenko, T., Cantarel, B. L., Duncan, A., Ley, R. E., Sogin, M. L., Jones, W. J., Roe, B. A., Affourtit, J. P., Egholm, M., Henrissat, B., Heath, A. C., Knight, R., & Gordon, J. I. (2009). A core gut microbiome in obese and lean twins. Nature, 457(7228), 480–484. https://doi.org/10.1038/nature07540   

Janda, J. M., & Abbott, S. L. (2007). 16S rRNA gene sequencing for bacterial identification in the diagnostic laboratory: Pluses, perils, and pitfalls. Journal of Clinical Microbiology, 45(9), 2761–2764. https://doi.org/10.1128/JCM.01228-07  

Human Microbiome Project Consortium. (2012). Structure, function and diversity of the healthy human microbiome. Nature, 486(7402), 207–214. https://doi.org/10.1038/nature11234
  


