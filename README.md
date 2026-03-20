# Indicador de estrés financiero

Proyecto de portafolio orientado a estimar un indicador de estrés financiero con variables macroeconómicas y financieras. El análisis se realiza a partir de un trabajo realizado en la clase de Economía Monetaria, donde, de acuerdo con el trabajo de Cerro y Meloni (2004) y otra literatura sobre indicadores de alerta temprana, se construía un indicador de turbulencia de mercado "MTI" calculado usando la variación del tipo de cambio nominal, las reservas internacionales y las tasas de interés (cada uno dividido por su desvío estándar).

En este trabajo se toma como definición de turbulencia aquel mes donde el valor MTI fuera mayor al valor de un desvío estándar, siendo ese el caso en 26 de los 234 meses registrados.

Luego, se realiza una regresión logística que nos indica que tan probable es que un mes determinado se considere de turbulencia financiera.

## Contenido

- [Indicador_estres.ipynb](Indicador_estres.ipynb): notebook principal con carga de datos, exploración, regresión logística y visualización de la serie estimada.
- `Datos Modelo.xlsx`: base utilizada por el notebook.
- `DatosLogit.xlsx`: salida generada con la probabilidad estimada y la tendencia suavizada.

## Qué hace el notebook


1. Carga de datos desde archivo local o desde Google Colab.
2. Exploración descriptiva y análisis de correlaciones.
3. Estimación de una regresión logística para aproximar la probabilidad de crisis.
4. Construcción y visualización de la serie estimada junto con una tendencia suavizada.

## Requisitos

El notebook fue pensado para ejecutarse en Python y utiliza:

- pandas
- numpy
- statsmodels
- seaborn
- matplotlib
- scikit-learn
- openpyxl

Instalar dependencias con:

```bash
pip install -r requirements.txt
```

## Ejecución

Abrir [Indicador_estres.ipynb](Indicador_estres.ipynb) en Jupyter o en Google Colab y ejecutá las celdas en orden.

Si se ejecuta localmente, el notebook intenta leer `Datos Modelo.xlsx` desde esta carpeta. En Colab, si el archivo no está disponible, permite cargarlo manualmente.
