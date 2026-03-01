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
4. **Exportar**: las opciones de exportación están ocultas y sólo accesibles para el autor mediante una contraseña.
   - Presiona `Ctrl+Shift+E` y escribe la contraseña correcta para mostrar los botones.
   - 🖨️ guarda la presentación como PDF vía la impresión del navegador.
   - 📄 genera y descarga un archivo PowerPoint (`.pptx`) con cada slide convertido en imagen.
   (La contraseña actual está codificada en el script; cámbiala si es necesario.)

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
