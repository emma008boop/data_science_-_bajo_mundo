
Es una función que se usa para crear diagramas de caja o boxplots. Es una de las mejores herramientas para visualizar la distribución de un conjunto de datos, ver su simetría y detectar valores atípicos 

# ¿Que significan las partes de un Boxplot?

Un diagrama de caja divide sus datos en cuartiles (Cuatro partes iguales)

- La primera linea es la **mediana** (el percentil 50). <mark style="background: #D2B3FFA6;">Divide los datos exactamente a la mitad.</mark>
- El limite inferior de la caja: Es el primer Quartil (percentil 25). <mark style="background: #D2B3FFA6;">El 25% de los datos es menor que este valor.</mark>
- El limite superior de la caja: es el tercer Quartil (percentil 75). El 75% de los datos es menor que este valor.
- **La altura de la caja:** Se conoce como el **Rango Intercuartílico (IQR)**, y se calcula como IQR=Q3−Q1. Aquí se con<mark style="background: #D2B3FFA6;"></mark>centra el 50% central de tus datos.
- Las lineas que sobresalen<mark style="background: #FF5582A6;"></mark> **(Los bigotes)**: se extienden hasta los valores máximos y minimos dentro de un limite razonable
- **Los puntos sueltos (Outliers):** Cualquier dato que esté más allá de los bigotes se dibuja como un punto individual. Son los **valores atípicos** o extremos.

--------------------------------------------------------------------------
## ¿Como interpretar una gráfica boxplot?

En esta imagen se Muestra que el minimo es la parte de abajo, y el inicio de la caja es el Quartil 1 (Que representa el 25%) y el resto seria el 75%

![[Pasted image 20260622212837.png]]

En el centro se encuentra la mediana de los datos. Quiere decir que marca la mitad de los datos. Luego veremos que por encima se representa el Quartil 3 y encima de el el otro 25% de la población.

![[Pasted image 20260622213034.png]]

Veremos que la caja entera representara el 50% de la población, mientras que el resto de los bigotes representará el 25%

![[Pasted image 20260622213238.png]]

Los boxplot también nos puede mostrar la distribución de nuestros datos.

![[Pasted image 20260622213416.png]]

- En el primero vemos que la simetría es negativa 
- En el ultimo apreciamos que es negativa
- Y distribución simétrica donde vemos una distribución equitativa de los datos

En estos diagramas también podremos encontrar información acerca de la [[Kurtosis]].


![[Pasted image 20260622213727.png]]

Aquí veremos una distribución platicurtica donde los extremos son raros y controlados

![[Pasted image 20260622213820.png]]

Aquí vemos una distribución leptocúrtica donde muestra que los outliers son mucho mas propensos a pasar. Los datos están concentrados entorno a la medida de tendencia central analizada.

----------------------------------------------------------------------

![[Pasted image 20260622202259.png]]


Para seaborn debemos usar la libreria mathplotlib ya que es dependencia de seaborn.


![[Pasted image 20260622212432.png]]


![[Pasted image 20260622212450.png]]

