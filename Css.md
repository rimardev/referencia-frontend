# CSS: Guía de Referencia Rápida

## Sintaxis

```css
/* Comentario */
selector {
    propiedad: valor;
}
```

## Valores

| Tipo    | Unidades                              |
| ------- | ------------------------------------- |
| Longitud | `px`, `em`, `%`, `in`, `cm`, `mm`, `pt`, `pc` |
| Colores | `#ff6633`, `rgb(0,255,0)`, `black`, `white`, `red`, `blue`, `gray` |

## Selectores

| Selector          | Descripción                                       |
| ----------------- | ------------------------------------------------- |
| `*`               | Todos los elementos                               |
| `div`             | Selecciona todos los `<div>`                      |
| `div > div`       | Elementos `<div>` que son hijos directos de otro `<div>` |
| `div span`        | Elementos `<span>` dentro de un `<div>`           |
| `.clase`          | Selecciona elementos de una clase específica      |
| `#id`             | Selecciona un elemento con un ID específico       |
| `a[href='x']`     | Selecciona un `<a>` con el atributo `href='x'`    |

## Pseudo-clases y Pseudo-elementos

| Pseudo-clase / Pseudo-elemento | Descripción                                      |
| ------------------------------ | ------------------------------------------------ |
| `:active`                      | Elemento seleccionado                            |
| `:focus`                       | Elemento enfocado                                |
| `:hover`                       | Elemento con el cursor sobre él                  |
| `:link`                        | Enlace no visitado                               |
| `:visited`                     | Enlace visitado                                  |
| `:first-child`                 | Primer hijo de otro elemento                     |
| `:before`                      | Contenido antes del elemento                     |
| `:after`                       | Contenido después del elemento                   |

## Propiedades de Cajas

| Propiedad     | Valores Ejemplo                                        |
| ------------- | ------------------------------------------------------ |
| `border`      | `border-left`, `border-bottom`, `border-top`, `border-right` |
| `border-width`| `thin`, `medium`, `thick`                              |
| `border-color`| `color`, `rgb(x,x,x)`                                  |
| `border-style`| `solid`, `dashed`, `dotted`                            |
| `margin`      | `margin-top`, `margin-right`, `margin-bottom`, `margin-left` |
| `padding`     | `padding-top`, `padding-right`, `padding-bottom`, `padding-left` |

## Posicionamiento

| Propiedad     | Valores Ejemplo                                        |
| ------------- | ------------------------------------------------------ |
| `position`    | `static`, `relative`, `absolute`, `fixed`              |
| `z-index`     | `auto`, `<número>`                                     |
| `top`, `right`, `bottom`, `left` | `<longitud>`, `auto`                 |
| `overflow`    | `visible`, `hidden`, `scroll`, `auto`                  |

## Dimensiones

| Propiedad     | Valores Ejemplo                                        |
| ------------- | ------------------------------------------------------ |
| `width`, `height` | `<longitud>`, `auto`                               |
| `max-width`, `max-height` | `<longitud>`, `none`                       |
| `min-width`, `min-height` | `<longitud>`                               |
| `line-height` | `<longitud>`, `normal`, `<número>`                     |
