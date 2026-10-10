# Puerto Madryn en 8 días — Guía interactiva (PWA)

Guía de viaje instalable: itinerario día por día (llegada de tarde el día 1, salida de tarde el último día), mapa, clima, fauna según la fecha, historia, tips y checklist offline. Configurable de 6 a 8 días desde ⚙️.

## Estructura

```
index.html      → la app completa
manifest.json   → metadata de la PWA (nombre, ícono, colores)
sw.js           → service worker para funcionamiento offline
icon-192.svg    → ícono chico
icon-512.svg    → ícono grande
```

## Deploy en GitHub Pages (gratis, 5 minutos)

1. Creá un repo nuevo en GitHub, por ejemplo `puerto-madryn-8-dias`.
2. Subí estos 5 archivos a la raíz del repo (no en una subcarpeta).
3. Andá a **Settings → Pages**.
4. En "Source" elegí la rama `main` y carpeta `/ (root)`. Guardá.
5. La URL queda en: `https://TU-USUARIO.github.io/puerto-madryn-8-dias/`

## Instalar como app

- **Android (Chrome)**: menú ⋮ → "Instalar app" / "Agregar a pantalla de inicio".
- **iPhone (Safari)**: compartir (□↑) → "Agregar a pantalla de inicio".

Las fotos (Wikimedia Commons), el mapa y el clima necesitan internet la primera vez que se cargan; después quedan en caché.

## Actualizar contenido

Los datos están en `BLOCKS` (días), `FAUNA`, `EXTRAS`, `TIPS`, `CHECKLIST_ITEMS` e `HISTORIA` dentro del `<script>` de `index.html`. Si cambiás archivos del app shell, subí la versión de `CACHE_NAME` en `sw.js` (`madryn-8dias-v1` → `v2`).

## Notas

- Las coordenadas de algunos puntos son aproximadas; confirmá horarios, precios y mareas antes de salir.
- El calendario de fauna es general: la presencia de ballenas, orcas y pingüinos varía cada año.
