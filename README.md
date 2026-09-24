# SMART Flexografía — Landing Page

Sitio estático (HTML/CSS/JS, sin build ni dependencias) para SMART Flexografía.

## Ver en local

```bash
python3 -m http.server 5500
```

Luego abre `http://localhost:5500`.

## Despliegue

Al ser un sitio 100% estático, se puede subir tal cual a cualquier hosting: Netlify, Vercel, GitHub Pages o un hosting compartido tradicional. Solo se necesita copiar `index.html`, `css/`, `js/` y `assets/`.

### GitHub Pages

El repo ya incluye el workflow [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml), que publica el sitio automáticamente en cada push a `main`. Para activarlo (solo una vez):

1. En GitHub, ir a **Settings → Pages**.
2. En **Source**, elegir **GitHub Actions**.
3. Hacer push a `main` (o re-ejecutar el workflow desde la pestaña Actions).

El sitio quedará publicado en la URL genérica de GitHub Pages:

```
https://leonelparrales22.github.io/Flexograf-a/
```

No se configuró ningún dominio propio (`CNAME`) porque todavía no se cuenta con uno. Cuando se adquiera un dominio, basta con agregar un archivo `CNAME` en la raíz del repo con el dominio y configurarlo en **Settings → Pages → Custom domain**; el resto del sitio no necesita cambios porque todas las rutas de `css/` y `js/` son relativas.

## Pendientes

- Reemplazar las ilustraciones SVG de la sección "Galería" (marcadas como "Imagen ilustrativa") por fotografías reales de planta/productos.
- Confirmar dirección exacta para reemplazar el mapa referencial de Quito por la ubicación precisa.
