# 🎯 REEMPLAZAR EXACTAMENTE ESTO EN web_botanica.html

## PASO A PASO: Busca y Reemplaza en tu editor de texto

---

## 📌 SECCIÓN 1: HERO - SLIDER (3 Diapositivas)

### Paso 1: Nombra tus imágenes así:
```
images/hero/
├── hero-slide-1.jpg   (Selva/naturaleza exuberante - 1920x1080)
├── hero-slide-2.jpg   (Bosque verde - 1920x1080)
└── hero-slide-3.jpg   (Bosque andino - 1920x1080)
```

### Paso 2: Busca esto en el HTML (línea ~244-252):
```css
    /* Placeholder slides with gradient backgrounds */
    .hero-slide:nth-child(1) {
      background: linear-gradient(135deg, #0d3b1f 0%, #1a5c35 40%, #2d8050 80%, #1a3a2a 100%);
    }
    .hero-slide:nth-child(2) {
      background: linear-gradient(135deg, #1a2e10 0%, #2d5a1e 40%, #4a8030 80%, #1f3b15 100%);
    }
    .hero-slide:nth-child(3) {
      background: linear-gradient(135deg, #2c1a0e 0%, #5c3a1e 40%, #8a5530 80%, #3d2512 100%);
    }
```

### Paso 3: Reemplázalo con ESTO:
```css
    /* Hero slides with background images */
    .hero-slide:nth-child(1) {
      background-image: url('images/hero/hero-slide-1.jpg');
    }
    .hero-slide:nth-child(2) {
      background-image: url('images/hero/hero-slide-2.jpg');
    }
    .hero-slide:nth-child(3) {
      background-image: url('images/hero/hero-slide-3.jpg');
    }
```

---

## 📌 SECCIÓN 2: MISIÓN - FOTO DE PERFIL

### Paso 1: Nombra tu imagen así:
```
images/mision/
└── emiliano-perfil.jpg   (Foto vertical 600x750 aprox)
```

### Paso 2: Busca esto en el HTML (línea ~1218-1233):
```html
    <div class="mision-photo-inner">
      <svg viewBox="0 0 300 380">
        <rect width="300" height="380" fill="url(#grad-botanical)"></rect>
        <!-- ... más líneas SVG ... -->
      </svg>
    </div>
```

### Paso 3: Reemplázalo con ESTO:
```html
    <div class="mision-photo-inner">
      <img src="images/mision/emiliano-perfil.jpg" alt="Emiliano Vargas - Fundador de Raíces Vivas" style="width: 100%; height: 100%; object-fit: cover;">
    </div>
```

---

## 📌 SECCIÓN 3: PROYECTO 1 - AMAZONÍA

### Paso 1: Nombra tus imágenes así:
```
images/proyectos/
├── proyecto-1-principal.jpg      (Imagen grande 800x600)
├── proyecto-1-thumb-1.jpg        (Miniatura 52x40)
├── proyecto-1-thumb-2.jpg        (Miniatura 52x40)
├── proyecto-1-thumb-3.jpg        (Miniatura 52x40)
└── proyecto-1-thumb-4.jpg        (Miniatura 52x40)
```

### Paso 2: Busca esto en el HTML (línea ~1307):
```html
      <div class="proyecto-visual-bg" style="background: linear-gradient(135deg,#1a5c35 0%,#2d8050 40%,#1a3a2a 100%);"></div>
```

### Paso 3: Reemplázalo con ESTO:
```html
      <div class="proyecto-visual-bg" style="background-image: url('images/proyectos/proyecto-1-principal.jpg'); background-size: cover; background-position: center;"></div>
```

### Paso 4: Busca esto en el HTML (línea ~1318-1321):
```html
      <div class="gallery-thumb">
        <div class="gallery-thumb-inner"></div>
      </div>
      <div class="gallery-thumb">
        <div class="gallery-thumb-inner"></div>
      </div>
      <div class="gallery-thumb">
        <div class="gallery-thumb-inner"></div>
      </div>
      <div class="gallery-thumb">
        <div class="gallery-thumb-inner"></div>
      </div>
```

### Paso 5: Reemplázalo con ESTO:
```html
      <div class="gallery-thumb">
        <div class="gallery-thumb-inner" style="background-image: url('images/proyectos/proyecto-1-thumb-1.jpg'); background-size: cover; background-position: center;"></div>
      </div>
      <div class="gallery-thumb">
        <div class="gallery-thumb-inner" style="background-image: url('images/proyectos/proyecto-1-thumb-2.jpg'); background-size: cover; background-position: center;"></div>
      </div>
      <div class="gallery-thumb">
        <div class="gallery-thumb-inner" style="background-image: url('images/proyectos/proyecto-1-thumb-3.jpg'); background-size: cover; background-position: center;"></div>
      </div>
      <div class="gallery-thumb">
        <div class="gallery-thumb-inner" style="background-image: url('images/proyectos/proyecto-1-thumb-4.jpg'); background-size: cover; background-position: center;"></div>
      </div>
```

---

## 📌 SECCIÓN 4: PROYECTO 2 - BOSQUE ANDINO (CUSCO)

### Paso 1: Nombra tus imágenes así:
```
images/proyectos/
├── proyecto-2-principal.jpg      (Imagen grande 800x600)
├── proyecto-2-thumb-1.jpg        (Miniatura 52x40)
├── proyecto-2-thumb-2.jpg        (Miniatura 52x40)
├── proyecto-2-thumb-3.jpg        (Miniatura 52x40)
└── proyecto-2-thumb-4.jpg        (Miniatura 52x40)
```

### Paso 2: Busca esto en el HTML (línea ~1381):
```html
      <div class="proyecto-visual-bg" style="background: linear-gradient(135deg,#2d5a1e 0%,#3a8558 40%,#245238 100%);"></div>
```

### Paso 3: Reemplázalo con ESTO:
```html
      <div class="proyecto-visual-bg" style="background-image: url('images/proyectos/proyecto-2-principal.jpg'); background-size: cover; background-position: center;"></div>
```

### Paso 4: Busca y reemplaza sus 4 miniaturas (línea ~1392-1405) igual que en el Proyecto 1, usando:
- `proyecto-2-thumb-1.jpg`
- `proyecto-2-thumb-2.jpg`
- `proyecto-2-thumb-3.jpg`
- `proyecto-2-thumb-4.jpg`

---

## 📌 SECCIÓN 5: PROYECTO 3 (Si existe)

### Paso 1: Nombra tus imágenes así:
```
images/proyectos/
├── proyecto-3-principal.jpg      (Imagen grande 800x600)
├── proyecto-3-thumb-1.jpg        (Miniatura 52x40)
├── proyecto-3-thumb-2.jpg        (Miniatura 52x40)
├── proyecto-3-thumb-3.jpg        (Miniatura 52x40)
└── proyecto-3-thumb-4.jpg        (Miniatura 52x40)
```

### Paso 2: Busca el tercer `.proyecto-card` en el HTML (aproximadamente línea ~1454)

### Paso 3: Reemplaza exactamente igual que los anteriores

---

## 📌 SECCIÓN 6: GALERÍA AL FINAL

### Paso 1: Nombra tus imágenes así:
```
images/galeria/
├── galeria-1.jpg
├── galeria-2.jpg
├── galeria-3.jpg
├── galeria-4.jpg
├── galeria-5.jpg
└── galeria-6.jpg
```

### Paso 2: Busca esto en el HTML (línea ~1750+, busca `.galeria-item`):
```html
      <div class="galeria-item"></div>
      <div class="galeria-item"></div>
      <div class="galeria-item"></div>
      <div class="galeria-item"></div>
      <div class="galeria-item"></div>
      <div class="galeria-item"></div>
```

### Paso 3: Reemplázalo con ESTO:
```html
      <div class="galeria-item" style="background-image: url('images/galeria/galeria-1.jpg'); background-size: cover; background-position: center;"></div>
      <div class="galeria-item" style="background-image: url('images/galeria/galeria-2.jpg'); background-size: cover; background-position: center;"></div>
      <div class="galeria-item" style="background-image: url('images/galeria/galeria-3.jpg'); background-size: cover; background-position: center;"></div>
      <div class="galeria-item" style="background-image: url('images/galeria/galeria-4.jpg'); background-size: cover; background-position: center;"></div>
      <div class="galeria-item" style="background-image: url('images/galeria/galeria-5.jpg'); background-size: cover; background-position: center;"></div>
      <div class="galeria-item" style="background-image: url('images/galeria/galeria-6.jpg'); background-size: cover; background-position: center;"></div>
```

---

## ✅ RESUMEN DE CAMBIOS

| Sección | Qué Cambiar | Carpeta | Cantidad de Imágenes |
|---------|-------------|---------|----------------------|
| **Hero** | 3 gradients CSS | `images/hero/` | 3 |
| **Misión** | 1 SVG → 1 img | `images/mision/` | 1 |
| **Proyecto 1** | 1 gradient + 4 divs | `images/proyectos/` | 5 |
| **Proyecto 2** | 1 gradient + 4 divs | `images/proyectos/` | 5 |
| **Proyecto 3** | 1 gradient + 4 divs | `images/proyectos/` | 5 |
| **Galería** | 6 divs | `images/galeria/` | 6 |
| **TOTAL** | | | **28 imágenes** |

---

## 🔧 CÓMO HACER LOS CAMBIOS

### Opción 1: Con Buscar y Reemplazar (Recomendado)
1. Abre `web_botanica.html` en tu editor (VSCode, Sublime, Notepad++, etc)
2. Presiona: `Ctrl+H` (o `Cmd+H` en Mac)
3. En "Buscar" pega el código VIEJO
4. En "Reemplazar" pega el código NUEVO
5. Haz clic en "Reemplazar" (o "Reemplazar Todo")
6. Guarda: `Ctrl+S`

### Opción 2: Manual
1. Busca el código con `Ctrl+F`
2. Borra el código viejo
3. Escribe el código nuevo
4. Guarda: `Ctrl+S`

---

## 📋 CHECKLIST FINAL

- [ ] He creado la carpeta `images/`
- [ ] He creado las subcarpetas: `hero`, `mision`, `proyectos`, `galeria`
- [ ] He optimizado mis imágenes (comprimidas)
- [ ] He nombrado todas las imágenes exactamente como se indica
- [ ] He reemplazado los 3 slides del HERO
- [ ] He reemplazado la foto del MISION
- [ ] He reemplazado los proyectos (imágenes principales)
- [ ] He reemplazado los thumbnails de los proyectos
- [ ] He reemplazado la galería
- [ ] He guardado el archivo HTML
- [ ] He abierto en el navegador y verifico que aparecen las imágenes

---

## 🚀 ¡LISTO! Sigue estos pasos y tus imágenes aparecerán perfectamente.
