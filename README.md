# Práctica de Vectores de Objetos en C++

Este repositorio contiene la solución algorítmica a un ejercicio de gestión de inventarios utilizando C++, ideal como práctica para fortalecer los fundamentos de programación y explorar prácticas de codificación segura orientadas a la ciberseguridad.

## Descripción
El programa refactoriza un sistema de inventario básico. En lugar de usar múltiples arreglos paralelos, agrupa las propiedades de los productos (nombre y precio) mediante el uso de un `struct`. Estos objetos se almacenan dinámicamente utilizando el contenedor `std::vector` de la biblioteca estándar de C++ (STL).

## Características Principales
* **Uso de `struct`:** Agrupa lógicamente los datos relacionados en una sola entidad `Producto`.
* **Asignación Dinámica de Memoria:** Utiliza `std::vector` para permitir que el inventario crezca en tiempo de ejecución (`push_back()`).
* **Programación Defensiva:** Implementa el método `at()` y bloques `try-catch` para validar los accesos a la memoria. Esto es vital para prevenir vulnerabilidades comunes como accesos a índices inválidos o desbordamientos.
* **Iteradores eficientes:** Utiliza bucles `for` basados en rangos con referencias constantes (`const auto&`) para iterar sin realizar copias innecesarias de memoria.
