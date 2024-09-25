
# **Tutorial Pràctic de CSS: Conceptes Bàsics**

## **1. Introducció al CSS**

CSS (Cascading Style Sheets) és el llenguatge que permet aplicar estils a documents HTML. Permet separar el contingut de la presentació, la qual cosa facilita la gestió i manteniment del disseny. CSS es pot aplicar de tres maneres:

- **Inline CSS**: s'aplica directament a l'element HTML.
- **Internal CSS**: es defineix dins d'una etiqueta `<style>` a la capçalera de l'HTML.
- **External CSS**: s'aplica mitjançant un fitxer CSS extern vinculat amb l'etiqueta `<link>`.

### **Exemple de CSS Bàsic:**

```html
<!DOCTYPE html>
<html lang="ca">
<head>
  <meta charset="UTF-8">
  <title>Exemple CSS Bàsic</title>
  <style>
    h1 {
      color: blue; /* Defineix el color del text del títol */
    }
  </style>
</head>
<body>
  <h1>Això és un títol estilitzat amb CSS</h1>
</body>
</html>
```

### **Anàlisi:**
- L'estil `h1 { color: blue; }` aplica un color blau a tots els elements `<h1>`. La separació del contingut i el disseny és clau per a una bona estructura del projecte.

### **Exercici 1:**
Canvia el color del text del títol a **vermell** i experimenta amb altres propietats com `font-size`, `font-family`, i `text-align`.

---

## **2. Selectors CSS**

Els selectors són essencials per aplicar estils a elements específics. La seva especificitat determina quins estils prevalen quan es produeixen conflictes. 

### **Tipus de Selectors:**
- **Selector d'etiqueta**: selecciona tots els elements d'un tipus (ex. `<h1>`).
- **Selector d'identificador**: selecciona un element únic amb un `id` (especificat amb `#`).
- **Selector de classe**: selecciona tots els elements amb una classe específica (especificat amb `.`).
- **Selector de descendant**: selecciona elements dins d'un altre element (ex. `div p` selecciona tots els `<p>` dins d'un `<div>`).

### **Exemple:**

```css
h1 {
  color: green; /* Estil per a tots els h1 */
}

#principal {
  color: red; /* Selector d'identificador */
}

.important {
  font-weight: bold; /* Selector de classe */
}
```

### **Anàlisi:**
- Els selectors d'identificador i de classe permeten aplicar estils a elements específics, facilitant la personalització del disseny sense afectar altres elements.

### **Exercici 2:**
Afegeix una segona classe anomenada `secondary` i aplica-la a un altre paràgraf amb un color de text diferent.

---

## **3. Propietats de Text**

CSS ofereix múltiples propietats per estilitzar el text, la qual cosa inclou colors, mides, tipus de lletra i alineació. La comprensió d'aquestes propietats és crucial per a una presentació efectiva del contingut.

### **Propietats Comunes:**
- `color`: especifica el color del text (ex: `color: #333;`).
- `font-size`: controla la mida de la lletra (ex: `font-size: 16px;`).
- `font-family`: defineix el tipus de lletra (ex: `font-family: 'Helvetica', sans-serif;`).
- `text-align`: controla l'alineació del text (ex: `text-align: center;`).

### **Exemple:**

```css
p {
  color: navy;
  font-size: 18px;
  font-family: Arial, sans-serif;
  text-align: justify; /* Justifica el text */
}
```

### **Anàlisi:**
- L'alineació `justify` crea una aparença neta i ordenada en documents llargs. La tipografia adequada pot millorar la llegibilitat i l'atractiu visual de la pàgina.

### **Exercici 3:**
Crea un text centrat amb una mida de lletra de 24px i utilitza una tipografia personalitzada com `Courier New`.

---

## **4. Colors i Fons**

Els colors es poden aplicar als elements a través de les propietats `color` per al text i `background-color` per al fons. Conèixer els diferents formats de color (noms, hexadecimals, RGB, RGBA) és important per a un disseny efectiu.

### **Exemple:**

```css
body {
  background-color: lightgray; /* Color de fons */
}

h1 {
  color: darkblue; /* Color del text */
}
```

### **Anàlisi:**
- Els colors poden definir-se utilitzant noms com `lightgray`, codis hexadecimals com `#D3D3D3`, o funcions RGB com `rgb(211, 211, 211)`. L'ús de `rgba` permet especificar un valor d'opacitat, útil per a efectes de superposició.

### **Exercici 4:**
Estableix un fons de color gradient (utilitzant `linear-gradient`) i aplica diferents colors als elements de text.

---

## **5. Marge, Padding i Border**

Aquestes propietats controlen l'espai dins i fora dels elements i són fonamentals per al disseny i la distribució del contingut.

### **Definicions:**
- `margin`: espai extern entre un element i altres elements.
- `padding`: espai intern entre el contingut i les vores de l'element.
- `border`: crea un contorn al voltant de l'element.

### **Exemple:**

```css
div {
  margin: 20px; /* Espai extern */
  padding: 10px; /* Espai intern */
  border: 2px solid black; /* Vora */
}
```

### **Anàlisi:**
- La propietat `margin` pot ser específica per a cada costat: `margin-top`, `margin-right`, `margin-bottom`, `margin-left`, proporcionant flexibilitat en el disseny.
- La propietat `box-sizing` controla si el padding i la vora s'inclouen dins de les dimensions especificades de l'element, simplificant el càlcul de l'espai ocupat.

### **Exercici 5:**
Crea un quadrat amb un marge de 50px, un padding de 20px, i una vora de 5px amb un color de vora diferent.

---

## **6. Models de Caixa (Box Model)**

El model de caixa és un concepte fonamental que determina com es representen els elements a la pàgina. Inclou les propietats de `width`, `height`, `padding`, `border`, i `margin`.

### **Exemple:**

```css
div {
  width: 200px; /* Ample de l'element */
  height: 100px; /* Altura de l'element */
  padding: 10px; /* Espai intern */
  margin: 20px; /* Espai extern */
  border: 2px solid green; /* Vora */
}
```

### **Anàlisi:**
- El model de caixa determina l'espai ocupat per un element a la pàgina i com es relaciona amb altres elements. És important comprendre com cada propietat afecta l'espai total ocupat.
- Ajustar `box-sizing` a `border-box` pot simplificar l'estil, ja que el padding i la vora es consideren dins de les dimensions especificades.

### **Exercici 6:**
Experimenta amb la propietat `box-sizing: border-box;` i observa com afecta a la mida de l'element.

---

## **7. Layout amb Flexbox**

Flexbox és una tècnica moderna que facilita la creació de dissenys flexibles i responsius. Permet controlar la direcció, l'alineació i la distribució de l'espai entre els elements d'un contenidor.

### **Exemple:**

```css
.container {
  display: flex; /* Activa Flexbox */
  justify-content: center; /* Alinea els elements horitzontalment al centre */
  align-items: center; /* Alinea els elements verticalment al centre */
  height: 100vh; /* Altura del contenidor */
}
```

### **Anàlisi:**
- `flex-direction` controla la direcció dels elements (horitzontal o vertical), i `flex-wrap` determina si els elements han d'ajustar-se a la línia següent si no hi ha prou espai.
- Utilitzar Flexbox millora la distribució i l'alineació dels elements en diferents mides de pantalla.

### **Exercici 7:**
Crea una disposició amb tres caixes que estiguin distribuïdes de manera equitativa horitzontalment i verticalment, experimentant amb `justify-content` i `align-items`.

---

## **8. Estilització de Botons**

Els bot

ons són elements interactius clau que poden influir en la usabilitat i l'estètica d'una pàgina. És fonamental aplicar estils que els facin atractius i fàcils d'utilitzar.

### **Exemple de Botó:**

```css
button {
  background-color: blue; /* Color de fons */
  color: white; /* Color del text */
  border: none; /* Sense vora */
  padding: 10px 20px; /* Espai intern */
  cursor: pointer; /* Cursor de mà al passar sobre el botó */
  transition: background-color 0.3s; /* Transició suau per al canvi de color */
}

button:hover {
  background-color: darkblue; /* Color de fons al passar el cursor */
}
```

### **Anàlisi:**
- Els efectes de transició poden millorar la interactivitat dels botons i fer que l'experiència d'usuari sigui més agradable.
- Personalitzar els estils de botons pot millorar la seva visibilitat i facilitar l'accés a les funcions.

### **Exercici 8:**
Crea un botó amb efectes de transició que canviï de color al passar el cursor i experimenta amb les propietats `hover` i `focus`.

---
