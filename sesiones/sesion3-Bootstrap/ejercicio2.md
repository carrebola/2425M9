### Pàgina Web Portfoli Complexa amb Bootstrap 5

A continuació, crearem una pàgina de portfoli moderna i sofisticada amb temàtica professional utilitzant Bootstrap 5. Aquesta pàgina inclourà una secció de presentació (hero section), un sistema de navegació avançat, galeria de projectes, testimonis, formulari de contacte, i un peu de pàgina amb enllaços socials.

---

### Tutorial pas a pas per crear la pàgina del portfoli

Aquest tutorial et guiarà pas a pas per construir la pàgina del portfoli utilitzant Bootstrap 5, amb detalls sobre els elements HTML i les classes utilitzades en cada fase.

#### **Pas 1: Estructura bàsica del document HTML**
1. **Crea l'estructura del document HTML**:
   - Utilitza l'etiqueta `<!DOCTYPE html>` per definir el tipus de document.
   - Afegeix les etiquetes `<html>`, `<head>`, i `<body>` per construir l'estructura principal.

2. **Capçalera (`<head>`)**:
   - Afegeix l'etiqueta `<meta charset="UTF-8">` per establir la codificació de caràcters.
   - Inclou `<meta name="viewport" content="width=device-width, initial-scale=1.0">` per assegurar que la pàgina sigui responsiva.
   - Defineix el títol amb `<title>Portfoli Professional</title>`.
   - Inclou els enllaços a Bootstrap, Google Fonts i Font Awesome:
     ```html
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
     <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
     <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
     ```
   - Afegiu estils personalitzats dins d'una etiqueta `<style>`.

#### **Pas 2: Crear la secció Hero**
1. **Afegeix la secció Hero (`<header>`)**:
   - Utilitza l'etiqueta `<header>` amb la classe `hero-section` per definir la capçalera amb una imatge de fons.
   - Inclou una etiqueta `<div>` dins del `header` per centrar el contingut.
   - Afegeix un títol amb `<h1 class="display-4">Hola, soc un Dissenyador Web</h1>`.
   - Inclou un paràgraf amb la classe `lead` per donar-li un estil destacat.
   - Afegeix un botó amb la classe `btn btn-primary mt-3` per cridar a l'acció:
     ```html
     <a href="#projects" class="btn btn-primary mt-3">Explora els meus projectes</a>
     ```

#### **Pas 3: Crear la barra de navegació (Navbar)**
1. **Utilitza `<nav>` per a la barra de navegació**:
   - Utilitza les classes `navbar`, `navbar-expand-lg`, `navbar-dark`, i `bg-dark` per configurar l'estil de la barra.
   - Afegiu el logotip de la pàgina amb `<a class="navbar-brand" href="#">Portfoli</a>`.
   - Utilitza un botó d'expandir (`navbar-toggler`) per fer la barra responsiva en pantalles petites.
   - Inclou les opcions de navegació dins d'una llista `<ul>` amb classes `navbar-nav ms-auto` per alinear-les a la dreta.
   - Defineix cada element del menú amb `<li>` i `<a class="nav-link">` per enllaçar a les diferents seccions de la pàgina (Inici, Projectes, Testimonis, Contacte).

#### **Pas 4: Afegir la galeria de projectes**
1. **Crea la secció de projectes (`<section>`)**:
   - Utilitza la classe `container` per centrar i donar marges adequats a la secció.
   - Afegiu un títol amb `<h2 class="fw-bold">` i un subtítol amb `<p class="text-muted">` per explicar la secció.

2. **Organitza els projectes en graelles (`<div class="row">`)**:
   - Utilitza columnes amb la classe `col-md-4` per dividir els projectes en tres columnes.
   - Afegeix una targeta Bootstrap (`<div class="card">`) per a cada projecte amb imatges (`<img class="card-img-top">`) i text (`<div class="card-body">`).
   - Utilitza la classe `project-card` per a afegir transicions d'efecte "hover".

#### **Pas 5: Afegir la secció de testimonis**
1. **Crea una nova secció de testimonis (`<section>`)**:
   - Utilitza la classe `container` per assegurar un bon format responsiu.
   - Afegeix un títol i un subtítol per introduir la secció de testimonis.

2. **Organitza els testimonis en una fila (`<div class="row">`)**:
   - Utilitza columnes (`<div class="col-md-6">`) per mostrar dos testimonis costat a costat.
   - Defineix cada testimoni dins d'una div amb la classe `testimonial`, amb un paràgraf per al text del client i un footer amb `blockquote-footer` per al nom del client.

#### **Pas 6: Afegir un formulari de contacte**
1. **Crea la secció de contacte (`<section>`)**:
   - Utilitza la classe `container` per centrar el contingut.
   - Crea una fila amb `<div class="row">` i col·loca el formulari al centre amb `<div class="col-md-6 mx-auto">`.

2. **Defineix el formulari (`<form>`)**:
   - Utilitza la classe `border p-4 shadow` per donar estils al formulari.
   - Afegeix camps de text amb `<label>` i `<input class="form-control">` per al nom i correu electrònic.
   - Utilitza `<textarea class="form-control">` per al camp de missatge.
   - Inclou un botó d'enviament amb la classe `btn btn-primary w-100`.

#### **Pas 7: Crear un botó per obrir un modal**
1. **Afegeix un botó per obrir un modal**:
   - Utilitza la classe `btn btn-secondary` i el data attribute `data-bs-toggle="modal"` per configurar el botó que obre el modal.

2. **Defineix el modal (`<div class="modal">`)**:
   - Utilitza les classes `modal`, `modal-dialog`, i `modal-content` per crear l'estructura del modal.
   - Inclou un títol (`<h5 class="modal-title">`), el contingut (`<div class="modal-body">`) i els botons d'accions (`<div class="modal-footer">`).

#### **Pas 8: Crear el peu de pàgina (Footer)**
1. **Afegeix el footer (`<footer>`)**:
   - Utilitza les classes `text-center`, `bg-dark` i `text-light` per donar estil al peu de pàgina.
   - Inclou un missatge de copyright amb `<p>`.
   - Afegeix enllaços socials amb `<a>` i icones de Font Awesome per crear enllaços a les xarxes socials.

#### **Pas 9: Afegir els scripts de Bootstrap**
1. **Inclou els scripts de Bootstrap**:
   - Afegeix els scripts de Bootstrap al final del document, abans de tancar l'etiqueta `<body>` per assegurar el correcte funcionament dels components dinàmics:
     ```html
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
     ```

---
