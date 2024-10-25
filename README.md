# ft_printf

Este proyecto forma parte del currículo de la escuela 42, específicamente del campus 42 Barcelona. El objetivo de `ft_printf` es recrear la función `printf` de la biblioteca estándar de C (declarada en `<stdio.h>`), replicando su funcionalidad principal y algunas de sus variantes.

## Descripción

La función `ft_printf` permite mostrar en la salida estándar una variedad de formatos de datos (caracteres, cadenas, enteros, hexadecimales, etc.), de forma similar a `printf` en C. Este proyecto implica un manejo avanzado de estructuras, especificadores de formato y la manipulación de punteros y buffers, además de una gestión precisa de la memoria.

## Objetivos

- Desarrollar una comprensión más profunda del manejo de argumentos variádicos.
- Practicar la manipulación de punteros y buffers en C.
- Implementar y optimizar funciones de formato complejas.

## Especificaciones

`ft_printf` debe ser capaz de manejar los siguientes especificadores de formato:

- `%c`: Caracter individual.
- `%s`: Cadena de caracteres.
- `%p`: Puntero en formato hexadecimal.
- `%d` / `%i`: Entero en base 10.
- `%u`: Entero sin signo en base 10.
- `%x` / `%X`: Entero sin signo en hexadecimal (en minúscula / mayúscula).
- `%%`: Caracter de porcentaje.

Cada uno de estos especificadores debe ser interpretado correctamente y sin causar fugas de memoria ni errores de segmentación.

## Instalación

1. Clona el repositorio en tu máquina local:

    ```bash
    git clone https://github.com//ft_printf.git
    cd ft_printf
    ```

2. Compila el proyecto:

    ```bash
    make
    ```

3. Incluye `libftprintf.a` en tu proyecto, y usa `ft_printf` como lo harías con la función `printf`.

## Uso

Aquí hay un ejemplo de uso de `ft_printf` en tu código:

```c
#include "ft_printf.h"

int main() {
    ft_printf("Hola, mundo!\n");
    ft_printf("Número: %d\n", 42);
    ft_printf("Hexadecimal: %x\n", 255);
    return 0;
}
