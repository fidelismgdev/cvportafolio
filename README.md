# 🚀 Portafolio de Ricardo Torres — Jekyll + GitHub Pages

Portafolio profesional construido con Jekyll, listo para desplegar en GitHub Pages.

## 📁 Estructura del Proyecto

```
portfolio/
├── _config.yml              # Configuración de Jekyll
├── _data/
│   └── profile.yml          # ⭐ TUS DATOS (edita aquí primero)
├── _includes/
│   ├── nav.html             # Barra de navegación
│   └── footer.html          # Pie de página
├── _layouts/
│   ├── default.html         # Layout base
│   ├── home.html            # Layout de inicio
│   └── project.html         # Layout de proyecto individual
├── _projects/               # ⭐ TUS PROYECTOS (agrega .md aquí)
│   ├── 01-ecommerce-dashboard.md
│   ├── 02-landing-corporativa.md
│   ├── 03-task-manager.md
│   └── 04-blog-api.md
├── assets/
│   ├── css/main.css         # Estilos principales
│   ├── js/main.js           # JavaScript (animaciones, scroll)
│   └── images/              # Imágenes (screenshots, avatar)
├── index.html               # Página principal
├── Gemfile                  # Dependencias Ruby
└── README.md                # Este archivo
```

## ⚡ Inicio Rápido

### 1. Personaliza tus datos

Edita el archivo `_data/profile.yml` con tu información real:
- Nombre, email, ubicación
- Links de redes sociales
- Habilidades y niveles
- Experiencia laboral
- Educación

### 2. Agrega tus proyectos

Crea archivos `.md` en la carpeta `_projects/` con este formato:

```yaml
---
title: "Nombre del Proyecto"
tags: ["React", "Node.js"]
link: "https://github.com/tu-usuario/proyecto"
image: "/assets/images/proyecto.png"  # opcional
order: 1
---

Descripción del proyecto aquí...
```

### 3. Agrega imágenes

Coloca tus imágenes en `assets/images/`:
- Screenshots de proyectos
- Tu foto de perfil (opcional)

## 🖥️ Desarrollo Local

```bash
# Instalar dependencias
bundle install

# Iniciar servidor local
bundle exec jekyll serve

# Abrir en http://localhost:4000/portfolio/
```

## 🌐 Deploy en GitHub Pages

### Opción A: GitHub Pages automático

1. Crea un repositorio en GitHub llamado `portfolio` (o el nombre que prefieras)
2. Sube todos los archivos:

```bash
git init
git add .
git commit -m "Initial commit - portfolio"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/portfolio.git
git push -u origin main
```

3. Ve a **Settings → Pages** en tu repositorio
4. En "Source", selecciona **GitHub Actions**
5. Crea el archivo `.github/workflows/jekyll.yml` (incluido abajo)

### Opción B: Si usas `tu-usuario.github.io`

1. Crea un repo llamado `tu-usuario.github.io`
2. En `_config.yml`, cambia `baseurl` a `""` (vacío)
3. Sube los archivos y GitHub lo despliega automáticamente

## 🎨 Personalización

### Cambiar colores
Edita las CSS variables en `assets/css/main.css`:

```css
:root {
  --accent: #d4a853;        /* Color dorado principal */
  --bg-primary: #0a0a0a;    /* Fondo oscuro */
  --text-primary: #f0ece4;  /* Texto claro */
}
```

### Cambiar tipografía
Modifica las fuentes en el mismo archivo:

```css
:root {
  --font-display: 'Playfair Display', serif;
  --font-body: 'DM Sans', sans-serif;
  --font-mono: 'JetBrains Mono', monospace;
}
```

## 📄 Licencia

Uso personal. Siéntete libre de modificarlo para tu propio portafolio.
