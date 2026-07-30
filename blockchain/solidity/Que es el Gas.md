Es la unidad de medida que se usa en solidity y Ethereum para medir el esfuerzo computacional necesario para ejecutar operadpres en la EVM

# Para que sirve?

## Prevenir ataques de denegacion de servicio

En lenguajes de programacion tradicionales, si un programador comete un error y crea un bucle infinito **while(true)**, el programa se congela.

En la blockchain, si no existiera el GAS, alguien podria enviar un contrato con un bucle infinito y detener toda la red Ethereum para siempre. Gracias al Gas, si un programa entra en un bucle infinito, se ejecutara solo hasta que el usuario se quede sin GAS