# <h1 align=center> **PROYECTO INDIVIDUAL** </h1>
# <h1 align=center>**`Machine Learning Operations (MLOps)`**</h1>


## <h2 align=center>**`Introducción y descripción del Proyecto`**</h2>

**¡Bienvenido/a a mi proyecto individual de Machine Learning Operations (MLOps)!**

En este proyecto, mi objetivo es llevar un modelo de recomendación que he desarrollado en un entorno de Data Science al mundo real, abordando los desafíos del ciclo de vida completo de un proyecto de Machine Learning.

Imaginate esto: Empezaste a trabajar como Data Scientist en Steam, una plataforma multinacional de videojuegos. El mundo es bello y vas a crear tu primer modelo de ML que soluciona un problema de negocio: Steam pide que te encargues de crear un sistema de recomendación de videojuegos para usuarios.

Vas a sus datos y te das cuenta que la madurez de los mismos es poca: Datos anidados, de tipo raw, no hay procesos automatizados para la actualización de nuevos productos, entre otras cosas… haciendo tu trabajo imposible.

## <h2 align=center>**`Proceso de Extracción, Transformación y Carga (ETL)`** </h2>

En el marco de este proyecto, se nos asignaron tareas específicas relacionadas con la manipulación de datos, las cuales formaron parte integral del proceso conocido como Extracción, Transformación y Carga (ETL). Para brindarte una comprensión más detallada de cómo se llevaron a cabo estas transformaciones, a continuación, te ofrecemos una breve sinopsis de las actividades realizadas:

+ Desanidamiento de campos: Algunos campos, como "reviews" y "genres", se encontraban anidados en el conjunto de datos. Se implementó un proceso de desanidamiento con el fin de abrir estos campos y permitir su integración de manera más efectiva.

+ Normalización de formatos de fechas: Alineamos las fechas presentes en el conjunto de datos al formato AAAA-mm-dd para asegurar una mayor uniformidad. Además, creamos una nueva columna llamada "year" para extraer el año de la fecha de estreno.

+ Identificación y corrección de duplicados y formatos incorrectos: Llevamos a cabo una minuciosa revisión en busca de valores duplicados o con formatos incorrectos, aplicando las correcciones necesarias o eliminando los registros afectados.

+ Evaluación de la relevancia de las columnas y su eliminación, en caso de no ser útiles para la API o los modelos posteriores.

Estas acciones de transformación de datos desempeñaron un papel fundamental en la preparación del conjunto de datos, garantizando su adecuación para el análisis subsiguiente y su aplicación en el desarrollo del proyecto.


**El código se encuentra  en el apartado de Links, te redireccionan a un Google Drive donde están todos los archivos de Google Colab.**
https://drive.google.com/drive/folders/1pI7uhIHCqwEqkYCA-tH5ECTJVzv03Oqq?usp=sharing




### En esta etapa del proyecto, se propone disponibilizar los datos de la empresa mediante el uso del framework FastAPI. Se han definido 6 funciones para los endpoints que serán consumidos en la API.

+ def **PlayTimeGenre( *`genero` : str* )**:
    Debe devolver `año` con mas horas jugadas para dicho género.

+ def **UserForGenre( *`genero` : str* )**:
    Debe devolver el usuario que acumula más horas jugadas para el género dado y una lista de la acumulación de horas jugadas por año.

+ def **UsersRecommend( *`año` : int* )**:
   Devuelve el top 3 de juegos MÁS recomendados por usuarios para el año dado.

+ def **UsersNotRecommend( *`año` : int* )**:
   Devuelve el top 3 de juegos MENOS recomendados por usuarios para el año dado.

+ def **sentiment_analysis( *`año` : int* )**:
    Según el año de lanzamiento, se devuelve una lista con la cantidad de registros de reseñas de usuarios que se encuentren categorizados con un análisis de sentimiento.

+ def **recomendacion_juego( *`id de producto`* )**:
    Ingresando el id de producto, deberíamos recibir una lista con 5 juegos recomendados similares al ingresado.

## <h2 align=center> **`Links`**</h2>

- Deploy del Proyecto (Render): https://proyecto-individual-dt-henry.onrender.com
- Google Colab donde se realizaron todos los procesos (Drive): https://drive.google.com/drive/folders/1pI7uhIHCqwEqkYCA-tH5ECTJVzv03Oqq?usp=sharing
- Video del Proyecto: https://drive.google.com/file/d/1oTvnDH4tIM_Qo6Fsbv9YNUiF80bKJuIs/view?usp=sharing
