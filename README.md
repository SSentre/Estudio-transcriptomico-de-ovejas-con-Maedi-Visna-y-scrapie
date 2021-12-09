# Estudio transcriptomico de ovejas con Maedi-Visna y scrapie

En este repositorio se encuentran recopilados los archivos con el código de comandos que se ha ido ejecutando para ir avanzando en la realización del trabajo y en la obtención de resultados usando como modelo el análisis de la muestra MS1 que pertenece al grupo de estudio de ovejas con la enfermedad lentiviral Maedi-Visna infectadas además con *scrapie*.

En trabajo se inició queriendo analizar los datos de RNA-seq con la herramienta TopHat2 por lo que la carpeta **1. TopHat2** contiene los primeros pasos.
- El archivo llamado **Workflow TopHat2 alineamiento contra genoma oveja.txt** además de tener los comandos necesarios para realizar el alineamiento de las muestras con TopHat2 tiene los comandos que se usaron en el proceso de control de calidad con PRINSEQ-lite.
- El archivo llamado **Workflow TopHat2 lecturas sin alinear.txt** contiene los comandos que se han utilizado para seleccionar las lecturas no alineadas obtenidas en el paso anterior con TopHat2 y el alineamiento de estas lecturas contra el genoma del lentivirus Maedi-Visna.

La carpeta **2. STAR** contiene los archivos con el código relevante al análisis con la herramienta STAR.
- El archivo llamado **Workflow STAR alineamiento genoma oveja.txt** contiene los comandos necesarios para realizar el alineamiento de las muestras de estudio contra el genoma de referencia de oveja.
- El archivo llamado **Workflow STAR lecturas sin alinear.txt** contiene los comandos que se han utilizado para seleccionar las lecturas no alineadas obtenidas en el paso anterior de alineamiento con STAR y el alineamiento de estas lecturas contra el genoma del lentivirus Maedi-Visna tanto con la herramienta Bowtie2 como con STAR.

La carpeta **3. R + Bioconductor** contiene los archivos con el *counting* de cada una de las muerstras obtenido gracias a los alienamientos con STAR, un archivo .txt con la información de las muestras a analizar, un archivo .RMD con el worfflow y los comandos que se han utilizado en R y *Bioconductor* para realizar el análisis de expresión diferencial y un archivo .HTML con el output de R Markdown de esos comandos.
