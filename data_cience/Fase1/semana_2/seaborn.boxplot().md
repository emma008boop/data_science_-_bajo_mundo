#Cargar datos de ejemplo 
datos = sns.load_dataset("tips")

#Crear un boxplot basico Queremos ver la distribución de la cuenta total ('total_bill') según el día de la semana ('day')

sns.boxplot(x="day", y="total_bill", data=datos)

#Mostrar el grafico
plt.show()


Para definir el tamaño de la ventana del grafico (Ancho - Alto)
plt.figure(figsize=(8, 6))

Personalizar con titulos y etiquetas limpias 
plt.tittle(f"Distribucion de {columna_y} por {columna_x}", fontsize=14, fontweight="bold")
plt.
