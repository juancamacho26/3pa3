# INTEGRANTES GRUPO #6
- Alfonso Vega
- Julian Martinez
- Juan Camacho


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
```
    
# Documentación del Código para operaciones

## Funciones

### `get_ascii(character)`

Esta función toma un carácter como entrada y devuelve su valor ASCII correspondiente. Utiliza la función `ord()` para obtener el valor ASCII del carácter.

### `get_binary(character)`

Esta función toma un carácter como entrada y devuelve su representación binaria. Utiliza la función `ord()` para obtener el valor ASCII del carácter y luego aplica la función `bin()` para obtener la representación binaria. La representación binaria se devuelve como una cadena, eliminando los dos primeros caracteres que corresponden al prefijo "0b".

### `get_results(word)`

Esta función toma una palabra como entrada y devuelve una lista de tuplas que contienen cada carácter de la palabra, su valor ASCII y su representación binaria. Utiliza un bucle `for` para iterar sobre cada carácter en la palabra y utiliza las funciones `get_ascii()` y `get_binary()` para obtener los resultados individuales de cada carácter. Los resultados se almacenan en una lista de tuplas.

## Punto de Entrada Principal

No se proporciona un punto de entrada principal en este código. Las funciones `get_ascii()`, `get_binary()` y `get_results()` pueden ser utilizadas por otros módulos o scripts según sea necesario.

# Paso a paso para trabajar con el repositorio

1. **Clonar el repositorio**: El primer paso es clonar el repositorio a tu máquina local utilizando el comando `git clone`. Este comando crea una copia local del repositorio en tu directorio de trabajo actual.
   ```
   git clone <URL_del_repositorio>
    ```
2. **Cambiar al directorio del repositorio**: Navega al directorio del repositorio clonado utilizando el comando cd. Este comando te permite moverte al directorio específico donde se encuentra el repositorio clonado.
```
   cd <directorio_del_repositorio>
 ```
3. **Verificar el estado del repositorio**: Puedes utilizar el comando git status para ver el estado actual del repositorio local. Te muestra información sobre los archivos modificados, los archivos sin rastrear y los cambios pendientes de confirmar.
```
  git status
 ```
 4. **Crear una rama de trabajo**: Es una buena práctica crear una rama de trabajo separada para realizar tus cambios sin afectar la rama principal (por lo general, llamada main o master). Utiliza el comando git branch para crear una nueva rama y git checkout para cambiar a esa rama.Crear una rama de trabajo: Es una buena práctica crear una rama de trabajo separada para realizar tus cambios sin afectar la rama principal (por lo general, llamada main o master). Utiliza el comando git branch para crear una nueva rama y git checkout para cambiar a esa rama
```
git branch <nombre_de_la_rama>
git checkout <nombre_de_la_rama>
 ```
 5. **Realizar modificaciones**: Realiza las modificaciones necesarias en los archivos del repositorio utilizando tu editor de código preferido.

6. **Agregar los cambios**: Utiliza el comando git add para agregar los cambios realizados en los archivos al área de preparación, lo que indica que deseas incluir esos cambios en tu próxima confirmación.
```
git add <archivos_modificados>
 ```
 7. **Realizar una confirmación**: Realiza una confirmación (commit) de los cambios utilizando el comando git commit. Asegúrate de incluir un mensaje descriptivo que explique los cambios realizados.
```
git commit -m "Mensaje descriptivo de los cambios"
 ```
 8. 
 **Subir los cambios al repositorio remoto**: Utiliza el comando git push para subir tus cambios a la rama correspondiente en el repositorio remoto.
 ```
git push origin <nombre_de_la_rama>
 ```
