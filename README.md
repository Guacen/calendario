# Adviento de Andrea

App web de un solo archivo para el calendario de adviento de 14 cajitas: carta de Papá Noel, etiqueta para raspar y 14 cajitas que se pueden abrir cuando ella quiera y en cualquier orden. Cada cajita guarda la fecha en que se abrió, foto, comentario, calificación, "ya lo probé" y favorito, y la bitácora se puede exportar.

- Publicada en GitHub Pages: `https://guacen.github.io/calendario/`
- Los datos se guardan solo en el celular (IndexedDB). Nada sale del teléfono salvo el archivo que se exporte.

## Editar textos

Todo está en el bloque `CONFIG`, al inicio del `<script>` de `index.html`: nombre, firma, guía, cartas de Jorge y mensajes de Papá Noel.

Los mensajes siguen el orden en que ella abre las cajitas, no el número de la cajita: la 1.ª, la 7.ª (`cartaMitad`) y la 14.ª que abra traen carta de Jorge, y las demás traen mensaje de Papá Noel.

Si cambias `index.html`, sube también la versión del caché en `sw.js` (por ejemplo `adviento-v2` → `adviento-v3`) para que el celular reciba el cambio.

## Probar sin tocar la bitácora real

`?prueba` guarda en una base de datos aparte, así que lo que hagas ahí no se mezcla con la bitácora de verdad.
