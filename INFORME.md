# MBM_G7

## Objetivo   
Comparar la microbiota intestinal entre individuos obesos y normopeso mediante análisis de secuenciación 16S y determinar si existe diferencia significativa entre su microbiota.
## 1.Introducción  
La obesidad es una enfermedad multifactorial considerada uno de los principales problemas de salud pública a nivel mundial, debido a su relación con enfermedades metabólicas como diabetes tipo 2, hipertensión y trastornos cardiovasculares. En los últimos años, diversas investigaciones han demostrado que la microbiota intestinal desempeña un papel importante en el metabolismo energético, la digestión y la regulación del sistema inmunológico. La microbiota intestinal está compuesta por millones de microorganismos, principalmente bacterias, que habitan en el tracto gastrointestinal y mantienen una relación simbiótica con el organismo humano.
Diversos estudios han evidenciado que las personas con obesidad presentan alteraciones en la composición y diversidad de su microbiota intestinal en comparación con individuos con peso normal. Cambios en la abundancia relativa de ciertos grupos bacterianos, como los filos Firmicutes y Bacteroidetes, se han asociado con una mayor capacidad de extracción de energía de los alimentos y con procesos inflamatorios relacionados con el aumento de peso corporal. Por ello, el análisis de la microbiota intestinal se ha convertido en un área de gran interés dentro de la microbiología y la bioinformática.  

 
El gen 16S rRNA es un marcador molecular presente en todas las bacterias que contiene regiones conservadas y variables, lo que permite identificar y comparar comunidades bacterianas mediante secuenciación. La importancia del uso del gen 16S como marcador radica en que forma parte del ribosoma bacteriano, estructura encargada de la síntesis de proteínas. Algunas regiones de este gen son altamente conservadas entre distintas bacterias, mientras que otras presentan variaciones entre especies, característica que permite identificar géneros bacterianos y, en algunos casos, especies específicas (Janda & Abbott, 2007). Además, su estudio es fundamental para analizar la diversidad microbiana y la microbiota intestinal, como en el caso de este proyecto.  
La metagenómica basada en 16S permite estimar qué bacterias están presentes en una muestra, así como determinar su abundancia relativa, diversidad bacteriana y diferencias entre grupos. Estos análisis constituirán la base para comparar la microbiota intestinal de individuos normopeso y con obesidad. Esta ómica representa la principal herramienta utilizada en este proyecto, ya que permite analizar la comunidad bacteriana completa presente en muestras fecales y no únicamente microorganismos aislados. Aunque la metagenómica es el eje central del estudio, otras ciencias ómicas como la metabolómica, transcriptómica, proteómica y genómica también guardan relación, debido a su aporte en la comprensión integral de los procesos biológicos asociados a la microbiota y la obesidad (Janda & Abbott, 2007; Handelsman, 2004).  

Además del objetivo principal de comparar la microbiota intestinal entre individuos obesos y normopeso, el proyecto permitirá explorar la relación entre la microbiota y obesidad mediante la identificación de bacterias asociadas al metabolismo y el análisis de la diversidad bacteriana de cada individuo. De este modo, el uso de herramientas de metagenómica y bioinformática permitirá comprender cómo la microbiota intestinal se relaciona con la obesidad. La integración de la secuenciación 16S y el análisis computacional servirá como base para identificar diferencias microbianas entre ambos grupos, contribuyendo al estudio de enfermedades metabólicas, al desarrollo de habilidades bioinformáticas y, potencialmente, a la generación de futuras estrategias aplicadas al campo de la salud (Human Microbiome Project Consortium, 2012; Janda & Abbott, 2007).

## 2. Metodología  
### 1. Obtención de datos  
La datos se obtendrán a través de bases de datos públicas del NCBI de la secuenciación de la subunidad 16S de un individuo con normopeso y un individuo con sobrepeso. 
Secuencia de la persona sana: SRR37389193
Secuencia de la persona obesa: SRR25916244
### 2. Almacenamiento de la información y control de calidad 
Se utilizará la palataforma Galaxy para el procesamiento, análisis y visualización de los datos.
Las secuencias obtenidas serán evaluadas mediante FastQC para verificar parámetros de calidad como longitud de lecturas, contenido GC y presencia de adaptadores.   
### 3. Procesamiento de secuencias  
Las lecturas serán filtradas y limpiadas para eliminar secuencias de baja calidad y posibles contaminantes utilizando herramientas disponibles en Galaxy como FASTQC, MULTIQC Y FASTP.
Se utilizó la plataforma Kraken 2 para la clasificación taxonómica de las secuencias a través de una base de datos de genomas de referencia. Finalmente para una mejor visualización se utilizó la herramienta Krona, que transformó los datos obtenidos en un gráfico circular multinivel. 
### 4. Comparación de microbiota  
Se comparará la composición bacteriana entre el individuo normopeso y el individuo con sobrepeso, evaluando diferencias en abundancia y diversidad microbiana.
### 5. Visualización e interpretación biológica  
Los resultados serán representados mediante gráficos y herramientas de visualización taxonómica. Finalmente, se realizará una interpretación biológica de las diferencias observadas en la microbiota intestinal.

## 3. Resultados




Individuo obeso:  

En las Figuras presentadas a continuación  se muestran los principales resultados obtenios despuès del análisis FASTQC, MultiQc y fastp obtenidas para la secuencia 16s del individuo obeso.  

<img width="486" height="276" alt="image" src="https://github.com/user-attachments/assets/ecc5cd59-f3b9-4267-ab91-05849183a8d9" />    

Figura 1. Estadísticas bàsicas FastQC_Individuo obeso   



<img width="531" height="349" alt="Screenshot (2)" src="https://github.com/user-attachments/assets/79037fca-80d5-4f1f-a1f3-711a0fceb07c" />  

Figura 2. Análisis de calidad de la secuencia de bases_Individuo obeso  

<img width="464" height="269" alt="image" src="https://github.com/user-attachments/assets/722fcdd5-0127-479b-9f5d-c8a7c79320ad" />  


Figura 3. Calidad por base de las secuencias evaluadas mediante FastQC_Contenido por secuencia de bases   

<img width="538" height="278" alt="image" src="https://github.com/user-attachments/assets/78e1bff4-04f6-4b5b-8ff1-033bf6c6ade7" />  

Figura 4. MultiQC con datos filtrados_individuo obeso 

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/6b73e4bf-44dc-4462-8c97-c61893e56ded" />  
Figura 5.  Reporte taxonómico generado mediante Kraken2 para la muestra del individuo normopeso.  
Se observa la clasificación taxonómica de bacterias presentes en la microbiota intestinal a diferentes niveles taxonómicos.  

<img width="1600" height="887" alt="WhatsApp Image 2026-05-15 at 11 07 53 PM" src="https://github.com/user-attachments/assets/447baad9-bd6f-44db-85c0-54b6ebaa2e63" />
Figura 6. Visualización taxonómica de la microbiota intestinal del individuo normopeso mediante Krona.
El gráfico circular interactivo muestra la abundancia relativa de los principales grupos bacterianos identificados a partir de las secuencias 16S rRNA analizadas con Kraken2.

 



En las Figuras presentadas a continuación  se muestran los principales resultados obtenios despuès del análisis FASTQC, MultiQc y fastp obtenidas para la secuencia 16s del individuo normopeso.  


<img width="292" height="199" alt="image" src="https://github.com/user-attachments/assets/c4663767-8193-4696-a9c0-14ddc316a75b" />


Figura 5. Estadísticas bàsicas FastQC_Individuo normopeso


<img width="487" height="289" alt="image" src="https://github.com/user-attachments/assets/fccb3345-b480-426a-8692-d60ba92bb21f" />


Figura 6. Análisis de calidad de la secuencia de bases_Individuo normopeso 


<img width="1236" height="692" alt="image" src="https://github.com/user-attachments/assets/a313b2e3-85b8-4800-a2f3-23d8ceb6834d" />


Figura 7. Calidad por base de las secuencias evaluadas mediante FastQC_Contenido por secuencia de bases   


<img width="1648" height="1042" alt="image" src="https://github.com/user-attachments/assets/295876e0-ac96-47f9-a99d-9e968d7fc41d" />

Figura 8. MultiQC con datos filtrados_individuo normopeso

<img width="2968" height="1374" alt="image" src="https://github.com/user-attachments/assets/1c7975c8-42db-4b73-b559-bd6c5d1c3646" />

Figura 9. Reporte taxonómico generado mediante Kraken2 para la muestra del individuo normopeso.
Se observa la clasificación taxonómica de bacterias presentes en la microbiota intestinal a diferentes niveles taxonómicos.


<img width="2890" height="1468" alt="image" src="https://github.com/user-attachments/assets/6cd9f2b2-42ac-42a8-b3c3-074b40058b7c" />

Figura 10.Visualización taxonómica de la microbiota intestinal del individuo normopeso mediante Krona.
El gráfico circular interactivo muestra la abundancia relativa de los principales grupos bacterianos identificados a partir de las secuencias 16S rRNA analizadas con Kraken2.

## 4. Discusión 

El análisis taxonómico preliminar realizado mediante Kraken2 y visualizado con Krona permitió observar diferencias en la composición bacteriana entre el individuo normopeso y el individuo con obesidad. En ambos casos se identificó una microbiota dominada principalmente por bacterias pertenecientes a los filos Bacteroidetes y Firmicutes, considerados los grupos bacterianos predominantes del intestino humano (Human Microbiome Project Consortium, 2012).

En el individuo normopeso se observó una distribución bacteriana más diversa y equilibrada, con representación importante de grupos pertenecientes a Clostridia, Oscillospirales y Ruminococcaceae. Diversos estudios han descrito que una mayor diversidad bacteriana intestinal suele asociarse con un estado metabólico saludable y con funciones beneficiosas como fermentación de fibra y producción de ácidos grasos de cadena corta (Qin et al., 2010), por otro lado, el individuo con obesidad presentó una distribución menos homogénea y predominio de ciertos grupos bacterianos en comparación con el individuo sano. Estas alteraciones microbianas han sido relacionadas con obesidad y con una mayor capacidad de extracción energética de los alimentos, además de procesos inflamatorios asociados al metabolismo (Turnbaugh et al., 2006; Ley et al., 2006).

Los resultados obtenidos coinciden con investigaciones previas donde se ha reportado que cambios en la abundancia relativa de Firmicutes y Bacteroidetes pueden asociarse con obesidad y alteraciones metabólicas. Sin embargo, debido a que este estudio incluyó únicamente dos muestras individuales, los resultados deben considerarse preliminares y descriptivos, ya que factores como dieta, edad, ambiente y estilo de vida también influyen significativamente sobre la microbiota intestinal (Turnbaugh et al., 2009).


## 5 Aplicaciones y ejemplos 

El análisis taxonómico de la microbiota intestinal posee múltiples aplicaciones clínicas y biomédicas, ya que permite identificar alteraciones en la composición bacteriana asociadas con diversas enfermedades metabólicas y gastrointestinales. Mediante herramientas bioinformáticas como Kraken2 y visualizadores como Krona es posible caracterizar los microorganismos presentes en el intestino y comparar diferencias entre individuos sanos y pacientes con distintas patologías.

En enfermedades como obesidad y diabetes tipo 2, diversos estudios han reportado cambios en la abundancia relativa de bacterias pertenecientes a los filos Firmicutes y Bacteroidetes, los cuales pueden influir en procesos relacionados con metabolismo energético, inflamación y absorción de nutrientes. Asimismo, el estudio de la microbiota intestinal también tiene aplicaciones en enfermedades inflamatorias intestinales, evaluación del efecto de probióticos y prebióticos, nutrición personalizada y análisis de respuesta a tratamientos farmacológicos.

Estos enfoques contribuyen al desarrollo de estrategias de medicina personalizada y permiten comprender mejor la relación entre microbiota y salud humana. Sin embargo, debido a la influencia de factores como dieta, edad, ambiente y estilo de vida, es necesario realizar estudios con un mayor número de muestras para obtener conclusiones clínicas más robustas y representativas.


## 6. Conclusiones  

Se logró obtener y procesar secuencias 16S rRNA de un individuo normopeso y un individuo con obesidad provenientes de bases de datos públicas del NCBI, permitiendo desarrollar un flujo de trabajo bioinformático reproducible.

El análisis de calidad mediante FastQC y MultiQC mostró que ambas muestras presentaron lecturas de buena calidad, contenido GC estable y longitudes adecuadas para continuar con el análisis taxonómico.

La herramienta fastp permitió realizar el filtrado y limpieza de las secuencias, optimizando los datos para posteriores análisis de microbiota intestinal.

El análisis taxonómico realizado con Kraken2 y visualizado mediante Krona evidenció diferencias preliminares en la composición bacteriana entre el individuo sano y el individuo con obesidad.

En ambas muestras predominaron bacterias pertenecientes a los filos Firmicutes y Bacteroidetes, grupos microbianos comúnmente asociados a la microbiota intestinal humana.

La integración de herramientas bioinformáticas como Galaxy, Kraken2 y Krona permitió fortalecer habilidades en análisis de datos ómicos y facilitó la interpretación biológica de comunidades microbianas intestinales.


## 7. Link de tutorial 

https://training.galaxyproject.org/training-material/topics/microbiome/tutorials/nanopore-16S-metagenomics/tutorial.html  

## 8. Referencias bibliográficas  

Ley, R. E., Turnbaugh, P. J., Klein, S., & Gordon, J. I. (2006). Microbial ecology: Human gut microbes associated with obesity. Nature, 444(7122), 1022–1023. https://doi.org/10.1038/4441022a  

Qin, J., Li, R., Raes, J., Arumugam, M., Burgdorf, K. S., Manichanh, C., et al. (2010). A human gut microbial gene catalogue established by metagenomic sequencing. Nature, 464(7285), 59–65. https://doi.org/10.1038/nature08821  

Turnbaugh, P. J., Ley, R. E., Mahowald, M. A., Magrini, V., Mardis, E. R., & Gordon, J. I. (2006). An obesity-associated gut microbiome with increased capacity for energy harvest. Nature, 444(7122), 1027–1031. https://doi.org/10.1038/nature05414
World Health Organization. (2024). Obesity and overweight. https://www.who.int/news-room/fact-sheets/detail/obesity-and-overweight  

Handelsman, J. (2004). Metagenomics: Application of genomics to uncultured microorganisms. Microbiology and Molecular Biology Reviews, 68(4), 669–685. https://doi.org/10.1128/MMBR.68.4.669-685.2004  

Turnbaugh, P. J., Hamady, M., Yatsunenko, T., Cantarel, B. L., Duncan, A., Ley, R. E., Sogin, M. L., Jones, W. J., Roe, B. A., Affourtit, J. P., Egholm, M., Henrissat, B., Heath, A. C., Knight, R., & Gordon, J. I. (2009). A core gut microbiome in obese and lean twins. Nature, 457(7228), 480–484. https://doi.org/10.1038/nature07540   

Janda, J. M., & Abbott, S. L. (2007). 16S rRNA gene sequencing for bacterial identification in the diagnostic laboratory: Pluses, perils, and pitfalls. Journal of Clinical Microbiology, 45(9), 2761–2764. https://doi.org/10.1128/JCM.01228-07  

Human Microbiome Project Consortium. (2012). Structure, function and diversity of the healthy human microbiome. Nature, 486(7402), 207–214. https://doi.org/10.1038/nature11234
  


