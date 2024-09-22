# Referencia de Flexbox CSS.

## Propiedades del Contenedor Flex

| Propiedad       | Descripción                                                                                                                                           |
|-----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|
| `display`       | Define un elemento como contenedor flex. Valor común: [`flex`].                                                                                          |
| `flex-direction`| Dirección en la que se colocarán los items dentro del contenedor: [`row`] [`row-reverse`] [`column`] [`column-reverse`].   |
| `flex-wrap`     | Define si los items deben ajustarse o no a múltiples líneas: [`nowrap`] [`wrap`] [`wrap-reverse`].                                  |
| `justify-content`| Alinea los items a lo largo del eje principal: [`flex-start`] [`flex-end`] [`center`] [`space-between`] [`space-around`] [`space-evenly`]. |
| `align-items`   | Alinea los items a lo largo del eje transversal: [`flex-start`] [`flex-end`] [`center`] [`baseline`] [`stretch`]. |
| `align-content` | Alinea las líneas del contenedor cuando hay espacio adicional en el eje transversal. Solo aplica cuando hay múltiples líneas: [`flex-start`] [`flex-end`] [`center`] [`space-between`] [`space-around`] [`stretch`]. |
| `gap`           | Define la separación entre los items (espacio entre filas y columnas).                                                                   |

## Propiedades de los Flex Items

| Propiedad    | Descripción                                                                                               |
|--------------|-----------------------------------------------------------------------------------------------------------|
| `order`      | Cambia el orden en el que se muestran los items dentro del contenedor. Valor por defecto: [`0`]. |
| `flex-grow`  | Define la capacidad de un items para crecer si es necesario. Valor por defecto: [`0`].           |
| `flex-shrink`| Define la capacidad de un items para encogerse si es necesario. Valor por defecto: [`1`].        |
| `flex-basis` | Define el tamaño base de un item antes de que se distribuyan los espacios disponibles. Valores: cualquier valor de tamaño CSS. |
| `align-self` | Alinea un solo item a lo largo del eje transversal, sobrescribiendo [`align-items`] del contenedor. Valores: [`auto`] [`flex-start`] [`flex-end`] [`center`] [`baseline`] [ `stretch`]. |
