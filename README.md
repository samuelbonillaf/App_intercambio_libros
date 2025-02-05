# App_intercambio_libros
Proyecto 4to Semestre BD

# Levantamiento de Requerimientos

## Proyecto: Biblioteca Digital - Intercambio de Libros

### Lista de Requerimientos

| Código | Nombre                           | Descripción                                                             | Prerrequisitos |
| ------ | -------------------------------- | ----------------------------------------------------------------------- | -------------- |
| #01    | Registro de Usuario              | Las personas deben registrarse para intercambiar libros                 | NO APLICA      |
| #02    | Creación de categorías           | Establecer las categorías de los libros                                 | NO APLICA      |
| #03    | Registro de libro                | Ingresar los datos básicos del libro a registrar                        | #02            |
| #04    | Calificación del libro           | Calificación basada en estado físico y calidad literaria                | #01, #02       |
| #05    | Registro de intercambio          | Guardar la fecha de intercambio, libros, fecha de devolución y dueño    | #01, #03       |
| #06    | Registro de donaciones           | Ingresar los datos necesarios para realizar donaciones                  | #01, #03       |
| #07    | Sistema de comentarios y reseñas | Permitir a los usuarios dejar opiniones sobre los libros intercambiados | #01, #03       |
| #08    | Sistema de sanciones             | Penalizar a usuarios que no devuelvan libros en la fecha estipulada     | #01, #05       |
| #09    | Búsqueda y filtros               | Buscar libros por título, autor, categoría o estado físico              | #02, #03       |
| #10    | Estadísticas Usuario             | Cantidad de libros donados e intercambiados                             | #01, #03, #05  |
| #11    | Estadísticas Libros              | Popularidad, estado promedio, cantidad de intercambios                  | #03, #05       |

---

## Consideraciones

- Las categorías se definen previamente y el usuario elige cuáles aplican a su libro.
- El estado físico del libro y su calidad literaria se promedian para determinar su calificación.
- Solo libros con calificaciones similares podrán ser intercambiados entre sí.
- Se debe definir qué estadísticas serán necesarias para análisis de usuarios y libros.
- El sistema de sanciones debe considerar tiempos máximos de préstamo y reincidencias.

---

## Preguntas a Resolver

1. ¿Es necesario tener algún tipo de notificaciones, por correo electrónico por ejemplo?
2. ¿Es realmente necesario tener un historial de Intercambios?
3. ¿Es necesario tener algún reporte de actividades, como tendencias, usuarios más activos, etc.?
4. ¿Es realmente necesario tener un sistema de reseñas y comentarios?


