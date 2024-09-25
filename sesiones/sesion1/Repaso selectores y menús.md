# **Tutorial de Selectors CSS i Menú Desplegable**

## **1. Introducció als Selectors CSS**

Els selectors CSS són una part fonamental per aplicar estils als elements HTML. Permeten seleccionar elements específics per a aplicar-los diferents propietats d'estil. En aquest tutorial, explorarem els diferents tipus de selectors i com combinar-los per obtenir resultats més específics.

---

## **2. Tipus de Selectors CSS**

### **2.1. Selector d'Element**

Selecciona tots els elements d'un tipus específic.

```css
p {
  color: blue;
}
```

### **2.2. Selector d'Identificador**

Selecciona un element amb un `id` únic.

```css
#principal {
  background-color: lightgrey;
}
```

### **2.3. Selector de Classe**

Selecciona tots els elements amb una classe específica.

```css
.important {
  font-weight: bold;
}
```

### **2.4. Selector d'Attribute**

Selecciona elements en funció d'un atribut.

```css
a[target="_blank"] {
  color: red;
}
```

### **2.5. Selector de Descendant**

Selecciona elements dins d'un altre element.

```css
div p {
  font-size: 14px;
}
```

### **2.6. Selector Adjacent**

Selecciona un element que immediatament segueix un altre.

```css
h1 + p {
  margin-top: 0;
}
```

### **2.7. Selector de Grup**

Aplica els mateixos estils a múltiples elements.

```css
h1, h2, h3 {
  color: darkgreen;
}
```

### **2.8. Selector Universal**

Selecciona tots els elements de la pàgina.

```css
* {
  box-sizing: border-box;
}
```

---

## **3. Combinació de Selectors**

Els selectors es poden combinar per aplicar estils de manera més precisa. Aquí hi ha alguns exemples:

### **3.1. Selector de Classe i Identificador**

```css
#principal .important {
  color: orange; /* Aplica només a elements amb classe 'important' dins del element amb id 'principal' */
}
```

### **3.2. Selector d'Element i Classe**

```css
p.important {
  text-decoration: underline; /* Aplica a tots els paràgrafs amb la classe 'important' */
}
```

### **3.3. Combinació de Descendants i Classes**

```css
div .important {
  background-color: yellow; /* Aplica a tots els elements amb la classe 'important' dins de qualsevol div */
}
```

### **3.4. Selector de Descendants Amb Múltiples Nivells**

```css
ul li a {
  color: purple; /* Aplica a tots els enllaços dins de qualsevol <li> dins d'un <ul> */
}
```

---

## **4. Mini Tutorial: Menú Desplegable amb Hover**

Ara que hem cobert els selectors, anem a crear un menú amb submenús que es despleguen amb l'efecte `hover`.

### **HTML per al Menú:**

```html
<!DOCTYPE html>
<html lang="ca">
<head>
  <meta charset="UTF-8">
  <title>Menú Desplegable</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <nav>
    <ul>
      <li><a href="#">Inici</a></li>
      <li>
        <a href="#">Serveis</a>
        <ul>
          <li><a href="#">Disseny</a></li>
          <li><a href="#">Desenvolupament</a></li>
          <li><a href="#">Manteniment</a></li>
        </ul>
      </li>
      <li><a href="#">Contacte</a></li>
    </ul>
  </nav>
</body>
</html>
```

### **CSS per al Menú:**

```css
nav {
  background-color: #333; /* Color de fons del menú */
}

nav ul {
  list-style-type: none; /* Elimina les marques de la llista */
  padding: 0; /* Elimina el padding per defecte */
  margin: 0; /* Elimina el marge per defecte */
}

nav ul li {
  position: relative; /* Necessari per posicionar el submenú */
}

nav ul li a {
  display: block; /* Fa que l'enllaç ocupi tot l'espai del <li> */
  padding: 10px;
  color: white; /* Color del text */
  text-decoration: none; /* Elimina el subratllat */
}

nav ul li ul {
  display: none; /* Amaga el submenú per defecte */
  position: absolute; /* Permet que el submenú es posiciona relativament al seu pare */
  left: 0; /* Posiciona el submenú a l'esquerra */
  top: 100%; /* Col·loca el submenú just a sota del menú principal */
  background-color: #444; /* Color de fons del submenú */
}

nav ul li:hover ul {
  display: block; /* Mostra el submenú quan es passa el cursor per sobre del <li> */
}

nav ul li ul li a {
  padding: 10px; /* Espai dins dels enllaços del submenú */
}
```

### **Anàlisi:**
- En utilitzar `display: none` i `display: block`, podem controlar la visibilitat dels submenús. La regla `nav ul li:hover ul` assegura que el submenú aparegui quan es passa el cursor sobre el seu element pare.
- Aquesta tècnica millora l'experiència de l'usuari, permetent una navegació més fluida i organitzada.

---

