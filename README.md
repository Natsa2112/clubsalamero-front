# Club Salamero Front

Landing page de **Club Salamero** — servicio de suscripción de picadas artesanales argentinas. Construido con [Astro](https://astro.build) 6, CSS nativo y JavaScript vanilla.

## Estructura del proyecto

```text
/
├── public/
│   ├── favicon.ico
│   └── favicon.svg
├── src/
│   ├── assets/
│   │   └── images/
│   │       ├── caja.avif
│   │       └── picada.avif
│   ├── components/
│   │   ├── BoxContents.astro
│   │   ├── FAQ.astro
│   │   ├── Features.astro
│   │   ├── Footer.astro
│   │   ├── Header.astro
│   │   ├── Hero.astro
│   │   ├── HowItWorks.astro
│   │   ├── Plans.astro
│   │   ├── Producers.astro
│   │   ├── Products.astro
│   │   └── Testimonials.astro
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       ├── box-contents.css
│       ├── faq.css
│       ├── features.css
│       ├── footer.css
│       ├── global.css
│       ├── header.css
│       ├── hero.css
│       ├── how-it-works.css
│       ├── plans.css
│       ├── producers.css
│       ├── products.css
│       └── testimonials.css
├── astro.config.mjs
├── details.md
├── package.json
├── pnpm-workspace.yaml
├── todo.md
└── tsconfig.json
```

## Secciones del sitio

| Sección      | Componente           | Descripción                                   |
|--------------|----------------------|-----------------------------------------------|
| Header       | `Header.astro`       | Navbar fija con menú hamburguesa responsive   |
| Hero         | `Hero.astro`         | Portada con CTA, badges y contadores animados |
| Features     | `Features.astro`     | Grid "Por qué elegirnos"                      |
| Products     | `Products.astro`     | Galería "Box de este mes"                     |
| Plans        | `Plans.astro`        | 3 planes de suscripción                       |
| Box Contents | `BoxContents.astro`  | "Qué viene en la caja"                        |
| How It Works | `HowItWorks.astro`   | Timeline "Cómo funciona"                      |
| Producers    | `Producers.astro`    | Tarjetas de productores                       |
| Testimonials | `Testimonials.astro` | Slider de testimonios                         |
| FAQ          | `FAQ.astro`          | Acordeón de preguntas frecuentes              |
| Footer       | `Footer.astro`       | Footer con CTA y links                        |

## Comandos

| Comando | Acción |
|---------|--------|
| `pnpm install` | Instala dependencias |
| `pnpm dev` | Inicia servidor local en `localhost:4321` |
| `pnpm build` | Build producción en `./dist/` |
| `pnpm preview` | Previsualiza build local |

## Stack

- **Framework:** Astro 6 (SSG)
- **Estilos:** CSS nativo con custom properties
- **Fuentes:** Playfair Display + Inter (Google Fonts)
- **Iconos:** Font Awesome 6.5.1
- **JS:** Solo vanilla (sin frameworks de frontend)
