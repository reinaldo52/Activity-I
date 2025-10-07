
CONJUNTO DE DATOS SINTÉTICO: DESERCIÓN ESCOLAR UNIVERSITARIA

DESCRIPCIÓN GENERAL
Este conjunto de datos sintético fue creado con el objetivo de simular un escenario realista
de deserción escolar universitaria durante el primer año académico. Permite desarrollar
modelos de aprendizaje supervisado para predecir la deserción de estudiantes y diseñar
estrategias de retención.

El dataset fue generado utilizando Python (NumPy y Pandas) con 500 registros que incluyen
variables demográficas, académicas y financieras, además de la variable de resultado:
Deserción (Sí/No).

------------------------------------------------------------
VARIABLES INCLUIDAS
------------------------------------------------------------
1. Edad: numérica (entero) - Edad del estudiante (15–40, con atípicos fuera de 17–25).
2. Género: categórica - Masculino / Femenino / Otro.
3. Lugar_Origen: categórica - Rural / Urbano.
4. Promedio_Bachillerato: numérica (float) - Promedio (0–10, con atípicos).
5. Examen_Admision: numérica (float) - Resultado del examen de admisión (0–100).
6. Calif_Primer_Semestre: numérica (float) - Promedio del primer semestre (0–10).
7. Nivel_Socioeconomico: categórica - Bajo / Medio / Alto.
8. Beca: categórica - Sí / No.
9. Ayuda_Financiera: categórica - Sí / No.
10. Desercion: categórica - Variable objetivo (Sí / No).

------------------------------------------------------------
VALORES NULOS Y ATÍPICOS
------------------------------------------------------------
VALORES NULOS
Se introdujo un 3% de valores nulos aleatorios en las columnas:
- Promedio_Bachillerato
- Examen_Admision
- Calif_Primer_Semestre
- Nivel_Socioeconomico

Esto se realizó usando df.sample(frac=0.03) para simular registros incompletos.

VALORES ATÍPICOS
Se introdujeron manualmente:
- Edad: valores extremos como 10, 30, 35, 40.
- Promedio_Bachillerato: valores 1, 2, 10 fuera de la media.
Con el fin de representar datos reales fuera de rango esperado.

------------------------------------------------------------
GENERACIÓN DEL DATASET
------------------------------------------------------------
1. Se usaron NumPy y Pandas para crear variables aleatorias.
2. Se establecieron distribuciones realistas (edad centrada en 20 años).
3. Se calculó probabilidad de deserción influida por rendimiento y nivel socioeconómico.
4. Se generó variable binaria “Desercion” (Sí/No) basada en dicha probabilidad.

------------------------------------------------------------
USO DEL DATASET
------------------------------------------------------------
Este conjunto de datos puede emplearse para:
- Entrenar modelos de aprendizaje supervisado (clasificación binaria).
- Analizar factores asociados a la deserción.
- Evaluar estrategias de intervención educativa y predicción temprana.

------------------------------------------------------------
ARCHIVOS INCLUIDOS
------------------------------------------------------------
- datos_desercion_sinteticos.csv → Dataset con 500 registros.
- README.txt → Descripción del conjunto de datos.
