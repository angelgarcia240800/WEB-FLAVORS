# Changelog

Todas las modificaciones notables a este proyecto serán documentadas en este archivo según el estándar [Semantic Versioning](https://semver.org/).

## [1.0.0] - 2026-09-23 (Lanzamiento Sitio Web y Despliegue en GitHub Pages)

### Infraestructura & Despliegue
- **Alojamiento en GitHub Pages**: Infraestructura nativa en la nube de GitHub con SSL gratuito y CDN global.
- **Automatización CI/CD**: Flujo de trabajo en GitHub Actions (`deploy.yml`) para despliegue automático del contenido de la carpeta `web/` ante cambios en la rama `main`.

### Portal Web & Frontend
- **Páginas del Sitio**: Inicio (`index.html`), Nosotros (`nosotros.html`), Menú & Precios (`menu.html`), Galería (`galeria.html`) y Contacto (`contacto.html`).
- **Diseño & Estilos**: Hojas de estilo CSS modular (`styles.css`) con diseño responsive, paleta corporativa y tipografías de Google Fonts.
- **Integración WhatsApp**: Enlaces directos para pedidos automatizados vía chat.
