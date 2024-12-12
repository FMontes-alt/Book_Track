# Explicación de Cómo Introducir un Libro en una Base de Datos

## ¿Qué es una Base de Datos?

Una base de datos es como un archivo muy organizado, donde podemos guardar información de manera que sea fácil de buscar, modificar o eliminar cuando sea necesario. En lugar de tener una hoja de cálculo gigante o papeles desordenados, la base de datos organiza todo en **"tablas"**.

---

## Paso 1: Preparar la Tabla para Guardar los Libros

En la base de datos, necesitamos crear una **tabla** que sea específica para almacenar los datos de los libros. Imagina que cada fila de la tabla es un libro y cada columna es un detalle del libro (como el título, el autor, etc.).

La tabla podría llamarse **Libros**, y tendría varias **columnas** o **campos** donde guardaremos la información:

| ID  | Título              | Autor              | Género        | Año de publicación | Estado   | Reseña                            |
|-----|---------------------|--------------------|---------------|--------------------|----------|-----------------------------------|
| 1   | El Gran Gatsby      | F. Scott Fitzgerald| Ficción       | 1925               | Leyendo  | "Una obra maestra de la literatura." |
| 2   | Matar a un Ruiseñor | Harper Lee         | Drama         | 1960               | Leído    | "Muy emotiva y conmovedora."        |

---

## Paso 2: Insertar un Libro Nuevo

Para agregar un libro a esta tabla, hacemos lo siguiente:

1. **Especificamos la información del libro**: como el título, el autor, el género, el año de publicación, el estado del libro (si ya fue leído, si estamos leyéndolo, o si está pendiente) y la reseña personal.
2. **Colocamos esta información en la nueva fila** de la tabla de libros.

Por ejemplo, si queremos agregar el libro *Cien años de soledad* de Gabriel García Márquez, la información que tendríamos sería algo así:

- **Título**: Cien años de soledad
- **Autor**: Gabriel García Márquez
- **Género**: Realismo Mágico
- **Año de publicación**: 1967
- **Estado**: Pendiente
- **Reseña**: "No lo he leído aún, pero sé que es una obra importante."

Entonces, en la base de datos, esta nueva entrada se vería como una nueva fila en la tabla de libros:

| ID  | Título                  | Autor                        | Género            | Año de publicación | Estado    | Reseña                                      |
|-----|-------------------------|------------------------------|-------------------|--------------------|-----------|---------------------------------------------|
| 1   | El Gran Gatsby          | F. Scott Fitzgerald          | Ficción           | 1925               | Leyendo   | "Una obra maestra de la literatura."        |
| 2   | Matar a un Ruiseñor     | Harper Lee                   | Drama             | 1960               | Leído     | "Muy emotiva y conmovedora."                |
| 3   | Cien años de soledad    | Gabriel García Márquez       | Realismo Mágico  | 1967               | Pendiente | "No lo he leído aún, pero sé que es una obra importante." |

---

## Paso 3: ¿Cómo se Realiza Esta Acción en la Base de Datos?

Cuando queremos agregar un libro, la base de datos ejecuta una **instrucción** o **consulta** llamada "INSERT" para insertar la nueva fila en la tabla. Esta consulta incluye toda la información del libro que estamos agregando.
