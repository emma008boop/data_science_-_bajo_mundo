
## ¿Para que sirve?

Sirve para visualizar la distribucion de una variable continua o discreta. te permite ver de un vistazo donde se agrupan los datos, que tan dispersos están si la distribucion es simetrica o sesgada y si hay multiples picos (bimodalidad).

### Los calculculos detrás 

El histograma no gráfica los datos crudos uno a uno, primero hace una transformacion estadistica llamada <mark style="background: #FFF3A3A6;">binning </mark> [[BIN (Los intervalos)]] (agrupación de intervalos) 

- 1. Calculo del rango total: Se busca el valor máximo (*Xmax*​) y el minimo (*Xmin*​) de tus datos
- 2. Definición de los intervalos (BINS): El rango completo se divide en k subintervalos de igual ancho. El ancho de cada intervalo (*W*) se calcula como:
- ![[Pasted image 20260621212843.png]]

Nota: Si no defines [[BIN (Los intervalos)]], Seaborn usa reglas automáticas como la de **Freedman-Diaconis** [[Freedman-Diaconis]], que calcula el ancho óptimo basado en el rango intercuartílico (IQR) y el número total de datos (n):


![[Pasted image 20260621212950.png]]

- 3. Conteo de frecuencias: Cuenta cuantos puntos de datos caen dentro de cada intervalo. la altura de cada barra representada este conteo (O la densidad/probabilidad, si cambias el parámetro stat)

Para seaborn debemos usar la libreria mathplotlib ya que es dependencia de seaborn.

![[Pasted image 20260622211758.png|631]]

![[Pasted image 20260622211813.png]]

