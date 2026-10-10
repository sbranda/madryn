# Mis viajes — Tucumán + Puerto Madryn

```
index.html        → portada con acceso a ambas guías
tucuman/          → app de Tucumán (index, manifest, sw, íconos)
madryn/           → app de Puerto Madryn (index, manifest, sw, íconos)
```

## Deploy en GitHub Pages
1. Creá un repo (ej. `viajes`) y subí el contenido de esta carpeta a la raíz.
2. Settings → Pages → rama `main`, carpeta `/ (root)`.
3. URLs: `https://TU-USUARIO.github.io/viajes/tucuman/` y `.../madryn/`.

Cada app tiene su propio service worker (alcance de su carpeta) y su propio caché, así que se instalan y actualizan por separado. Al cambiar archivos de una app, subí la versión de `CACHE_NAME` en su `sw.js`.
