# Right Journey
## Elige el lugar perfecto para tu viaje de mochilero

Right Journey es una aplicación que permite realizar búsqueda basada en parámetros dados por el usuario. El objetivo de esta aplicación web es dar recomendaciones de lugares, pero de aquellos que sean poco conocidos. De tal manera que el turismo sea más amplio y poco centralizado. 

## Tecnologias
Las tecnologías usadas para ente proyecto son ampliamente basadas en Azure 
- App Services 
    - Wordpress
    - Trigger sobre tweets relacionados a los parámetros de búsqueda
    - Proceso de filtrado de resultados
- Data Lake
- Cognitive Services 
    - Text Analytics
- API de Twitter
- 
    
## Diagrama de proceso
En este diagrama se muestra el proceso de trabajo, posiblemente cambien según se haga más complejo el proceso de trabajo
https://miro.com/app/board/uXjVOacnOsM=/?invite_link_id=106616686074


## Proceso
El proceso se puede resumir en los siguientes pasos 

- Aplicación web con formulario solicitando los parámetros de búsqueda (Opciones de viaje, temáticas, popularidad, etc)
- El trigger recibe los parámetros de búsqueda y comienza a realizar la búsqueda de tweets relacionados con la ayuda de la API de Twitter
- Se ordenan y filtrar aquellos resultados que cumplan ciertas características (tiempo de publicación y que se clasifique como reseña y/o visita)
- Se guardan los resultados importantes en la base de datos como un Data Lake. 
- Mediante un trigger y Text Analytics de App Services, se filtran y contabilizan los resultados guardados en el Data Lake, de tal de solo extraer aquello relevante
- Se ordenan y dan formato a los resultados para ser mostrados dentro de la aplicación web
- Se envían los datos resultantes al usuario para su evaluación

## Demo
- https://framer.com/share/Hack-oudini--bcfdWKtipUxrv4P9Z4U4/tPXs5Djc3#tPXs5Djc3

## Tiktok 
- https://www.tiktok.com/@sirjohn125/video/7043596397685361926?lang=es&is_copy_url=0&is_from_webapp=v1&sender_device=pc&sender_web_id=7020516431687173637

## Integrantes 
- sa318728@uaeh.edu.mx
- juan.gonzalezf@alumno.buap.mx
- uriel.Alatorre@comunidad.unam.mx
- inv1020@innovaccion.mx

