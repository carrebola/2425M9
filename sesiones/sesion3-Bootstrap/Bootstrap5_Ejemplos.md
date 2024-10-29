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

## 17. Agregar título y contenido a una tarjeta

Para agregar un título y contenido a una tarjeta, se utilizan las clases `.card-title` y `.card-text`.

```html
<div class="card">
  <div class="card-body">
    <h5 class="card-title">Título de la tarjeta</h5>
    <p class="card-text">Contenido de la tarjeta</p>
  </div>
</div>
```

## 18. Crear un formulario

Para crear un formulario, se utiliza la etiqueta `<form>` y las clases de Bootstrap como `.form-group` para agrupar los elementos.

```html
<form>
  <div class="mb-3">
    <label for="exampleInputEmail1" class="form-label">Correo electrónico</label>
    <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
    <div id="emailHelp" class="form-text">Nunca compartiremos tu correo con nadie más.</div>
  </div>
  <div class="mb-3">
    <label for="exampleInputPassword1" class="form-label">Contraseña</label>
    <input type="password" class="form-control" id="exampleInputPassword1">
  </div>
  <button type="submit" class="btn btn-primary">Enviar</button>
</form>
```

## 19. Agrupar botones en un formulario

Para agrupar botones, se utiliza `.btn-group`.

```html
<div class="btn-group" role="group" aria-label="Basic example">
  <button type="button" class="btn btn-primary">Izquierda</button>
  <button type="button" class="btn btn-primary">Centro</button>
  <button type="button" class="btn btn-primary">Derecha</button>
</div>
```

## 20. Crear una tabla

Para crear una tabla, se utiliza la clase `.table`.

```html
<table class="table">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">Nombre</th>
      <th scope="col">Apellido</th>
      <th scope="col">Usuario</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Mark</td>
      <td>Otto</td>
      <td>@mdo</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Jacob</td>
      <td>Thornton</td>
      <td>@fat</td>
    </tr>
  </tbody>
</table>
```

## 21. Ajustar el tamaño de una tabla

Para hacer una tabla más pequeña, se usa `.table-sm`.

```html
<table class="table table-sm">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">Nombre</th>
      <th scope="col">Apellido</th>
      <th scope="col">Usuario</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Mark</td>
      <td>Otto</td>
      <td>@mdo</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Jacob</td>
      <td>Thornton</td>
      <td>@fat</td>
    </tr>
  </tbody>
</table>
```

## 22. Crear un modal

Para crear un modal, se utilizan las clases `.modal`, `.modal-dialog` y `.modal-content`.

```html
<!-- Botón para abrir el modal -->
<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
  Lanzar modal
</button>

<!-- Modal -->
<div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModalLabel">Título del modal</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Cerrar"></button>
      </div>
      <div class="modal-body">
        Contenido del modal
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cerrar</button>
        <button type="button" class="btn btn-primary">Guardar cambios</button>
      </div>
    </div>
  </div>
</div>
```

## 23. Crear una lista no ordenada

Para crear una lista no ordenada sin estilo de viñetas, se usa `.list-unstyled`.

```html
<ul class="list-unstyled">
  <li>Elemento sin viñeta 1</li>
  <li>Elemento sin viñeta 2</li>
  <li>Elemento sin viñeta 3</li>
</ul>
```

## 24. Crear una barra de navegación

Para crear una barra de navegación, se usa `.navbar` y `.navbar-expand-*` para ajustar su tamaño.

```html
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <a class="navbar-brand" href="#">Navbar</a>
  <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNav">
    <ul class="navbar-nav">
      <li class="nav-item">
        <a class="nav-link active" aria-current="page" href="#">Inicio</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Características</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Precios</a>
      </li>
    </ul>
  </div>
</nav>
```

## 25. Crear un menú desplegable

Para crear un menú desplegable, se usa `.dropdown` y `.dropdown-menu`.

```html
<div class="dropdown">
  <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton" data-bs-toggle="dropdown" aria-expanded="false">
    Menú desplegable
  </button>
  <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton">
    <li><a class="dropdown-item" href="#">Acción 1</a></li>
    <li><a class="dropdown-item" href="#">Acción 2</a></li>
    <li><a class="dropdown-item" href="#">Acción 3</a></li>
  </ul>
</div>
```

## 26. Crear una alerta

Para crear una alerta, se usa `.alert` junto con clases de color como `.alert-primary`.

```html
<div class="alert alert-primary" role="alert">
  Esta es una alerta primaria—¡échale un vistazo!
</div>
```

## 27. Utilizar Flexbox

Para utilizar Flexbox, se usa `.d-flex` para definir un contenedor como flex.

```html
<div class="d-flex justify-content-between">
  <div>Elemento 1</div>
  <div>Elemento 2</div>
</div>
```

## 28. Alinear elementos en línea con Flexbox

Para alinear elementos verticalmente, se usa `.align-items-*`.

```html
<div class="d-flex align-items-center">
  <div>Elemento alineado</div>
</div>
```

## 29. Ajustar la dirección de los elementos con Flexbox

Para cambiar la dirección de los elementos, se usa `.flex-row` o `.flex-column`.

```html
<div class="d-flex flex-column">
  <div>Elemento 1</div>
  <div>Elemento 2</div>
</div>
```

## 30. Centrar los elementos con Flexbox

Para centrar elementos horizontal y verticalmente, se usa `.justify-content-center` y `.align-items-center`.

```html
<div class="d-flex justify-content-center align-items-center" style="height: 200px;">
  <div>Elemento centrado</div>
</div>
```
