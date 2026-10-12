# Sistemas recomendadores

Notebook de la lección de sistemas recomendadores, ejecutado con 45,466 películas.

## Contenido

- Ranking ponderado con percentil 90 de votos (C = 5.618207215134; m = 160).
- Recomendaciones por sinopsis con TF-IDF y similitud coseno.
- Recomendaciones por keywords y géneros con CountVectorizer.
- Integración automática de actores y director al añadir data/credits.csv. Ese archivo no estaba entre los materiales recibidos; los resultados guardados corresponden al modelo parcial.

## Ejecutar

Instala las dependencias con `pip install -r requirements.txt`, inicia `jupyter notebook` desde la raíz y abre `sistemas_recomendadores.ipynb`. Ejecuta todas las celdas en orden.

Los archivos movies_metadata.csv y keywords.csv de la lección están incluidos en data/. El notebook calcula similitudes por consulta para evitar una matriz completa de unos 16.5 GB. Detecta títulos ambiguos y permite resolverlos con movie_id.

## Verificación

Todas las celdas se ejecutaron correctamente. Se verificaron el orden del ranking, la exclusión de la película consultada, los límites de similitud y los títulos inexistentes. Estas comprobaciones no miden calidad con usuarios reales.

Datos históricos de películas hasta 2017, procedentes del material del curso (The Movies Dataset / MovieLens). Las recomendaciones no representan preferencias personales ni catálogos actuales.
