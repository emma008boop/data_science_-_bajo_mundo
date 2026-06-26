Sirve para controlar el comportamiento de tu archivo dependiendo de **CÓMO** lo estés ejecutando.

## Escenario A: Tú ejecutas el archivo directamente

Si abres tu terminal en Linux Mint y escribes:
 ``python3 modulo1_eda.py



Python dice: _"Este es el archivo principal que el usuario quiere correr"_. Por lo tanto, le asigna a la variable oculta el valor de `"__main__"`. Como `__name__` es igual a `"__main__"`, el `if` se cumple y **se ejecuta la función `inicializar_base_de_datos()`**.
