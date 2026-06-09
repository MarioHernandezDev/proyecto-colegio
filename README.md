# 🏫 Programa de Convivencia Escolar · CEIP El Zahor

> Sitio web de una sola página que documenta y difunde las iniciativas de convivencia, inclusión e igualdad del centro educativo.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Sin dependencias](https://img.shields.io/badge/dependencias-ninguna-brightgreen?style=flat-square)

---

## 📋 Descripción

Página web institucional desarrollada para el **CEIP El Zahor** con el objetivo de presentar de forma visual y accesible las cinco iniciativas del Plan de Convivencia del curso. Diseñada para ser mostrada en reuniones con familias, jornadas de puertas abiertas y para su difusión en el blog del centro.

---

## ✨ Iniciativas recogidas

| # | Sección | Descripción |
|---|---------|-------------|
| 01 | **Recreos Inclusivos** | Cuadrantes de juego y gestión de material para Infantil, Primaria y Secundaria |
| 02 | **Bibliopatio** | Espacio lector al aire libre durante los recreos, impulsado con donaciones de las familias |
| 03 | **Día de la Familia** | Jornada comunitaria de renovación y pintura de las zonas de juego del patio |
| 04 | **Compromiso por la Igualdad** | Participación en el certamen provincial "Araceli Morales" contra la violencia de género |
| 05 | **Policromía Deportiva** | Exposición artística de Sergio Padial Fajardo sobre diversidad e inclusión en el deporte |

---

## 🗂️ Estructura del proyecto

```
/
├── index.html              # Página principal (single page)
├── styles.css              # Estilos globales con variables CSS y modo oscuro
├── assets/
│   ├── img/
│   │   ├── hero-bg.jpg
│   │   ├── recreo1-4.jpg
│   │   ├── poster1-2.jpg
│   │   ├── donacion-libros.jpg
│   │   └── concurso1-5.jpg
│   └── video/
│       └── bibliopatio.mp4
└── README.md
```

---

## 🎨 Diseño y tecnología

El sitio está construido en **HTML, CSS y JavaScript vanilla**, sin ninguna librería o framework externo, lo que garantiza máxima portabilidad y tiempo de carga mínimo.

### Paleta de color

| Token | Hex | Uso |
|-------|-----|-----|
| `--navy` | `#1B2C5E` | Títulos, navbar, botones principales |
| `--teal` | `#2A7F7F` | Acentos, enlaces activos, divisores |
| `--gold` | `#C8963A` | Detalles, citas, degradados |

### Tipografía

- **Fraunces** — Títulos y encabezados (serif expresivo)
- **Inter** — Cuerpo de texto y navegación (sans-serif legible)

### Funcionalidades incluidas

- 🌙 **Modo oscuro / claro** con persistencia en `localStorage`
- 🎬 **Telón cinemático** de apertura en el hero
- 📍 **Dot-nav lateral** con indicador de sección activa
- 🖼️ **Lightbox** de galería con navegación por teclado y gestos
- 📊 **Barra de progreso** de lectura
- ♿ **Accesibilidad** — roles ARIA, foco visible, soporte `prefers-reduced-motion`
- 📱 **Diseño responsive** — móvil, tablet y escritorio
- 🔍 **Reveal on scroll** con animaciones escalonadas

---

## 🚀 Puesta en marcha

No requiere instalación ni servidor. Basta con clonar el repositorio y abrir el archivo en el navegador:

```bash
git clone https://github.com/tu-usuario/convivencia-escolar.git
cd convivencia-escolar
# Abrir index.html en el navegador
open index.html   # macOS
start index.html  # Windows
```

Para una experiencia completa con los vídeos locales, se recomienda servirlo con un servidor local sencillo:

```bash
# Con Python
python -m http.server 8000

# Con Node.js (npx)
npx serve .
```

Luego visita `http://localhost:8000` en el navegador.

---

## 📁 Añadir imágenes y vídeos

Coloca los archivos en `assets/img/` y `assets/video/` respetando los nombres indicados en la tabla de estructura. Si una imagen no existe, el sitio muestra automáticamente un **placeholder** sin romper el diseño.

---

## 📝 Personalización rápida

| Qué cambiar | Dónde |
|-------------|-------|
| Nombre del centro | `<title>` y `.brand-title` en el `<header>` |
| Colores corporativos | Variables `:root` en `styles.css` |
| Textos de cada sección | Directamente en los bloques `<section>` de `index.html` |
| Enlace al blog | Atributo `href` del botón `.btn-blog` en la sección `#familia` |

---

## ♿ Accesibilidad

El sitio cumple con las pautas básicas de **WCAG 2.1 nivel AA**:

- Contraste de color superior a 4.5:1 en texto principal
- Todos los elementos interactivos tienen `aria-label` o texto visible
- Navegación completa por teclado (Tab, Escape, flechas en lightbox)
- Las animaciones se desactivan si el usuario activa `prefers-reduced-motion`

---

## 📄 Licencia

Proyecto de uso interno del **CEIP El Zahor**. Los contenidos (imágenes, vídeos y textos) pertenecen a la comunidad educativa del centro. El código puede reutilizarse libremente para otros centros educativos con fines no comerciales.

---

<div align="center">
  Hecho con dedicación por la comunidad educativa del <strong>CEIP El Zahor</strong> · 2025
</div>