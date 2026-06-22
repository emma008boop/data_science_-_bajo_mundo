## 📐 FASE 2 (Continuación): Análisis Avanzado e Infraestructura Eficiente (Mes 6 al 10)
*El objetivo aquí es dominar cómo la computadora gestiona la memoria, optimizar tus algoritmos y migrar los procesos críticos al motor ultra veloz de Rust.*

---

### 🧠 MES 6: Estructuras de Datos y Eficiencia Algorítmica (Big O)
*El objetivo de este mes es que entiendas cómo la computadora lee la memoria y cómo medir la velocidad de tu código escrito tanto en Python como en Rust.*

- [ ] **Semana 21: Notación Big O y Complejidad Temporal/Espacial**
    - [ ] **Qué estudiar:** Complejidad del tiempo y notación asintótica ($O(1)$, $O(\log n)$, $O(n)$, $O(n^2)$). Cómo calcular cuántas operaciones hace tu script cuando la base de datos de camiones crece a millones de filas.
    - [ ] **Enfoque Práctico:** Medir los tiempos de ejecución de bucles aninados en Python y entender por qué se "congela" la pantalla con muchos datos.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Evaluar tus scripts de seguros del Mes 5 para detectar "cuellos de botella" (partes del código que ralentizan todo el proceso).

- [ ] **Semana 22: Estructuras de Datos Eficientes (Arrays vs. Linked Lists en memoria)**
    - [ ] **Qué estudiar:** Cómo se guardan los datos en la memoria RAM físicamente. Punteros, direccionamiento y asignación de memoria.
    - [ ] **En Rust:** Introducción a la sintaxis básica de Rust, tipos de datos primitivos y el manejo de vectores (`Vec<T>`).
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Almacenar los registros de camiones en estructuras de datos de Rust optimizadas para ocupar la menor cantidad de memoria RAM posible.

- [ ] **Semana 23: Tablas Hash (Hash Maps) y Búsqueda Eficiente**
    - [ ] **Qué estudiar:** Algoritmos de Hash y colisiones. Búsqueda en tiempo constante $O(1)$.
    - [ ] **En Rust:** Uso de `HashMap` nativo en Rust.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Crear un índice en memoria donde busques instantáneamente el historial de un camión usando su número de placa (VIN) como "llave", sin tener que recorrer toda la base de datos fila por fila.
        - **Trading:** Buscar al instante el precio de un ticker de criptomoneda en un diccionario de alta velocidad.

- [ ] **Semana 24: Algoritmos de Ordenamiento Eficiente (Merge Sort / Quick Sort)**
    - [ ] **Qué estudiar:** Principio de "Divide y Vencerás". Comparación de eficiencia entre ordenamientos básicos ($O(n^2)$) y avanzados ($O(n \log n)$).
    - [ ] **En Rust:** Implementar algoritmos de ordenamiento aplicados a estructuras personalizadas (`Structs`).
    - [ ] **Aplicación Práctica:**
        - **Seguros/Trading:** Ordenar las pólizas de seguros por fecha de vencimiento o las órdenes de trading por precio en el menor tiempo informático posible.

---

### 🦀 MES 7: Rust para Procesamiento de Datos Masivos (Data Pipelines de Alta Velocidad)
*Aquí dejas descansar a Python por un momento y migras la limpieza matemática de datos al motor ultra veloz de Rust.*

- [ ] **Semana 25: El Sistema de Tipos de Rust y "Ownership" (Propiedad)**
    - [ ] **Qué estudiar:** Las reglas de oro de Rust: *Ownership*, *Borrowing* (Préstamos) y *References*. Por qué Rust no necesita un recolector de basura (a diferencia de Python) y cómo esto evita retrasos (*gc-pauses*) en sistemas en tiempo real.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Escribir tus primeras funciones en Rust que manipulen cadenas de texto y números de pólizas de seguros de forma segura, garantizando cero fugas de memoria (*memory leaks*).

- [ ] **Semana 26: Procesamiento de Archivos Gigantes (I/O Eficiente)**
    - [ ] **Qué estudiar:** Lectura de buffers, manejo de archivos planos (CSVs, JSONs de gigabytes de tamaño) de manera secuencial y eficiente.
    - [ ] **En Rust:** Uso de la librería estándar `std::fs::File` y el crate `csv`.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Procesar un CSV de 5 Gigabytes con millones de registros de telemetría de camiones (rutas GPS). Crear un script en Rust que lo lee y limpia en segundos sin desbordar la memoria RAM (evitando el error de *Out of Memory* de Python).

- [ ] **Semana 27: El Crate Polars en Rust (El reemplazo ultra-rápido de Pandas)**
    - [ ] **Qué estudiar:** Expresiones perezosas (*Lazy Evaluation*) y optimización de consultas en memoria.
    - [ ] **En Rust:** Uso del crate `Polars` (escrito nativamente en Rust).
    - [ ] **Aplicación Práctica:**
        - **Seguros/Trading:** Replicar los análisis estadísticos descriptivos del Mes 1 (promedios, desviaciones estándar de primas de camiones) pero ejecutándose a una velocidad hasta 100 veces mayor que en Python.

- [ ] **Semana 28: Multihilo y Paralelismo Básico (Concurrencia Segura)**
    - [ ] **Qué estudiar:** Hilos de procesamiento (`Threads`). Cómo usar todos los núcleos del procesador de tu computadora al mismo tiempo. Las garantías de seguridad de Rust frente a condiciones de carrera (*Race Conditions*).
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Dividir la base de datos de seguros en 4 partes y procesar cada parte simultáneamente en un núcleo de tu CPU diferente, reduciendo el tiempo de cálculo a la cuarta parte.

---

### 🤖 MES 8: Algoritmia Avanzada para Decisiones en Tiempo Real (Árboles y Grafos)
*Los datos del mundo real no siempre vienen en tablas limpias; a veces vienen en redes interconectadas. Este mes dominas esas estructuras.*

- [ ] **Semana 29: Árboles Binarios de Búsqueda y Árboles AVL**
    - [ ] **Qué estudiar:** Estructuras jerárquicas balanceadas. Búsqueda y ordenamiento en tiempo logarítmico $O(\log n)$.
    - [ ] **Aplicación Práctica:**
        - **Trading:** Entender cómo los exchanges de criptomonedas o la bolsa de valores organizan el *Order Book* (Libro de Órdenes de compra y venta) utilizando estructuras de árbol para emparejar compradores y vendedores al instante.

- [ ] **Semana 30: Teoría de Grafos y Algoritmos de Ruta Corta**
    - [ ] **Qué estudiar:** Nodos y Aristas. Representación de redes mediante matrices de adyacencia. Algoritmo de Dijkstra o $A^*$.
    - [ ] **En Rust:** Implementación de un grafo básico.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Analizar las rutas de los camiones asegurados. Calcular cuál es la ruta más eficiente y segura, correlacionándola con los datos de accidentes del Mes 2 para sugerir cambios de ruta a la empresa transportadora.

- [ ] **Semana 31: Programación Dinámica**
    - [ ] **Qué estudiar:** Optimización mediante la memorización de subproblemas ya resueltos. Pasar de algoritmos exponenciales $O(2^n)$ a polinomiales $O(n)$.
    - [ ] **Aplicación Práctica:**
        - **Trading:** Optimizar los algoritmos de cálculo de indicadores técnicos (como medias móviles exponenciales) para no re-calcular todo el historial desde cero cada vez que entra un nuevo precio al mercado por milisegundo.

- [ ] **Semana 32: Colas de Prioridad (Priority Queues y Heaps)**
    - [ ] **Qué estudiar:** Estructuras que priorizan ciertos elementos sobre otros automáticamente en tiempo $O(\log n)$.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Crear un sistema automático que ordene los reclamos de los camiones que van entrando a la base de datos, dándole prioridad inmediata a los accidentes graves sobre los reclamos menores de vidrios rotos.

---

### 🔌 MES 9: Conectividad Eficiente (APIs, WebSockets y Redes de Alta Velocidad)
*Tus algoritmos son rápidos en memoria, ahora aprenderás a recibir y enviar datos del mundo exterior a la velocidad de la luz.*

- [ ] **Semana 33: Arquitectura de Redes para Software Cuantitativo**
    - [ ] **Qué estudiar:** Diferencia crítica entre protocolos TCP (seguro pero más lento) y UDP (ultra-rápido pero sin garantías de entrega). ¿Qué es la latencia de red?
    - [ ] **Aplicación Práctica:**
        - **Infraestructura:** Diseñar la arquitectura de comunicación de datos de tu infraestructura para balancear consistencia y velocidad.

- [ ] **Semana 34: WebSockets para Streaming de Datos en Tiempo Real**
    - [ ] **Qué estudiar:** Mantener conexiones de red persistentes bidireccionales en lugar de hacer peticiones HTTP repetitivas (*Polling*).
    - [ ] **En Rust:** Implementación de un cliente WebSocket con crates como `tokio` y `tungstenite`.
    - [ ] **Aplicación Práctica:**
        - **Trading:** Conectarte al WebSocket en vivo de un exchange de criptomonedas (como Binance) o un proveedor de datos financieros para recibir el precio de Bitcoin segundo a segundo directamente en tu terminal de Rust.

- [ ] **Semana 35: Concurrencia Asíncrona (Async/Await) en Rust**
    - [ ] **Qué estudiar:** El motor asíncrono de Rust (`Tokio`). Cómo procesar miles de conexiones de red entrantes sin bloquear el hilo principal de ejecución.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Crear un servidor microservicio de alta eficiencia que escuche las actualizaciones que envían los dispositivos GPS de los camiones asegurados en tiempo real.

- [ ] **Semana 36: Serialización y Deserialización Eficiente (Serde)**
    - [ ] **Qué estudiar:** Cómo transformar texto plano (JSON) a bytes estructurados en memoria y viceversa con el mínimo impacto en la CPU.
    - [ ] **En Rust:** Dominar el crate `serde`.
    - [ ] **Aplicación Práctica:**
        - **Trading/Seguros:** Traducir los datos binarios o cadenas JSON que vienen de la API de seguros o del feed de trading a variables tipadas de Rust en microsegundos.

---

### 🤝 MES 10: Integración Híbrida (El Sistema de Producción)
*En este mes unes el cerebro analítico de Python con los músculos de alta velocidad de Rust en un solo sistema unificado.*

- [ ] **Semana 37: Creación de Bindings (Conectar Rust con Python)**
    - [ ] **Qué estudiar:** El crate `PyO3`. Cómo escribir funciones críticas y pesadas en Rust y llamarlas directamente desde un script de Python como si fuera una librería común nativa.
    - [ ] **Aplicación Práctica:**
        - **Herramientas:** Tomar el algoritmo de ordenamiento y filtrado masivo que hiciste en Rust (Mes 7) y empaquetarlo para poder usarlo dentro de tus cuadernos de *Jupyter Notebook* de Python.

- [ ] **Semana 38: El Pipeline Híbrido Aplicado a Seguros**
    - [ ] **Enfoque Práctico:**
        1. **Paso 1 (Rust):** Extrae millones de datos de la base de datos de seguros de camiones y procesa la limpieza a nivel de bytes en milisegundos.
        2. **Paso 2 (Python):** Recibe la matriz limpia generada por Rust y entrena el modelo de Machine Learning (Mes 5) de forma veloz.
    - [ ] **Aplicación Práctica:** Crear el pipeline definitivo de analítica en tu trabajo que junta lo mejor de ambos lenguajes.

- [ ] **Semana 39: El Pipeline Híbrido Aplicado a Trading (Tu primer Bot HFT simulado)**
    - [ ] **Enfoque Práctico:**
        1. **Paso 1 (Rust):** Escucha el feed del mercado por WebSockets a alta velocidad, calcula indicadores en microsegundos y filtra anomalías.
        2. **Paso 2 (Python):** Evalúa mediante estadística e inferencia si hay oportunidad de negocio.
    - [ ] **Aplicación Práctica:** Tener un simulador de trading algorítmico corriendo localmente con datos reales de mercado.

- [ ] **Semana 40: Pruebas de Estrés (Benchmarking) y Optimización de Código**
    - [ ] **Qué estudiar:** Herramientas de perfilado de código (`Criterion` en Rust, `cProfile` en Python). Encontrar líneas específicas de código que consumen demasiada CPU.
    - [ ] **Aplicación Práctica:**
        - **Optimización:** Optimizar tu sistema integrado hasta asegurar que el tiempo de respuesta total esté por debajo de los estándares profesionales internacionales.