
![image](https://github.com/user-attachments/assets/6138aa96-a997-46fd-8b0d-253ea5289308)

### Enunciat: Creació d'una pàgina web futbolística amb Bootstrap 5

L'objectiu d'aquest exercici és construir una pàgina web temàtica de futbol utilitzant diversos conceptes i elements de Bootstrap 5. Cada pas se centra en un concepte o element nou. Segueix els passos per completar la pàgina.

---

### **Pas 1: Estructura inicial del document HTML**

1. **Crea l’estructura base de l’HTML**: Afegeix les etiquetes necessàries (`<!DOCTYPE html>`, `<html>`, `<head>`, `<body>`), incloent els enllaços per Bootstrap i defineix la informació de metadades.

---

### **Pas 2: Afegir un encapçalament**

1. **Inclou una etiqueta `<header>`** dins del cos de la pàgina amb la classe per donar-li un estil de fons verd i text blanc (`bg-success` i `text-white`).
2. Centra el contingut dins de l'encapçalament utilitzant la classe `text-center`.

---

### **Pas 3: Crear una barra de navegació (Navbar)**

1. **Utilitza l'etiqueta `<nav>`** amb les classes `navbar`, `navbar-expand-lg`, i `bg-light` per crear la barra de navegació.
2. Afegeix un contenidor fluid i crea una llista de navegació amb les classes `navbar-nav` per als enllaços dins de la barra.

---

### **Pas 4: Crear una secció amb targetes utilitzant el sistema de graelles (Grid System)**

1. **Afegeix una secció amb l'etiqueta `<main>`** i utilitza el sistema de graelles de Bootstrap (`container` i `row`).
2. Crea **tres columnes** utilitzant les classes `col-md-4` i dins de cada columna afegeix una **targeta** (`card`) que inclogui una imatge (`card-img-top`), un títol (`card-title`) i un text (`card-text`).

---

### **Pas 5: Crear un formulari amb estils de Bootstrap**

1. Afegeix un **formulari** dins de l'etiqueta `<main>`, utilitzant la classe `form-control` per als camps de text i la classe `btn` per al botó d'enviament.
2. Afegeix classes com `border`, `shadow` i `p-3` per afegir estils addicionals al formulari com marges, ombres i espaiat.

---

### **Pas 6: Afegir un modal per mostrar informació del pròxim partit**

1. Crea un **botó** dins del formulari amb les classes `btn` i `btn-secondary` que obri un **modal**.
2. Defineix l’estructura del modal amb les etiquetes corresponents (`<div>`) i afegeix les classes `modal`, `modal-dialog`, `modal-content`, `modal-header`, etc.

---

### **Pas 7: Afegir una alerta de Bootstrap**

1. Afegeix una **alerta** just sota el formulari utilitzant l'etiqueta `<div>` i la classe `alert`.
2. Personalitza l'alerta amb la classe `alert-warning` per indicar una notificació important (per exemple, sobre el davanter que ha marcat 100 gols).

---

### **Pas 8: Crear un peu de pàgina (Footer)**

1. Afegeix un **peu de pàgina** (`<footer>`) amb la classe `bg-light` i centra el text utilitzant `text-center`.
2. Inclou un missatge de copyright dins del peu de pàgina.

---

### **Pas 9: Revisar la pàgina i afegir scripts de Bootstrap**

1. Afegeix els **scripts de Bootstrap** al final de la pàgina, abans de tancar l'etiqueta `<body>`, per assegurar que totes les funcionalitats (com el modal) funcionin correctament.

--- 
