# GAITEX — Web bilingüe

Primera muestra de la web de GAITEX, con seis páginas independientes y selector Español / English. Proyecto estático en HTML, CSS y JavaScript; no necesita npm, compilación, servidor de aplicaciones ni servicios de Sites para publicarse.

## Archivos

| Archivo | Contenido |
| --- | --- |
| `index.html` | Inicio breve y accesos a las secciones |
| `nosotros.html` | Presentación y alcance del full package |
| `productos.html` | Prendas y materiales |
| `proceso.html` | Recorrido interactivo y plazo de referencia |
| `destinos.html` | Destinos internacionales |
| `contacto.html` | Formulario de solicitud |
| `style.css` | Colores, tipografías y diseño adaptable |
| `app.js` | Textos en ambos idiomas, navegación e interacciones |
| `assets/` | Logo y fotografías de referencia |
| `.nojekyll` | Publicación estática sin procesamiento Jekyll |

## 1. Subir el proyecto a GitHub desde el navegador

1. Descomprime `GAITEX-web-GitHub.zip` en tu computadora.
2. Inicia sesión en [GitHub](https://github.com).
3. Haz clic en **+ → New repository**. Nombre sugerido: `gaitex-web`.
4. Elige la visibilidad. Para usar GitHub Pages con GitHub Free, utiliza un repositorio **Public**: el código será visible. Un repositorio privado puede servir para guardar el trabajo, pero Pages en repositorios privados requiere un plan compatible.
5. Marca **Add a README file** y pulsa **Create repository**.
6. Dentro del repositorio, selecciona **Add file → Upload files**.
7. Arrastra el CONTENIDO de la carpeta extraída: los HTML, `app.js`, `style.css`, `assets/` y los archivos de documentación. No subas el ZIP ni una carpeta adicional que encierre toda la web. Se puede reemplazar el README inicial por el incluido aquí.
8. Escribe un mensaje como `Primera versión de GAITEX` y confirma los cambios en `main`. Si GitHub propone una rama nueva, abre y fusiona el pull request para incorporar los archivos a `main`.
9. Comprueba que `index.html` esté en la raíz, al mismo nivel que `README.md`, y que las imágenes estén dentro de `assets/`.

Los archivos que empiezan por punto pueden estar ocultos en Windows. El ZIP incluye `.nojekyll`; si no se subió, puedes crearlo desde **Add file → Create new file**, nombrarlo `.nojekyll` y guardar una línea vacía. `.gitignore` es opcional para la publicación.

Con esto, el código ya está guardado en tu cuenta. Activar la web es un paso separado.

## 2. Publicar con GitHub Pages

1. En el repositorio, abre **Settings → Pages**.
2. En **Build and deployment → Source**, elige **Deploy from a branch**.
3. Selecciona **main** y **/(root)**; pulsa **Save**.
4. Espera a que termine la publicación. Revisa **Actions** si aparece un error. Después, vuelve a **Settings → Pages** para encontrar el enlace del sitio.
5. Si el repositorio se llama `gaitex-web`, la dirección habitual será `https://TU-USUARIO.github.io/gaitex-web/`. Sustituye `TU-USUARIO` por tu nombre de usuario; GitHub mostrará la dirección definitiva.

Al activar Pages, la web será accesible públicamente. Esta versión no utiliza el acceso privado de la muestra alojada en Sites.

## 3. Continuar trabajando

- **Textos:** los textos visibles se cargan desde los objetos `es` y `en` de `app.js`, incluidos los bloques `Object.assign`. Cambia ambos idiomas. Editar solo un texto marcado con `data-i18n` en el HTML no modifica su traducción cargada al abrir la web.
- **Estructura:** edita el HTML de la página correspondiente. El encabezado y el pie se repiten en cada HTML; si modificas el menú, actualízalo en las seis páginas.
- **Diseño:** edita `style.css`. Los colores principales están definidos en `:root`.
- **Fotografías:** reemplaza las imágenes de `assets/` y ajusta rutas y textos alternativos cuando corresponda.
- **Cambios posteriores:** sube los archivos modificados a `main`; Pages vuelve a publicar los cambios automáticamente.
- **Desarrollo local:** abre la carpeta en tu editor. Si tienes Python instalado, ejecuta `python -m http.server 8000` desde esa carpeta y visita `http://localhost:8000`. Ctrl+C detiene el servidor. También puedes usar Live Server en VS Code.

## Estado del prototipo

- Fotografías provisionales; reemplazarlas por imágenes propias antes de la versión final.
- Correo y teléfono comercial pendientes de confirmar.
- El formulario valida los campos y descarga una solicitud `.txt`. No envía correos ni almacena pedidos. El envío real requiere conectar un servicio o backend.
- El recorrido muestra el proceso; no consulta estados reales de pedidos.
- Los 90 días son un plazo de referencia desde la recepción de la orden de compra, sujeto a las características y condiciones del pedido.
- Las fuentes se cargan desde Google Fonts, con tipografías de respaldo si no están disponibles.

## Recursos visuales

Logo proporcionado por GAITEX. Fotografías provisionales obtenidas de Unsplash:

- [Referencia de prenda tejida](https://images.unsplash.com/photo-1434389677669-e08b4cac3105)
- [Referencia de camiseta](https://images.unsplash.com/photo-1576566588028-4147f3842f27)

No se atribuyen estas prendas a GAITEX ni se afirma que la referencia tejida sea baby alpaca.

## Documentación oficial

- [Subir archivos a un repositorio](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)
- [Configurar la publicación de GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
- [Qué es GitHub Pages y planes compatibles](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages)
