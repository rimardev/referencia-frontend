## Referencia Media Queries.

### Tabla de Breakpoints referenciales de Bootstrap

| **Breakpoint**       | **Dimension**   | **Class Bootstrap**  |
|----------------------|-----------------|----------------------|
| Extra small          | `<576px`        | none                 |
| Small                | `≥576px`        | _sm_                 |
| Medium               | `≥768px`        | _md_                 |
| Large                | `≥992px`        | _lg_                 |
| Extra large          | `≥1200px`       | _xl_                 |
| Extra extra large    | `≥1400px`       | _xxl_                |

---

### Ejemplo de Uso

```css
@media (max-width: 576px) {
    body {
        background: black;
    }
}
```
Este ejemplo cambia el color de fondo a negro cuando el ancho de la pantalla es menor o igual a 576px.

### Resumen - Media Queries

**Media Query**: Un bloque de CSS que se ejecuta bajo ciertas condiciones, generalmente relacionadas con el ancho de la pantalla (breakpoints).

**Breakpoint**: Puntos específicos en los que se producen cambios estéticos en una página web según el ancho de la pantalla. Ejemplo: cambiar de dos a tres columnas en una galería de imágenes cuando el ancho supera los 768px.

**Uso de Flexbox y CSS Grid**: Las media queries permiten ajustar la distribución y orientación de elementos con Flexbox y CSS Grid, haciendo la página responsive. Ejemplo: cambiar la orientación de un menú o la disposición de columnas en una grilla según el tamaño de la pantalla.

**Recomendación Mobile First**: Escribir las media queries desde los anchos más pequeños a los más grandes, siguiendo la filosofía "Mobile First" para asegurar una experiencia de usuario óptima en todos los dispositivos.

**Tipos de Media:**
- `all`: Aplica a todos los medios.
- `screen`: Utilizado para dispositivos con pantalla.
- `print`: Para la impresión de documentos.
- `speech`: Para sintetizadores de voz.

**Operador** `and`: Permite combinar varias condiciones en un solo breakpoint, como el ancho mínimo y máximo de un dispositivo.

### Condiciones en Media Queries
Las más comunes son el ancho (`min-width`, `max-width`), pero también se puede usar la orientación del dispositivo (`landscape`, `portrait`).

