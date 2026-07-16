
---------------------------------------

# Configurar CORS

Configurar CORS es imprescindible para cuando queremos conectar nuestra api a un puerto. Sirve para que el navegador no bloquee la ruta externa, es una configuracion por defecto que usa nuestro navegador para protegernos de ataques externos. [[Configuracion CORS]]

--------------------------------------
# Definir Endpoints

Definir un endpoint es equivalente a decir en que ruta web nuestra api podra enviar respuestas o recibir peticiones. Es el punto de comunicacion entre nuestra web con nuestro core

[[Configuracion de Endpoints]]

---------------------------------------

## Codigo para levantar Endpoint con uvicorn

uvicorn main:app --reload
