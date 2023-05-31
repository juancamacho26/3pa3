# Documentación del Código para menu

## Funciones

### `get_ascii(char)`

Esta función toma un carácter como entrada y devuelve su valor ASCII correspondiente. Se utiliza para generar la representación ASCII de un solo carácter.

### `get_binary(char)`

Esta función toma un carácter como entrada y devuelve su representación binaria. Utiliza el valor ASCII del carácter y lo convierte en una cadena binaria. Se utiliza para generar la representación binaria de un solo carácter.

### `get_results(word)`

Esta función toma una palabra como entrada y devuelve una lista de tuplas que contienen el carácter, su valor ASCII y su representación binaria. Utiliza las funciones `get_ascii()` y `get_binary()` para obtener los resultados individuales de cada carácter en la palabra. Se utiliza para generar la representación ASCII y binaria de una palabra.

### `menu()`

Esta función es el punto de entrada principal del programa. Muestra un menú interactivo al usuario, solicitando una opción (1 o 2) para seleccionar una operación. Luego, solicita la entrada del usuario (carácter o palabra) según la opción seleccionada y muestra los resultados correspondientes utilizando las funciones anteriores. Además, ofrece la opción de salir del programa.

### `sys.exit()`

Esta función se utiliza para finalizar la ejecución del programa de manera abrupta cuando el usuario selecciona la opción de salida.

## Punto de Entrada Principal

```python
if __name__ == "__main__":
    menu()
