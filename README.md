
# Análisis de Clúster de Reseñas de Clientes de Amazon

## Descripción del Proyecto

Este proyecto aplica **clustering (agrupación)** usando **Machine Learning no supervisado** para identificar segmentos de usuarios según su comportamiento de reseñas en Amazon.

Usamos técnicas de **PySpark** para procesar grandes volúmenes de datos de reseñas, generamos perfiles de usuarios y aplicamos **K-Means** para segmentarlos en grupos significativos. Además visualizamos los resultados con gráficos y reducción de dimensión usando PCA.

---

## 📂 Dataset

El dataset utilizado se puede descargar desde **Kaggle**:

👉 https://www.kaggle.com/datasets/vivekprajapati2048/amazon-customer-reviews

Este dataset contiene reseñas de clientes de Amazon con información como:

- `CustomerID`
- `Score` (calificación)
- `HelpfulnessNumerator` (votos útiles)
- `HelpfulnessDenominator` (total de votos)
- Texto de reseña
- Otras variables descriptivas

---

## 📥 Cómo descargar el dataset

1. Visita el siguiente enlace:
   
   https://www.kaggle.com/datasets/vivekprajapati2048/amazon-customer-reviews

2. Inicia sesión en Kaggle (si no tienes cuenta, regístrate).

3. Descarga el archivo comprimido.

4. Descomprime el archivo y localiza el archivo `.csv` para usarlo en el proyecto.

---

## 📁 Estructura del proyecto

amazon-review-clustering/

│

├── analisis_clustering.ipynb       ← Notebook principal con el código

├── dataset.csv                     ← Archivo CSV con los datos (no incluido por tamaño)

├── README.md                       ← Archivo de documentación (este)

└── requirements.txt                

---

## Tecnologías utilizadas

Este proyecto fue desarrollado con:

- **Python**
- **PySpark** (procesamiento distribuido)
- **Pandas** (conversión para visualizaciones)
- **Matplotlib** (gráficos)
- **Seaborn** (visualizaciones estadísticas)
- **NumPy**
- **Jupyter Notebook / Databricks**

---

## Cómo ejecutar el notebook

### Paso 1: Preparar el entorno

Si vas a trabajar de forma local:

1. Asegúrate de tener Python instalado.
2. Instala las bibliotecas necesarias con requirements.txt:

```bash
pip install -r requirements.txt
```
co con:

```bash
pip install pyspark pandas numpy matplotlib seaborn
```

Si usas Databricks, no necesitas instalar nada adicional.

### Paso 2: Colocar el dataset

Después de descargar y descomprimir el dataset:
	1.	Ubica el archivo .csv dentro de tu carpeta del proyecto.
	2.	Asegúrate de que esté accesible desde el notebook, por ejemplo:

amazon-review-clustering/dataset.csv



### Paso 3: Abrir y ejecutar el Notebook
	1.	Abre el archivo analisis_clustering.ipynb.
	2.	Ejecuta las celdas en orden desde arriba hacia abajo.
	3.	Verifica que al cargar el dataset no haya errores de ruta.
	4.	Continúa con la preparación de datos, clustering y visualizaciones.


## Metodología

El análisis sigue estos pasos principales:
	1.	Carga y exploración del dataset
	2.	Feature engineering — agregación por usuario
	3.	Escalamiento de variables usando StandardScaler
	4.	Aplicación de K-Means clustering
	5.	Resumen estadístico por cluster
	6.	Visualización de resultados
	•	Gráfica de barras
	•	Boxplot de distribución
	•	PCA para visualización 2D

---
## Resultados

El análisis generó:
	•	Segmentos de usuarios con comportamientos distintos.
	•	Perfiles de clientes según actividad y satisfacción.
	•	Gráficas que permiten visualizar y comparar clusters.
	•	Reducción de dimensionalidad para representación 2D.


## Interpretación de los resultados

Los clusters identificados muestran segmentos diferenciados de usuarios:
	•	Usuarios más activos
	•	Usuarios críticos
	•	Usuarios altamente satisfechos
	•	Usuarios con alto impacto en votos útiles

Estos segmentos tienen aplicación práctica en:
	•	Estrategias de marketing
	•	Sistemas de recomendación
	•	Mejora de experiencia del cliente


---

## 📌 Notas importantes
	•	El dataset no está incluido por restricciones de tamaño.
	•	Para grandes volúmenes es preferible ejecutar el notebook en entornos como Databricks o Google Colab.
	•	Asegúrate de tener suficiente memoria si trabajas localmente.



Proyecto de Clustering para análisis de comportamiento en grandes volúmenes de datos

---
