**Bound significa limitado. IO bound es cuando el codigo esta limitado por la espera.  
  
CPU bound es cuando el codigo esta limitado por el trabajo, la cpu esta al 100% haciendo calculos.   
  
Si la tarea es IO bound conviene concurrencia porque no tiene sentido que todos los nucleos de la cpu si todos esperan a que lleguen los datos. Un nucleo que aproveche cada espera para empezar otra tarea es suficiente  
  
Si la tarea es CPU Bound, conviene paralelismo porque si la cpu esta sufriendo 100% con una tarea no se puede alternar con otra, se necesita otro nucleo trabajando.**