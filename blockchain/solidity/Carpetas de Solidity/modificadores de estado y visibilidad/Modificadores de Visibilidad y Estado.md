En las funciones, la visibilidad define quien puede llamarlas y como leen/escribern informacion

## Visibilidad de funciones

- public: Accesible desde fuera y dentro del contrato
- private: Solo accesible dentro del contrato actual
- internal: Accesible dentro del contrato y contratos que hereden de el 
- external: Solo se puede llamar desde afuera del contrato.

Palabras clebe de lectura de estados:

- view: Promete que la funcion solo lle la blockchain, no modifica nada (No cuesta gas si se llama externamente)
- pure: Promete que ni lee ni escribe en la en la blockchain (solo trabaja con parametros pesados)

![[Pasted image 20260725181240.png]]
