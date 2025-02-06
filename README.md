# App_intercambio_libros
Proyecto 4to Semestre BD

 Levantamiento de Requerimientos

## Proyecto: Biblioteca Digital - Intercambio de Libros

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

1. **Registro de usuario**  
   El usuario debe contar con los siguientes datos para completar el registro:  
   - Nombre  
   - Apellido  
   - Tipo de documento  
   - Número de documento  

   Con estos datos se podrá crear el usuario y guardarlo.  

2. **Creación de categorías**  
   El administrador debe contar con los siguientes datos para crear una categoría:  
   - ID único  
   - Nombre de la categoría
   - Descripción  
   - Imagen que represente la categoría  

3. **Registro de libro**
   El administrador debe contar con los siguientes datos para registrar un libro:
   - Nombre del libro
   - ID único
   - Estado físico (estos datos se obtendrán mediante el apartado "Calificación del libro", punto 4)
   - Autores
   - Editorial
   - Año de publicación
   - Categorías
   - Imagen

4. **Calificación del libro**  
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
   
---



