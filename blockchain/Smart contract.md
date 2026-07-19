Un ***contrato inteligente***, es un programa que se ejecuta de forma automatica cuando se cumplen unas condiciones especificas.

1. Pones el dinero (condicion)
2. Seleccionas el producto (Instruccion)
3. La maquina te entrega el refresco de forma automatica

No hay cajero humano que se encargue de la transaccion ni decidiendo si te da el refresco o no. El codigo de la maquina garantiza el trato. En la blockchain funciona igual, pero manejando activos digitales, registros o firmas de forma transparente, inmutable

# Concepto en Solidity

Solidity  fue diseñado exclusivamente para la VM de ethereum. Su enfoque es muy similar a POO

- En solidity, un contrato es como una pequeña caja fuerte que contiene tanto reglas (el codigo) como los datos (el estado).
- Es intuitivo pero pesado. Es facil de programar, pero hace que la red trabaje de forma secuencial (Proceso detras de otro), lo que puede volver las trransacciones lentas y caras (carga fees) cuando hay congestion de red 
- UN contrato en terminos de solidity, es una coleccion de codigo (Funciones) y datos (el estado) que residen en una direccione especifica en el Blockchain Ethereum.

# Concepto en Rust

Rust no se creo para blockchain, pero es un lenguaje que blockchain modernas como solana, polkadot o near adaptaron para sus contratos