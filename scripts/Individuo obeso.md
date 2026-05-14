# Individuo obeso

## Objetivo

Realizar una línea de comando para la ejecución del control de calidad de datos de secuenciación pertenecientes a un individuo obeso.

## Obtención de la secuencia

Los datos de secuenciación utilizados pertenecen al gen 16S rRNA de microbiota intestinal obtenidos a través de bases de datos públicas del NCBI en formato FASTQ.

La secuencia del individuo obeso es: **SRR25916244**

## Flujo de trabajo

1. Obtención de la secuencia a través de la base de datos.
2. Creación del repositorio del trabajo.
3. Mover el archivo a utilizar al repositorio.
4. Aplicación de la herramienta FastQC para control de calidad de las secuencias.
5. Visualización de resultados en formato HTML.

## Obtención de los datos

Descargar la secuencia `SRR25916244.fastq.gz`

## Creación del repositorio

```bash
mkdir Proyecto_final_g7
```

## Traslado del archivo de la carpeta Descargas al repositorio

```bash
mv SRR25916244.fastq.gz /home/maquina_virtual/Proyecto_final_g7
```

## Extracción de documentos del archivo comprimido

```bash
gunzip SRR25916244.fastq.gz
```

## Visualización del encabezado del archivo

```bash
head SRR25916244.fastq
```

## Aplicación de la herramienta bioinformática FastQC

```bash
fastqc SRR25916244.fastq
```

## Visualización de los resultados

```bash
xdg-open SRR25916244_fastqc.html
```
