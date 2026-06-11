# Club Salamero Front — Plan de Desarrollo

## Fase 1: Configuración del Proyecto

- [x] `package.json` — Metadatos del proyecto, scripts (dev/build/preview/astro), dependencia `astro ^6.4.2`
- [x] `pnpm-workspace.yaml` — Configuración de workspace pnpm (permite builds de esbuild y sharp)
- [x] `pnpm-lock.yaml` — Lockfile de dependencias
- [x] `tsconfig.json` — TypeScript config estricto que extiende `astro/tsconfigs/strict`
- [x] `astro.config.mjs` — Configuración de Astro (actualmente vacío, sin integraciones)
- [x] `.gitignore` — Ignora dist/, .astro/, node_modules/, .env*, .vscore/, .idea/, .vercel/, .netlify/, logs, .DS_Store
- [x] `.vscode/extensions.json` — Recomienda extensión `astro-build.astro-vscode`
- [x] `.vscode/launch.json` — Configuración de lanzamiento para dev server
- [x] `node_modules/` — Dependencias instaladas

## Fase 2: Documentación

- [x] `README.md` — Template básico de Astro (genérico)
- [x] `details.md` — Documentación detallada del proyecto en español

## Fase 3: Estructura Core

- [x] `src/layouts/Layout.astro` — Shell HTML: meta tags, Google Fonts, Font Awesome, favicons, `<slot />`
- [x] `src/pages/index.astro` — Página única: importa Layout + 11 componentes y los compone en orden

## Fase 4: Componentes

- [x] `src/components/Header.astro` — Navbar fija superior con logo, enlaces, CTA y menú hamburguesa responsive
- [x] `src/components/Hero.astro` — Hero principal: fondo animado, badge, headline gradiente, CTA, contadores con animación
- [x] `src/components/Features.astro` — Sección "Por qué elegirnos": grid de 4 columnas con tarjetas
- [x] `src/components/Products.astro` — "Box de este mes": galería de 9 productos en grid responsive
- [x] `src/components/Plans.astro` — "Elegí tu plan": 3 planes de suscripción con precios y features
- [x] `src/components/BoxContents.astro` — "Qué viene en la caja": layout 2 columnas con items numerados
- [x] `src/components/HowItWorks.astro` — "Cómo funciona": timeline vertical de 4 pasos
- [x] `src/components/Producers.astro` — "Conocé a los productores": grid de productores con blockquote
- [x] `src/components/Testimonials.astro` — Slider de testimonios con auto-avance y dots
- [x] `src/components/FAQ.astro` — Acordeón de preguntas frecuentes con toggle y CTA final
- [x] `src/components/Footer.astro` — Footer completo: CTA banner, links, redes, copyright

## Fase 5: Estilos

- [x] `src/styles/global.css` — Reset, variables CSS (colores, fuentes, spacing), utilidades (.container, .btn, etc.)
- [x] `src/styles/fonts.css` — Declaraciones @font-face para fuentes locales
- [x] `src/styles/header.css` — Estilos de navbar fija, menú hamburguesa, overlay mobile
- [x] `src/styles/hero.css` — Hero full-viewport, fondos gradientes, blobs animados, contadores
- [x] `src/styles/features.css` — Grid de 4 columnas, tarjetas con sombra y hover
- [x] `src/styles/products.css` — Grid auto-fill de productos, image placeholders
- [x] `src/styles/plans.css` — Tarjetas de planes, columna central destacada, badge flotante
- [x] `src/styles/box-contents.css` — Layout 2 columnas, items con hover, tags de colores
- [x] `src/styles/how-it-works.css` — Timeline vertical, círculos numerados, línea gradiente
- [x] `src/styles/producers.css` — Grid de productores, blockquote, íconos centrados
- [x] `src/styles/testimonials.css` — Slider horizontal, tarjetas centradas, dots de navegación
- [x] `src/styles/faq.css` — Acordeón con borde, icono +/- rotatorio, transición max-height
- [x] `src/styles/footer.css` — Footer oscuro, CTA banner, grid de links, copyright

## Fase 6: Assets

- [x] `src/assets/images/caja.avif` — Foto de la caja de suscripción
- [x] `src/assets/images/picada.avif` — Foto de picada/board
- [x] `public/favicon.svg` — SVG favicon (cubierto: negro en claro, blanco en oscuro)
- [x] `public/favicon.ico` — Favicon legacy
- [x] `src/assets/images/img.txt` — Descartado (no necesario)
- [x] `src/assets/fonts/` — Fuentes descargadas localmente (Inter + Playfair Display)

## Fase 7: Build y Archivos Generados

- [x] `.astro/settings.json` — Config interna de Astro
- [x] `.astro/types.d.ts` — Referencias de tipos Astro
- [x] `.astro/content.d.ts` — Declaraciones de content collections (vacío)
- [x] `.astro/collections/` — Directorio vacío para collections
- [x] `dist/index.html` — Build estático HTML generado
- [x] `dist/favicon.svg` — Copia de public/
- [x] `dist/favicon.ico` — Copia de public/
- [x] `dist/_astro/index.BebMxDIP.css` — CSS bundled y minificado