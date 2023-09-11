---
title: "Solemne 1"
description: "En parejas diseñen y construyan un lente de Snapchat utilizando la integración SnapML. Pueden utilizar cualquiera de los templates de machine learning disponibles en la documentación de Snap. "
featured: true
seriesId: Solemnes
orderInSeries: 1
pubDate: "Sept 09 2023"
tags:
  - Snapchat
  - Filter
---

Empesamos con una lluvia de ideas con la cual llegamos a la decision algo estilo comic, en nuestras refrencias nos inspiramos en spider-verse y con eso en mente buscamos fotos que nos sirviera para entrenar el modelo.
nuestra idea es que dentro del filtro se vaya cambiando a diferentes estilos mientras que uno vaya tocando la pantalla.

| Intento 1 | Intento 2 |
| --- | ----------- |
| ![Imagen_Style_1](~/assets/Test_1.jpg) | ![Imagen_Style_2](~/assets/style_image.png) |
|  | |

| Intento 3 | Intento 3 |
| --- | ----------- |
| ![Imagen_Style_1](~/assets/style_A.png) | ![Imagen_Style_1](~/assets/style_A.png) |
|  | |

Nos fuimos al google colab y empezamos a crear el modelo

![screenshot](~/assets/image.png)
| |  |
| --- | ----------- |
| ![screenshot](~/assets/TestA.png) | ![screenshot](~/assets/TestB.png) |
| ![screenshot](~/assets/TestC.png) | | 

| Modelo 1 | Modelo 2 |
| --- | ----------- |
| ![Imagen_Style_1](~/assets/IMG_0992.jpg) | ![Imagen_Style_2](~/assets/Test_2.jpeg) |

| Modelo 3 |  |
| --- | ----------- |
| ![Imagen_Style_1](~/assets/Style3.jpg) | ![Imagen_Style_1](~/assets/Style3.jpg) |
|  | |

Una vez terminado de crear el modelo nos pusimos a crear el filtro en snapchat lens.

Lo primero que hicimos fue usar el template de style transfer y tratar de remplacar los ML components para ir agregando los modelos, para probar el cambio de estilo primero intentamops con el script behavior, luego de varios intentos no resulto.

por lo que empezamos a investigar en youtube y logramos encontrar una forma de hacerlo con los script graph.

![Image](~/assets/ScriptGraph.png)

Luego de eso nos encontramos con otro problema, no lograbamos que se loopiara. Tiempo despues descubrimos que era porque estabamos usando directamente  los ML components. Investigando un poco más encontramos la forma correcta de hacerlo, que es creando screen image y ML components por cada Style asignandolos al Script Graph que conseguimos anteriormente. 

![Image](~/assets/Valores.png)

Finalmente le agregamos un texto para indicar la intencion del filtro.

|  | Gameplay Click en la imagen Para verlo|
| --- | ----------- |
|  | [![Link Del Gamplay](~/assets/Texto.jpg)](https://youtube.com/shorts/0htxqKCDGVs?feature=share) |
|  | |
