# Proyecto Web – FP DAM

Proyecto de desarrollo de un sitio web corporativo como parte de una tarea del ciclo formativo de FP DAM.

El objetivo: aplicar buenas prácticas de HTML semántico, CSS moderno y diseño responsive, cumpliendo los requisitos técnicos establecidos en la actividad.


## Decisiones de diseño

### Colores
Se ha utilizado una paleta de colores sobria y profesional, adecuada para un entorno de consultoría:
- Azul oscuro como color principal, para transmitir seriedad y confianza.
- Tonos claros de fondo para mejorar la legibilidad.
- Un color acento discreto para destacar llamadas a la acción.

Los colores se han definido mediante variables CSS (`:root`) para facilitar la coherencia visual y el mantenimiento del código.
 

### Tipografías
Se han empleado dos tipografías:
- **Inter** para el cuerpo del texto, por su buena legibilidad en pantallas.
- **Source Serif 4** para los encabezados, con el objetivo de aportar contraste y jerarquía visual.

Ambas fuentes se importan desde Google Fonts y se gestionan mediante variables CSS.
 

### Estructura
El sitio está compuesto por varias páginas HTML, todas ellas con una estructura semántica común:
- "<header>"  con logo y navegación.
- "<main>" con el contenido principal de cada página.
- " <footer>" con información legal y enlaces.

Cada página desarrolla un requisito concreto:
- "index.html": Hero con efecto parallax, servicios con Flexbox y llamada a la acción.
- "contacto.html": Formulario con validación HTML5 y estilos de foco y estado.
- "cronologia.html": Tabla con efecto zebra mediante "nth-child".
- "proyecto-reservas.html": Layout con "main" y "aside" usando Flexbox.
- "aviso-legal.html": Contenido legal básico.

 
## Decisiones técnicas

- Se ha utilizado **Flexbox** para la alineación y estructura de los elementos (navegación, hero, tarjetas, layouts).
- El diseño es **responsive**, con un punto de ruptura principal en 768px mediante media queries.
- El efecto **parallax** se ha implementado únicamente en la portada usando "background-attachment: fixed", desactivándolo en dispositivos móviles por motivos de compatibilidad.
- El CSS está organizado por bloques y comentarios para facilitar la lectura y el mantenimiento.
- Se ha aplicado "box-sizing: border-box" de forma global.
 

## Dificultades encontradas y soluciones

- **Problemas de responsive en formularios y navegación**:  
  Se solucionaron estructurando correctamente los elementos y ajustando el comportamiento con Flexbox y media queries.

- **Conflictos de estilos en el menú de navegación**:  
  Se resolvió limitando el alcance de los estilos mediante clases específicas (".main-nav") para evitar efectos no deseados en otros elementos.

- **Compatibilidad del efecto parallax en móviles**:  
  Se desactivó el parallax en pantallas pequeñas para evitar errores de renderizado.
  
