Este tipo es nativo de solidity y es crucial. Representa una direccion de una billetera o de otro contrato inteligente (una llave publica de 20 bytes). En rust tendrias que definirlo como un array de bytes o struct personalizado, pero aqui es un tipo primitivo.

# Tiene dos variantes

- address: Una direccion comun. Solo puede leer info
- address payable. Una direccion especial que tiene permitivo recibir Ether (dinearo nativo de la red)

![[Pasted image 20260718103930.png]]

