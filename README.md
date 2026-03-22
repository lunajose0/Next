# El Cuaderno Digital — Blog con Next.js 14

Blog personal construido con Next.js 14, App Router y CSS Modules. Estética editorial cálida con tipografía serif y paleta crema/terracota.

## Vista previa

Cuatro páginas completas:
- **Inicio** — Hero editorial, artículos destacados, mini sobre mí y newsletter
- **Blog** — Lista filtrable de artículos
- **Sobre mí** — Habilidades, línea de tiempo y CTA de contacto
- **Contacto** — Formulario con validación en cliente

## Tecnologías

- [Next.js 14](https://nextjs.org/) — App Router, Server Components
- [React 18](https://react.dev/) — Hooks, Client Components
- [CSS Modules](https://github.com/css-modules/css-modules) — Estilos encapsulados por componente

## Instalación

Requiere Node.js 18.17 o superior.

```bash
# Clonar el repositorio
git clone https://github.com/tu-usuario/blog-nextjs.git
cd blog-nextjs

# Instalar dependencias
npm install

# Iniciar servidor de desarrollo
npm run dev
```

Abre [http://localhost:3000](http://localhost:3000) en tu navegador.

## Scripts disponibles

| Comando | Descripción |
|---|---|
| `npm run dev` | Servidor de desarrollo en puerto 3000 |
| `npm run build` | Build de producción optimizado |
| `npm run start` | Servidor de producción (requiere build previo) |
| `npm run lint` | Análisis estático con ESLint |

## Estructura del proyecto

```
blog-nextjs/
├── app/
│   ├── layout.js          # Layout raíz (Navbar + Footer)
│   ├── page.js            # Página de inicio
│   ├── page.module.css
│   ├── blog/
│   │   ├── page.js        # Listado del blog
│   │   └── page.module.css
│   ├── sobre/
│   │   ├── page.js        # Página sobre mí
│   │   └── page.module.css
│   └── contacto/
│       ├── page.js        # Formulario de contacto
│       └── page.module.css
├── components/
│   ├── Navbar.js
│   ├── Navbar.module.css
│   ├── Footer.js
│   └── Footer.module.css
├── styles/
│   └── globals.css
├── next.config.js
└── package.json
```

## Personalización

1. Cambia los datos del autor en `app/sobre/page.js`
2. Reemplaza los artículos de ejemplo en `app/blog/page.js` y `app/page.js`
3. Actualiza los enlaces de contacto en `components/Footer.js` y `app/contacto/page.js`
4. Modifica los colores en `styles/globals.css` (variables CSS)

## Deploy en Vercel

```bash
npm install -g vercel
vercel
```

O conecta el repositorio directamente desde el [dashboard de Vercel](https://vercel.com).

## Deploy en Netlify

```bash
npm run build
# Sube la carpeta .next con el adaptador de Next.js para Netlify
```

## Licencia

MIT — Libre para usar y modificar.
