### Guia d'ús de Bootstrap 5

**Bootstrap 5** és un framework de codi obert que facilita el desenvolupament web responsiu i modern. Ofereix una col·lecció d'eines per dissenyar pàgines web, amb components predissenyats i utilitats que s'integren fàcilment en qualsevol projecte.

A continuació, et presento una guia ràpida dels elements i aspectes més rellevants de Bootstrap 5.

### 1. **Instal·lació de Bootstrap 5**
Pots integrar Bootstrap al teu projecte de dues maneres principals:
- **CDN**: La manera més fàcil és incloure un enllaç a la capçalera del teu document HTML.
```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
```
- **NPM**: Si utilitzes un gestor de paquets com npm:
```bash
npm install bootstrap
```

### 2. **Sistema de Graelles (Grid System)**
El sistema de graelles de Bootstrap 5 es basa en una malla de 12 columnes, que facilita la creació de dissenys responsius. Els elements es col·loquen dins de files (`.row`) i columnes (`.col`).

Exemple bàsic:
```html
<div class="container">
  <div class="row">
    <div class="col">Columna 1</div>
    <div class="col">Columna 2</div>
    <div class="col">Columna 3</div>
  </div>
</div>
```

### 3. **Tipografia**
Bootstrap inclou estils de tipografia predeterminats per a la majoria d'elements de text. Alguns exemples:
- **Encapçalaments**: `h1` a `h6`, o `.h1` a `.h6`.
- **Text en negreta**: Usa la classe `.fw-bold` per a aplicar negreta.
- **Text en cursiva**: Usa la classe `.fst-italic`.

Exemple:
```html
<h1 class="h3">Aquest és un encapçalament de nivell 3</h1>
<p class="fw-bold">Text en negreta</p>
<p class="fst-italic">Text en cursiva</p>
```

### 4. **Botons**
Els botons de Bootstrap es poden personalitzar fàcilment amb les classes predeterminades com `.btn` i variacions de color.
```html
<button type="button" class="btn btn-primary">Botó primari</button>
<button type="button" class="btn btn-secondary">Botó secundari</button>
```
També pots utilitzar classes com `.btn-lg` o `.btn-sm` per modificar la mida dels botons.

### 5. **Formularis**
Bootstrap ofereix dissenys elegants per a formularis, amb classes per a cada tipus d'input.
```html
<form>
  <div class="mb-3">
    <label for="exampleInputEmail1" class="form-label">Adreça de correu electrònic</label>
    <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
  </div>
  <button type="submit" class="btn btn-primary">Enviar</button>
</form>
```
Algunes utilitats per formularis inclouen `.form-control`, `.form-check`, `.input-group`, etc.

### 6. **Alertes**
Pots mostrar missatges d'alerta amb estils predeterminats per a diferents tipus de missatges (informació, èxit, alerta, error):
```html
<div class="alert alert-success" role="alert">
  Operació completada amb èxit!
</div>
<div class="alert alert-danger" role="alert">
  Hi ha hagut un error.
</div>
```

### 7. **Navegació (Navbar)**
Bootstrap 5 inclou dissenys responsius per a les barres de navegació. Aquests poden ser estils simples o amb elements desplegables.
```html
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Brand</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Inici</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Característiques</a>
        </li>
      </ul>
    </div>
  </div>
</nav>
```

### 8. **Cards (Targetes)**
Les targetes són una forma de mostrar contingut dins de contenidors amb marges i estils.
```html
<div class="card" style="width: 18rem;">
  <img src="image.jpg" class="card-img-top" alt="Imatge">
  <div class="card-body">
    <h5 class="card-title">Títol de la targeta</h5>
    <p class="card-text">Això és una targeta amb una mica de text.</p>
    <a href="#" class="btn btn-primary">Anar en algun lloc</a>
  </div>
</div>
```

### 9. **Taules**
Pots utilitzar Bootstrap per dissenyar taules responsives amb estils predeterminats. La classe `.table` ofereix un estil net i senzill per a les taules.
```html
<table class="table">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">Nom</th>
      <th scope="col">Cognom</th>
      <th scope="col">Usuari</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Joan</td>
      <td>Pérez</td>
      <td>@joanp</td>
    </tr>
  </tbody>
</table>
```

### 10. **Modal**
Un modal és una finestra emergent que es pot utilitzar per mostrar informació, formularis o altres elements.
```html
<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
  Obrir modal
</button>

<div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModalLabel">Títol del modal</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Tancar"></button>
      </div>
      <div class="modal-body">
        Contingut del modal aquí.
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Tancar</button>
        <button type="button" class="btn btn-primary">Guardar canvis</button>
      </div>
    </div>
  </div>
</div>
```

### 11. **Icones**
Bootstrap 5 ja no inclou les icones de forma predeterminada, però es poden utilitzar les **Bootstrap Icons** amb un paquet separat. 
Pots afegir-les amb aquest enllaç:
```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap-icons/font/bootstrap-icons.css" rel="stylesheet">
```

### 12. **Flexbox i Utilities**
Bootstrap fa ús intensiu de Flexbox per permetre la creació de dissenys flexibles. Utilitza classes com `.d-flex`, `.align-items-center`, `.justify-content-between`, etc., per manipular el comportament dels elements dins d'un contenidor flex.
```html
<div class="d-flex justify-content-between">
  <div>Píxel 1</div>
  <div>Píxel 2</div>
</div>
```

---

Aquesta és una guia bàsica per començar a utilitzar Bootstrap 5. Explorar la [documentació oficial de Bootstrap](https://getbootstrap.com/docs/5.0/getting-started/introduction/) t'ajudarà a aprofundir més en cada component.
