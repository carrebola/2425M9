# **Barra de progreso con el scroll**

Este código crea una animación que muestra una **barra de progreso en la parte superior de la pantalla** y que se llena conforme el usuario hace scroll. También incluye un efecto de aparición en elementos cuando entran en pantalla.
```html
<!DOCTYPE html>
<html lang="es">
	<head>
		<meta charset="UTF-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<title>Animación al hacer Scroll</title>
		<style>
			/* Estilos generales para el cuerpo de la página */
			body {
				font-family: Arial, sans-serif;
				margin: 0;
				padding: 0;
				display: flex;
				flex-direction: column;
				align-items: center;
			}

			/* Espaciador para forzar el desplazamiento y probar la animación */
			.spacer {
				height: 100vh;
				display: flex;
				align-items: center;
				justify-content: center;
				font-size: 24px;
				color: #555;
			}

			/* Elementos animados que aparecen al hacer scroll */
			.animado {
				background-color: brown;
				color: white;
				opacity: 0;
				transform: translateY(50px);
				transition: opacity 0.6s ease-out, transform 0.6s ease-out;
			}

			/* Clase aplicada cuando el elemento entra en pantalla */
			.animado.visible {
				opacity: 1;
				transform: translateY(0);
			}

			/* Barra de progreso en la parte superior de la página */
			.progress-bar {
				position: fixed;
				top: 0;
				left: 0;
				width: 0;
				height: 5px;
				background-color: #3498db;
				/* Usa una animación basada en el desplazamiento */
				animation: progressAnimation linear;
				animation-timeline: scroll();
			}

			/* Definición de la animación para la barra de progreso */
			@keyframes progressAnimation {
				from {
					width: 0;
				}
				to {
					width: 100%;
				}
			}
		</style>
	</head>
	<body>
		<!-- Barra de progreso que se llenará con el scroll -->
		<div class="progress-bar"></div>

		<!-- Espaciador inicial para probar el desplazamiento -->
		<div class="spacer">Desplázate hacia abajo</div>

		<!-- Elemento que se animará al entrar en pantalla -->
		<div class="animado">
			<h2>Contenido animado</h2>
			<p>Este contenido aparecerá con una animación al entrar en pantalla.</p>
		</div>

		<!-- Espaciador final para extender la página -->
		<div class="spacer">Fin del contenido</div>

		<script>
			document.addEventListener("DOMContentLoaded", function () {
				const elementos = document.querySelectorAll(".animado");

				const opciones = {
					root: null, // Observa respecto al viewport
					rootMargin: "0px",
					threshold: 0.1, // El 10% del elemento visible
				};

				const callback = (entradas, observador) => {
					entradas.forEach((entrada) => {
						if (entrada.isIntersecting) {
							entrada.target.classList.add("visible");
							observador.unobserve(entrada.target); // Deja de observar el elemento
						}
					});
				};

				const observer = new IntersectionObserver(callback, opciones);

				elementos.forEach((elemento) => {
					observer.observe(elemento);
				});
			});
		</script>
	</body>
</html>

```
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
