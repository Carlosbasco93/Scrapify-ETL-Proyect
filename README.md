![portada](https://github.com/Carlosbasco93/Scrapify-ETL-Proyect/blob/main/images/portada.jpg)

# Scrapify-ETL-Proyect

## Objetivo del proyecto:
El proyecto de la semana 4 del Bootcamp de Data Analyst consiste en realizar un proceso completo ETL. Con esto podremos:

    - Familiarizarnos con los procesos de obtener datos (APIs, Scraping, Databases de 
    diferentes páginas web...)
    - Transformar los datos y limpiarlos según sea necesario.
    - Cargar los datos limpios en una BBDD sobre la que poder realizar consultas.


### Requesitos:
    - Obtener datos provenientes de al menos 3 fuentes de información diferentes.
    - Utilizar al menos 2 métodos de obtención de información


## Dirección tomada:

He optado por realizar la extracción de datos sobre la aplicación de Spotify. Para ello:

    - Accederé con mis credenciales para llegar al listado completo de las canciones que dí "Like" para proceder a 
    escrapear la información que se me ofrece en ese apartado. (1400 canciones aprox)
    - Enriqueceré este listado obteniendo los géneros en los que los artistas están catalogados junto a su 
    número de seguidores.
    - Realizaré una comparación de estas canciones contra una BBDD de Kaggle sobre los Top Hits de 2000-2019 
    para buscar coincidencias.
    
    
### Principales problemas sorteados:
    - Obtener la máxima cantidad de canciones evitando en la medida de lo posible la obtención de duplicados 
    para facilitar la labor de limpieza.
    - Controlar los casos en los que no podamos obtener toda la información de los artistas/canciones que queramos.
    
### Imagenes:
#### Selenium

-Login:

<img src="https://raw.githubusercontent.com/Carlosbasco93/Scrapify-ETL-Proyect/main/images/1.png" width="700">

-Accede a la lista de las canciones que te gustan:

<img src="https://raw.githubusercontent.com/Carlosbasco93/Scrapify-ETL-Proyect/main/images/2.png" width="700">

-Va realizando scroll tomando las canciones:

<img src="https://raw.githubusercontent.com/Carlosbasco93/Scrapify-ETL-Proyect/main/images/3.png" width="700">

-Escrapearemos los resultados de los links de todos los grupos buscados:

<img src="https://raw.githubusercontent.com/Carlosbasco93/Scrapify-ETL-Proyect/main/images/4.png" width="700">


#### SQL

-Vista previa de la BBDD SQL que queda tras ejecutar el código:

<img src="https://raw.githubusercontent.com/Carlosbasco93/Scrapify-ETL-Proyect/main/images/5.png" width="700">

#### Resultados

-Listado liked songs vista previa:

<img src="https://raw.githubusercontent.com/Carlosbasco93/Scrapify-ETL-Proyect/main/images/Muestra%20Liked_songs.png" width="700">


-Coincidencias vs top hits 2000-2019:

<img src="https://raw.githubusercontent.com/Carlosbasco93/Scrapify-ETL-Proyect/main/images/Cruce%20Liked%20vs%20Top%20songs.png" width="700">

-Tus grupos con mayor frecuencia:

<img src="https://raw.githubusercontent.com/Carlosbasco93/Scrapify-ETL-Proyect/main/images/Num_songs%20-%20Grupo.png" width="700">


#### Otras utilidades:

-Busqueda por género de tus canciones:

<img src="https://raw.githubusercontent.com/Carlosbasco93/Scrapify-ETL-Proyect/main/images/Query%20busqueda%20por%20genero.png" width="500">


-Actualizar la BBDD buscando los grupos sin categoría asignada:

<img src="https://raw.githubusercontent.com/Carlosbasco93/Scrapify-ETL-Proyect/main/images/Query%20grupos%20desconocidos.png" width="500">


#### Fuentes empleadas:
    Spotify - https://open.spotify.com/
    EveryNoiseAtOnce - https://everynoise.com/
    Kaggle - https://www.kaggle.com/datasets/muhmores/spotify-top-100-songs-of-20152019
