# Changelog

Todas las modificaciones notables a este proyecto serán documentadas en este archivo según el estándar [Semantic Versioning](https://semver.org/).

## [1.2.0] - 2026-09-23 (Automatización de Despliegue sin Comentarios & Respaldo de Módulo)

### Infraestructura & Automatización CI/CD
- **Limpieza Automática de Comentarios en Producción**: Se incorporó un paso en el pipeline de GitHub Actions (`deploy.yml`) que elimina automáticamente los comentarios HTML (`<!-- ... -->`) y CSS (`/* ... */`) de los archivos antes de desplegarlos en GitHub Pages.
- **Preservación del Código Fuente Local**: La base de código en el repositorio conserva todos los comentarios explicativos y educativos para el equipo y tutores académicos.

### Módulos & Documentación
- **Respaldo de Sección de Comentarios (Web3Forms)**: El código completo del formulario de Web3Forms y el muro de opiniones fue respaldado en `SECCION_COMENTARIOS_WEB3FORMS.md` para ser incorporado cuando el equipo lo decida.

## [1.1.0] - 2026-09-23 (Mejoras y Correcciones del Carrusel en Nosotros)

### Frontend & Experiencia de Usuario (Puro HTML y CSS)
- **Carrusel 100% Puro HTML y CSS**: Reestructuración completa sin JavaScript, cumpliendo con la arquitectura nativa del proyecto.
- **Flechitas de Navegación Manual**: Incorporación de botones de navegación anterior (`❮`) y siguiente (`❯`) vinculados a radio buttons y `<label>`.
- **Selección Directa por Indicadores**: Círculos inferiores interactivos para saltar directamente a cualquiera de las 4 fotos con estado activo animado.
- **Sincronización de Pausa en Hover**: Corrección de desincronización al pasar el mouse, pausando simultáneamente tanto la pista de fotos como los círculos inferiores (`animation-play-state: paused`).
- **Eliminación de Salto de Scroll**: Corrección del tirón de pantalla al hacer clic en las flechas desde los bordes del viewport mediante `display: none` en `.carousel__radio`.

## [1.0.0] - 2026-09-23 (Lanzamiento Sitio Web y Despliegue en GitHub Pages)

### Infraestructura & Despliegue
- **Alojamiento en GitHub Pages**: Infraestructura nativa en la nube de GitHub con SSL gratuito y CDN global.
- **Automatización CI/CD**: Flujo de trabajo en GitHub Actions (`deploy.yml`) para despliegue automático del contenido de la carpeta `web/` ante cambios en la rama `main`.

### Portal Web & Frontend
- **Páginas del Sitio**: Inicio (`index.html`), Nosotros (`nosotros.html`), Menú & Precios (`menu.html`), Galería (`galeria.html`) y Contacto (`contacto.html`).
- **Diseño & Estilos**: Hojas de estilo CSS modular (`styles.css`) con diseño responsive, paleta corporativa y tipografías de Google Fonts.
- **Integración WhatsApp**: Enlaces directos para pedidos automatizados vía chat.
