
# **GRUPO DE TRABAJO PROYECTO FINAL**  


# Proyecto:
**Comparación de microbiota intestinal entre individuos normopeso y obesos mediante secuenciación 16S rRNA y herramientas bioinformáticas**  


# **Integrantes**  
-Dylan Ron ☺️     
-Estefany German ☺️    
-Vanessa Terán😏      
-Vanesa Naranjo😏    

# **Objetivo**    
Comparar la microbiota intestinal entre individuos obesos y normopeso mediante análisis de secuenciación 16S y determinar si existe diferencia significativa entre su microbiota.      


# **Dataset**  
SRR25916244 Individuo obeso  
SRX32302418 Individuo sano  


# **Flujo de trabajo** 
```mermaid
flowchart LR
A[Datos crudos] --> B[Control de calidad] 
B --> C[Filtrado]
C --> D[Alineamiento]
D --> E[Cuantificación]
E --> F[Análisis diferencial]
F --> G[Visualización]
```

1. Descarga de datos
- Descarga de las secuencias SRR25916244 y SRX32302418 desde la base de datos SRA.

2. Control de calidad
- Evaluación de la calidad de las lecturas mediante FastQC.

3. Filtrado y recorte
- Eliminación de adaptadores y secuencias de baja calidad usando FasQ

4. Análisis bioinformático
- Procesamiento y comparación de las muestras mediante Galaxy.

5. Obtención de resultados
- Comparación de la microbiota intestinal entre individuo obeso y sano.

6. Interpretación
- Análisis de diferencias observadas en la composición microbiana.
Descarga
 
# **Resultados**  
<p align="justify">El análisis de calidad de las muestras mediante FastQC y MultiQC mostró secuencias de alta calidad, con valores Phred cercanos a 30 y contenido GC esperado para microbiota intestinal analizada por secuenciación 16S. Tras el filtrado, se observó una mínima pérdida de bases, indicando datos confiables para análisis posteriores.</p>

<p align="justify">El análisis taxonómico con Kraken2 y Krona evidenció predominio de los filos Firmicutes y Bacteroidetes en ambas muestras. El individuo normopeso presentó una microbiota más diversa y equilibrada, mientras que el individuo con obesidad mostró cambios en la abundancia bacteriana asociados previamente con alteraciones metabólicas. Debido al reducido número de muestras, los resultados deben considerarse preliminares.</p>

