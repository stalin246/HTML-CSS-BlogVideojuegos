### README - CSS Flexbox y Grid

#### Introducción

Este documento resume los conceptos clave y usos prácticos de CSS Flexbox y Grid, herramientas esenciales para el diseño web responsivo. Se abordan también los fragmentos de código específicos usados para estructurar y estilizar componentes web de manera eficiente.

---

### CSS Flexbox

Flexbox es un modelo de diseño unidimensional que ofrece un método eficiente para alinear y distribuir espacio entre ítems de un contenedor, incluso cuando su tamaño es desconocido o dinámico.

#### Propiedades Principales de Flexbox

- `display: flex;` - Activa el modelo Flexbox para un contenedor.
- `flex-direction:` - Define la dirección de los ítems en el contenedor (horizontal o vertical).
- `justify-content:` - Alinea los ítems en el eje principal (horizontal).
- `align-items:` - Alinea los ítems en el eje transversal (vertical).
- `flex-wrap:` - Permite que los ítems se envuelvan en múltiples líneas dentro del contenedor.
- `align-content:` - Alinea las líneas dentro del contenedor cuando hay espacio extra en el eje transversal.
- `gap:` - Establece el espacio entre los ítems.

#### Uso Práctico de Flexbox

Flexbox es ideal para componentes de interfaz de usuario donde necesitas un control fino sobre la alineación y el espaciado, como barras de navegación, galerías de imágenes y formularios. Por ejemplo:

```css
.navegacion {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 15rem;
}
```

---

### CSS Grid

Grid es un modelo de diseño bidimensional que maneja tanto filas como columnas, ideal para diseños complejos y multidimensionales.

#### Propiedades Principales de Grid

- `display: grid;` - Activa el modelo de cuadrícula.
- `grid-template-columns:` y `grid-template-rows:` - Define el tamaño y la cantidad de filas y columnas.
- `grid-gap:` - Establece el espacio entre filas y columnas (uso antiguo, reemplazado por `gap:`).
- `grid-column:` y `grid-row:` - Permite colocar ítems en columnas y filas específicas.
- `justify-items:` y `align-items:` - Alinea ítems individualmente en su celda.
- `justify-content:` y `align-content:` - Alinea el grid completo dentro del contenedor.

#### Uso Práctico de Grid

Grid es excelente para crear diseños complejos que implican múltiples áreas de contenido, como maquetas de páginas web, tableros de instrumentos y aplicaciones de diseño de periódicos. Ejemplo:

```css
.contenedor__grid {
    display: grid;
    grid-template-columns: 1fr 2fr;
    grid-template-rows: repeat(10, 1fr);
    margin: 0 0 0 9rem;
    column-gap: 2rem;
}
```

---

