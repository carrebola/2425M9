
# Ejemplos de Bootstrap 5

## 1. Clase para crear un margen superior

Para aplicar un margen superior en Bootstrap 5, se utiliza la clase `mt-*`, donde `*` varía de 0 a 5, dependiendo del tamaño deseado.

```html
<div class="mt-3">Contenido con margen superior moderado</div>
```

## 2. Contenedor fluido

Para crear un contenedor que ocupe todo el ancho de la pantalla, se usa `.container-fluid`.

```html
<div class="container-fluid">
  Contenido dentro de un contenedor fluido
</div>
```

## 3. Agrupar elementos con clases

Bootstrap 5 ofrece `.d-flex` para agrupar elementos y organizar su disposición con Flexbox.

```html
<div class="d-flex">
  <div class="p-2">Elemento 1</div>
  <div class="p-2">Elemento 2</div>
</div>
```

## 4. Crear una fila

Para dividir contenido en filas y columnas, se utiliza `.row`.

```html
<div class="row">
  <div class="col">Columna 1</div>
  <div class="col">Columna 2</div>
</div>
```

## 5. Columna con ancho fijo

Para una columna con ancho ajustado al contenido, se usa `.col-auto`.

```html
<div class="row">
  <div class="col-auto">Columna ajustada</div>
  <div class="col">Columna flexible</div>
</div>
```

## 6. Tamaño de letra

Para ajustar el tamaño del texto, usamos `fs-*`, donde `*` varía de 1 a 6.

```html
<p class="fs-1">Texto grande</p>
<p class="fs-6">Texto pequeño</p>
```

## 7. Crear un botón

Un botón en Bootstrap 5 se crea con `.btn` y variantes de color, como `.btn-primary`.

```html
<button class="btn btn-primary">Botón primario</button>
```

## 8. Crear un borde

Para aplicar un borde, usamos `.border`.

```html
<div class="border">Contenido con borde</div>
```

## 9. Aplicar un borde superior

Para un borde superior, usamos `.border-top`.

```html
<div class="border-top">Contenido con borde superior</div>
```

## 10. Borde redondeado

Para aplicar bordes redondeados, utilizamos `.rounded`.

```html
<div class="rounded">Borde redondeado</div>
```

## 11. Borde sólido

Bootstrap 5 aplica bordes sólidos por defecto. Para ajustar el grosor, se usa `.border-1` a `.border-5`.

```html
<div class="border border-3">Borde sólido y grueso</div>
```

## 12. Borde múltiple

Bootstrap 5 no soporta directamente bordes múltiples; sin embargo, puede lograrse con CSS personalizado.

```html
<style>
  .multiple-borders {
    border: 3px solid black;
    box-shadow: 0 0 0 3px red;
  }
</style>
<div class="multiple-borders">Borde múltiple</div>
```

## 13. Fondo de color

Para aplicar un fondo de color, usamos `bg-*` como `bg-primary` o `bg-secondary`.

```html
<div class="bg-primary text-white p-3">Fondo de color primario</div>
```

## 14. Iconos de Font Awesome

Para integrar iconos, añadimos las clases de Font Awesome.

```html
<i class="fa fa-home"></i> Icono de inicio
```

## 15. Menú de navegación

Para crear un menú de navegación, usamos `.navbar` y `.navbar-expand-*`.

```html
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <a class="navbar-brand" href="#">Logo</a>
</nav>
```

## 16. Crear una tarjeta

Una tarjeta se crea con `.card`.

```html
<div class="card">
  <div class="card-body">
    Contenido de la tarjeta
  </div>
</div>
```

... (continúa el archivo con los restantes ejemplos y descripciones)