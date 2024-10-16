# **Tutorial para Crear un Portfolio con Bootstrap 5**

En este tutorial, te guiaré paso a paso para crear un sitio web tipo portfolio utilizando **Bootstrap 5**. A medida que avancemos, te explicaré cómo utilizar las clases de Bootstrap para crear un sitio moderno, responsivo y atractivo. ¡Vamos a empezar!



### 1. Crear la Estructura Básica del Proyecto

Primero, necesitas crear un archivo HTML llamado `index.html`. Este archivo debe tener la estructura básica de HTML, incluyendo enlaces a los archivos CSS y JavaScript de Bootstrap 5. Esto te permitirá utilizar todos los estilos y componentes de Bootstrap sin problemas. Asegúrate de incluir las etiquetas `<meta>` para la codificación de caracteres y para hacer que la página sea responsiva en todos los dispositivos.

### 2. Crear la Barra de Navegación

A continuación, debes añadir una barra de navegación en la parte superior de la página. Esta barra de navegación debe ser responsiva y estar estilizada con un fondo oscuro. Utiliza clases como `navbar`, `navbar-expand-lg` para crear una barra de navegación que se expanda en dispositivos grandes y colapse en dispositivos más pequeños. Usa `navbar-dark` y `bg-dark` para un estilo oscuro.

La barra de navegación debe contener enlaces a las diferentes secciones de tu página (Inici, Sobre Mi, Projectes, Galeria, Contacte). También debes incluir un botón de alternar (`navbar-toggler`) que permita mostrar u ocultar los enlaces en pantallas pequeñas.

### 3. Sección de Presentación (Hero Section)

La sección de presentación debe captar la atención del visitante. Utiliza un contenedor que incluya un encabezado principal con un mensaje de bienvenida, un párrafo de descripción y un botón de llamada a la acción. La sección debe tener un fondo atractivo con una imagen de gran tamaño que ocupe todo el ancho disponible, utilizando clases como `bg-dark`, `text-white`, y `py-5` para agregar un padding vertical.

El texto debe estar centrado (`text-center`) y debes usar clases como `display-4` para el encabezado y `lead` para el párrafo de descripción. El botón de llamada a la acción debe utilizar la clase `btn btn-warning` para destacar.

### 4. Sección "Sobre Mi"

La sección "Sobre Mi" debe proporcionar información sobre ti y tus habilidades. Utiliza el sistema de rejilla de Bootstrap (`container`, `row`, `col-md-4`, `col-md-8`) para organizar la sección en dos columnas: una para tu imagen y otra para el texto descriptivo.

La imagen debe ser responsiva (`img-fluid`) y tener un borde redondeado (`rounded-circle`) para darle un aspecto más amigable. Utiliza un contenedor con fondo claro (`bg-light`), un padding (`p-5`), y un borde redondeado (`rounded-3`) para mejorar el diseño y la presentación.

### 5. Sección de Proyectos

En la sección de proyectos, debes mostrar una serie de tarjetas que representen los proyectos que has desarrollado. Utiliza el componente `card` de Bootstrap para crear estas tarjetas. Cada tarjeta debe incluir una imagen en la parte superior, un título, una descripción breve del proyecto, y un botón que permita al usuario ver más detalles.

Usa el sistema de rejilla (`row`, `col-md-4`) para organizar las tarjetas y asegúrate de que todas tengan la misma altura utilizando la clase `h-100`. Cada tarjeta debe tener una sombra sutil (`shadow-sm`) para destacar visualmente.

### 6. Galería de Fotos

La galería de fotos debe mostrar una serie de imágenes con enlaces a versiones más grandes de las mismas. Utiliza el sistema de rejilla (`row`, `col-md-4`) para organizar las imágenes en columnas. Las imágenes deben ser responsivas (`img-fluid`) y estar estilizadas con bordes redondeados (`rounded`) y una sombra (`shadow-sm`).

Cada imagen debe estar envuelta en un enlace (`<a>`) que apunte a una versión de mayor resolución para que los usuarios puedan ver más detalles. Asegúrate de incluir el atributo `target="_blank"` para que los enlaces se abran en una nueva pestaña.

### 7. Sección de Contacto

La sección de contacto debe incluir un formulario que permita a los visitantes comunicarse contigo. Utiliza componentes de formulario de Bootstrap (`form`, `form-control`) para crear campos de entrada para el nombre, correo electrónico, y un área de texto para el mensaje.

Cada campo de entrada debe estar estilizado con una clase de sombra sutil (`shadow-sm`) y el botón de enviar debe utilizar la clase `btn btn-warning` para destacar. Además, el botón debe ocupar todo el ancho del formulario (`w-100`) para que sea más fácil de interactuar en dispositivos móviles.

### 8. Footer (Pie de Página)

El pie de página debe incluir información adicional sobre ti y enlaces a tus redes sociales. Utiliza el sistema de rejilla (`container`, `row`, `col-lg-4`, `col-md-6`) para organizar el contenido en diferentes columnas.

Debes incluir una columna con una breve descripción sobre ti, otra con enlaces a las diferentes secciones de la página, y una última columna con iconos de redes sociales (Facebook, Twitter, Instagram, LinkedIn). Utiliza las clases `bg-dark`, `text-white`, y `p-4` para darle un estilo atractivo y consistente con el resto del sitio.



