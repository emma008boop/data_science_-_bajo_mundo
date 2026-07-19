Como desarrollador en el ecosistema blockchain, el trabajo no consiste en mantener la red ni conectar nodos (eso lo hacen los validadores e ingenieros de infraestructura). El rol principal se divide en dos grandes areas: 
- Desarrollo core (crear o mejorar la blockchain )
- Desarrollo de aplicaciones (crear lo que corre encima de ella)

# Escribir las reglas de negocio (Smart contracts)

Esta es la tarea mas comun usando Solidity o Rust, se diseñan los programas que controlan el dinero, los activos o los permisos de una app descentralizada (dApp)

# Blindar el codigo (Seguridad y optimizacion de Gas)

A diferencia del desarrollo web tradicional, donde un error se soluciona con un parche rapido en el servidor, en Web3 un error de codigo significa que los usuarios pierden millones de dolares de forma irreversible

- Como desarrollador, se pasa el 30% del tiempo escribiendo código y el 70% restante escribiendo pruebas (_tests_) ultra estrictas, simulando ataques cibernéticos y optimizando el código para que consuma el menor Gas posible (haciendo que las transacciones sean baratas para los usuarios).

# Conectar el blockchain con el mundo real

La blockchain por si sola esta aislada. Los usuarios no quieren interactuar con la terminal de Linux negra usando comandos complejos; quieren usar una aplicacion en su telefono o navegador 

# Crear infraestructura de la red

Aqui es donde entra rust con fuerza. Si se trabaja para una blockchain como solana, Polkadot o una capa 2 (layer 2) de Ethereum, no escribes contratos inteligentes normales; escribes el software que los nodos ejecutan

- Se diseña cómo la red procesa las transacciones en paralelo para que sea más rápida, cómo se comunican los nodos entre sí (protocolos P2P) o cómo se encriptan los datos en la base de datos de los bloques.