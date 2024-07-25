# PosicionamientoCSS

# Ejemplos de Posicionamiento en CSS

Este documento proporciona ejemplos y explicaciones de diferentes tipos de posicionamiento en CSS: `relative`, `absolute`, `fixed`, `sticky`, `float` y `z-index`.

## Índice de Ejemplos

1. [Posicionamiento Relativo (`relative`)](#posicionamiento-relativo-relative)
2. [Posicionamiento Absoluto (`absolute`)](#posicionamiento-absoluto-absolute)
3. [Posicionamiento Fijo (`fixed`)](#posicionamiento-fijo-fixed)
4. [Posicionamiento Pegajoso (`sticky`)](#posicionamiento-pegajoso-sticky)
5. [Flotante (`float`)](#flotante-float)
6. [Índice Z (`z-index`)](#índice-z-z-index)

## Posicionamiento Relativo (`relative`)

El elemento se posiciona en relación a su posición normal en el flujo del documento. Los ajustes `top`, `left`, `bottom`, y `right` desplazan el elemento desde su posición original.

### Ejemplo:

```html
<div style="position: relative; top: 20px; left: 30px; background-color: lightgray; padding: 10px;">
    Este es un elemento con posicionamiento relativo.
</div>
```

## Posicionamiento Absoluto (`absolute`)

El elemento se posiciona en relación a su primer contenedor posicionado (no estático). Sale del flujo normal del documento, lo que significa que no afecta a la posición de otros elementos.

### Ejemplo:

```html
<div style="position: relative; background-color: lightgray; padding: 10px;">
    Contenedor relativo
    <div style="position: absolute; top: 10px; right: 10px; background-color: lightcoral; padding: 10px;">
        Este es un elemento con posicionamiento absoluto.
    </div>
</div>
```

## Posicionamiento Fijo (`fixed`)

El elemento se posiciona en relación a la ventana del navegador y no se mueve al hacer scroll.

### Ejemplo:

```html
<div style="position: fixed; top: 0; left: 0; width: 100%; background-color: yellow; padding: 10px;">
    Este es un elemento con posicionamiento fijo.
</div>
```

## Posicionamiento Pegajoso (`sticky`)

El elemento se comporta como relativo hasta que alcanza una posición de desplazamiento específica, después de lo cual se comporta como fijo.

### Ejemplo:

```html
<div style="position: sticky; top: 0; background-color: lightblue; padding: 10px;">
    Este es un elemento con posicionamiento pegajoso.
</div>
```

## Flotante (`float`)

El elemento se desplaza a la izquierda o a la derecha, permitiendo que otros elementos fluyan a su alrededor.

### Ejemplo:

```html
<div style="float: left; width: 50%; background-color: pink; padding: 10px;">
    Este es un elemento flotante a la izquierda.
</div>
<div style="float: right; width: 50%; background-color: lightgreen; padding: 10px;">
    Este es un elemento flotante a la derecha.
</div>
<div style="clear: both;"></div>
```

## Índice Z (`z-index`)

El índice Z determina el orden de apilamiento de los elementos posicionados. Los elementos con mayor `z-index` se apilan por encima de los elementos con menor `z-index`.

### Ejemplo:

```html
<div style="position: relative; z-index: 1; background-color: red; width: 100px; height: 100px;">
    Elemento con z-index 1
</div>
<div style="position: relative; z-index: 2; background-color: blue; width: 100px; height: 100px; margin-top: -50px;">
    Elemento con z-index 2
</div>
```

