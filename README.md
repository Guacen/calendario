# Adviento de Andrea

App web de un solo archivo para el calendario de adviento de 14 cajitas: carta de Papá Noel, elección de fecha de inicio (11 o 15 de diciembre), una cajita por día con foto, comentario, calificación, "ya lo probé" y favorito, y exportación de la bitácora.

- Publicada en GitHub Pages: `https://guacen.github.io/calendario/`
- Los datos se guardan solo en el celular (IndexedDB). Nada sale del teléfono salvo el archivo que se exporte.

## Editar textos

Todo está en el bloque `CONFIG`, al inicio del `<script>` de `index.html`: nombre, firma, guía, mensajes de Jorge (primer día, Nochebuena, último día) y mensajes de Papá Noel por fecha.

Si cambias `index.html`, sube también la versión del caché en `sw.js` (`adviento-v1` → `adviento-v2`) para que el celular reciba el cambio.

## Probar sin tocar la bitácora real

- `?prueba` abre todas las cajitas y guarda en una base aparte.
- `?prueba&hoy=2026-12-24` simula una fecha.
