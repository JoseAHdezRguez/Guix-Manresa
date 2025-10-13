# GUIX Manresa - Sitio Web Corporativo

Sitio web oficial de GUIX Manresa, empresa de construcción y acabados con más de 10 años de experiencia en Barcelona.

## 📋 Descripción del Proyecto

Este es un sitio web estático desarrollado para GUIX Manresa, una empresa familiar de construcción fundada en 2013 en Manresa, Barcelona. El sitio web presenta los servicios de la empresa, su portafolio de proyectos y información de contacto.

## 🏗️ Arquitectura del Proyecto

### Estructura de Archivos
```
├── index.html          # Página principal con todas las secciones
├── style.css           # Estilos CSS con diseño responsivo
├── WARP.md            # Guía para desarrollo con WARP
├── README.md          # Este archivo de documentación
├── Logo.png           # Logo principal de la empresa
├── logo-movil.svg     # Logo optimizado para móviles
├── hero.jpg           # Imagen de fondo del hero
└── assets/            # Carpeta con imágenes de servicios y portafolio
    ├── muros.jpg
    ├── pladur.png
    ├── yeso.jpg
    ├── mortero.jpg
    ├── Cocina*.webp     # Imágenes de cocinas renovadas
    └── Sala*.webp       # Imágenes de salas renovadas
```

### Tecnologías Utilizadas
- **HTML5**: Estructura semántica de la página
- **CSS3**: Estilos modernos con Flexbox y CSS Grid
- **Diseño Responsivo**: Mobile-first approach
- **Optimización**: Imágenes en formato WebP

## 🚀 Desarrollo Local

### Requisitos Previos
- Navegador web moderno
- Servidor local (opcional pero recomendado)

### Ejecutar el Sitio Localmente

#### Opción 1: Python (Recomendado)
```bash
# Navegar al directorio del proyecto
cd "D:\Workspace\Guix-Manresa\papi\Guix-Manresa"

# Iniciar servidor local
python -m http.server 8000

# Abrir en navegador: http://localhost:8000
```

#### Opción 2: Node.js
```bash
# Si tienes Node.js instalado
npx serve .

# O instalar globally
npm install -g serve
serve .
```

#### Opción 3: PHP
```bash
# Si tienes PHP instalado
php -S localhost:8000
```

## 🎨 Características de Diseño

### Paleta de Colores
- **Azul Principal**: #1e40af
- **Azul Secundario**: #3b82f6
- **Azul Oscuro**: #1a365d
- **Fondo Claro**: #f8fafc
- **Texto**: #333

### Secciones del Sitio
1. **Header**: Navegación con logo y menú
2. **Hero**: Presentación principal con call-to-action
3. **Sobre Nosotros**: Misión, visión y valores
4. **Estadísticas**: Años de experiencia y logros
5. **Servicios**: Portfolio de servicios técnicos
6. **Reformas**: Galería de proyectos residenciales
7. **Contacto**: Información de contacto
8. **Footer**: Información de la empresa

### Responsive Design
- **Desktop**: Logo 120px, navegación completa
- **Tablet**: Adaptación de grids y espaciados
- **Mobile**: Logo 70px, navegación compacta

## 📝 Gestión de Contenido

### Actualizar Información de la Empresa
```html
<!-- Contacto: Línea 287-319 en index.html -->
<section id="contacto">
  <!-- Actualizar información de contacto aquí -->
</section>
```

### Agregar Nuevas Imágenes de Servicios
1. Optimizar imágenes (preferiblemente WebP)
2. Subir a la carpeta del proyecto
3. Actualizar referencias en `index.html`
4. Mantener tamaño mínimo de 280px de ancho

### Modificar Estilos
- Colores principales: Líneas 16, 54, 139 en `style.css`
- Tamaños de logo: Líneas 278, 295 en `style.css`
- Breakpoints responsivos: Línea 283 en `style.css`

## 🔧 Comandos de Git

### Comandos Básicos
```bash
# Ver estado del repositorio
git status

# Ver historial de cambios
git log --oneline -10

# Agregar cambios
git add .

# Hacer commit
git commit -m "Descripción del cambio"

# Subir cambios
git push origin main

# Bajar cambios remotos
git pull origin main
```

### Flujo de Trabajo Recomendado
1. Realizar cambios locales
2. Probar en servidor local
3. Agregar y hacer commit de cambios
4. Push a repositorio remoto
5. Verificar en producción

## 📦 Optimización

### Imágenes
- **Formato**: WebP para fotografías, SVG para logos
- **Tamaño**: Máximo 200KB por imagen
- **Dimensiones**: Servicios 280px mínimo, Hero 1200px

### Performance
- CSS minificado en producción
- Imágenes optimizadas
- Carga lazy para imágenes (futuro)

## 🌐 Despliegue

### Hosting Recomendado
- **GitHub Pages**: Gratuito para repositorios públicos
- **Netlify**: Despliegue automático desde Git
- **Vercel**: Integración con repositorios

### Variables de Entorno
No se requieren variables de entorno para este proyecto estático.

## 📞 Información de la Empresa

**GUIX Manresa**
- **Ubicación**: Manresa, Barcelona, España
- **Fundada**: 2013
- **Experiencia**: +10 años en construcción
- **Especialidades**: 
  - Construcción de muros y tabiques
  - Sistemas Pladur®
  - Aislamiento térmico y acústico
  - Aplicación de yeso y morteros
  - Proyectos completos de construcción

## 🤝 Contribución

### Reportar Problemas
1. Crear issue en el repositorio
2. Describir el problema detalladamente
3. Incluir capturas de pantalla si es necesario

### Mejoras
1. Fork del repositorio
2. Crear rama feature
3. Realizar cambios
4. Pull request con descripción detallada

## 📄 Licencia

Este proyecto es propiedad de GUIX Manresa. Todos los derechos reservados.

---

**Contacto del Desarrollador**: Para soporte técnico o consultas sobre el código, contactar al administrador del repositorio.

**Última Actualización**: Octubre 2025