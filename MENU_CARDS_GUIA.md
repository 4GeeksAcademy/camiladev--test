# Guía de Tarjetas de Menú - Green Leaf Restaurant

## 📋 Descripción General

Sistema de tarjetas reutilizables para mostrar platos del menú. Incluye múltiples variaciones y es completamente responsive.

---

## 🎨 Características Principales

✅ **Efecto Hover** - Las tarjetas se elevan y la imagen hace zoom
✅ **Sombras Suaves** - Diseño elegante y orgánico
✅ **Bordes Redondeados** - Esquinas suaves (12px)
✅ **Espaciado Limpio** - Basado en sistema de espacios consistente
✅ **Completamente Responsive** - Se adapta a cualquier dispositivo

---

## 📱 Variaciones de Diseño

### 1. **Tarjeta Vertical Estándar** (Por defecto)

```html
<article class="menu-card">
    <div class="menu-card-image">
        <img src="imagen.jpg" alt="Descripción">
    </div>
    <div class="menu-card-content">
        <h3 class="menu-card-title">Nombre del Plato</h3>
        <p class="menu-card-description">Descripción del plato...</p>
        <div class="menu-card-footer">
            <div class="menu-card-price">
                <span class="menu-card-price-label">Precio</span>
                <span class="menu-card-price-value">$14.99</span>
            </div>
            <button class="menu-card-button">Añadir al carrito</button>
        </div>
    </div>
</article>
```

### 2. **Tarjeta con Badge**

Agrega badges para destacar información especial:

```html
<div class="menu-card-image">
    <img src="imagen.jpg" alt="Plato">
    <span class="menu-card-badge vegan">100% Vegano</span>
</div>
```

**Tipos de Badge:**
- `.menu-card-badge.vegan` - Verde (100% Vegano)
- `.menu-card-badge.popular` - Dorado (Favorito)
- `.menu-card-badge.new` - Naranja (Nuevo)

### 3. **Tarjeta Destacada**

```html
<article class="menu-card featured">
    <!-- contenido -->
</article>
```

Agrega un borde verde claro para destacar platos especiales.

### 4. **Tarjeta Horizontal**

Para una vista más compacta en listados grandes:

```html
<article class="menu-card horizontal">
    <div class="menu-card-image">
        <img src="imagen.jpg" alt="Plato">
    </div>
    <div class="menu-card-content">
        <!-- contenido -->
    </div>
</article>
```

En móvil, se convierte automáticamente a vertical.

### 5. **Tarjeta Deshabilitada**

```html
<article class="menu-card disabled">
    <!-- contenido -->
</article>
```

Muestra "No disponible" sobre la tarjeta y reduce la opacidad.

---

## 📊 Información Nutricional Adicional

Incluye información importante con iconos:

```html
<div class="menu-card-info">
    <div class="menu-card-info-item">
        <span class="menu-card-info-icon">🌱</span>
        <span>Vegano</span>
    </div>
    <div class="menu-card-info-item">
        <span class="menu-card-info-icon">⭐</span>
        <span>Orgánico</span>
    </div>
    <div class="menu-card-info-item">
        <span class="menu-card-info-icon">💪</span>
        <span>Proteína</span>
    </div>
</div>
```

---

## 💰 Precios

### Precio Simple
```html
<div class="menu-card-price">
    <span class="menu-card-price-label">Precio</span>
    <span class="menu-card-price-value">$14.99</span>
</div>
```

### Precio con Descuento
```html
<div class="menu-card-price">
    <span class="menu-card-price-label">Precio</span>
    <span class="menu-card-price-value">$14.99</span>
    <span class="menu-card-price-original">$19.99</span>
</div>
```

Muestra el precio original tachado en gris.

---

## 🔘 Botones

Tipos de botones en tarjetas:

```html
<!-- Botón estándar -->
<button class="menu-card-button">Añadir al carrito</button>

<!-- Botons con diferentes estilos -->
<button class="menu-card-button">Ordenar Ahora</button>
<button class="menu-card-button">Añadir</button>
```

---

## 📐 Sistema de Grid

### Contenedor con Grid Automático

```html
<div class="menu-cards-container">
    <!-- Tarjetas -->
</div>
```

Adapta automáticamente el número de columnas según el ancho.

### Grid de 2 Columnas

```html
<div class="menu-cards-container grid-2">
    <!-- Tarjetas -->
</div>
```

### Grid de 3 Columnas

```html
<div class="menu-cards-container grid-3">
    <!-- Tarjetas -->
</div>
```

---

## 📱 Puntos de Quiebre Responsive

| Dispositivo | Ancho | Columnas | Tamaño Imagen |
|-------------|-------|----------|---------------|
| Desktop | 1200px+ | 3 | 220px |
| Tablet | 768px-1199px | 2 | 200px |
| Móvil | 480px-767px | 1 | 180px |
| Móvil pequeño | <480px | 1 | 160px |

---

## 🎯 Ejemplo Completo de Sección

```html
<section>
    <div class="container">
        <h2>Nuestro Menú</h2>
        <div class="menu-cards-container grid-3">
            
            <article class="menu-card">
                <div class="menu-card-image">
                    <img src="ensalada.jpg" alt="Ensalada Verde">
                    <span class="menu-card-badge vegan">100% Vegano</span>
                </div>
                <div class="menu-card-content">
                    <h3 class="menu-card-title">Ensalada Verde Fresca</h3>
                    <div class="menu-card-info">
                        <div class="menu-card-info-item">
                            <span class="menu-card-info-icon">🌱</span>
                            <span>Orgánico</span>
                        </div>
                    </div>
                    <p class="menu-card-description">Lechugas frescas con aliño de limón y aceite de oliva.</p>
                    <div class="menu-card-divider"></div>
                    <div class="menu-card-footer">
                        <div class="menu-card-price">
                            <span class="menu-card-price-label">Precio</span>
                            <span class="menu-card-price-value">$12.99</span>
                        </div>
                        <button class="menu-card-button">Añadir al carrito</button>
                    </div>
                </div>
            </article>
            
            <!-- Más tarjetas aquí -->
            
        </div>
    </div>
</section>
```

---

## 🎨 Variables CSS Personalizables

Edita estas variables en `:root` para cambiar colores:

```css
:root {
    /* Colores principales */
    --color-dark-green: #1a5c3a;
    --color-forest-green: #2d7a4a;
    --color-sage-green: #6b9d7d;
    
    /* Tonos tierra */
    --color-earth-orange: #d4714d;
    --color-natural-gold: #c9a961;
    
    /* Espaciado */
    --spacing-lg: 24px;
    --spacing-xl: 32px;
    
    /* Bordes */
    --border-radius-lg: 12px;
    
    /* Sombras */
    --shadow-md: 0 4px 12px rgba(26, 92, 58, 0.1);
    --shadow-xl: 0 12px 32px rgba(26, 92, 58, 0.15);
}
```

---

## 🎭 Efectos Hover

- **Elevación**: Las tarjetas suben 8px
- **Sombra**: Aumenta de `shadow-md` a `shadow-xl`
- **Zoom de Imagen**: 8% de zoom en la imagen
- **Botón**: Cambia color y se desplaza 2px

---

## ♿ Accesibilidad

- Soporte para `:focus-visible` en botones
- Contraste de colores optimizado
- Atributos `alt` en imágenes
- Semántica HTML con `<article>`

---

## 📦 Clase CSS Completa

```
.menu-card
├── .menu-card-image
│   ├── img
│   └── .menu-card-badge (opcional)
├── .menu-card-content
│   ├── .menu-card-title
│   ├── .menu-card-info (opcional)
│   │   └── .menu-card-info-item
│   ├── .menu-card-description
│   ├── .menu-card-divider (opcional)
│   └── .menu-card-footer
│       ├── .menu-card-price
│       │   ├── .menu-card-price-label
│       │   ├── .menu-card-price-value
│       │   └── .menu-card-price-original (opcional)
│       └── .menu-card-button
```

---

## 💡 Tips y Buenas Prácticas

1. **Imágenes**: Usa imágenes de 400x300px para mejor calidad
2. **Descripciones**: Mantén descripciones cortas (1-2 líneas)
3. **Precios**: Formatea siempre con símbolo de moneda
4. **Badges**: Usa solo un badge por tarjeta
5. **Grid**: En desktop usa `grid-3`, en landing pages usa automático
6. **Alt text**: Siempre incluye descripciones útiles para accesibilidad

---

## 🔗 Archivos Relacionados

- `css/style.css` - Estilos completos
- `menu-cards-example.html` - Ejemplos prácticos
- `index.html` - Landing page principal

---

## 📝 Changelog

### v1.0 (Inicial)
- Sistema base de tarjetas de menú
- Variaciones: vertical, horizontal, featured, disabled
- Badges: vegan, popular, new
- Información nutricional
- Precios simples y con descuento
- Grid responsivo 1-3 columnas
- Efectos hover suave
- Diseño orgánico y natural
