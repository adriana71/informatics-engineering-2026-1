# Arreglos Dinámicos en Java

## Ejercicios Básicos 🧮

### Ejercicio 1 – Crear y llenar un ArrayList

**Instrucciones:**

1. Crea un `ArrayList` de tipo `String` llamado `frutas`.
2. Agrega al menos 5 frutas.
3. Imprime el tamaño del arreglo.
4. Imprime todos los elementos usando:

   * un `for` tradicional
   * un `for-each`

**Salida esperada (ejemplo):**

```
Cantidad de frutas: 5
Manzana
Pera
Banana
...
```

### Ejercicio 2 – Modificar y eliminar elementos

**Instrucciones:**

1. Crea un `ArrayList<Integer>` llamado `numeros`.
2. Agrega los números del 1 al 10.
3. Cambia el valor del índice 4 por 100.
4. Elimina el número en la posición 2.
5. Muestra la lista final.

**Preguntas de reflexión:**

* ¿Qué sucede con los índices después de eliminar un elemento?
* ¿Cómo cambia el tamaño del `ArrayList`?

---

##  Parte 2: Aplicación Práctica 🤓

### Ejercicio 3 – Sistema simple de estudiantes

Crea un programa que:

1. Declare un `ArrayList<String>` llamado `estudiantes`.
2. Permita:

   * Agregar 3 nombres manualmente.
   * Mostrar la lista.
   * Eliminar un estudiante específico.
   * Verificar si un nombre existe usando `contains()`.

**Extra (opcional):**
Pedir los nombres por teclado usando `Scanner`.

## Parte 3: Código con Errores (Depuración) :shipit:

### Ejercicio 4 – Identifica y corrige los errores

Los estudiantes deben:

* Identificar los errores.
* Explicar por qué ocurren.
* Corregir el código.
* Escribir la versión corregida.


###  Código con errores:

```java
import java.util.ArrayList;

public class PruebaLista {

    public static void main(String[] args) {

        ArrayList lista = new ArrayList<String>();

        lista.add("Uno");
        lista.add("Dos");
        lista.add("Tres");

        System.out.println("Elemento en posición 3: " + lista.get(3));

        for (int i = 0; i <= lista.size(); i++) {
            System.out.println(lista.get(i));
        }

        lista.remove("Cuatro");

        System.out.println("Tamaño final: " + lista.length());
    }
}
```

## Parte 4: Desafío Final (Nivel Superior)

### Ejercicio 5 – Mini inventario 🏪

Crea un programa que:

* Almacene productos en un `ArrayList`.
* Permita agregar productos.
* Eliminar productos.
* Mostrar la lista ordenada (usa `Collections.sort()`).
* Mostrar cuántos productos hay.

