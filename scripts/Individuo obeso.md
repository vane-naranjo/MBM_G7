Script individuo obeso
Objetivo

Realizar una línea de comando para la ejecución del control de calidad de datos de secuenciación pertenecientes a un individuo obeso.

Obtención de la secuencia

Los datos de secuenciación utilizados pertenecen al gen 16S rRNA de microbiota intestinal obtenidos a través de bases de datos públicas del NCBI en formato FASTQ.
La secuencia del individuo obeso: SRR25916244

Flujo de trabajo
Obtención de la secuencia a través de la base de datos
Creación del repositorio del trabajo
Mover el archivo a utilizar al repositorio
Aplicación de la herramienta FastQC para control de calidad de las secuencias
Visualización de resultados en formato HTML
1. Obtención de los datos
Descargar la secuencia SRR25916244.fastq.gz
Creación del repositorio
mkdir Proyecto_final_g7
Traslado del archivo de la carpeta de Descargas al repositorio
mv SRR25916244.fastq.gz /home/maquina_virtual/Proyecto_final_g7
Extracción de documentos del archivo comprimido
gunzip SRR25916244.fastq.gz
Visualización del encabezado del archivo
head SRR25916244.fastq
Aplicación de la herramienta bioinformática
fastqc SRR25916244.fastq
(FastQC)
Visualización de los resultados
xdg-open SRR25916244_fastqc.html
