## Referencia de Flexbox CSS.

### Propiedades del Contenedor Flex

| Propiedad       | Descripción                                                                                                                                           |
|-----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|
| `display`       | Define un elemento como contenedor flex. Valor común: `flex`.                                                                                          |
| `flex-direction`| Define la dirección en la que se colocarán los elementos flexibles dentro del contenedor. Valores: `row`, `row-reverse`, `column`, `column-reverse`.   |
| `flex-wrap`     | Define si los elementos flexibles deben ajustarse o no a múltiples líneas. Valores: `nowrap`, `wrap`, `wrap-reverse`.                                  |
| `justify-content`| Alinea los elementos flexibles a lo largo del eje principal. Valores: `flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `space-evenly`. |
| `align-items`   | Alinea los elementos flexibles a lo largo del eje transversal (perpendicular al principal). Valores: `flex-start`, `flex-end`, `center`, `baseline`, `stretch`. |
| `align-content` | Alinea las líneas del contenedor cuando hay espacio adicional en el eje transversal. Solo aplica cuando hay múltiples líneas. Valores: `flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `stretch`. |
| `gap`           | Define la separación entre los elementos flexibles (espacio entre filas y columnas).                                                                   |

### Propiedades de las Flex Items

| Propiedad    | Descripción                                                                                               |
|--------------|-----------------------------------------------------------------------------------------------------------|
| `order`      | Cambia el orden en el que se muestran los elementos flexibles dentro del contenedor. Valor por defecto: `0`. |
| `flex-grow`  | Define la capacidad de un elemento flexible para crecer si es necesario. Valor por defecto: `0`.           |
| `flex-shrink`| Define la capacidad de un elemento flexible para encogerse si es necesario. Valor por defecto: `1`.        |
| `flex-basis` | Define el tamaño base de un elemento antes de que se distribuyan los espacios disponibles. Valores: cualquier valor de tamaño CSS. |
| `align-self` | Alinea un solo elemento flexible a lo largo del eje transversal, sobrescribiendo `align-items` del contenedor. Valores: `auto`, `flex-start`, `flex-end`, `center`, `baseline`, `stretch`. |
