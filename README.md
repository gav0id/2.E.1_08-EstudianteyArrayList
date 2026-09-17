Ejercicio 2.E.1 08 - Estudiante

Lógica del programa
Para resolver este ejercicio, diseñé la clase `Estudiante` incorporando el uso de colecciones dinámicas. Importé la clase `ArrayList` de la biblioteca `java.util` para poder almacenar una cantidad indeterminada de notas. Definí dos atributos: `nombre` (String) y `calificaciones` (ArrayList de tipo Double).

En el constructor, además de asignar el nombre, inicialicé la lista de calificaciones para crear el objeto en memoria y evitar errores al momento de agregar datos.

Desarrollé el comportamiento de la clase a través de tres métodos:
1. `agregarNota(double nota)`: Implementé una validación condicional (`if`) para asegurar que solo se guarden en la lista las notas válidas (entre 0 y 10 inclusive).
2. `calcularPromedio()`: Utilicé un bucle `for-each` para recorrer la lista de calificaciones, acumular la suma de todas las notas y finalmente retornar el promedio dividiendo esa suma por el tamaño total de la lista (`calificaciones.size()`).
3. `haAprobado()`: Reutilicé el método `calcularPromedio()` dentro de un condicional para evaluar si el estudiante alcanza la nota mínima de aprobación (6.0), retornando `true` o `false` según corresponda.

Dentro del método `main`, desarrollé la siguiente lógica de prueba:
1. Instancié un objeto `Estudiante` llamado "Benito".
2. Intenté agregar varias notas usando el método `agregarNota()`. A propósito, incluí una nota inválida (15.0) para comprobar que la lógica de validación funciona correctamente y la rechaza.
3. Imprimí por consola el promedio final y el estado de aprobación para verificar que los cálculos iterativos y las condiciones devuelven los resultados esperados.

Ejecución en consola
<img width="1366" height="722" alt="imagen" src="https://github.com/user-attachments/assets/428b3b40-6c0a-41ed-be9e-eeb3c0ce70ad" />

