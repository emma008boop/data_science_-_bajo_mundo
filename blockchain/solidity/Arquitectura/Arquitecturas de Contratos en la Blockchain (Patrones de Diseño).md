Cuando subes el codigo a la blockchain, este es inmutable. Si cometes un error o quieres añadir una funcion al cryptobanco, no puede ser simplemente reemplazar el archivo. Por eso existen diferentes arquitecturas de diseño para el sistema de contratos

# Patron 1: #ContratoMonolitico

Todo el sistema vive dentro de un unico contrato inteligente. Las variables de saldo, las funciones de deposito, retiro y logica de administracion estan en el mismo archivo 

- Caracteristicas
	- Es muy facil de programar y entender; consume menos Gas al desplegarse porque es un solo bloque
	- Usarlo para proyectos pequeños, MVP herramientas de un solo uso o contratos educativo
	- La desventaja es que si el proyecto crece, el archivo se vuelve inmanejable y hay un limite fisico de tamaño para los contratos en Ethereum

# Patron 2 #ArquitecturaDeFabrica

Un contrato principal se encarga de crear y desplegar automaticamente otros contratos secundarios identicos 

- Caracteristicas
	- 