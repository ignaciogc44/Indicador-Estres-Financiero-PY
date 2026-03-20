# Indicador de estrés financiero

Proyecto de portafolio orientado a estimar un indicador de estrés financiero a partir de variables macroeconómicas y financieras.

## Contenido

- [Indicador_estres.ipynb](Indicador_estres.ipynb): notebook principal con carga de datos, exploración, regresión logística y visualización de la serie estimada.
- `Datos Modelo.xlsx`: base utilizada por el notebook.
- `DatosLogit.xlsx`: salida generada con la probabilidad estimada y la tendencia suavizada.

## Qué hace el notebook

El análisis sigue este flujo:

1. Carga de datos desde archivo local o desde Google Colab.
2. Exploración descriptiva y análisis de correlaciones.
3. Estimación de una regresión logística para aproximar la probabilidad de crisis.
4. Construcción y visualización de la serie estimada junto con una tendencia suavizada.

## Requisitos

El notebook fue pensado para ejecutarse en Python 3 y utiliza principalmente:

- pandas
- numpy
- statsmodels
- seaborn
- matplotlib
- scikit-learn
- openpyxl

Podés instalar las dependencias con:

```bash
pip install -r requirements.txt
```

## Ejecución

Abrí [Indicador_estres.ipynb](Indicador_estres.ipynb) en Jupyter o en Google Colab y ejecutá las celdas en orden.

Si se ejecuta localmente, el notebook intentará leer `Datos Modelo.xlsx` desde esta carpeta. En Colab, si el archivo no está disponible, permite cargarlo manualmente.
