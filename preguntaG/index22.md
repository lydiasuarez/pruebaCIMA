---
layout: default
title: Apartado B
parent: Preguntas Genómica
nav_order: 2
---


# Apartado B

## Hemos iniciado el estudio del hepatocarcinoma recientemente, necesitamos saber la expresión de XBP1, ATF6 y CD36 en TCGA en el gráfico que consideres más explicativo. También hemos visto que se han publicado estos dos experimentos: GSE11536 y GSE154964 el primero más relacionado con HCV, también nos gustaría saber la expresión de estos genes en estos dos estudios. Explica los problemas que te han surgido y como los has resuelto.


### 1. Genes XBP1, ATF6 y CD36 de TCGA.

La expresión de los genes XBP1, ATF6 y CD36 de TCGA vamos a representarla por separado mediante un diagrama de cajas (boxplot). Para ello, utilizaremos la matriz que obtuvimos con los datos de expresión de todos los genes en el ejercicio de AI. Filtramos para cada boxplot por nuestro gen de interés para muestras con cáncer y sanas. A continuación puede observar el código de uno de los ejemplos:

```r
p <- ggplot(LIHC_matrix, aes(x=diagnosis, y=CD36, color=diagnosis))

p + 
geom_boxplot(fill= c("#66CC66","red3"), alpha=0.6,) + 
geom_jitter(size= 0.3, colour=c("black"), alpha=0.7) +
scale_color_manual(values=c("darkgreen","darkred"), name="Samples", labels=c("Health", "Tumor")) +
labs(x="Samples", y="CD36 Expression levels") +
coord_flip() +
theme(legend.position = c(0.92, 0.15),
      legend.title = element_text( size = 21),
      legend.text = element_text(size = 15))
```

El resultado se puede ver en las siguientes imágenes:

![image](./XBP1.jpg)

![image](./ATF6.jpg)

![image](./CD36.jpg)

### 2. Experimentos GSE11536 y GSE154964.

En cuanto a la expresión de estos mismos genes en los experimentos GSE11536 y GSE154964, no he podido encontrar la información relativa a la expresión de dichos genes individualmente. Por lo que ha sido imposible realizar este apartado del ejercicio.

