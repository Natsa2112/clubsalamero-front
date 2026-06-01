# Club Salamero

## Descripción
Landing page moderna para **Club Salamero**, un servicio de suscripción de picadas artesanales argentinas. Inspirado en El Club del Salame.

## Stack Tecnológico
- **pnpm** - Gestor de paquetes
- **Astro 6** - Framework web estático
- **CSS nativo** - Variables CSS, Flexbox, Grid, diseño responsive
- **Google Fonts** - Playfair Display (serif) + Inter (sans-serif)
- **Font Awesome** - Iconografía via CDN

## Estructura de Componentes
| Archivo | Ruta | Propósito |
|---------|------|-----------|
| `Layout.astro` | `src/layouts/` | HTML shell, meta, fuentes, CSS global |
| `Header.astro` | `src/components/` | Navegación + menú hamburguesa mobile |
| `Hero.astro` | `src/components/` | Sección principal con CTA |
| `Features.astro` | `src/components/` | Bloques de ventajas (4 columnas) |
| `Products.astro` | `src/components/` | Galería de productos destacados |
| `Plans.astro` | `src/components/` | Tres planes de suscripción |
| `BoxContents.astro` | `src/components/` | Qué viene en la caja (4 ítems) |
| `HowItWorks.astro` | `src/components/` | 4 pasos del proceso |
| `Producers.astro` | `src/components/` | Cards de productores/regiones |
| `Testimonials.astro` | `src/components/` | Slider/cards de testimonios |
| `FAQ.astro` | `src/components/` | Acordeón de preguntas frecuentes |
| `Footer.astro` | `src/components/` | Footer completo |
| `index.astro` | `src/pages/` | Página principal (composición) |

## Diseño Visual
- **Colores**: Tonos tierra (marrón #5C2E1E, beige #F5F0EB, burdeos #8B1A1A, verde oliva #5A7A4A, dorado #D4A853)
- **Tipografía**: Playfair Display (títulos, serif artesanal) + Inter (cuerpo, sans-serif)
- **Formas**: Bordes redondeados suaves (8-12px), sombras sutiles
- **Responsive**: Mobile-first, breakpoints a 768px y 1024px

## Funcionalidades
- Menú hamburguesa responsive con JS puro
- Selector de planes con precios dinámicos
- Acordeón FAQ con JS puro
- Slider de testimonios con JS puro
- Formulario newsletter con validación básica
- Enlaces WhatsApp y anclas internas (#secciones)
- Navegación suave (scroll behavior)

## Rendimiento & Accesibilidad
- `loading="lazy"` en imágenes
- Alt descriptivas
- Contraste suficiente
- HTML semántico (header, main, section, footer)
- CSS optimizado sin dependencias externas (salvo Font Awesome CDN)

## Páginas
- `/` — Landing page principal con todas las secciones
