# **Barra de progreso con el scroll**

Este código crea una animación que muestra una **barra de progreso en la parte superior de la pantalla** y que se llena conforme el usuario hace scroll. También incluye un efecto de aparición en elementos cuando entran en pantalla.

---

### **📌 Explicación por secciones**

#### **1️⃣ Estilos Generales**
```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
}
```
✔ Define una fuente base.  
✔ Elimina márgenes y padding para una mejor estructura.  
✔ Usa `display: flex` para centrar el contenido.  

---

#### **2️⃣ Espaciador para el Scroll**
```css
.spacer {
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 24px;
    color: #555;
}
```
✔ **Hace que la página sea más larga**, generando un scroll necesario para ver el efecto.  
✔ `height: 100vh;` ocupa toda la altura de la ventana del navegador.  
✔ `display: flex;` centra el texto en el espacio.  

---

#### **3️⃣ Animación de elementos que entran en pantalla**
```css
.animado {
    opacity: 0;
    transform: translateY(50px);
    transition: opacity 0.6s ease-out, transform 0.6s ease-out;
}
```
✔ **Los elementos inician ocultos** (`opacity: 0`).  
✔ `transform: translateY(50px);` los mueve 50px hacia abajo.  
✔ `transition: opacity 0.6s, transform 0.6s;` hace que la animación sea suave.  

Cuando un elemento entra en pantalla, se activa esta regla:
```css
.animado.visible {
    opacity: 1;
    transform: translateY(0);
}
```
✔ Hace que el elemento **aparezca gradualmente** (`opacity: 1`).  
✔ Lo mueve a su posición original (`translateY(0)`).  

---

#### **4️⃣ Barra de Progreso (Scroll)**
```css
.progress-bar {
    position: fixed;
    top: 0;
    left: 0;
    width: 0;
    height: 5px;
    background-color: #3498db;
    animation: progressAnimation linear;
    animation-timeline: scroll();
}
```
✔ `position: fixed;` la mantiene siempre en la parte superior.  
✔ `width: 0;` inicia vacía.  
✔ `height: 5px;` establece el grosor de la barra.  
✔ `background-color: #3498db;` le da color azul.  
✔ `animation: progressAnimation linear;` usa la animación para cambiar el ancho.  
✔ `animation-timeline: scroll();` **hace que la animación avance con el scroll**.

---

#### **5️⃣ Animación de la Barra de Progreso**
```css
@keyframes progressAnimation {
    from {
        width: 0;
    }
    to {
        width: 100%;
    }
}
```
✔ **Anima el ancho de la barra** desde `0%` hasta `100%`.  
✔ Como `animation-timeline: scroll();`, la animación avanza a medida que el usuario hace scroll.  

---

### **🚀 Resultado Final**
1️⃣ La barra de progreso **se llena automáticamente** al hacer scroll.  
2️⃣ Los elementos `.animado` **aparecen con animación** cuando entran en pantalla.  
3️⃣ Todo está hecho **solo con CSS** sin necesidad de JavaScript.  

📌 **Si necesitas ajustes o mejoras, dime! 😊**
