# 🎨 Sass Framework

Un framework CSS moderno y completo construido con Sass que proporciona componentes reutilizables, utilidades flexibles y un sistema de grid responsive.

## ✨ Características

- **🎯 Sistema de variables completo** - Colores, tipografías, espaciado y más
- **🧩 Componentes reutilizables** - Botones, tarjetas, formularios, modales
- **📱 Totalmente responsive** - Grid system y breakpoints modernos
- **🎭 Animaciones suaves** - Transiciones y animaciones CSS optimizadas
- **🔧 Utilidades flexibles** - Clases helper para desarrollo rápido
- **⚡ Performance optimizado** - CSS comprimido y eficiente
- **🎨 Fácil personalización** - Variables Sass para personalización completa

## 🚀 Instalación

### Prerrequisitos

- Node.js (versión 14 o superior)
- npm o yarn

### Pasos de instalación

1. **Clona el repositorio**
   ```bash
   git clone https://github.com/tuusuario/sass-framework.git
   cd sass-framework
   ```

2. **Instala las dependencias**
   ```bash
   npm install
   ```

3. **Compila el CSS**
   ```bash
   npm run build
   ```

4. **Inicia el servidor de desarrollo**
   ```bash
   npm start
   ```

## 📁 Estructura del Proyecto

```
sass-framework/
├── scss/
│   ├── main.scss              # Archivo principal
│   ├── base/
│   │   ├── _variables.scss    # Variables globales
│   │   ├── _reset.scss        # Reset CSS
│   │   ├── _typography.scss   # Estilos de tipografía
│   │   └── _global.scss       # Estilos globales
│   ├── components/
│   │   ├── _buttons.scss      # Componentes de botones
│   │   ├── _cards.scss        # Componentes de tarjetas
│   │   ├── _forms.scss        # Componentes de formularios
│   │   └── _modal.scss        # Componentes de modales
│   ├── layout/
│   │   ├── _header.scss       # Estilos del header
│   │   ├── _navigation.scss   # Estilos de navegación
│   │   ├── _footer.scss       # Estilos del footer
│   │   └── _grid.scss         # Sistema de grid
│   └── utilities/
│       ├── _helpers.scss      # Clases helper
│       └── _animations.scss   # Animaciones
├── css/
│   └── main.css               # CSS compilado
├── js/
│   └── main.js                # JavaScript principal
├── images/                    # Imágenes del proyecto
├── index.html                 # Página de ejemplo
├── package.json               # Configuración de npm
└── README.md                  # Documentación
```

## 🎨 Variables Sass

### Colores

```scss
$primary-color: #3498db;
$secondary-color: #2ecc71;
$accent-color: #e74c3c;
$dark-color: #2c3e50;
$light-color: #ecf0f1;
$white: #ffffff;
$black: #000000;
```

### Tipografía

```scss
$font-family-primary: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
$font-size-base: 16px;
$line-height-base: 1.6;
```

### Breakpoints

```scss
$breakpoint-sm: 576px;
$breakpoint-md: 768px;
$breakpoint-lg: 992px;
$breakpoint-xl: 1200px;
$breakpoint-xxl: 1400px;
```

## 🧩 Componentes

### Botones

```html
<!-- Botones básicos -->
<button class="btn btn-primary">Primary</button>
<button class="btn btn-secondary">Secondary</button>
<button class="btn btn-accent">Accent</button>

<!-- Variantes -->
<button class="btn btn-outline-primary">Outline</button>
<button class="btn btn-ghost">Ghost</button>

<!-- Tamaños -->
<button class="btn btn-primary btn-sm">Small</button>
<button class="btn btn-primary btn-lg">Large</button>

<!-- Estados -->
<button class="btn btn-primary btn-loading">Loading</button>
<button class="btn btn-primary" disabled>Disabled</button>
```

### Tarjetas

```html
<!-- Tarjeta básica -->
<div class="card">
  <div class="card-header">
    <h4 class="card-title">Título de la tarjeta</h4>
  </div>
  <div class="card-body">
    <p class="card-text">Contenido de la tarjeta</p>
    <button class="btn btn-primary">Acción</button>
  </div>
</div>

<!-- Tarjeta con imagen -->
<div class="card">
  <img src="image.jpg" alt="Descripción" class="card-img-top">
  <div class="card-body">
    <h4 class="card-title">Tarjeta con imagen</h4>
    <p class="card-text">Descripción de la imagen</p>
  </div>
</div>

<!-- Variantes -->
<div class="card card-primary">...</div>
<div class="card card-secondary">...</div>
<div class="card card-accent">...</div>
```

### Formularios

```html
<form>
  <div class="form-group">
    <label for="name" class="form-label required">Nombre</label>
    <input type="text" id="name" class="form-control" placeholder="Tu nombre">
  </div>
  
  <div class="form-group">
    <label for="email" class="form-label">Email</label>
    <input type="email" id="email" class="form-control" placeholder="tu@email.com">
  </div>
  
  <div class="form-group">
    <label for="message" class="form-label">Mensaje</label>
    <textarea id="message" class="form-control" rows="4"></textarea>
  </div>
  
  <div class="form-check">
    <input type="checkbox" id="newsletter" class="form-check-input">
    <label for="newsletter" class="form-check-label">Newsletter</label>
  </div>
  
  <button type="submit" class="btn btn-primary">Enviar</button>
</form>
```

### Modales

```html
<!-- Trigger del modal -->
<button class="btn btn-primary" data-toggle="modal" data-target="#myModal">
  Abrir Modal
</button>

<!-- Modal -->
<div class="modal" id="myModal">
  <div class="modal-dialog modal-dialog-centered">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title">Título del Modal</h5>
        <button class="modal-close">&times;</button>
      </div>
      <div class="modal-body">
        <p>Contenido del modal</p>
      </div>
      <div class="modal-footer">
        <button class="btn btn-secondary" data-dismiss="modal">Cerrar</button>
        <button class="btn btn-primary">Guardar</button>
      </div>
    </div>
  </div>
</div>
```

## 📱 Sistema de Grid

```html
<!-- Container -->
<div class="container">
  <div class="row">
    <div class="col-12 col-md-6 col-lg-4">
      <!-- Contenido -->
    </div>
    <div class="col-12 col-md-6 col-lg-4">
      <!-- Contenido -->
    </div>
    <div class="col-12 col-md-6 col-lg-4">
      <!-- Contenido -->
    </div>
  </div>
</div>

<!-- Grid responsivo -->
<div class="row">
  <div class="col-sm-12 col-md-6 col-lg-3">Columna 1</div>
  <div class="col-sm-12 col-md-6 col-lg-3">Columna 2</div>
  <div class="col-sm-12 col-md-6 col-lg-3">Columna 3</div>
  <div class="col-sm-12 col-md-6 col-lg-3">Columna 4</div>
</div>
```

## 🎭 Animaciones

```html
<!-- Animaciones básicas -->
<div class="animate-fade-in">Aparece con fade</div>
<div class="animate-slide-in-up">Desliza hacia arriba</div>
<div class="animate-scale-in">Escala hacia adentro</div>

<!-- Animaciones con delay -->
<div class="animate-fade-in animate-delay-1">Delay 0.1s</div>
<div class="animate-fade-in animate-delay-2">Delay 0.2s</div>

<!-- Animaciones en hover -->
<div class="hover-scale">Escala al hacer hover</div>
<div class="hover-lift">Se eleva al hacer hover</div>
<div class="hover-glow">Brilla al hacer hover</div>

<!-- Animaciones al hacer scroll -->
<div class="animate-on-scroll">Aparece al hacer scroll</div>
```

## 🔧 Utilidades

### Espaciado

```html
<!-- Márgenes -->
<div class="m-0">Sin margen</div>
<div class="m-1">Margen pequeño</div>
<div class="m-2">Margen mediano</div>
<div class="m-3">Margen grande</div>

<!-- Padding -->
<div class="p-0">Sin padding</div>
<div class="p-1">Padding pequeño</div>
<div class="p-2">Padding mediano</div>
<div class="p-3">Padding grande</div>

<!-- Direccionales -->
<div class="mt-3">Margen superior</div>
<div class="mb-3">Margen inferior</div>
<div class="ml-3">Margen izquierdo</div>
<div class="mr-3">Margen derecho</div>
```

### Display y Flexbox

```html
<!-- Display -->
<div class="d-none">Oculto</div>
<div class="d-block">Bloque</div>
<div class="d-flex">Flex</div>
<div class="d-grid">Grid</div>

<!-- Flexbox -->
<div class="d-flex justify-content-center">Centrado</div>
<div class="d-flex align-items-center">Alineado vertical</div>
<div class="d-flex flex-column">Columna</div>
<div class="d-flex flex-wrap">Wrap</div>
```

### Colores y Fondos

```html
<!-- Colores de texto -->
<p class="text-primary">Texto primario</p>
<p class="text-secondary">Texto secundario</p>
<p class="text-accent">Texto de acento</p>
<p class="text-muted">Texto atenuado</p>

<!-- Fondos -->
<div class="bg-primary">Fondo primario</div>
<div class="bg-secondary">Fondo secundario</div>
<div class="bg-light">Fondo claro</div>
<div class="bg-dark">Fondo oscuro</div>
```

## 📝 Scripts Disponibles

```bash
# Compilar CSS comprimido
npm run build

# Compilar CSS expandido (para desarrollo)
npm run build:expanded

# Compilar y observar cambios
npm run watch

# Modo desarrollo (compilar + servidor)
npm run dev

# Iniciar servidor local
npm run serve

# Iniciar todo (desarrollo + servidor)
npm start

# Limpiar archivos CSS
npm run clean
```

## 🎨 Personalización

### Modificar Variables

Edita el archivo `scss/base/_variables.scss` para personalizar:

```scss
// Cambiar colores principales
$primary-color: #your-color;
$secondary-color: #your-color;
$accent-color: #your-color;

// Cambiar tipografía
$font-family-primary: 'Your Font', sans-serif;
$font-size-base: 18px;

// Cambiar breakpoints
$breakpoint-lg: 1024px;
```

### Agregar Nuevos Componentes

1. Crea un nuevo archivo en `scss/components/_tu-componente.scss`
2. Importa en `scss/main.scss`:
   ```scss
   @import 'components/tu-componente';
   ```

### Agregar Nuevas Utilidades

1. Crea un nuevo archivo en `scss/utilities/_tu-utilidad.scss`
2. Importa en `scss/main.scss`:
   ```scss
   @import 'utilities/tu-utilidad';
   ```

## 🌐 Navegadores Soportados

- Chrome (últimas 2 versiones)
- Firefox (últimas 2 versiones)
- Safari (últimas 2 versiones)
- Edge (últimas 2 versiones)
- Internet Explorer 11+

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 🤝 Contribuir

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📞 Soporte

Si tienes alguna pregunta o necesitas ayuda:

- 📧 Email: irvonm92@gmail.com

## 🙏 Agradecimientos

- [Inter Font](https://rsms.me/inter/) - Tipografía principal
- [Sass](https://sass-lang.com/) - Preprocesador CSS
- Comunidad de desarrolladores web

---

**¡Disfruta usando Sass Framework! 🎉** # Sass---fm
