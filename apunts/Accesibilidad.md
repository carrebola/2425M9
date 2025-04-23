# 🧭 Apuntes sobre Accesibilidad Web

## 🌐 Introducción

La accesibilidad web se refiere al diseño de sitios, aplicaciones y contenidos digitales que pueden ser utilizados por cualquier persona, en cualquier situación y con cualquier tecnología. No se trata solo de cumplir normas, sino de crear experiencias inclusivas que funcionen para la diversidad real de usuarios.

---

## 🌍 ¿Por qué es importante?

- **Diversidad de personas**: Todos navegamos de formas distintas: con teclado, con voz, con pantallas pequeñas, con poca conexión o en entornos ruidosos.
- **Diseño universal**: Un sitio accesible beneficia tanto a quienes usan lectores de pantalla como a quienes acceden desde un móvil bajo el sol o con una sola mano libre.
- **Mejora de la calidad**: Suele implicar código más limpio, mayor rendimiento y mejor usabilidad.
- **Cumplimiento normativo**: Muchas normativas exigen niveles mínimos de accesibilidad.
- **Reputación y alcance**: Se amplía el público y se refuerzan valores de inclusión y responsabilidad social.

---

## 🧱 Principios fundamentales (POUR)

1. **Perceptible**: La información y los componentes deben ser presentados de forma que puedan ser percibidos por los usuarios.
2. **Operable**: La interfaz debe poder usarse mediante diferentes métodos de entrada, como teclado o voz.
3. **Comprensible**: El contenido debe ser claro y la navegación predecible.
4. **Robusto**: El contenido debe ser compatible con diversas tecnologías, incluidas las de asistencia.

---

## 🧩 Buenas prácticas en el diseño accesible

- Usa **HTML semántico** para estructurar el contenido (`<main>`, `<section>`, `<nav>`, `<button>`, etc.).
- Incluye **texto alternativo** para imágenes y elementos gráficos.
- Asegura la **navegación por teclado**.
- **No dependas solo del color** para transmitir información.
- Garantiza **buen contraste** entre texto y fondo.
- Crea **interacciones predecibles y claras**.
- Proporciona **alternativas accesibles** para audio, vídeo y animaciones.
- Optimiza el diseño para **todo tipo de dispositivos y condiciones**.

---

## 📘 WCAG 2.2 – Pautas de Accesibilidad para el Contenido Web

Las WCAG (Web Content Accessibility Guidelines), desarrolladas por el W3C, ofrecen una guía internacional para lograr contenidos accesibles. La versión 2.2, publicada en octubre de 2023, añade nuevos criterios orientados a mejorar la experiencia de uso para personas con diversidad funcional cognitiva, motriz y tecnológica.

### 🪜 Niveles de conformidad

- **Nivel A**: requisitos básicos.
- **Nivel AA**: nivel recomendado para sitios públicos y comerciales.
- **Nivel AAA**: accesibilidad avanzada.

### 📋 Ejemplos por nivel (WCAG 2.2)

| Nivel | Criterio | Descripción |
|-------|----------|-------------|
| A     | 2.4.11 Enfoque no oculto | El foco del teclado debe ser visible. |
| A     | 3.2.6 Modo de entrada consistente | No cambiar entre métodos de entrada sin aviso. |
| AA    | 2.4.7 Enfoque visible | El foco debe ser evidente durante la navegación. |
| AA    | 2.5.7 Arrastrar accesible | Debe ofrecerse una alternativa al arrastre. |
| AA    | 2.5.8 Destino del puntero | Botones deben tener al menos 24x24 píxeles. |
| AAA   | 3.3.7 Mecanismo de ayuda | Debe existir asistencia disponible y constante. |

---

## 🛠 Herramientas para evaluar accesibilidad

- **Lighthouse**: Herramienta integrada en Chrome DevTools para auditar accesibilidad y rendimiento.
- **axe DevTools**: Extensión que identifica problemas según WCAG y sugiere soluciones.
- **WAVE**: Superpone indicadores de accesibilidad en la interfaz para su análisis visual.
- **WebAIM Contrast Checker**: Evalúa el contraste de color entre texto y fondo.
- **Lectores de pantalla**: NVDA, VoiceOver y JAWS permiten probar cómo se percibe el contenido sin vista.

---

## 📐 Normativas y estándares clave

- **WCAG 2.0 / 2.1 / 2.2** (W3C)
- **EN 301 549** (normativa europea para TIC)
- **Real Decreto 1112/2018** (España)

---

## 👥 Diversidad de personas, contextos y dispositivos

- Personas que usan teclado, comandos de voz o dispositivos adaptados.
- Navegación desde móviles con condiciones de luz o conexión adversas.
- Usuarios que necesitan ampliar texto o simplificar lenguaje.
- Contextos con ruido ambiental o limitaciones temporales de interacción.

---

## 🧪 Evaluación y diseño centrado en la diversidad

La accesibilidad requiere combinar herramientas automáticas con pruebas manuales y humanas. Considera siempre:

- Una **estructura semántica coherente**.
- **Interacciones claras y alcanzables sin ratón**.
- **Compatibilidad con tecnologías de asistencia**.

---

## 💻 Ejemplo de página HTML accesible

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Página Accesible</title>
</head>
<body>
  <header>
    <h1>Mi sitio web accesible</h1>
    <nav aria-label="Menú principal">
      <ul>
        <li><a href="#inicio">Inicio</a></li>
        <li><a href="#servicios">Servicios</a></li>
        <li><a href="#contacto">Contacto</a></li>
      </ul>
    </nav>
  </header>
  <main>
    <section id="inicio">
      <h2>Bienvenido</h2>
      <p>Este sitio está diseñado para ser usable por todos, sin importar el dispositivo o la situación.</p>
    </section>
    <section id="servicios">
      <h2>Servicios</h2>
      <ul>
        <li>Desarrollo web accesible</li>
        <li>Consultoría UX</li>
        <li>Auditoría de accesibilidad</li>
      </ul>
    </section>
    <section id="contacto">
      <h2>Contacto</h2>
      <form>
        <label for="nombre">Nombre:</label>
        <input type="text" id="nombre" name="nombre" required>

        <label for="email">Correo electrónico:</label>
        <input type="email" id="email" name="email" required>

        <label for="mensaje">Mensaje:</label>
        <textarea id="mensaje" name="mensaje"></textarea>

        <button type="submit">Enviar</button>
      </form>
    </section>
  </main>
  <footer>
    <p>&copy; 2025 Mi sitio accesible</p>
  </footer>
</body>
</html>
```

Este ejemplo aplica múltiples buenas prácticas alineadas con los principios WCAG 2.2:

- **HTML semántico** mejora la **perceptibilidad** y la **robustez**.
- **Etiquetas correctamente asociadas en formularios** mejoran la **comprensibilidad**.
- **Navegación por teclado** y uso de `aria-label` refuerzan la **operabilidad**.
- Se respeta la jerarquía de encabezados y se evita depender del color.

---

## 🏷️ Etiquetas y atributos HTML que mejoran la accesibilidad

### 📌 Etiquetas semánticas importantes
- `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`: Estructura clara.
- `<h1>` a `<h6>`: Jerarquía semántica del contenido.
- `<button>`: Elemento interactivo reconocido por lectores de pantalla.
- `<form>`, `<label>`, `<fieldset>`, `<legend>`: Formularios estructurados.
- `<ul>`, `<ol>`, `<li>`: Listas con significado.
- `<table>`, `<thead>`, `<tbody>`, `<caption>`, `<th>`: Tablas comprensibles.

### 📎 Atributos clave con ejemplos
- **`alt`**: Texto alternativo para imágenes.
  ```html
  <img src="grafico.png" alt="Gráfico de crecimiento trimestral">
  ```
- **`aria-label`**: Etiqueta textual directa.
  ```html
  <button aria-label="Cerrar ventana">X</button>
  ```
- **`aria-labelledby`**: Usa el contenido de otro elemento como etiqueta.
  ```html
  <h2 id="titulo-form">Contacto</h2>
  <form aria-labelledby="titulo-form">...</form>
  ```
- **`aria-describedby`**: Información complementaria para lectores de pantalla.
  ```html
  <input type="text" aria-describedby="ayuda">
  <small id="ayuda">Debe contener entre 6 y 12 caracteres.</small>
  ```
- **`role`**: Define propósito cuando no es evidente.
  ```html
  <div role="button" tabindex="0">Abrir menú</div>
  ```
- **`tabindex`**: Orden de navegación con teclado.
  ```html
  <a href="#" tabindex="0">Accesible</a>
  <div tabindex="-1">Enfocable manualmente</div>
  ```
- **`lang`**: Idioma del documento o fragmento.
  ```html
  <html lang="es">
  ```
- **`title`**: Información contextual adicional.
  ```html
  <abbr title="World Wide Web Consortium">W3C</abbr>
  ```
- **`required`, `disabled`, `readonly`**: Estado de campos de formulario.
  ```html
  <input type="email" required>
  <input type="text" disabled>
  ```

Estos elementos y atributos son esenciales para cumplir los principios de las WCAG y asegurar que el contenido sea accesible para todo tipo de usuarios y dispositivos.

---

## 📎 Anexo: Pautas WCAG 2.2 organizadas por principios

### 🔍 Perceptible
- **1.1.1 Contenido no textual** (A): Proporcionar texto alternativo.
- **1.2.1 Solo audio y solo vídeo (pregrabado)** (A): Ofrecer alternativa textual o descripción.
- **1.2.2 Subtítulos (pregrabado)** (A): Subtítulos para contenido con audio.
- **1.3.1 Información y relaciones** (A): Usar marcado semántico para transmitir estructura.
- **1.3.2 Secuencia significativa** (A): Presentar contenido en orden lógico.
- **1.3.3 Características sensoriales** (A): No depender únicamente de color, forma o posición.
- **1.4.3 Contraste (mínimo)** (AA): Ratio mínimo de 4.5:1 para texto.
- **1.4.10 Reflujo** (AA): Contenido visible sin pérdida de funcionalidad al hacer zoom.

### 🖱️ Operable
- **2.1.1 Teclado** (A): Todo debe ser accesible mediante teclado.
- **2.1.2 Sin trampas de teclado** (A): No atrapar al usuario con el teclado.
- **2.4.1 Evitar bloques** (A): Permitir saltar bloques repetitivos.
- **2.4.3 Orden del foco** (A): Orden lógico de navegación.
- **2.4.4 Propósito de los enlaces** (A): Texto del enlace debe indicar su destino.
- **2.4.6 Encabezados y etiquetas** (AA): Encabezados claros y útiles.
- **2.4.7 Enfoque visible** (AA): El foco debe ser visible.
- **2.5.1 Gestos del puntero** (A): Evitar gestos complejos como deslizamientos.
- **2.5.7 Arrastrar accesible** (AA): Ofrecer método alternativo a arrastrar.
- **2.5.8 Destino del puntero** (AA): Área clicable mínima de 24x24 px.

### 🧠 Comprensible
- **3.1.1 Idioma de la página** (A): Especificar el idioma principal.
- **3.2.1 Al enfocar** (A): No cambiar contexto automáticamente.
- **3.3.1 Identificación de errores** (A): Identificar campos con errores.
- **3.3.2 Etiquetas e instrucciones** (A): Proporcionar instrucciones claras.
- **3.3.3 Sugerencias ante errores** (AA): Propuestas para resolver errores.
- **3.3.7 Mecanismo de ayuda** (AAA): Acceso constante a ayuda o soporte.

### ⚙️ Robusto
- **4.1.1 Análisis** (A): Código correctamente estructurado.
- **4.1.2 Nombre, función, valor** (A): Controles y formularios accesibles a tecnologías de asistencia.
- **4.1.3 Estado actualizado** (AA): Cambios de estado comunicados de forma accesible.

---

## 🧠 Conclusión

Diseñar para la accesibilidad es diseñar para la diversidad real del mundo. No se trata solo de cumplir con estándares, sino de crear experiencias justas, sostenibles y centradas en las personas.

