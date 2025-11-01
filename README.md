#Análisis Comparativo de Textos Históricos: Guerra de los 30 Años vs. Guerras Napoleónicas

por: David Alejandro Restrepo Tuberquia

Este proyecto realiza un análisis de procesamiento de lenguaje natural (PLN) para comparar la estructura, longitud y contenido temático de dos textos clave que describen conflictos fundamentales en la historia europea.

#Metodología del Análisis

El proceso se dividió en tres fases principales utilizando Python:

1. Preprocesamiento y Normalización
Se aplicó un proceso riguroso de limpieza a los textos originales (brutos) para garantizar la precisión del análisis temático:

- Limpieza de Ruido: Eliminación de etiquetas HTML, URLs, y emojis.

- Estandarización: Conversión a minúsculas y eliminación de espacios/saltos de línea extra, asegurando que la puntuación estuviera separada correctamente para el conteo de frases.

- Separación de Versiones: Se mantuvieron variables separadas para el texto original (bruto) y el texto limpio (pwn, nwn) para garantizar la inmutabilidad de la fuente.

2. Análisis Estructural Básico (Sin spaCy)
 
Se calcularon métricas básicas para entender la estructura de cada discurso:

- Párrafos, Frases y Palabras: Conteo basado en saltos de línea y signos de puntuación de fin de frase.

- Complejidad Sintáctica: Medición de la Longitud Media de Frase (palabras por frase) para inferir la densidad y el estilo de redacción de cada texto.

3. Análisis Temático Avanzado (con spaCy)
  
Para revelar el núcleo temático de cada discurso, se utilizó la librería spaCy (modelo en español es_core_web_sm)

- Lematización: Cada palabra fue reducida a su raíz o lema, garantizando que las variaciones de una misma palabra se cuenten juntas

- Filtrado: Eliminación de stopwords (palabras comunes como "el", "de", "y") y signos de puntuación.Frecuencia: Se utilizó Counter para obtener las palabras temáticas más frecuentes de cada texto.

4. Resultados y Conclusiones Temáticas

El análisis temático, basado en las palabras clave predominantes después del filtrado, reveló una profunda diferencia en la visión de la soberanía y el conflicto en cada periodo

4.1. Guerra de los 30 Años (Texto 1)

- Los temas centrales están íntimamente ligados a la religión y el dominio espiritual.

- La toma de territorio no solo implicaba la adquisición de tierras, sino la "toma de las almas de quienes viven allí".

- El significado de la posesión territorial estaba directamente relacionado con la fe y la posibilidad de "ir al cielo o al infierno", reflejando la "gran influencia eclesiástica" en el Estado europeo de mediados del siglo XVII.

4.2. Guerras Napoleónicas (Texto 2)

- El foco temático se desplaza hacia el poder secular, la soberanía nacional y la ideología de la Ilustración.

- Se observa una "toma simbólica del poder" con la "tierra como eje central".

- El texto refleja la "libertad 'Ilustrada' que representaba Napoleón" en oposición a la nobleza tradicional.

5. Conclusión General


El análisis de frecuencias temáticas ilustra la transformación histórica de Europa. El discurso asociado a la Guerra de los 30 Años revela un concepto de Estado con fuerte influencia eclesiástica y soberanía basada en una propiedad de origen percibido como divino. Por contraste, el texto de las Guerras Napoleónicas muestra el surgimiento de estados modernos cuya soberanía se fundamenta en un sentido de pertenencia profundo y nacionalista, un concepto que ha perdurado hasta el día de hoy.
