# Análisis de la evolución de la matriz energética de México

## Introducción

En este proyecto se analiza la evolución de la matriz energética de México a partir de datos históricos de consumo energético. El análisis busca caracterizar la participación de fuentes de energía limpia a lo largo del tiempo y utilizar esta evolución como referencia empírica para la construcción de una trayectoria de mitigación.

Los datos utilizados provienen del repositorio **Energy Data** de [Our World in Data](https://github.com/owid/energy-data), específicamente del archivo `owid-energy-data.csv`. Este conjunto contiene información histórica sobre producción y consumo de diferentes fuentes de energía para distintos países.

A partir de los datos correspondientes a México se calcula la proporción de energía proveniente de fuentes limpias respecto al consumo energético total. Posteriormente, se evalúan diferentes funciones matemáticas para representar la evolución temporal de esta proporción.

Se consideran ajustes lineales, cuadráticos, cúbicos, logísticos, Gompertz y sigmoides, comparando su desempeño para identificar las trayectorias que mejor describen los datos observados. Finalmente, se selecciona una trayectoria cuadrática como alternativa intermedia entre las trayectorias sigmoidal libre y sigmoidal acotada en $1$.

## Objetivo

Construir y evaluar una trayectoria matemática que represente la evolución de la proporción de energía limpia en México, utilizando datos históricos como referencia empírica para utilizarla como referencia en la construcción de la función techo de mitigación `miuup` del modelo DICE.

Los objetivos específicos son:

* Procesar y analizar los datos energéticos de México.
* Calcular la proporción de energía limpia respecto al consumo energético total.
* Explorar la evolución temporal de esta proporción.
* Ajustar diferentes funciones matemáticas a los datos.
* Comparar el desempeño de los distintos ajustes.
* Seleccionar una trayectoria adecuada para utilizarla como referencia en el análisis de mitigación.
