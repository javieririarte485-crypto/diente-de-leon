# Diente de León — sitio web

Sitio estático. No necesita build ni dependencias.

## Estructura
- `index.html` — página principal
- `aviso-de-privacidad.html` — se sirve en `/aviso-de-privacidad` (cleanUrls)
- `support.js` — runtime que renderiza la página
- `assets/` — fotos, logo y patrón
- `vercel.json` — URLs limpias + caché de imágenes

## Publicar en Vercel con GitHub
1. Crea un repo nuevo en GitHub (ej. `diente-de-leon`).
2. Sube el CONTENIDO de esta carpeta a la raíz del repo (arrastrando los archivos en github.com > Add file > Upload files, o con git).
3. En vercel.com: Add New → Project → importa ese repo.
4. Framework Preset: **Other**. Build Command: vacío. Output Directory: vacío (raíz). Deploy.
5. Dominio: Project → Settings → Domains → agrega tu dominio y sigue los DNS que indique Vercel.

Cada vez que hagas push a `main`, Vercel vuelve a publicar solo.
