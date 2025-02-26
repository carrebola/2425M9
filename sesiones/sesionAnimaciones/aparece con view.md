# Animar elemento al entrar en en la pantalla

Para lograr que un elemento se anime al entrar en pantalla de manera eficiente y con amplio soporte en navegadores modernos, la solución más recomendada es utilizar la **API de Intersection Observer** en combinación con animaciones CSS. Esta API permite detectar cuándo un elemento entra o sale del viewport, desencadenando acciones específicas, como iniciar una animación.

### **Implementación con Intersection Observer y CSS**

A continuación, se presenta un ejemplo práctico de cómo implementar esta funcionalidad:

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animación al entrar en pantalla</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .spacer {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
            color: #555;
        }
        .animado {
            opacity: 0;
            transform: translateY(50px);
            transition: opacity 0.6s ease-out, transform 0.6s ease-out;
        }
        .animado.visible {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>

    <div class="spacer">Desplázate hacia abajo</div>

    <div class="animado">
        <h2>Contenido animado</h2>
        <p>Este contenido aparecerá con una animación al entrar en pantalla.</p>
    </div>

    <div class="spacer">Fin del contenido</div>

    <script>
        document.addEventListener("DOMContentLoaded", function() {
            const elementos = document.querySelectorAll('.animado');

            const opciones = {
                root: null, // Observa respecto al viewport
                rootMargin: '0px',
                threshold: 0.1 // El 10% del elemento visible
            };

            const callback = (entradas, observador) => {
                entradas.forEach(entrada => {
                    if (entrada.isIntersecting) {
                        entrada.target.classList.add('visible');
                        observador.unobserve(entrada.target); // Deja de observar el elemento
                    }
                });
            };

            const observer = new IntersectionObserver(callback, opciones);

            elementos.forEach(elemento => {
                observer.observe(elemento);
            });
        });
    </script>

</body>
</html>
```

### **Explicación del Código**

1. **HTML**: Se estructura la página con un espacio antes y después del contenido animado para permitir el desplazamiento.

2. **CSS**:
   - `.animado`: Define el estilo inicial del elemento, ocultándolo con `opacity: 0` y desplazándolo hacia abajo con `transform: translateY(50px)`.
   - `.animado.visible`: Estilo aplicado cuando el elemento es visible, estableciendo `opacity: 1` y `transform: translateY(0)` para mostrarlo y posicionarlo correctamente.

3. **JavaScript**:
   - Se utiliza `IntersectionObserver` para observar los elementos con la clase `.animado`.
   - Cuando un elemento entra en el viewport (al menos un 10% visible), se le añade la clase `visible` y se deja de observar para evitar que la animación se repita.

### **Compatibilidad de Navegadores**

La API de Intersection Observer es compatible con la mayoría de los navegadores modernos, incluyendo Chrome, Firefox, Edge y Safari. Para obtener información detallada sobre la compatibilidad, puedes consultar la documentación de [MDN Web Docs](https://developer.mozilla.org/es/docs/Web/API/Intersection_Observer_API).

### **Conclusión**

Utilizar la API de Intersection Observer junto con animaciones CSS es una forma moderna y eficiente de animar elementos al entrar en pantalla, garantizando una amplia compatibilidad y un rendimiento óptimo en navegadores actuales. 
