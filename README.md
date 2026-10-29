# GAITEX — Sitio completo con diseño unificado

Las seis páginas comparten el diseño aprobado: verde oliva, composición clara, elementos textiles, tipografía DM Sans, navegación redondeada, selector Español / English y pie de página común.

## Subir esta actualización a GitHub

1. Descomprime `GAITEX-sitio-unificado.zip`.
2. En el repositorio `gaitex-web`, entra en **Add file → Upload files**.
3. Arrastra TODOS los archivos de la carpeta descomprimida, sin una carpeta contenedora. Reemplaza los archivos con los mismos nombres.
4. Guarda con **Commit changes** en `main`.
5. Espera a que la publicación de Pages termine en verde. Abre la web y pulsa Ctrl+F5 si fuera necesario.

Todo está al mismo nivel: los seis HTML, `style.css`, `app.js`, `logo.png`, `hero.jpg`, `knit.jpg` y el nuevo fondo `textile-desktop.jpg`. No es necesario crear ni subir una carpeta `assets`. Los HTML incluyen un identificador de versión en las rutas de CSS y JavaScript para evitar cargar versiones anteriores guardadas en el navegador.

No necesitas borrar otros archivos del repositorio. Cada HTML carga exclusivamente el nuevo `style.css` y el nuevo `app.js`.

## Contenido y funciones conservadas

- Inicio, Nosotros, Productos, Proceso, Destinos y Contacto son páginas independientes.
- El idioma se conserva durante la navegación y puede cambiarse en cada página.
- Materiales: algodón pima, jersey, piqué y baby alpaca; evaluación de otras propuestas de tela.
- Proceso interactivo de cuatro etapas y lead time de referencia de 90 días desde la recepción de la orden de compra, sujeto a las características y condiciones del pedido.
- Destinos internacionales existentes.
- Formulario con nombre, apellido, correo y mensaje, validación de campos y descarga de consulta TXT. No se ha conectado un servicio de envío; no se confirma ningún envío a GAITEX.

## Verificación

Se visitaron las seis páginas en español e inglés, en escritorio de 1440 px y celular de 390 px. También se comprobó el ancho de 320 px en inglés. No se detectaron desbordamientos horizontales, imágenes faltantes o traducciones indefinidas.

Se comprobaron el encabezado y pie comunes, la fuente DM Sans en todas las páginas, las cuatro etapas en ambos idiomas, la validación del formulario, las descargas en ambos idiomas y la conservación de campos al cambiar de idioma. No hubo errores de consola durante las pruebas.

## Editar el sitio

- `style.css`: todo el diseño, tipografía, colores y adaptación móvil.
- `app.js`: textos en español e inglés e interacciones. Los textos del inicio tienen claves que empiezan por `h_`.
- Cada HTML: estructura de su página. Si cambias los enlaces del menú o el pie, actualiza las seis páginas.
- Las imágenes están en la raíz del proyecto. El fondo textil decorativo es conceptual y fue generado con IA; no representa instalaciones ni mercancía real de GAITEX.

No se necesitan npm, compilación ni dependencias de ejecución. Las fuentes se cargan desde Google Fonts, con respaldo Arial/sans-serif.
