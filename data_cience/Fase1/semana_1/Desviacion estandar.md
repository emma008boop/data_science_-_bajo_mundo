La **Desviación Estándar** toma esa misma idea de "distancia", pero le hace un pequeño truco matemático: **eleva las distancias al cuadrado** antes de promediarlas, y al final saca una **raíz cuadrada**.

Imagina que tienes 3 datos: los rendimientos de una accion fueron de -10%, 0% y +10%. El promedio es 0%.

Si calculas la distancia de cada dato al promedio directamente:
- El primer dato esta a -10 del promedio 
- El segundo esta a 0%
- el tercero esta a 10%
Si simplemente sumas esas distancias para promediarlas, las distancias negativas y las positivas se cancelan:

![[Pasted image 20260622215135.png]]

¡Nos daría que la distancia promedio es cero y que no hay volatilidad! Para evitar que los números negativos destruyan a los positivos, la desviación estándar hace lo siguiente:

- **Calcula la distancia de cada dato al promedio** (igual que tú dijiste).
    
- **Eleva cada distancia al cuadrado:** Así, −10 al cuadrado se convierte en +100 (adiós al signo negativo) y 10 al cuadrado se convierte en +100.
    
- **Suma y promedia esos cuadrados:** A esto se le llama _Varianza_.
    
- **Saca la raíz cuadrada del resultado:** Como elevamos todo al cuadrado al principio (lo que alteró nuestra escala original), sacamos la raíz cuadrada para regresar el número a su tamaño y unidad original (en este caso, volver a porcentaje %).

## En resumen:

La desviación estándar es la distancia entre cada dato de una población y su promedio. Pero elevada al cuadrado para que los números negativos no afecten el resultado. 

La ventaja que tiene la Desviacion estandar es que castiga mas fuerte a los valores extremos, es decir, cuando elevas un número al cuadrado, la distancia no crece de forma lineal (como 1,2,3...), sino de forma exponencial (como 1,4,9...). Entre más grande sea la distancia original, el resultado al cuadrado se vuelve monstruosamente más grande.

**elevas al cuadrado para que los negativos no destruyan el resultado**, y luego calculas el promedio de esos cuadrados.