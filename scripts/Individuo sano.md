# Individuo sano  
## Objetivo  
Realizar una línea de comando para la ejecución del control de calidad de datos de secuenciación pertenecientes a un
individuo sano.
### Obtención de la secuencia  
Los datos de secuenciación a utilizar pertenecen al gen 16S rRNA de microbiota intestinal obtenidos a través bases de 
datos públicas del NCBI en formato FASTQ. La secuencia del individuo sano: SRR37389193.  
### Flujo de trabajo
1. Obtención de la secuencia a través de la base de datos
2. Creación del repositorio del trabajo
3. Mover el archivo a utilizar al repositorio.
4. Aplicación de la herramienta FastQC para control de calidad de las secuencias.
5. Visualización de resultados en el despliegue de una nueva ventana del archivo en formato html.  

--- 

:bookmark: 1
 Obtención de los datos  
Decargar la secuencia SRR37389193.fastaq.gz
---
### Creación del repostorio

```text
mkdir Proyecto_final_g7

```  
---
### Traslado del archivo de la carpeta de Descargas al repositorio

```text
mv SRR37389193.fastq.gz /home/maquina virtual/Proyecto_final_g7

```  
---
### Extracción de documentos del archivo comprimido

```text
gunzip SRR37389193.fastq.gz

```  
---
### Visualización del encabezado del archivo

```text
head SRR37389193.fastq

```  
---
### Aplicación de la herramienta bioinformática

```text
fastq SRR37389193.fastq

```  
---
### Visualización de los resultados

```text
xdg-open SRR37389193.fastq

```




