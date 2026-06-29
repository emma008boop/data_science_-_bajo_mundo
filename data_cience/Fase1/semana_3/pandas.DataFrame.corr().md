Este metodo calcula el coheficiente de correlacion entre todas las columnas numericas de un Dframe. Por defecto usa la correlacion pearson [[Coheficiente de correlacion de Pearson]]

`import pandas as pd # Creamos un dataset de juguete 
`datos = { 

	`'Precio': [20000, 25000, 15000, 30000],
	`'Kilometraje': [50000, 30000, 80000, 10000], 
	`'Año': [2018, 2020, 2015, 2022] 
	
	}
	
	` df = pd.DataFrame(datos)
	 
	 # Calculamos la correlación 
	 matriz_corr = df.corr() print(matriz_corr)

