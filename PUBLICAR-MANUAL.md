# Cómo Publicar el Manual de Usuario

Este documento explica cómo importar y publicar el manual de usuario en diferentes plataformas de documentación web.

---

## Estructura del Manual

```
docs/
├── manual-usuario/
│   ├── README.md                    # Índice principal
│   ├── 01-productos.md              # Gestión de productos
│   ├── 02-ventas.md                 # Gestión de ventas
│   ├── 03-clientes.md               # Gestión de clientes
│   ├── 04-formas-entrega.md         # Métodos de envío
│   ├── 05-formas-pago.md            # Medios de pago
│   ├── 06-promociones.md            # Promociones
│   ├── 07-cupones.md                # Cupones de descuento
│   └── 08-configuracion-tienda.md   # Configuración general
└── PUBLICAR-MANUAL.md               # Este archivo
```

---

## Opción 1: GitBook (Recomendada)

**GitBook** es ideal para documentación de usuario, con interfaz limpia y búsqueda integrada.

### Pasos:

1. **Crear cuenta** en [gitbook.com](https://www.gitbook.com)

2. **Crear un nuevo espacio** (Space)
   - Click en "Create a space"
   - Selecciona "Documentation"

3. **Importar desde Git** (Opción A)
   - Settings → Integrations → GitHub/GitLab
   - Conecta tu repositorio
   - Configura la carpeta `/docs/manual-usuario`

4. **Importar archivos manualmente** (Opción B)
   - Crea una nueva página por cada archivo .md
   - Copia el contenido de cada archivo
   - GitBook parseará el Markdown automáticamente

5. **Configurar navegación**
   - Arrastra las páginas para ordenarlas
   - El README.md será la página principal

6. **Publicar**
   - Click en "Publish"
   - Obtendrás una URL como: `https://tu-empresa.gitbook.io/manual`

### Características:
- ✅ Gratis para proyectos públicos
- ✅ Búsqueda integrada
- ✅ Responsive (móvil y desktop)
- ✅ Sync con Git
- ✅ Personalización de marca

---

## Opción 2: Docusaurus

**Docusaurus** (de Meta) es perfecto si quieres hostear la documentación en tu propio servidor.

### Instalación:

```bash
# Crear proyecto Docusaurus
npx create-docusaurus@latest manual-ayuda classic

# Entrar al directorio
cd manual-ayuda

# Copiar los archivos de documentación
# Copia la carpeta docs/manual-usuario a docs/ del proyecto Docusaurus
```

### Configurar `docusaurus.config.js`:

```javascript
module.exports = {
  title: 'Manual de Usuario',
  tagline: 'Panel de Administración',
  url: 'https://tu-dominio.com',
  baseUrl: '/ayuda/',
  
  presets: [
    [
      'classic',
      {
        docs: {
          routeBasePath: '/',
          sidebarPath: require.resolve('./sidebars.js'),
        },
      },
    ],
  ],
  
  themeConfig: {
    navbar: {
      title: 'Manual de Usuario',
      logo: {
        alt: 'Logo',
        src: 'img/logo.svg',
      },
    },
  },
};
```

### Configurar `sidebars.js`:

```javascript
module.exports = {
  tutorialSidebar: [
    'README',
    {
      type: 'category',
      label: 'Catálogo',
      items: ['01-productos'],
    },
    {
      type: 'category',
      label: 'Ventas',
      items: ['02-ventas', '03-clientes'],
    },
    {
      type: 'category',
      label: 'Configuración',
      items: [
        '04-formas-entrega',
        '05-formas-pago',
        '08-configuracion-tienda',
      ],
    },
    {
      type: 'category',
      label: 'Marketing',
      items: ['06-promociones', '07-cupones'],
    },
  ],
};
```

### Publicar:

```bash
# Build para producción
npm run build

# El contenido estará en /build
# Sube a tu servidor o usa Vercel/Netlify
```

---

## Opción 3: ReadTheDocs

**ReadTheDocs** es popular para documentación técnica y es completamente gratuito.

### Pasos:

1. **Crear archivo `mkdocs.yml`** en la raíz:

```yaml
site_name: Manual de Usuario - Panel Admin
nav:
  - Inicio: manual-usuario/README.md
  - Productos: manual-usuario/01-productos.md
  - Ventas: manual-usuario/02-ventas.md
  - Clientes: manual-usuario/03-clientes.md
  - Formas de Entrega: manual-usuario/04-formas-entrega.md
  - Formas de Pago: manual-usuario/05-formas-pago.md
  - Promociones: manual-usuario/06-promociones.md
  - Cupones: manual-usuario/07-cupones.md
  - Configuración: manual-usuario/08-configuracion-tienda.md

theme:
  name: material
  language: es
  palette:
    primary: indigo
    accent: indigo

markdown_extensions:
  - tables
  - admonition
  - toc:
      permalink: true
```

2. **Crear cuenta** en [readthedocs.org](https://readthedocs.org)

3. **Importar proyecto**
   - Click en "Import a Project"
   - Conecta tu repositorio de GitHub/GitLab
   - ReadTheDocs detectará el `mkdocs.yml`

4. **Build y publicar**
   - El build es automático
   - URL: `https://tu-proyecto.readthedocs.io`

---

## Opción 4: GitHub Pages

**GitHub Pages** es gratuito y se integra directamente con tu repositorio.

### Pasos:

1. **Crear archivo `_config.yml`** en `/docs`:

```yaml
title: Manual de Usuario
description: Panel de Administración
theme: just-the-docs
color_scheme: light

aux_links:
  "Ir al Panel":
    - "https://tu-panel.com"

nav_enabled: true

footer_content: "Manual de Usuario - Tu Empresa"
```

2. **Habilitar GitHub Pages**
   - Ve a Settings → Pages
   - Source: Deploy from a branch
   - Branch: `main` → `/docs`
   - Click Save

3. **URL del sitio**
   - `https://tu-usuario.github.io/tu-repo/`

---

## Opción 5: Notion

**Notion** es ideal si ya usas Notion para gestión interna.

### Pasos:

1. **Crear una nueva página** en Notion

2. **Importar Markdown**
   - Click en "..." → Import → Markdown
   - Selecciona los archivos .md uno por uno

3. **Organizar**
   - Crea subpáginas para cada sección
   - Usa el README.md como página principal

4. **Compartir públicamente**
   - Click en "Share"
   - Activa "Share to web"
   - Copia el link público

---

## Comparativa Rápida

| Plataforma | Gratis | Personalización | Facilidad | Búsqueda |
|------------|--------|-----------------|-----------|----------|
| **GitBook** | ✅ Básico | ⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ✅ |
| **Docusaurus** | ✅ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ✅ |
| **ReadTheDocs** | ✅ | ⭐⭐⭐ | ⭐⭐⭐⭐ | ✅ |
| **GitHub Pages** | ✅ | ⭐⭐⭐ | ⭐⭐⭐⭐ | ❌ |
| **Notion** | ✅ Básico | ⭐⭐ | ⭐⭐⭐⭐⭐ | ✅ |

---

## Recomendación

Para un **manual de usuario de producto**, recomiendo:

1. **GitBook** - Si quieres algo rápido, profesional y sin código
2. **Docusaurus** - Si quieres control total y hostearlo en tu dominio

---

## Personalización Adicional

### Agregar logo e imágenes

Crea una carpeta `/docs/manual-usuario/images/` y agrega:
- Screenshots del panel
- Iconos
- Diagramas

Referencias en Markdown:
```markdown
![Descripción](./images/mi-imagen.png)
```

### Agregar videos

Puedes embeber videos de YouTube:
```markdown
[![Video](https://img.youtube.com/vi/VIDEO_ID/0.jpg)](https://www.youtube.com/watch?v=VIDEO_ID)
```

---

## Mantenimiento

- **Actualiza el manual** cuando haya cambios en el panel
- **Versionado**: Considera tener versiones si hay cambios grandes
- **Feedback**: Agrega un formulario de feedback en cada página
