
Cuando compilas usando forge build, el compilador toma el codigo legible para humanos y la traduce en dos cosas que van dentro de una carpeta llamada out/

- Bytecode: Es una cadena gigante de numeros hexadecimales (codigo maquina) que entiende la EVM
- El ABI (Application Binary Interface): Es un archivo JSON que funciona como el "Manual de instrucciones" de tu contrato. Le dice a las aplicaciones de afuera (como pagina web o un script de rust) que funciones tiene el contrato y que parametros necesitas para activarse

## La memoria de la EVM ¿Donde se guardan los datos?

Mientras Rust gestiona la memoria entre el Stack y el Heap. En la EVM, la memoria fisica no existe; esta emulada en la blockchain y se divide estrictamente en 3 ubicaciones de almacenamiento 

1. storage: (El disco duro permanente)
	- Es el estado global del contrato. Todo lo que declares suelto dentro del contrato (fuera de las funciones) vive aqui
	- Se guarda para siempre en los miles de nodos de la blockchain
	- Es extremadamente caro. Modificar o guardar datos en el storage es la operacion que mas dinero cuesta en solidity. El compilador organiza el storage en slots de 32 bytes de forma secuencial
2. memory (La memoria RAM temporal)
	- Una memoria bolatil que se crea cuando una funcion empieza a ejecutarse y se destruye por completo cuando la funcion termina
	- se usa para procesar datos intermedios dentro de una funcion
	- Muy barato a comparacion de storage
3. calldata (El buzon de entrada)
- Es un area de memoria especial, de solo lectura, donde se guardan los argumentos que un usuario envia cuando llama a una funcion desde fuera de la blockchain
- No puedes modificar los datos que estan el calldata
- es el almacenamiento mas barato de todos. El compilador te obligara a usarlo para arrays o strings si la funcion recibe datos externos y no necesita modificarlos