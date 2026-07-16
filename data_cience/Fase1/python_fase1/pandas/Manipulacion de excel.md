## Pandas

lee tu archivo excel usando el motor openpyxl y lo convierte en un DataFrame (DF). Un DF es como una tabla de excel virtual que vive en la memoria de python, con sus filas y columnas listas para ser manipuladas

df = pd.read_excel(EXCEL_PATH, engine='openpyxl')

Podemos traer esos datos de excel a [[Sqlite3]]

conn = sqlite3.connect(DB_PATH)

Con esta funcion podremos abrir el archivo que contiene la bd y si no existe la db aun, la crea con los datos. <mark style="background: #BBFABBA6;">La variable conn guarda esa conexion abierta</mark>

Finalmente, podremos volcar los datos a SQL y cerrar la conexion 

df.to_sql('accounts', conn, if_exists='replace', index=False)
conn.close()

