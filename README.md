# Presentación: Servicio al Cliente Cara a Cara

Presentación web en una sola página (`index.html`) sobre estrategias de atención personalizada y CRM.

## Contenido

- 16 diapositivas con navegación tipo presentación.
- Diseño responsive para escritorio y móvil.
- Animaciones visuales, tarjetas, tablas y módulos temáticos.

## Cómo usar

1. Abre `index.html` en tu navegador.
2. Navega entre paneles con:
   - Botones `←` y `→`
   - Teclado: `ArrowLeft`, `ArrowRight`, `Espacio`, `Home`, `End`
   - Toque (swipe) en dispositivos móviles
3. El scroll vertical se usa para desplazarte dentro de las diapositivas largas (no cambia de panel con la rueda del mouse).
4. **Exportar**: las opciones de exportación están ocultas y sólo accesibles para el autor mediante una contraseña. Para mayor seguridad:
   - la clave nunca se guarda en texto claro; se compara su SHA‑256 con un hash almacenado en el script.
   - tras introducirla (combinación `Ctrl+Shift+E`), el estado se guarda en `sessionStorage` y las opciones permanecen visibles hasta que se cierra el navegador.
   - 🖨️ guarda la presentación como PDF vía la impresión del navegador.
   - 📄 genera un archivo PowerPoint (`.pptx`) que ahora procesa **todas las diapositivas** y vuelve a la slide original al terminar. Si el PPTX no funciona bien, revisa la consola para posibles errores; el script intentará cargar dinámicamente `html2canvas` si no está disponible.
   - 🖼️ descarga una **imagen PNG de la página completa** (body) con un solo clic. Este proceso también depende de `html2canvas`; si no hay conexión a CDN el botón mostrará un error en consola.
   
> ⚠️ **Sin red**: el repositorio ya incluye `html2canvas.min.js` en la raíz, así que las exportaciones funcionan sin conexión. Si actualizas la versión o quieres usar otra, reemplaza ese archivo. En caso de que lo borres, el script intentará recuperar la librería desde el CDN.

   (Cambia el hash o la clave dentro de la sección de scripts según prefieras.)

> 🔒 **Protección de URLs:** La diapositiva de cierre no muestra las direcciones completas; cada referencia aparece como un icono clicable. Si necesitas modificar este comportamiento, edita el CSS dentro de la sección `/* ===== CLOSING ===== */` en `index.html`.

## Presentadores

- Yudy Vanessa Martinez Leguizamon
- Jhonatan David Martinez Ramirez

## Estructura del proyecto

- `index.html`: contiene estilos, contenido y scripts de navegación.

## Personalización rápida

- Cambiar título de portada: busca `cover-title`.
- Cambiar subtítulo: busca `cover-sub`.
- Cambiar nombres de presentadores: busca `cover-presenters`.
- Ajustar cantidad total de paneles: se calcula automáticamente según los elementos `.slide`.
- Modificar comportamiento de enlaces de cierre: revisa estilos bajo la sección `/* ===== CLOSING ===== */` para cambiar icono o mostrar texto.

## Requisitos

- Navegador moderno (Chrome, Edge, Firefox, Safari).
- No requiere instalación de dependencias ni servidor.
