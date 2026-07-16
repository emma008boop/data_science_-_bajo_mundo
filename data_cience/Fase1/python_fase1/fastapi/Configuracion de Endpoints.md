@app.get() -> Sirve para establecer el tipo de comunicacion o permisos tendra nuestra web con nuestra api

@app.get("<mark style="background: #ADCCFFA6;">/api/v1/accounts</mark>") -> Con esto definiremos cual es la ruta 

---------------------------------------
@app.get("api/v1/accounts)
def get_accounts(<mark style="background: #D2B3FFA6;">search: str = Query(None)</mark>):


Le dice FastApi que la funcion puede recibir un parametro opcional en la URL (ej. `/api/v1/accounts?search=Nestle`).

Si no se envia, search vale None 