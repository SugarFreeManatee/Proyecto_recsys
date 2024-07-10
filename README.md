# Proyecto_recsys

Basado en [Spotify-Recomendation-System](https://github.com/abdelrhmanelruby/Spotify-Recommendation-System)
### Requerimientos
1. Python 3.10
2. Para instalar requerimientos:
`pip install -r requirements.txt`
### Ejecución
1. Generar features: Correr todas las celdas en Reading1M_feature_extraction.ipynb. Requiere credenciales de spotify.
2. Preprocesamiento de playlists: Correr preprocess.ipynb para generar un archivo de playlists filtradas que contiene solo tracks con features conocidas. Necesario para hacer refinement.
3. Crear embeddings iniciales: Correr todas las celdas de word2vec.ipynb
4. Refinement: Correr notebook contrastive_training.ipynb
5. Generar set de test: Correr test_set.ipynb
6. Entrenamiento LSTM y testeo: Correr notebook prediction.ipynb