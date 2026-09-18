# Viraró Bodegón — Landing profesional

Landing estática HTML + CSS para **Viraró Bodegón Parrilla**, Sarmiento 1334, CABA. El proyecto está preparado para reemplazar el front de WordPress en la raíz de `https://virarobodegon.com.ar/` sin cambiar la URL principal.

## Incluye

- HTML semántico y responsive, sin framework ni JavaScript de navegación.
- Título, meta description, canonical, Open Graph, Twitter Card y jerarquía de headings alineados con la propuesta real.
- Contenido rastreable sobre **parrilla libre**, **tenedor libre**, comida abundante, merienda libre y ubicación en Buenos Aires.
- Datos estructurados Schema.org para `Restaurant`, `WebSite`, `WebPage`, `BreadcrumbList` y `FAQPage`.
- Enlace directo a Google Reviews y Google Maps.
- Cartas oficiales en PDF con URLs reales y apertura en nueva pestaña.
- Botón flotante de WhatsApp con Font Awesome 7.3.1 hacia `https://wa.me/5491138833144`.
- Imágenes locales dentro de `img/` con dimensiones declaradas cuando corresponde.
- `robots.txt` y `sitemap.xml` preparados para la raíz de `virarobodegon.com.ar`.

## Archivos principales

- `index.html`: estructura, contenido SEO, CTA y Schema.org.
- `styles.css`: sistema visual responsive.
- `img/`: logo, fotografías y piezas visuales del proyecto.
- `pdf/`: las cinco cartas oficiales, conservando las rutas `/pdf/` que utiliza el sitio actual.
- `robots.txt`: reglas de rastreo y sitemap oficial.
- `sitemap.xml`: URL canónica de la homepage.
- `brand-spec.md`: inventario y origen de assets.

## Migración a la raíz del dominio

1. Realizar una copia de seguridad completa de WordPress, base de datos, archivos y `.htaccess` antes de reemplazar producción.
2. Confirmar que el dominio mantiene HTTPS y que `https://virarobodegon.com.ar/` responde con `index.html`.
3. Copiar a la raíz el contenido publicado de este repositorio: `index.html`, `styles.css`, `img/`, `pdf/`, `robots.txt` y `sitemap.xml`.
4. Mantener disponibles las URLs históricas que todavía reciben tráfico o enlaces, especialmente los PDFs oficiales. Si alguna URL antigua deja de existir, redirigirla con `301` a su equivalente real o responder `404/410` cuando el contenido haya sido eliminado.
5. No bloquear el HTML, CSS, imágenes ni PDFs mediante `robots.txt`.
6. Verificar en Search Console las variantes `https://virarobodegon.com.ar/` y `https://www.virarobodegon.com.ar/`, enviar `https://virarobodegon.com.ar/sitemap.xml` y solicitar inspección de la URL principal después de publicar.
7. Revisar que canonical, Open Graph, Schema.org, sitemap, imágenes, enlaces internos y enlaces a PDFs sigan apuntando a la URL final oficial.
8. Medir tráfico, indexación, errores 404, cobertura, consultas y rendimiento antes y después de la sustitución.

La migración no debe hacerse sobre producción sin backup ni sin conservar el mapa de URLs históricas.

## Fuentes oficiales

- Sitio actual: https://virarobodegon.com.ar/
- Google Business Profile: https://maps.app.goo.gl/YizcpD8SQLwdLg4g8
- Google Maps: https://www.google.com/maps/place/Bodeg%C3%B3n+Parrilla+en+Buenos+Aires+Virar%C3%B3/
- Google Reviews y ubicación: https://maps.app.goo.gl/qJC3uUd1gL3Up48Z9
- Instagram: https://www.instagram.com/virarobodegon/
- Facebook: https://www.facebook.com/virarobrasas

## Publicación

El repositorio es público y se publica mediante GitHub Pages como entorno de revisión. Esta entrega no modifica el sitio WordPress de producción.
