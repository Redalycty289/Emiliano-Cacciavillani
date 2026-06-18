# Guía de Personalización - Reemplazo de Imágenes

## Estructura de Carpetas

Tu proyecto ahora tiene esta estructura para las imágenes:

```
proyecto/
├── images/
│   ├── hero/              (3 imágenes del slider principal)
│   ├── mision/            (1 foto de perfil)
│   ├── proyectos/         (9 imágenes: 3 proyectos x 3 imágenes c/u)
│   └── galeria/           (múltiples fotos de galería)
├── web_botanica.html      (tu archivo principal)
└── GUIA_IMAGENES.md       (este archivo)
```

---

## 1. SECCIÓN HERO - Slider (3 diapositivas)

**Ubicación en HTML:** Líneas 244-252 (en la sección `<style>`)

**Qué debes hacer:**
1. Coloca 3 imágenes en `/images/hero/`:
   - `slide-1.jpg` (Selva exuberante)
   - `slide-2.jpg` (Bosque verde)
   - `slide-3.jpg` (Bosque andino/terrestre)

2. **Reemplaza en el HTML estos estilos CSS:**

```css
/* CAMBIAR DE ESTO (líneas 244-252): */
.hero-slide:nth-child(1) {
  background: linear-gradient(135deg, #0d3b1f 0%, #1a5c35 40%, #2d8050 80%, #1a3a2a 100%);
}
.hero-slide:nth-child(2) {
  background: linear-gradient(135deg, #1a2e10 0%, #2d5a1e 40%, #4a8030 80%, #1f3b15 100%);
}
.hero-slide:nth-child(3) {
  background: linear-gradient(135deg, #2c1a0e 0%, #5c3a1e 40%, #8a5530 80%, #3d2512 100%);
}

/* A ESTO: */
.hero-slide:nth-child(1) {
  background-image: url('images/hero/slide-1.jpg');
}
.hero-slide:nth-child(2) {
  background-image: url('images/hero/slide-2.jpg');
}
.hero-slide:nth-child(3) {
  background-image: url('images/hero/slide-3.jpg');
}
```

---

## 2. SECCIÓN MISIÓN - Foto de Perfil

**Ubicación en HTML:** Líneas 1218-1233 (dentro del div `.mision-photo-inner`)

**Qué debes hacer:**
1. Coloca tu foto en `/images/mision/`:
   - `emiliano.jpg` (Foto de perfil, aspecto 4:5)

2. **Reemplaza el SVG con una imagen:**

```html
<!-- CAMBIAR DE ESTO (líneas 1218-1233): -->
<div class="mision-photo-inner">
  <svg viewBox="0 0 300 380">
    <!-- (aquí hay mucho código SVG) -->
  </svg>
</div>

<!-- A ESTO: -->
<div class="mision-photo-inner">
  <img src="images/mision/emiliano.jpg" alt="Emiliano Vargas - Fundador de Raíces Vivas" style="width:100%; height:100%; object-fit:cover;">
</div>
```

---

## 3. SECCIÓN PROYECTOS - Proyecto 1 (Amazonía)

**Ubicación en HTML:** Líneas 1306-1325

**Qué debes hacer:**
1. Coloca 4 imágenes en `/images/proyectos/`:
   - `proyecto-1-main.jpg` (imagen principal del proyecto)
   - `proyecto-1-thumb-1.jpg` (miniatura 1)
   - `proyecto-1-thumb-2.jpg` (miniatura 2)
   - `proyecto-1-thumb-3.jpg` (miniatura 3)

2. **Reemplaza la imagen principal (línea 1307):**

```html
<!-- CAMBIAR DE ESTO: -->
<div class="proyecto-visual-bg" style="background: linear-gradient(135deg,#1a5c35 0%,#2d8050 40%,#1a3a2a 100%);">

<!-- A ESTO: -->
<div class="proyecto-visual-bg" style="background-image: url('images/proyectos/proyecto-1-main.jpg'); background-size: cover; background-position: center;">
```

3. **Reemplaza las 3 miniaturas (líneas 1318-1320):**

```html
<!-- CAMBIAR DE ESTO: -->
<div class="gallery-thumb">
  <div class="gallery-thumb-inner"></div>
</div>
<div class="gallery-thumb">
  <div class="gallery-thumb-inner"></div>
</div>
<div class="gallery-thumb">
  <div class="gallery-thumb-inner"></div>
</div>

<!-- A ESTO: -->
<div class="gallery-thumb">
  <div class="gallery-thumb-inner" style="background-image: url('images/proyectos/proyecto-1-thumb-1.jpg'); background-size: cover; background-position: center;"></div>
</div>
<div class="gallery-thumb">
  <div class="gallery-thumb-inner" style="background-image: url('images/proyectos/proyecto-1-thumb-2.jpg'); background-size: cover; background-position: center;"></div>
</div>
<div class="gallery-thumb">
  <div class="gallery-thumb-inner" style="background-image: url('images/proyectos/proyecto-1-thumb-3.jpg'); background-size: cover; background-position: center;"></div>
</div>
```

---

## 4. SECCIÓN PROYECTOS - Proyecto 2 (Cusco - Bosque Andino)

**Ubicación en HTML:** Líneas 1379-1398

**Qué debes hacer:**
1. Coloca 4 imágenes en `/images/proyectos/`:
   - `proyecto-2-main.jpg`
   - `proyecto-2-thumb-1.jpg`
   - `proyecto-2-thumb-2.jpg`
   - `proyecto-2-thumb-3.jpg`

2. **Aplica los mismos cambios que en Proyecto 1:**
   - Reemplaza el `background` por `background-image: url('images/proyectos/proyecto-2-main.jpg')`
   - Reemplaza las 3 miniaturas con las URLs correspondientes

---

## 5. SECCIÓN PROYECTOS - Proyecto 3 (Tercera iniciativa)

**Ubicación en HTML:** Líneas 1452-1471

**Qué debes hacer:**
1. Coloca 4 imágenes en `/images/proyectos/`:
   - `proyecto-3-main.jpg`
   - `proyecto-3-thumb-1.jpg`
   - `proyecto-3-thumb-2.jpg`
   - `proyecto-3-thumb-3.jpg`

2. **Aplica los mismos cambios que en Proyectos 1 y 2**

---

## 6. SECCIÓN GALERÍA - Fotos de galería

**Ubicación en HTML:** Líneas ~1730+ (dentro de `.galeria-items`)

**Qué debes hacer:**
1. Coloca todas tus fotos de galería en `/images/galeria/`:
   - `foto-1.jpg` a `foto-N.jpg` (ajusta según cuántas tengas)

2. **Reemplaza cada item de galería:**

```html
<!-- CAMBIAR DE ESTO: -->
<div class="galeria-item"></div>

<!-- A ESTO (repite para cada foto): -->
<div class="galeria-item" style="background-image: url('images/galeria/foto-1.jpg'); background-size: cover; background-position: center;"></div>
<div class="galeria-item" style="background-image: url('images/galeria/foto-2.jpg'); background-size: cover; background-position: center;"></div>
<div class="galeria-item" style="background-image: url('images/galeria/foto-3.jpg'); background-size: cover; background-position: center;"></div>
<!-- ... más items -->
```

---

## Resumen de Archivos a Crear

| Carpeta | Cantidad | Nombres |
|---------|----------|---------|
| `hero/` | 3 | `slide-1.jpg`, `slide-2.jpg`, `slide-3.jpg` |
| `mision/` | 1 | `emiliano.jpg` |
| `proyectos/` | 12 | `proyecto-1-main.jpg`, `proyecto-1-thumb-1.jpg`, etc. |
| `galeria/` | 12+ | `foto-1.jpg`, `foto-2.jpg`, ... |

**Total mínimo: 28 imágenes**

---

## Tips

- **Formato:** JPG o PNG
- **Tamaño:** Optimiza las imágenes para web (< 500KB c/u idealmente)
- **Rutas:** Todas las imágenes deben referenciarse como `images/carpeta/archivo.jpg`
- **Alt text:** Si agregas `<img>` tags, siempre incluye atributos `alt`

¡Listo! Ahora solo sube tus imágenes a las carpetas correspondientes y reemplaza el código CSS y HTML según esta guía.
