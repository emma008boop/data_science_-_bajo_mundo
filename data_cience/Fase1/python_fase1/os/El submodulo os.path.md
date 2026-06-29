Los os no se ponen de acuerdo porque, windows usa \ para las rutas, mientras que linux y mac usan /  .El submodulo de os.path, resuelve este problema.


os.path.join(carpeta, archivo) -> une partes de una ruta de forma inteligente

os.path.exists(ruta) -> Devuelve True o False si el archivo o carpeta existe 

os.path.isfile(ruta) / os.path.isdir(ruta) -> Verifica si la ruta apunta a un archivo o una carpeta

![[Pasted image 20260629132349.png]]



Aveces cuando estamos programando, debemos tener en cuenta que el codigo no siempre se va a ejecutar en el mismo entorno. Puede que muevas la carpeta o que lo estes ejecutando desde otro pc.

Por eso debemos de pensar que no siempre las cosas seran estaticas. Por eso debemos pensar en eso desde el momento de escribir el codigo.

Una solucion a este problema seria usar una direccion de base dentro de nuestro mismo proyecto para que el sistema pueda ejecutar el scrip sin importar donde esta. Lo que sabemos al momento de escribir el codigo es la estructura de nuestro proyecto, por eso tomaremos como base la url de nuestro proyecto como ruta base de trabajo.

![[Pasted image 20260629133227.png]]

Y de ahi podremos empezar a jugar con las direcciones y ubicar el archivo que queramos dentro de nuestro proyecto

![[Pasted image 20260629133444.png]]
