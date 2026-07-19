Es el entorno donde escribes, compilas y pruebas el codigo. Hoy en dia existen dos arquitecturas dominantes en la industria.

## Arquitectura basada en Foundry

Es la que instalamos con ***forge init***. Esta escrita en Rust y es extremadamente rapida.

- Caracteristicas
	- Test y los scipts se escriben directamente en solidity. 
	- Ejecuta los test en milisegundos gracias a su entorno de Rust
	- Incluye herramientas avanzadas nativas como Fuzzung (Pasar miles de datos aleatorios a tus funciones para buscar errores ocultos)

## Estructura de carpetas

- src/: Contratos inteligentes principales
- test/: Pruebas en solidity
- script/: Scripts para desplegar a la red
- lib/: Dependencias y librerias externas


------------------------------------------

# Arquitectura basada en Hardhat

Es la arquitectura basica que ha dominado el mercado. Esta basada en Node.js

- Caracteristicas
	- Los contratos se escriben en solidity, pero las pruebas y los scripts de despliegue se escriben en js o ts
	- Tiene un ecosistema gigante de plugins antiguos 
	- Es notablemente mas lenta que Foundry al compilar y correr pruebas


-----------------------------------------
# Cual usar?

-  Usar Foundry por defecto para cualquier proyecto nuevo. Evitara tener que lidiar con configuraciones complejas de Node.js y acelerara el flujo de trabajo
- Usar Hardhat solo si entras a trabajar en un proyecto antiguo que ya tenga su infraestructura creada en JS/TS

