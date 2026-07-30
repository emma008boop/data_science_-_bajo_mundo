Es equivalente a HashMap<K, V> de Rust. Pero con una diferencia en el diseño. En Solidity, los mapping no guardan  las llaves ni se pueden iterar (No hay bucles for sobre ellos)

Si buscas una llave que no existe, el EVM no te da un error ni un None; Solo te devuelve el valor por defecto de el tipo de dato

![[Pasted image 20260718105856.png]]

#msgsender Es una variable global que contiene la direccion de Ethereum de quien esta ejecutando la funcion en este instante

## Como se asigna y de donde sale?

Cuando un usuario presiona un boton en Remix para ejecutar una funcion, la transaccion viene firmada por su billetera. Solidity detecta automaticamente esa billetera y la pone a tu disposicion en msg.sender

### Los 3 usos principales de msg.sender

- Puedes guardar informacion vinculada a un usuario especifico: Puedes usar msg.sender como la clave dentro de un mapping para asociar datos a la persona que ejecuta la funcion 

![[Pasted image 20260725224605.png]]

- Crear o modificar estructuras asociadas al usuario

![[Pasted image 20260725224641.png]]

- Cuando un usuario quiere consultar su propia informacion sin necesidad de pasar su direccion como parametro

![[Pasted image 20260725224852.png]]