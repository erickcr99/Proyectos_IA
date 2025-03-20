# 🎬 Sistema de Recomendación de Películas  

Este proyecto implementa un sistema de recomendación de películas utilizando **filtrado basado en contenido** y **filtrado colaborativo**. Es útil para plataformas de streaming, tiendas en línea y cualquier servicio que busque personalizar la experiencia del usuario.  

## 📜 Descripción del Proyecto  

El sistema sugiere películas a los usuarios con base en dos enfoques:  
1. **Filtrado Basado en Contenido**: Se analizan los géneros y características de las películas para encontrar similitudes.  
2. **Filtrado Colaborativo**: Se utilizan técnicas de descomposición en valores singulares (**SVD**) para predecir calificaciones y sugerir películas similares a las que el usuario ha visto.  

Los datos utilizados provienen del conjunto de datos [MovieLens](https://grouplens.org/datasets/movielens/), que contiene miles de calificaciones de usuarios sobre diferentes películas.  

## 🛠 Tecnologías Utilizadas  

- Python 🐍  
- Pandas 📊  
- NumPy 🔢  
- Scikit-learn 🤖  
- Matplotlib 📉  
- Seaborn 🎨  

## 🚀 Instalación  

1️⃣ **Clona este repositorio**  
git clone https://github.com/erickcr99/Proyectos_IA.git

2️⃣ Navega hasta la carpeta del proyecto
cd Proyectos_IA/Sistema_de_Recomendacion_de_Peliculas

3️⃣ Instala las dependencias necesarias
pip install -r requirements.txt

4️⃣ Abre el notebook en Google Colab o Jupyter Notebook y ejecútalo

## 📊 Visualización de Resultados
A lo largo de la libreta, se generan gráficos y tablas que muestran:
✅ La matriz TF-IDF de similitud de películas.
✅ La tabla de recomendaciones generadas para un usuario específico.
✅ La evaluación del sistema con métricas como RMSE.

## ✨ Uso
Puedes ejecutar la función de recomendación en el notebook de la siguiente manera:
# Obtener recomendaciones basadas en contenido
recomendaciones = content_based_recommendations("The Matrix", cosine_sim_df, num_recommendations=5)
print(recomendaciones)
# Obtener recomendaciones basadas en filtrado colaborativo
recomendaciones_usuario = collaborative_recommendations(1, user_movie_matrix, matrix_svd, num_recommendations=5)
print(recomendaciones_usuario)

## 🎯 Contribuciones
Si deseas mejorar este proyecto, ¡siéntete libre de contribuir! Puedes abrir un issue o enviar un pull request con mejoras.

## 📝 Licencia
Este proyecto se distribuye bajo la Licencia MIT.

## 📌 Desarrollado por Alejandro Erick Cano Rosas
📅 Fecha: Marzo 2025
