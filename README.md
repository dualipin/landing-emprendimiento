# 🚀 Emprendimiento - Landing Page

**Soluciones tecnológicas modernas para un mundo conectado**

Una landing page profesional y responsiva desarrollada con [Astro](https://astro.build/) para una empresa de software especializada en desarrollo de aplicaciones, consultoría tecnológica y soluciones empresariales personalizadas.

![Tech Stack](https://img.shields.io/badge/Astro-6.0+-FF5D01?logo=astro&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-4.2+-06B6D4?logo=tailwindcss&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-5+-3178C6?logo=typescript&logoColor=white)

---

## 📋 Tabla de Contenidos

- [Características](#características)
- [Requisitos](#requisitos)
- [Instalación](#instalación)
- [Desarrollo](#desarrollo)
- [Build y Deploy](#build-y-deploy)
- [Estructura del Proyecto](#estructura-del-proyecto)
- [Tecnologías](#tecnologías)
- [SEO](#seo)
- [Contacto](#contacto)

---

## ✨ Características

- ✅ **Diseño Responsivo** - Optimizado para móvil, tablet y desktop
- 📱 **Mobile-First** - Prioritario en dispositivos móviles
- 🎨 **Tema Oscuro/Claro** - Toggle de tema integrado
- ⚡ **Alto Rendimiento** - Optimizado con Astro (0 JavaScript por defecto)
- 🔍 **SEO Optimizado** - Meta tags, Open Graph, Schema.org
- 💫 **Animaciones Fluidas** - Fade-in animations on scroll
- 🎯 **CTAs Estratégicos** - Llamadas a acción bien posicionadas
- 📧 **Formulario de Contacto** - Integración lista para backend
- 🔗 **Navegación Anclada** - Smooth scroll a secciones
- 🎭 **DaisyUI Components** - Componentes UI profesionales

---

## 🛠️ Requisitos

- **Node.js** ≥ 22.12.0
- **npm** o **pnpm**

---

## 📥 Instalación

1. **Clonar o descargar el proyecto:**
```bash
git clone <repository-url>
cd landing-emprendimiento
```

2. **Instalar dependencias:**
```bash
npm install
```

---

## 🚀 Desarrollo

Inicia el servidor de desarrollo con hot reload:

```bash
npm run dev
```

El sitio estará disponible en `http://localhost:3000`

---

## 🏗️ Build y Deploy

### Generar build para producción:
```bash
npm run build
```

Esto crea una carpeta `dist/` con los archivos optimizados.

### Previsualizar el build:
```bash
npm run preview
```

### Deploy:
El proyecto puede desplegarse en:
- **Vercel** (recomendado para Astro)
- **Netlify**
- **GitHub Pages**
- **cualquier servidor estático**

---

## 📁 Estructura del Proyecto

```
landing-emprendimiento/
├── public/
│   ├── robots.txt              # Configuración para crawlers
│   └── og-image.png            # Imagen Open Graph (1200x630px)
├── src/
│   ├── assets/
│   │   └── logos/              # Logo en diferentes tamaños
│   ├── components/
│   │   ├── Navbar.astro        # Navegación principal
│   │   ├── Footer.astro        # Pie de página
│   │   ├── ThemeToggle.astro   # Selector de tema
│   │   ├── SEO.astro           # Componente SEO reutilizable
│   │   ├── common/             # Componentes comunes
│   │   │   ├── ProjectCard.astro
│   │   │   ├── ServiceItem.astro
│   │   │   ├── SkillCard.astro
│   │   │   └── TestimonialCard.astro
│   │   └── ui/                 # Componentes UI base
│   │       ├── Badge.astro
│   │       ├── Card.astro
│   │       ├── SectionTitle.astro
│   │       └── StatItem.astro
│   ├── constants/
│   │   └── site.ts             # Configuración global del sitio
│   ├── data/
│   │   ├── projects.ts         # Datos de proyectos
│   │   ├── services.ts         # Datos de servicios
│   │   ├── skills.ts           # Stack tecnológico
│   │   └── testimonials.ts     # Testimonios de clientes
│   ├── layouts/
│   │   └── Layout.astro        # Layout principal
│   ├── pages/
│   │   └── index.astro         # Página principal
│   ├── sections/               # Secciones de la página
│   │   ├── Hero.astro
│   │   ├── About.astro
│   │   ├── Skills.astro
│   │   ├── Projects.astro
│   │   ├── Services.astro
│   │   ├── Testimonials.astro
│   │   └── Contact.astro
│   ├── styles/
│   │   └── global.css          # Estilos globales
│   ├── types/
│   │   └── index.ts            # Tipos TypeScript
│   └── utils/
│       └── seo.ts              # Utilidades SEO
├── astro.config.mjs            # Configuración de Astro
├── tailwind.config.js          # Configuración de Tailwind
├── tsconfig.json               # Configuración de TypeScript
└── package.json
```

---

## 🛠️ Tecnologías

| Tecnología | Versión | Propósito |
|-----------|---------|----------|
| **Astro** | 6.0+ | Framework web moderno |
| **Tailwind CSS** | 4.2+ | Utility-first CSS |
| **TypeScript** | 5+ | Type safety |
| **DaisyUI** | 5.5+ | Componentes UI |
| **Lucide Icons** | 0.577+ | Iconografía |
| **Tailwind UI** | - | Animaciones |

---

## 🔍 SEO

El proyecto incluye optimizaciones SEO completas:

### Meta Tags
- ✅ Meta description dinámico
- ✅ Open Graph tags (Facebook, LinkedIn)
- ✅ Twitter Card tags
- ✅ Canonical URLs
- ✅ Hreflang alternates

### Datos Estructurados
- ✅ Schema.org JSON-LD
- ✅ Organization Schema
- ✅ LocalBusiness Schema

### Performance
- ✅ Lighthouse optimizado
- ✅ Core Web Vitals
- ✅ Lazy loading de imágenes
- ✅ Minificación automática

### Archivos SEO
- ✅ `robots.txt` - Guía para crawlers
- ✅ `sitemap.xml` - Generado automáticamente por Astro

---

## ⚙️ Configuración

### `/src/constants/site.ts`
Actualiza los valores para tu proyecto:

```typescript
export const SITE_URL = "https://tudominio.com";
export const SITE_DESCRIPTION = "Tu descripción";
export const SITE_KEYWORDS = "tus, palabras, clave";
export const COMPANY_NAME = "Tu Empresa";
export const TWITTER_HANDLE = "@tutwitter";
```

### `/astro.config.mjs`
Usa tu dominio real:

```javascript
export default defineConfig({
  site: 'https://tudominio.com',
  // ...
});
```

---

## 📊 Performance

Métricas objetivas:

- **Lighthouse Score**: 90+
- **LCP (Largest Contentful Paint)**: < 2.5s
- **FID (First Input Delay)**: < 100ms
- **CLS (Cumulative Layout Shift)**: < 0.1
- **Bundle Size**: < 50KB (sin assets)

---

## 🎨 Personalización

### Cambiar colores
Edita `tailwind.config.js`:
```javascript
theme: {
  colors: {
    primary: '#YourColor',
    // ...
  }
}
```

### Cambiar datos
Actualiza los archivos en `/src/data/`:
- `projects.ts` - Tus proyectos
- `services.ts` - Tus servicios
- `skills.ts` - Tu stack técnico
- `testimonials.ts` - Testimonios de clientes

### Cambiar contenido
Edita las secciones en `/src/sections/`:
- Cada archivo `.astro` corresponde a una sección

---

## 📧 Contacto

Para más información sobre Emprendimiento:

- **Email**: contacto@tudominio.com
- **Teléfono**: +52 0000000000
- **Ubicación**: Tabasco, México

---

## 📄 Licencia

Este proyecto es de uso privado. Todos los derechos reservados © 2024 Emprendimiento.

---

## 🚀 Próximos Pasos

- [ ] Actualizar datos reales (proyectos, servicios, etc.)
- [ ] Cambiar dominio en configuración
- [ ] Crear imagen OG personalizada
- [ ] Verificar en Google Search Console
- [ ] Auditar con Lighthouse
- [ ] Implementar backend para formulario de contacto
- [ ] Configurar analytics (Google Analytics, etc.)
- [ ] Optimizar imágenes
- [ ] Probar en dispositivos reales

---

Made with ❤️ by **Emprendimiento** | Powered by [Astro](https://astro.build/)
