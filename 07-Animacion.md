# CSS: Transiciones, Transformaciones y Animaciones
## Transiciones (transition)
La propiedad transition en CSS permite que los cambios en los estilos (como color, tamaño, etc.) ocurran de manera suave en lugar de instantánea. Define las propiedades que cambiaran, la duración, el tipo de animación como lineal o acelerada.
| **Componente**              | **Descripción**                                                | **Ejemplo**                            |
|-----------------------------|----------------------------------------------------------------|----------------------------------------|
| transition-property         | Propiedad(s) será(n) afectada(s) por la transición.            | `transition-property: width;`          |
| transition-duration         | Duración de la transición (en segundos o milisegundos).        | `transition-duration: 0.5s;`           |
| transition-timing-function  | Tipo de transición durante su duración (curva de aceleración). | `transition-timing-function: ease-in;` |
| transition-delay            | Retraso de inicio de transición (en segundos o milisegundos).  | `transition-delay: 0.2s;`              |

Si bien los componenetes se pueden usar por separado lo habitual es usarlo en una misma linea:

`transition: [property][duration][timing-function][delay]`;

### Ejemplo de uso
```css
.elemento {
  transition: background-color 0.5s ease-in 0.2s;
}

.elemento:hover {
  background-color: red;
}
```
### Opciones principales para `timing-function`
| **Valor**      | **Descripción**                                                                 |
|----------------|---------------------------------------------------------------------------------|
| `ease`         | Cambio suave (por defecto). Inicia lentamente, se acelera y luego desacelera.    |
| `linear`       | Cambio constante a lo largo de la transición (sin aceleración).                  |
| `ease-in`      | Inicia lentamente y luego acelera.                                               |
| `ease-out`     | Inicia rápido y luego desacelera.                                                |
| `ease-in-out`  | Comienza lento, se acelera en el medio y luego vuelve a desacelerar al final.    |
| `step-start`   | La transición se realiza de forma instantánea al inicio (salto abrupto).         |
| `step-end`     | La transición se realiza de forma instantánea al final (salto abrupto).          |
| `steps(n, start/end)` | Divide la transición en "n" pasos discretos. Con `start` o `end` define si el cambio ocurre al inicio o al final de cada paso. |
| `cubic-bezier(x1, y1, x2, y2)` | Permite definir una curva personalizada para la transición, usando puntos de control Bézier.  |

Nota: La opción cubic-bezier es la más avanzada, ya que te permite personalizar la curva de aceleración.


## Transformaciones (transform)


## Animaciones (animations)
