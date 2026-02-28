# Levalle Basketball - Sitio Web

Sitio web moderno y profesional para Levalle Basketball con diseño deportivo dinámico.

## 📁 Archivos incluidos

- `index.html` - Página principal con todas las secciones
- `sponsors.html` - Página dedicada al programa de sponsors

## 🚀 Cómo subir a GitHub Pages

### Opción 1: Repositorio nuevo

1. Creá un nuevo repositorio en GitHub (por ejemplo: `levalle-basketball`)
2. Subí ambos archivos HTML al repositorio
3. Andá a Settings → Pages
4. En "Source" seleccioná la rama `main` y la carpeta `/ (root)`
5. Guardá y esperá unos minutos
6. Tu sitio estará disponible en: `https://[tu-usuario].github.io/levalle-basketball/`

### Opción 2: Repositorio de usuario

1. Creá un repositorio con el nombre: `[tu-usuario].github.io`
2. Subí los archivos HTML
3. El sitio estará automáticamente en: `https://[tu-usuario].github.io/`

## 🎨 Características del diseño

### Página Principal (index.html)
- Hero section con imagen de fondo y call-to-actions
- Sección "Quiénes somos" con estadísticas
- Grid de categorías (Mosquitos, Premini/Mini, U14/U16, Primera)
- Galería de fotos (placeholders para tus imágenes reales)
- Preview del programa de sponsors
- Formulario de contacto
- Footer completo

### Página de Sponsors (sponsors.html)
- Beneficios detallados de ser sponsor
- 2 planes de pago claramente diferenciados:
  - Pago único: $80.000 (bonificado)
  - Plan cuotas: 5 x $20.000 (marzo-julio 2026)
- Grid de logos de sponsors actuales (placeholders)
- Proceso en 3 pasos
- Múltiples CTAs para conversión

## 🎨 Paleta de colores

- **Azul Profundo**: #113366 (principal)
- **Naranja Balón**: #E88121 (acento/CTAs)
- **Gris Halcón**: #A8B1B1 (secundario)
- **Blanco Off-White**: #F8F9FA (fondo)
- **Negro Carbono**: #1A1A1A (texto)

## ✨ Funcionalidades

- **Responsive**: Se adapta perfectamente a móviles, tablets y desktop
- **Animaciones**: Efectos de scroll y hover sutiles
- **Navegación suave**: Scroll suave entre secciones
- **Menú móvil**: Hamburger menu funcional
- **Formulario de contacto**: Listo para integrar con backend

## 📝 Personalización

### Reemplazar imágenes de fondo
Las imágenes actuales son de Unsplash (placeholders). Para usar tus propias fotos:

1. Subí tus imágenes al repositorio (creá una carpeta `images/`)
2. Reemplazá las URLs en el CSS:
   - Hero principal: línea ~150 en index.html
   - Galería: líneas con clase `.galeria-placeholder`
   - Hero sponsors: línea ~150 en sponsors.html

### Agregar logos de sponsors reales
En `sponsors.html`, buscá la sección `.sponsors-grid` y reemplazá los placeholders:

```html
<!-- Antes -->
<div class="sponsor-placeholder">
    <div class="icon">🏢</div>
    <div class="text">logo sponsor</div>
</div>

<!-- Después -->
<div class="sponsor-real">
    <img src="images/logo-sponsor.png" alt="Nombre Sponsor">
</div>
```

### Integrar formulario de contacto
El formulario actual solo muestra un alert. Para hacerlo funcional, podés:

1. **Formspree**: Agregá `action="https://formspree.io/f/[tu-id]"` al tag `<form>`
2. **EmailJS**: Implementá EmailJS en la función `handleSubmit()`
3. **Backend propio**: Conectá a tu API

### Agregar Google Analytics
Agregá antes del cierre de `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=TU-ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'TU-ID');
</script>
```

## 🔗 Enlaces importantes

- Instagram: [@basquetlevalle19](https://www.instagram.com/basquetlevalle19/)

## 📱 Redes sociales

Actualizá los enlaces de redes sociales en el footer de ambas páginas con tus URLs reales.

## ⚡ Optimizaciones recomendadas

1. **Comprimir imágenes**: Usá TinyPNG o similar antes de subirlas
2. **CDN**: Las fuentes ya están optimizadas desde Google Fonts
3. **Favicon**: Agregá un favicon.ico en la raíz del repo
4. **Meta tags**: Agregá Open Graph tags para compartir en redes
5. **Sitemap**: Generá un sitemap.xml para mejor SEO

## 🆘 Soporte

Si tenés dudas sobre personalización o implementación, podés:
- Revisar la documentación de GitHub Pages
- Consultar sobre el código específico que necesites modificar

## 📄 Licencia

Diseño custom creado para Levalle Basketball. Libre para uso del club.

---

**¡Éxitos con el sitio! 🏀**
