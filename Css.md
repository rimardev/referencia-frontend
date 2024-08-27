

## Sintaxis
```css
/* Comentario */
selector {
    propiedad: valor;
}
```

## Valor
- Medidas: `px` | `em` | `ex` | `%` | `in` | `cm` | `mm` | `pt` | `pc`
- Colores: `#ff6633` | `rgb(0,255,0)` | `black` | `white` | `red` | `blue` | `gray`

## Selector
- `*` : Todos los elementos
- `div` : `<div>`
- `div > div` : Elemento`<div>` dentro de `<div>`
- `div span` : Elemento `<span>` dentro de `<div>`
- `.clase` : Elementos con clase especifica
- `#id` : Elementos con un ID específico
- `a[href='x']` : Elemento `<a>` con atributo `href='x'`

## Pseudo-clases y Pseudo-elementos
- `:active` : Elemento seleccionado
- `:focus` : Elemento enfocado
- `:hover` : Elemento bajo el cursor
- `:link` : Enlace no visitado
- `:visited` : Enlace visitado
- `:first-child` : Primer hijo de otro elemento
- `:before` : Contenido antes del elemento
- `:after` : Contenido después del elemento

## Propiedades de Cajas
- **border**: `border-left`, `border-bottom`, `border-top`, `border-right`
- **border-width**: `thin`, `medium`, `thick`
- **border-color**: `color`, `rgb(x,x,x)`
- **border-style**: `solid`, `dashed`, `dotted`
- **margin**: `margin-top`, `margin-right`, `margin-bottom`, `margin-left`
- **padding**: `padding-top`, `padding-right`, `padding-bottom`, `padding-left`

## Posicionamiento
- **position**: `static`, `relative`, `absolute`, `fixed`
- **z-index**: `auto` | `<número>`
- **top**, **right**, **bottom**, **left**: `<longitud>` | `auto`
- **overflow**: `visible` | `hidden` | `scroll` | `auto`

## Dimensiones
- **width**, **height**: `<longitud>` | `auto`
- **max-width**, **max-height**: `<longitud>` | `none`
- **min-width**, **min-height**: `<longitud>`
- **line-height**: `<longitud>` | `normal` | `<número>`
