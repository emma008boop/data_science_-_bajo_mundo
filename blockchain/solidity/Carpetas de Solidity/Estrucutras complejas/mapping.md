Es equivalente a HashMap<K, V> de Rust. Pero con una diferencia en el diseño. En Solidity, los mapping no guardan  las llaves ni se pueden iterar (No hay bucles for sobre ellos)

Si buscas una llave que no existe, el EVM no te da un error ni un None; Solo te devuelve el valor por defecto de el tipo de dato

![[Pasted image 20260718105856.png]]
