# App_intercambio_libros
Proyecto 4to Semestre BD

 Levantamiento de Requerimientos

## Proyecto: Biblioteca Digital - Intercambio de Libros

# Consideraciones

El proyecto consistirá en un servicio que gestione los intercambios de libros entre múltiples usuarios y el administrador. El administrador creará un usuario para cada persona que desee intercambiar un libro con él, con el cual se asociarán los intercambios, donaciones y libros intercambiados o donados.

Además de llevar un registro de los usuarios, el administrador mantendrá un control de los libros disponibles, incluyendo aquellos recibidos por donaciones y los que han sido intercambiados. Para cada libro se registrará:

- **Estado físico**, descrito mediante una calificación numérica obtenida a partir de una lista de verificación (checklist), junto con una imagen.
- **Información del libro**, como título, autor, fecha de publicación, edición y editorial.
- **Estado de lectura**, indicando si el administrador ha leído o no el libro.
- **Categorías**, asignando el libro a una o varias categorías (ciencia ficción, fantasía, historia, educativo, etc.).

### Lista de Requerimientos

| Código | Nombre                           |
| ------ | -------------------------------- |
| #01    | Registro de Usuario              |
| #02    | Creación de categorías           |
| #03    | Registro de libro                |
| #04    | Calificación del libro           |
| #05    | Registro de intercambio          |
| #06    | Registro de donaciones           |
| #07    | Sistema de sanciones             |
| #08    | Búsqueda y filtros               |
| #9     | Estadísticas Usuario             | 
| #10    | Estadísticas Libros              |

---

## Especificaciones

**Registro de usuario**  
   El usuario debe contar con los siguientes datos para completar el registro:  
   - Nombre  
   - Apellido  
   - Tipo de documento  
   - Número de documento  

   Con estos datos se podrá crear el usuario y guardarlo.  

   **Creación de categorías**  
   El administrador debe contar con los siguientes datos para crear una categoría:  
   - ID único  
   - Nombre de la categoría
   - Descripción  
   - Imagen que represente la categoría  

 **Registro de libro**
   El administrador debe contar con los siguientes datos para registrar un libro:
   - Nombre del libro
   - ID único
   - Estado físico (estos datos se obtendrán mediante el apartado "Calificación del libro", punto 4)
   - Autores
   - Editorial
   - Año de publicación
   - Categorías
   - Imagen

   **Calificación del libro**  
   El administrador podrá obtener la calificación del libro teniendo en cuenta las respuestas de un cuestionario que asista en el análisis del estado actual del libro.  

   - **¿La portada está en buen estado?**  
     A. Sin daños
     B. Rasguños leves
     C. Doblada o con roturas  
     D. Desprendida o con daños severos  

   - **¿La encuadernación está intacta?**  
     A. Completamente intacta  
     B. Un poco suelta  
     C. Despegándose  
     D. Completamente separada  

   - **¿Las páginas tienen marcas o manchas?**  
     A. No  
     B. Ligeramente  
     C. Subrayadas con marcador  
     D. Muchas manchas o marcas  

   - **¿Hay páginas rotas?**  
     A. No
     B. Ligeramente  
     C. Bastantes páginas dañadas  
     D. Páginas faltantes  

   - **¿Cuál es el estado general del libro?**  
     A. Como nuevo  
     B. Buen estado  
     C. Regular  
     D. Malo
## Registro de Intercambios

Cada intercambio se registrará con los siguientes datos:

- **Libros intercambiados**
- **Usuario que realiza el intercambio**
- **Estado de los libros previo al intercambio**
- **Fecha del intercambio**
- **Fecha de devolución**, pactada en el momento del intercambio

## Registro de Donaciones

Las donaciones serán registradas con la siguiente información:

- **Usuario que realiza la donación**
- **Libro donado**
- **Calidad del libro** (determinando el acceso a otros libros según la cantidad y calidad de los donados)
- **Fecha de la donación**

## Sistema de Penalizaciones

Los usuarios que no cumplan con la fecha de devolución pactada serán penalizados. La penalización quedará registrada en su perfil y conllevará una sanción inicial de **7 días sin poder realizar intercambios**. Cada infracción posterior duplicará la duración de la sanción.

## Registro de Intercambio

Cada intercambio de libros debe ser registrado y asociado con el usuario que realizó el intercambio. Durante el intercambio, a la entrada de los libros, se debe evaluar su estado para reescribir la calificación del libro.

El registro debe tener:

- **Usuario que participó en el intercambio**
- **Libros del intercambio**
- **Fecha en que se produjo el intercambio**
- **Fecha en que se devolverán los libros**

## Registro de Donaciones

Cada donación debe ser registrada y asociada al usuario que la realizó.

El registro debe tener:

- **Usuario que donó el libro**
- **Libro que donó** (Incluye la calificación del libro)
- **Fecha en la que lo donó**

## Sistema de Sanciones

Los usuarios que no devuelvan un libro a tiempo de un intercambio serán penalizados impidiéndole realizar intercambios por un determinado periodo de tiempo (**7 días**), que se duplicará con cada penalización y se guardará una marca permanente en su perfil.

## Búsqueda y Filtros

Permite a los usuarios buscar libros según diferentes criterios para facilitar la navegación y localización de títulos en la plataforma. La búsqueda debe ser eficiente y permitir a los usuarios encontrar los libros deseados de manera rápida.

**Filtros Disponibles:**

- **Título:** Permite buscar un libro ingresando su nombre.
- **Autor:** Permite buscar un libro ingresando el autor.
- **Categoría:** Clasificación de libros basada en el sistema de categorías.
- **Estado Físico:** Permite buscar libros en función de su condición (nuevo, usado, deteriorado, etc.).

## Estadística de Usuario

Muestra estadísticas detalladas relacionadas con la actividad de cada usuario dentro de la plataforma. Estas estadísticas permiten al administrador visualizar el historial de donaciones, intercambios y sanciones, promoviendo una mayor transparencia y control sobre sus transacciones.

### Datos Requeridos:

- **Administrador:** Identificación única del administrador dentro del sistema.
- **Cantidad de libros donados:** Total de libros aportados por el administrador a la biblioteca digital.
- **Cantidad de libros intercambiados:** Número de libros intercambiados por el administrador.
- **Historial de intercambios:** Registro de todos los libros que el administrador ha prestado o recibido en préstamo.
- **Historial de sanciones:** Registro de penalizaciones impuestas al administrador por incumplimiento de normas.

## Estadísticas de Libros

Muestra información detallada sobre los libros y su estado físico promedio dentro de la biblioteca digital.

### Datos Requeridos:

- **Libro:** Identificación única del libro dentro del sistema.
- **Cantidad de intercambios:** Total de veces que un libro ha sido intercambiado.
- **Calificación promedio:** Promedio de las calificaciones otorgadas al libro por los usuarios.

   
---



