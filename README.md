# 🍓 WEB-FLAVORS

Sitio web oficial de **Batidos Flavors** — Batidos artesanales a base de frutas 100% naturales, yogurt casero y repostería artesanal en Quíbor, estado Lara.

- **Dominio Oficial:** [https://batidosflavors.shop](https://batidosflavors.shop)
- **Alojamiento:** GitHub Pages
- **Despliegue Continuo (CI/CD):** Cada cambio en la carpeta `web/` en la rama `main` se publica automáticamente a través de GitHub Actions.

---

## 🗂️ Estructura del Repositorio

El proyecto cuenta con dos entornos claramente organizados: la versión de producción web y una versión adaptada para defensas y presentaciones académicas:

```text
WEB-FLAVORS/
├── .github/
│   └── workflows/
│       └── deploy.yml        # Pipeline de despliegue continuo (CI/CD) a GitHub Pages
│
├── web/                      # 🚀 SITIO WEB OFICIAL EN PRODUCCIÓN (batidosflavors.shop)
│   ├── assets/               # Recursos multimedia clasificados por módulos
│   │   ├── carrusel/         # Fotos del carrusel continuo de la sección Nosotros
│   │   ├── favicon/          # Icono oficial del sitio (.ico)
│   │   ├── galeria/          # Fotografías de alta resolución para la galería interactiva
│   │   ├── inicio/           # Ilustraciones transparentes de productos destacados del home
│   │   ├── logo/             # Identidad visual (Logo oficial Batidos Flavors y Logo UPTAEB)
│   │   └── menu/             # Imágenes de productos de la carta y Menú digital descargable (.jpg)
│   ├── CNAME                 # Configuración de dominio personalizado (batidosflavors.shop)
│   ├── contacto.html         # Página de contacto, pedidos WhatsApp, Instagram y Google Maps interactivo
│   ├── favicon.ico           # Acceso directo para navegadores en la raíz
│   ├── galeria.html          # Galería visual de productos y creaciones
│   ├── index.html            # Portada principal, hero, destacados y opiniones
│   ├── menu.html             # Carta de precios completa clasificada por categorías y descarga de flyer
│   ├── nosotros.html         # Historia de la marca, misión, visión y carrusel continuo en CSS puro
│   └── styles.css            # Hoja de estilos central y responsiva
│
├── web-defensa/              # 🎓 VERSIÓN ADAPTADA PARA DEFENSA ACADÉMICA / OFFLINE
│   ├── assets/               # Recursos multimedia y capturas de pantalla de respaldo local
│   ├── contacto.html         # Contacto adaptado con capturas locales y modal CSS nativo (:target)
│   ├── galeria.html          # Galería comentada con guía didáctica
│   ├── index.html            # Portada comentada con explicaciones técnicas detalladas
│   ├── menu.html             # Menú y lista de precios comentada
│   ├── nosotros.html         # Nosotros comentado
│   └── styles.css            # Hoja de estilos con guía técnica completa y recomendaciones
│
├── CHANGELOG.md              # Historial oficial de versiones y cambios del proyecto
└── README.md                 # Documentación general y catálogo de recursos
```

---

## 🖼️ Catálogo de Imágenes y Recursos Multimedia (`web/assets/`)

Todas las imágenes contenidas en la versión de producción están organizadas en subcarpetas semánticas y vinculadas activamente en el código:

| Subcarpeta | Archivo | Ubicación en el sitio | Descripción del recurso |
| :--- | :--- | :--- | :--- |
| `logo/` | `logo.png` | Navbar, Hero y OpenGraph | Logotipo circular oficial con fondo crema y carita |
| `logo/` | `logouniversidad.png` | Footer (todas las páginas) | Logo oficial institucional de la UPTAEB |
| `favicon/` | `favicon.ico` | Encabezado (`<head>`) | Icono oficial de pestaña del navegador |
| `inicio/` | `inicio-pie-limon.png` | Inicio (`index.html`) | Tarjeta destacada de Pie de Limón Artesanal |
| `inicio/` | `inicio-fresa-brownie.png` | Inicio (`index.html`) | Tarjeta destacada de Fresas con Crema & Brownie |
| `inicio/` | `inicio-batido-chocolate.png` | Inicio (`index.html`) | Tarjeta destacada de Batido de Chocolate Clásico |
| `menu/` | `menu-pie-limon.png` | Menú (`menu.html`) | Imagen destacada de Pie de Limón en el menú |
| `menu/` | `menu-fresa-brownie.png` | Menú (`menu.html`) | Imagen destacada de Fresas con Crema & Brownie |
| `menu/` | `menu-yogur-cereal.png` | Menú (`menu.html`) | Imagen destacada de Yogurt natural & Frutas |
| `menu/` | `menu.jpg` | Menú (`menu.html`) | Flyer digital oficial en alta resolución para descarga |
| `carrusel/` | `nosotros-carrusel-1.jpg` | Nosotros (`nosotros.html`) | Foto 1 carrusel continuo (Pie de parchita) |
| `carrusel/` | `nosotros-carrusel-2.jpg` | Nosotros (`nosotros.html`) | Foto 2 carrusel continuo (Fresas con crema) |
| `carrusel/` | `nosotros-carrusel-3.jpg` | Nosotros (`nosotros.html`) | Foto 3 carrusel continuo (Batido especial) |
| `carrusel/` | `nosotros-carrusel-4.jpg` | Nosotros (`nosotros.html`) | Foto 4 carrusel continuo (Fresas con brownie) |
| `galeria/` | `galeria-1.jpg` | Galería (`galeria.html`) | Foto 1 (Piña con leche · Formato vertical) |
| `galeria/` | `galeria-2.jpg` | Galería (`galeria.html`) | Foto 2 (Choco Brownie) |
| `galeria/` | `galeria-3.jpg` | Galería (`galeria.html`) | Foto 3 (Toddy Oreo) |
| `galeria/` | `galeria-4.jpg` | Galería (`galeria.html`) | Foto 4 (Fresas con crema) |
| `galeria/` | `galeria-5.jpg` | Galería (`galeria.html`) | Foto 5 (Yogurt Flavors · Formato horizontal) |
| `galeria/` | `galeria-6.jpg` | Galería (`galeria.html`) | Foto 6 (Pie de parchita) |
| `galeria/` | `galeria-7.jpg` | Galería (`galeria.html`) | Foto 7 (Tus sabores favoritos · Formato horizontal) |
| `galeria/` | `galeria-8.jpg` | Galería (`galeria.html`) | Foto 8 (Batidos artesanales · Formato horizontal) |

---

## 🛠️ Tecnologías y Arquitectura

- **HTML5 Semántico:** Estructura accesible, meta etiquetas completas (OpenGraph, Twitter Cards) y diseño adaptativo.
- **CSS3 Puro y Modular:** Diseño responsivo con Flexbox y CSS Grid, variables globales (`:root`), animaciones fluidas (`@keyframes`) y soporte para temas.
- **Cero Dependencias JavaScript:** Interacciones avanzadas (menú hamburguesa móvil mediante checkbox hack, carrusel continuo de imágenes, modal de confirmación con pseudo-clase `:target`) implementadas 100% con CSS nativo.
- **Automatización CI/CD:** Flujo de trabajo en GitHub Actions que limpia comentarios de desarrollo y publica automáticamente el artefacto de producción en GitHub Pages.

---

## 👥 Datos Académicos e Institucionales

- **Institución:** Universidad Politécnica Territorial de Lara “Andrés Eloy Blanco” (UPTAEB).
- **Programa:** PNF en Informática · Trayecto II.
- **Equipo del Proyecto:**
  - Rodríguez, José A.
  - García, Ángel
- **Tutor Asesor:** Ing. Lorelys Alvarado.

---

## 📋 Historial de Versiones
Para consultar el registro cronológico de cambios, mejoras y versiones, visita el archivo [CHANGELOG.md](CHANGELOG.md).
