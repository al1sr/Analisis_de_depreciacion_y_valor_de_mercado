# Depreciation and market value analysis: cars in Ukraine

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

## Project description
This project carries out a detailed **Exploratory Data Analysis (EDA)** on a dataset of over **9,500 car sales** in Ukraine. 

The main objective is to identify pricing patterns, analyse vehicle depreciation and clean up inconsistencies to obtain reliable metrics for the second-hand market. It is a real-world data cleaning exercise where data quality takes precedence over quantity.

## Technologies used
* **Python**: the core language for the analysis.
* **Pandas**: the cornerstone for data manipulation and cleaning.
* **Matplotlib / Seaborn**: visualisation tools for outlier detection and distribution analysis.

## Phases of the analysis

### 1. Data cleaning and transformation 
Critical adjustments were made to ensure the integrity of the results:
* **Type conversion**: transformation of variables from `object` to `float` (specifically in the price and engine capacity columns).
* **Normalisation**: adjustment of decimal separators and removal of non-numeric characters.

### 2. Handling outliers 
To avoid statistical bias, filters were applied based on an understanding of the automotive market:
* **Prices**: the range was restricted to between **€500** and **€150,000**. This eliminates ‘bait ads’ and ultra-luxury vehicles that distort the mean.
* **Engine capacity (engV)**: the logical range between **0.5L and 7L** was maintained, eliminating data entry errors.

### 3. Key findings 
* **The ‘price 0’ conundrum**: it was found that **24.34%** of these cases correspond to new cars (2016 model year), indicating that the price is often ‘on request’ at dealerships.
* **Stabilisation**: following filtering, the closeness between the mean and the median confirms that the data now accurately reflects market reality.

## How to run it?

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/tu-usuario/tu-repositorio.git](https://github.com/tu-usuario/tu-repositorio.git)
   
2. **Run the notebook**

   To view or replicate this analysis, open the file `solucion_EDA_libre.ipynb` in your preferred environment:

* **Jupyter Notebook** or **JupyterLab**.
* **VS Code** (make sure you have the *Jupyter* extension installed).
* **Google Colab** (you can upload the `.ipynb` file directly to a new session).

3. **Dataset**

   The original dataset used for this study can be found at:

* **Kaggle:** [Car Sales Dataset in Ukraine](https://www.kaggle.com/dataset

## Academic context

This project was carried out as part of my work placement for the **Master’s in Data Science**, with the aim of demonstrating skills in:
* **Complex data cleaning**: handling incorrect data types and inconsistent formats.
* **Handling outliers**: applying business logic to filter outliers.
* **Statistical visualisation**: creating charts to extract market insights.

**Developed by:** Alicia Santamaría Román 

**Contact:** https://linkedin.com/in/aliciasantamariaroman
