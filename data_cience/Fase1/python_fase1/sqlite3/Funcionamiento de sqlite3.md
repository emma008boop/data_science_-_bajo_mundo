Orden Logico

<mark style="background: #FFB86CA6;">Conectar > Crear cursor > Ejecutar SQL > Guardar y cerrar</mark>


- Conectar: crea un archivo si no existe y abre la conexion 

	``conexion = sqlite3.connect("mi_bd.db")

- El cursor: Es el "Mensajero" que ejecuta las ordenes SQL
		``cursor.execute( consulta en qsl o )

- insertar datos
	cursor.execute("INSERT INTO usuarios (nombre, edad) VALUES ('Emma', 25)")

- GUARDAR Y CERRAR (Súper importante) conexion.commit() # Guarda los cambios en el archivo 
	- conexion.close() 
	- Cierra la conexión

## Datos

- Si en lugar de un nombre de archivo usas `sqlite3.connect(':memory:')`, la base de datos se creará temporalmente en la memoria RAM
- cursor: Es el objeto que se encarga de interactuar con los registros.
-  Pasas un signo de pregunta y las variables dentro de una tupla al final ``cursor.execute("SELECT * FROM usuarios WHERE nombre = ?", (nombre_usuario,))
