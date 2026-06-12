# KIT LIVE COMMERCE — Plataforma del curso

Sitio estático de una sola página (`index.html`). No necesita servidor: funciona con cualquier hosting estático (Vercel, Netlify, GitHub Pages).

## Opción A — Vercel por arrastrar y soltar (la más rápida, sin GitHub)

1. Entrá a https://vercel.com y creá una cuenta (gratis) o iniciá sesión.
2. Andá a https://vercel.com/new
3. Buscá la opción **"deploy a static project / Browse"** o simplemente **arrastrá esta carpeta** (la que contiene `index.html`) a la zona de subida.
4. Dejá la configuración por defecto (framework: **Other**) y tocá **Deploy**.
5. En ~30 segundos te da el link, tipo `https://kit-live-commerce.vercel.app`.

## Opción B — GitHub + Vercel (recomendada para actualizar fácil)

1. Creá un repositorio nuevo en https://github.com/new (por ej. `kit-live-commerce`), público o privado.
2. Subí el archivo `index.html` (botón **"uploading an existing file"** o `git push`).
3. Entrá a https://vercel.com/new → **Import** ese repositorio de GitHub.
4. Framework: **Other**. Tocá **Deploy**.
5. Listo: cada vez que actualices `index.html` en GitHub, Vercel redepliega solo.

### Subir por línea de comandos (opcional)
```bash
git init
git add index.html vercel.json
git commit -m "Kit Live Commerce"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/kit-live-commerce.git
git push -u origin main
```

## Notas importantes
- El sitio usa el **Google Apps Script** ya configurado para validar los códigos (no hay que tocar nada).
- La generación del certificado y descargas usan librerías por CDN (jsPDF, html2canvas) + Google Fonts → necesita internet, cosa que en Vercel/Netlify funciona normal.
- Para usar dominio propio (ej. `academia.magency.ar`): en Vercel → Project → **Settings → Domains** → agregás el dominio y seguís las instrucciones de DNS.

— by Magency · @magency.ar
