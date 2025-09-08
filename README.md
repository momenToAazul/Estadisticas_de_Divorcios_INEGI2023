# Estadística de Divorcios 2023 - INEGI  

## **Descripción**  
Este repositorio contiene un análisis de la **Estadística de Divorcios 2023 (INEGI)**.  
El objetivo principal fue construir modelos de predicción para la variable `dura_leg` (duración legal del matrimonio), aplicando técnicas de **limpieza, imputación, selección de características y modelado estadístico**.  

Se desarrolló un flujo de trabajo completo que abarca:  

- Revisión del diccionario y normalización de códigos especiales de INEGI.  
- Tratamiento de valores faltantes mediante **moda, media, mediana y KNN imputer**.  
- Detección y corrección de **outliers** e **inconsistencias** (validación entre edades y duración del matrimonio).  
- Análisis de **colinealidad** y generación de variables de interacción (ej. diferencia de edad, mismas características de los cónyuges).  
- Codificación de variables cualitativas con **One-Hot Encoding**.  
- Selección rápida de características basada en ranking de correlaciones y validación cruzada.  
- Construcción y evaluación de modelos predictivos:  
  - **Regresión lineal**.  
  - **Regresión polinomial**.  
- Inferencia estadística con `statsmodels` para interpretar coeficientes y significancia de las variables.  

## **Contenido del proyecto**  

- Importación y limpieza de la base de **Divorcios INEGI 2023**.  
- Procesamiento de valores faltantes y generación de nuevas variables.  
- Análisis exploratorio de correlaciones y reducción de dimensionalidad.  
- Entrenamiento de modelos:  
  - Evaluación del $R^2$ y del Error Cuadrático Medio (MSE).  
  - Comparación entre regresión lineal y polinomial.  
- Inferencia estadística sobre el modelo óptimo.  

## **Resultados principales**  

- El modelo de **regresión polinomial** obtuvo un desempeño superior ($R^2 \approx 0.74$), frente al modelo lineal ($R^2 \approx 0.71$).  
- Variables como la **edad al divorcio**, el **número de hijos**, la **custodia** y la **diferencia de edad al matrimonio** resultaron altamente significativas.  
- La metodología permitió **reducir inconsistencias** y asegurar interpretabilidad de los resultados.  

## **Documentos**  

- [Notebook editable en formato .ipynb](./ED_INEGI2023_Editable.ipynb)  
- [Reporte en formato .html](./ED_INEGI2023_Rerpote.html)  

## **Base de datos**  

En caso de ejecutar el notebook (`.ipynb`), es necesario descargar la base de datos directamente desde INEGI:  

🔗 [Base de datos INEGI - Estadística de Divorcios 2023 (CSV)](https://www.inegi.org.mx/app/descarga/ficha.html?tit=2340795&ag=0&f=csv)  
