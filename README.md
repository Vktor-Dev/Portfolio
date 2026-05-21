# victor.dev — Portfolio

Portfolio personal construido con [Astro](https://astro.build) y desplegado en GitHub Pages.

## Stack

- **Framework**: Astro 4
- **Estilos**: CSS puro con custom properties
- **Tipografía**: Inter (Google Fonts)
- **Deploy**: GitHub Pages via GitHub Actions

## Estructura

```
src/
├── components/
│   ├── Nav.astro          # Navbar sticky con blur
│   └── ProjectCard.astro  # Tarjeta reutilizable de proyecto
├── layouts/
│   └── Base.astro         # Layout HTML base
├── pages/
│   └── index.astro        # Página principal
└── styles/
    └── global.css         # Design tokens + utilidades
```

## Desarrollo local

```bash
npm install
npm run dev       # http://localhost:4321
npm run build     # genera /dist
npm run preview   # preview del build
```

## Deploy automático

Cada push a `main` despliega en GitHub Pages via GitHub Actions.
Configura en repo → Settings → Pages → Source: GitHub Actions.

## Personalización

1. Edita `src/pages/index.astro` — proyectos, skills, bio, links
2. Cambia colores en `src/styles/global.css` (variables `:root`)
3. Actualiza `astro.config.mjs` con tu dominio real
