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

El análisis preliminar realizado sobre las muestras SRR37389193 y SRR25916244, tanto para el individuo sano com opara el obeso mediante FastQC y MultiQC mostró que las secuencias presentan una calidad alta y estable a lo largo de las lecturas, con valores Phred cercanos a 30 y una longitud promedio aproximada de 301 pb y 149.7 Mbp. Además, el contenido GC se mantuvo en 51% en ambos casos,, valor esperado para comunidades bacterianas intestinales analizadas mediante secuenciación 16S.  El uso de secuencias 16S permite utilizar cebadores universales ya que son regiones conservadas, por lo que funcionan como marcadores moleculares para la identificación de especies bacterianas.  

Al analizar los resultados de análisis de calidad para las secuencias tanto del individuo normopeso como del individuo obeso  vemos que la calidad fue alta y tras el uso de los filtros no se quitaron gran cantidad de bases, esto es característico del comportamiento de lasecuencia 16s. Sin embargo,  aunque ambas muestras mostraron perfiles de calidad semejantes, esto no implica que posean exactamente la misma microbiota intestinal, ya que el análisis de calidad únicamente evalúa características técnicas de la secuenciación y no la composición taxonómica de los microorganismos presentes, porque no es posible concluir con exactitud si existe una diferencia entre la microbiota de ambos individuos.  

Biológicamente, estos resultados indican que las muestras poseen una adecuada calidad para continuar con análisis posteriores de microbiota intestinal y clasificación taxonómica. La estabilidad de la calidad y la uniformidad en la longitud de las secuencias sugieren que el proceso de secuenciación fue exitoso y que los datos son confiables para identificar comunidades bacterianas presentes en el individuo sano. Los resultados obtenidos determinan un perfil de referencia de un individuo sano para la identificación de alteraciones en la microbiota en individuos que presentan obesidad, una vez realizado el perfil taxonómico de modo que sea posible identificar desviaciones de filos como Bacteroidetes y Firmicutes, que son las poblaciones predominantes en el intestino del ser humano.




## 5. Conclusiones  

Se logró obtener y procesar secuencias de la subunidad 16S rRNA de individuos con normopeso y sobrepeso provenientes de bases de datos públicas del NCBI, permitiendo desarrollar un flujo de trabajo bioinformático reproducible.

El análisis de control de calidad mediante FastQC y MultiQC evidenció que ambas secuencias presentaron parámetros adecuados de calidad, incluyendo buena calidad por base, longitud de lectura uniforme y contenido GC estable, lo que permitió validar su uso para análisis posteriores.

La herramienta fastp permitió realizar el filtrado y limpieza de las lecturas, eliminando posibles secuencias de baja calidad y optimizando los datos para futuros análisis microbiológicos.

La plataforma Galaxy facilitó el procesamiento y visualización de los datos mediante una interfaz gráfica intuitiva, mientras que el uso de línea de comandos permitió comprender de manera más detallada el manejo directo de archivos y herramientas bioinformáticas.

La comparación preliminar entre ambas muestras mostró perfiles de calidad similares, sugiriendo que las diferencias biológicas que puedan encontrarse posteriormente estarían relacionadas con la composición microbiana y no con errores técnicos de secuenciación.

El proyecto permitió integrar conocimientos de microbiología, secuenciación y bioinformática, fortaleciendo habilidades en análisis de datos ómicos y uso de herramientas computacionales aplicadas al estudio del microbioma intestinal.



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
  


