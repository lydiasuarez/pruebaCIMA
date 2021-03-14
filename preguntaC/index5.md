---
layout: default
title: Pregunta crítica
nav_order: 5
---

## Que pega le ve a este análisis de AI, si le encuentra alguna. 




Tras leer el artículo adjuntado he podido llegar a la conclusión de dos pequeñas críticas en el análisis de AI. En primer lugar, cabe destacar el limitado número de muestras lo que dificulta el proceso de entrenamiento de los modelos de machine learning. Además, en los datos _perdidos_ de algunas muestras se ha optado por ser completados mediante un paquete de R en vez de eliminar dichas muestras ya que no hay una gran cantidad de ellas, esto hace que la presición de esos datos pueda no ser adecuada. Y, en segundo lugar, la alta variabilidad de los datos entre muestras con un mismo diagnóstico (sanas/enfermas) complica la clafisicación de dichos grupos provocando una gran dispersión de los datos sin hallar un mismo patrón común entre todos ellos.

En cuanto a los modelos de machine learning utilizados para el procesamiento de datos, no podría aventurarme a evaluarlos ya que desconozco alguno de ellos y necesitaría, anteriormente, haber trabajado con los datos apara poder determinar si podría realizar algún apunte de la pipeline desarrollada.
