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
    
