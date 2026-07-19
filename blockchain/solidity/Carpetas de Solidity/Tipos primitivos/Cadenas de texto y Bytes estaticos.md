El manejo de texto en la Blockchain es costoso en terminos de Gas, por lo que hay dos formas de tratarlo 

- bytes1 a bytes32: Guardan texto o datos binarios crudos de longitud fija. Son extremadamente eficientes y baratos de usar. Si necesitas guardar texto corto (como un nombre de usuario o un simbolo), usa esto en lugar de un String
- ***string: Cadena de texto de longitud dinamica (caracteres UTF-8). Son las mas caras de procesar***
![[Pasted image 20260718104326.png]]
