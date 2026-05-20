# Análisis de depreciación y valor de mercado: coches en Ucrania

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

## Descripción del proyecto
Este proyecto realiza un **Análisis Exploratorio de Datos (EDA)** detallado sobre un dataset de más de **9.500 ventas de automóviles** en Ucrania. 

El objetivo principal es identificar patrones de precios, analizar la depreciación de los vehículos y limpiar inconsistencias para obtener métricas fiables del mercado de segunda mano. Es un ejercicio de limpieza de datos real donde la calidad del dato prima sobre la cantidad.

---

## Tecnologías utilizadas
* **Python**: lenguaje base del análisis.
* **Pandas**: piedra angular para la manipulación y limpieza de datos.
* **Matplotlib / Seaborn**: herramientas de visualización para la detección de valores atípicos y análisis de distribución.

---

## Fases del análisis

### 1. Limpieza y transformación de datos 
Se realizaron ajustes críticos para asegurar la integridad de los resultados:
* **Conversión de tipos**: transformación de variables de `object` a `float` (específicamente en columnas de precio y cilindrada).
* **Normalización**: ajuste de separadores decimales y eliminación de caracteres no numéricos.

### 2. Tratamiento de valores atípicos (outliers) 
Para evitar sesgos estadísticos, se aplicaron filtros basados en el conocimiento del dominio del mercado automotriz:
* **Precios**: se acotó el rango entre **500€** y **150.000€**. Esto elimina "anuncios gancho" y vehículos de lujo extremo que distorsionan la media.
* **Cilindrada (engV)**: se mantuvo el rango lógico entre **0.5L y 7L**, eliminando errores de entrada de datos.

### 3. Hallazgos clave 
* **El enigma del "precio 0"**: se descubrió que el **24.34%** de estos casos corresponden a coches nuevos (año 2016), lo que indica que el precio suele ser "bajo consulta" en concesionarios.
* **Estabilización**: tras el filtrado, la cercanía entre la media y la mediana confirma que los datos ahora representan fielmente la realidad del mercado.

---

## ¿Cómo ejecutarlo?

1. **Clonar el repositorio:**
   ```bash
   git clone [https://github.com/tu-usuario/tu-repositorio.git](https://github.com/tu-usuario/tu-repositorio.git)
   
2. **Ejecutar el notebook**

   Para visualizar o replicar este análisis, abre el archivo `solucion_EDA_libre.ipynb` en tu entorno preferido:

* **Jupyter Notebook** o **JupyterLab**.
* **VS Code** (asegúrate de tener instalada la extensión de *Jupyter*).
* **Google Colab** (puedes subir el archivo `.ipynb` directamente a una nueva sesión).

3. **Dataset**

   El dataset original utilizado para este estudio puede encontrarse en:

* **Kaggle:** [Car Sales Dataset in Ukraine](https://www.kaggle.com/datasets/swatikhedekar/eda-on-car-sales-dataset-in-ukraine/data)

## Contexto académico

Este proyecto fue realizado como parte de mis prácticas del **Máster en Data Science**, con el objetivo de demostrar habilidades en:
* **Limpieza de datos complejos**: manejo de tipos de datos incorrectos y formatos inconsistentes.
* **Tratamiento de valores atípicos**: aplicación de lógica de negocio para filtrar *outliers*.
* **Visualización estadística**: creación de gráficos para extraer insights de mercado.

---

**Desarrollado por:** Alicia Santamaría Román 

**Contacto:** https://linkedin.com/in/aliciasantamariaroman
