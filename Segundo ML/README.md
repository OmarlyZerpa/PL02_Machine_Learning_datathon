![HenryLogo](https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png)

# Machine Learning

Segundo proyecto individual para la carrera de Date Science de Henry.

El desarrollo del proyecto se encuentra contenido en el cuaderno 'data.ipynb'

## Descripción del problema

El proyecto consiste en generar un modelo de Machine Learning capaz de clasificar propiedades del mercado inmobiliario de EEUU en tres categorias, basandose en el precio:

* 'low': Para precios entre 0 y 999 dólares.
* 'medium': Para precios entre 1000 y 1999 dólares.
* 'high': Para precios desde 2000 dólares en adelante.

Para esto nos fueron disponibilizados dos datasets conteniendo información sobre anuncios de propiedades en venta: uno para entrenar nuestros modelos (con información sobre el precio de cada inmueble) y el segundo lo usaríamos para generar las predicciones de nuestros modelos (sin la información sobre el precio de la propiedad).

Dentro de las columnas que compartían ambos datasets encontramos:

• Información de la  publicación del anuncio (url).

• La ubicación del inmuble tanto en términos de latitud y longitud, como region y estado en que se encuentra ubicada.

• Información relativa a la propiedad misma, como la cantidad de habitaciones, de baños, el área construida, el tipo de inmueble (casa, apartamento, etc.)

• Detalles del anuncio de venta como la descripción del inmueble.

## Solucion del problema

El enfoque para dar una solución al problema se concentró en tratar de limpiar los datos de la mejor manera posible para que, al momento de entrenar los modelos de ML, estos tuviesen la mejor posibilidad de dar un resultado satisfactorio.

Para esto, se realizo un analisis exploratorio de datos y algunas transformaciones, eliminando algunas columnas debido a que tenienan datos faltantes y no se tenie el criterio empleado para rellenar estos campo, estos cambios se pueden observar en la archivo 'data.ipynb'

Agrupadas las columnas necesarias para el estudio y realizado preporcesamiento y entrenamientos de los datos, se Implementar un modelo de clasificación con aprendizaje supervisado random forests.

## Resultados

El RandomForestClassifier  obtuvo una puntuación de accuracy de 0.8 y de recall de 0.98.  Se considera que el proceso seguramente puede mejorarse.
