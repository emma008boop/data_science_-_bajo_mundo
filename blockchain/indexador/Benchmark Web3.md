
# 1. Problema

En el desarrollo web2 tradicional, las bases de datos tradicionales permiten hacer consultas complejas al instante. En Web3, la blockchain es un registro contable, no una base de datos diseñada para consultas complejas.

  

Cuando un smart contract ejecuta una acción, emite un evento. Este evento queda grabado de forma permanente en los bloques de red


## Preguntas que necesita responder una aplicación descentralizada.

- ¿Cual es el historial de compras de este usuario en los ultimos 6 meses?

- ¿Cuales son los 10 pares de tokens con mayor volumen hoy?

Preguntarle esto a un nodo de EPC en el entorno de ethereum requiere leer bloque por bloque, lo cual es costoso en Gas y muy lento; lo cual genera un bloqueo de usuario.

## El reto


Los contratos inteligentes procesan dinero real en milisegundos; cuando ocurre un ataque o un bug critico en la blockchain:  

- Los atacantes usan Flash Loans para ejecutar exploits en una sola transaccion

- No hay administradores que puedan revertir una transaccion ya confirmada

- Deteccion tardia equivale a perdida total de fondos

Se necesita un sistema automatizado que escuche la red constantemente para detectar anomalias o transacciones sospechosas en el [[Mempool]] (Antes de que se confirmen) o inmediatamente en el bloque recien minado.

