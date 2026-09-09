# Aserradero Punky — sitio web

Sitio estático (HTML + CSS + JS, sin dependencias ni build) del Aserradero Punky, Misiones, Argentina.
Machimbre, tirantes y clavadores de pino al por mayor. Bilingüe español / portugués.

## Estructura

```
index.html      página completa
styles.css      estilos
app.js          cambio de idioma ES/PT + formulario que abre WhatsApp
assets/         fotos de planta y logo
```

## Publicar en GitHub Pages

1. Creá un repositorio nuevo en GitHub (por ejemplo `aserradero-punky`).
2. Subí **el contenido de esta carpeta** a la raíz del repositorio:

```bash
git init
git add .
git commit -m "Sitio Aserradero Punky"
git branch -M main
git remote add origin https://github.com/USUARIO/aserradero-punky.git
git push -u origin main
```

3. En GitHub: **Settings → Pages → Source: Deploy from a branch → Branch: `main` / `/ (root)` → Save**.
4. En 1–2 minutos queda online en `https://USUARIO.github.io/aserradero-punky/`.

Para usar un dominio propio (ej. `aserraderopunky.com.ar`), agregá un archivo `CNAME` con el dominio
y apuntá el DNS a GitHub Pages.

## Qué editar

- **WhatsApp:** variable `WHATSAPP` al inicio de `app.js` y el número visible en `index.html`.
- **Textos en español:** directamente en `index.html`.
- **Textos en portugués:** objeto `PT` en `app.js` (misma clave `data-i18n`).
- **Fotos:** reemplazá los archivos en `assets/` manteniendo los nombres.
- **Colores:** variables `--accent`, `--ink`, `--surface` al inicio de `styles.css`.

## Pendiente de confirmar

Medidas y largos de cada producto y el horario de atención son valores de referencia:
revisalos en `index.html` antes de publicar.
