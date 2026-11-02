# ENVEN – Sitio web de centros de datos

Sitio estático (HTML + CSS + JS) listo para **GitHub Pages**. Sin dependencias ni proceso de build.

```
index.html
css/styles.css
js/main.js
img/  logo.svg · favicon.svg · hero-rack.svg · sala-datacenter.svg
```

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub y sube estos archivos a la raíz.
2. Ve a **Settings → Pages**.
3. En *Build and deployment* elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
4. Espera 1–2 minutos: tu sitio quedará en `https://TU-USUARIO.github.io/NOMBRE-REPO/`.

## Personalización rápida

| Qué cambiar | Dónde |
|---|---|
| Nombre de marca "CORENODE" | `index.html` (header, footer, `<title>`) |
| Número de WhatsApp | Buscar `wa.me/00000000000` en `index.html` (formato internacional sin `+`) |
| Correo, teléfono, cobertura | Footer de `index.html` y `FALLBACK_EMAIL` en `js/main.js` |
| Colores | Variables `:root` al inicio de `css/styles.css` |
| Imágenes | Reemplaza los SVG de `img/` por fotos reales (`.jpg`/`.webp`) y actualiza el `src` |
| Testimonios | Hay un comentario con la estructura en la sección `#confianza` |

## Formulario de cotización

GitHub Pages no procesa formularios. Dos opciones en `js/main.js`:

- **Formspree (recomendado):** crea un formulario en formspree.io y pega su URL en `FORM_ENDPOINT`.
- **Sin configurar nada:** el formulario abre el correo del usuario con el mensaje prellenado (`mailto:`).

## Archivos de SEO

`robots.txt`, `sitemap.xml` e `img/og-image.png` (vista previa al compartir). El archivo `CNAME` ya está en tu repositorio; no lo sobrescribas.
