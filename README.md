# Prueba tecnica Galatea - Elowen


El proyecto contiene la solución de los niveles 2 y 3 de la prueba tecnica que consiste en construir un escenario que permita identificar si un manuscrito ingresado por orden de filas contiene una secuencia de al menos 4 apariciones de un mismo caracter. Para ello se emplo una infraestructura AWS con servicios Dynamo RDS y Lambda function bajo el lenguaje de java.

## Diagrama de flujo

![Diagrama de flujo](https://github.com/user-attachments/assets/23f33118-3062-4a0e-9617-e91a335df77c)



## Arquitectura de la solución

![Diagrama Arquitectura](https://github.com/user-attachments/assets/a4c32c6c-3272-49c6-bced-a8f6918c9320)



## ¿Cómo lo hago?
Para probar el proyecto se debe:
* Seleccionar pestaña Import
* Copiar y pegar el curl de la petición que se requiera 
* Enviar la petición


#### Request Clue
EndPoint de la solución: [https://9h0ovfjk8h.execute-api.us-east-2.amazonaws.com/dev/clue](https://9h0ovfjk8h.execute-api.us-east-2.amazonaws.com/dev/clue)


Curl:
curl --location 'https://9h0ovfjk8h.execute-api.us-east-2.amazonaws.com/dev/clue' \
--header 'Content-Type: application/json' \
--data '{
    "body": "{ \"manuscrit\": [\"mfjel\", \"aaaa\", \"zxcvb\", \"poiuy\"] }"
}'


Nota: el curl se encuentra anexo como "Curl RQ Clue.txt"


#### Request Stats
EndPoint de la solución: [https://9h0ovfjk8h.execute-api.us-east-2.amazonaws.com/dev/stats](https://9h0ovfjk8h.execute-api.us-east-2.amazonaws.com/dev/stats)


Curl: 
curl --location 'https://9h0ovfjk8h.execute-api.us-east-2.amazonaws.com/dev/stats'

Nota: el curl se encuentra anexo como "Curl RQ stats.txt"


#### Resultados de la prueba de performance

<img width="868" alt="Evidencias" src="https://github.com/user-attachments/assets/22a5baae-71e2-4872-a837-be7d6ed62d63">



