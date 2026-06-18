# Ejemplos de Código - Reemplazos Rápidos

## Paso 1: Abre el archivo `web_botanica.html` con tu editor de texto

---

## HERO - Busca y Reemplaza (Líneas 244-252)

### Encuentra este bloque:

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

### Reemplázalo con esto:

```css
    /* Placeholder slides with gradient backgrounds */
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

## MISIÓN - Busca y Reemplaza (Líneas 1218-1233)

### Encuentra este bloque (busca por `<div class="mision-photo-inner">`):

```html
          <div class="mision-photo-inner">
            <svg viewBox="0 0 300 380">
              <defs>
                <pattern id="moss-pattern" x="0" y="0" width="30" height="30" patternUnits="userSpaceOnUse">
                  <circle cx="15" cy="15" r="3" fill="rgba(125,196,148,.3)" />
                  <path d="M15,12 Q18,10 20,12" stroke="rgba(125,196,148,.4)" stroke-width="0.5" fill="none" />
                </pattern>
              </defs>
              <!-- ... más SVG ... -->
            </svg>
          </div>
```

### Reemplázalo con esto:

```html
          <div class="mision-photo-inner">
            <img src="images/mision/emiliano.jpg" alt="Emiliano Vargas - Fundador de Raíces Vivas" style="width:100%; height:100%; object-fit:cover;">
          </div>
```

---

## PROYECTO 1 - Imagen Principal (Línea 1307)

### Encuentra este código:

```html
            <div class="proyecto-visual-bg" style="background: linear-gradient(135deg,#1a5c35 0%,#2d8050 40%,#1a3a2a 100%);">
```

### Reemplázalo con esto:

```html
            <div class="proyecto-visual-bg" style="background-image: url('images/proyectos/proyecto-1-main.jpg'); background-size: cover; background-position: center;">
```

---

## PROYECTO 1 - Miniaturas (Líneas 1318-1320)

### Encuentra estos 3 bloques vacíos:

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
```

### Reemplázalos con esto:

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
```

---

## PROYECTO 2 - Imagen Principal (Línea 1381)

### Encuentra este código:

```html
            <div class="proyecto-visual-bg" style="background: linear-gradient(135deg,#2d5a1e 0%,#4a8030 40%,#2d5a1e 100%);">
```

### Reemplázalo con esto:

```html
            <div class="proyecto-visual-bg" style="background-image: url('images/proyectos/proyecto-2-main.jpg'); background-size: cover; background-position: center;">
```

---

## PROYECTO 2 - Miniaturas (Líneas ~1392-1394)

### Reemplaza los 3 thumbnails vacíos:

```html
              <div class="gallery-thumb">
                <div class="gallery-thumb-inner" style="background-image: url('images/proyectos/proyecto-2-thumb-1.jpg'); background-size: cover; background-position: center;"></div>
              </div>
              <div class="gallery-thumb">
                <div class="gallery-thumb-inner" style="background-image: url('images/proyectos/proyecto-2-thumb-2.jpg'); background-size: cover; background-position: center;"></div>
              </div>
              <div class="gallery-thumb">
                <div class="gallery-thumb-inner" style="background-image: url('images/proyectos/proyecto-2-thumb-3.jpg'); background-size: cover; background-position: center;"></div>
              </div>
```

---

## PROYECTO 3 - Imagen Principal (Línea 1454)

### Encuentra este código:

```html
            <div class="proyecto-visual-bg" style="background: linear-gradient(135deg,#5c3a1e 0%,#8a5530 40%,#5c3a1e 100%);">
```

### Reemplázalo con esto:

```html
            <div class="proyecto-visual-bg" style="background-image: url('images/proyectos/proyecto-3-main.jpg'); background-size: cover; background-position: center;">
```

---

## PROYECTO 3 - Miniaturas (Líneas ~1465-1467)

### Reemplaza los 3 thumbnails vacíos:

```html
              <div class="gallery-thumb">
                <div class="gallery-thumb-inner" style="background-image: url('images/proyectos/proyecto-3-thumb-1.jpg'); background-size: cover; background-position: center;"></div>
              </div>
              <div class="gallery-thumb">
                <div class="gallery-thumb-inner" style="background-image: url('images/proyectos/proyecto-3-thumb-2.jpg'); background-size: cover; background-position: center;"></div>
              </div>
              <div class="gallery-thumb">
                <div class="gallery-thumb-inner" style="background-image: url('images/proyectos/proyecto-3-thumb-3.jpg'); background-size: cover; background-position: center;"></div>
              </div>
```

---

## GALERÍA - Items de galería (Línea ~1730+)

### Encuentra todos los items vacíos de galería:

```html
            <div class="galeria-item"></div>
            <div class="galeria-item"></div>
            <div class="galeria-item"></div>
            <!-- ... más items vacíos -->
```

### Reemplázalos con esto (ajusta la cantidad según tus fotos):

```html
            <div class="galeria-item" style="background-image: url('images/galeria/foto-1.jpg'); background-size: cover; background-position: center;"></div>
            <div class="galeria-item" style="background-image: url('images/galeria/foto-2.jpg'); background-size: cover; background-position: center;"></div>
            <div class="galeria-item" style="background-image: url('images/galeria/foto-3.jpg'); background-size: cover; background-position: center;"></div>
            <div class="galeria-item" style="background-image: url('images/galeria/foto-4.jpg'); background-size: cover; background-position: center;"></div>
            <div class="galeria-item" style="background-image: url('images/galeria/foto-5.jpg'); background-size: cover; background-position: center;"></div>
            <div class="galeria-item" style="background-image: url('images/galeria/foto-6.jpg'); background-size: cover; background-position: center;"></div>
            <!-- Agrega más cuantos necesites -->
```

---

## Checklist Final

- [ ] Creé carpetas: `images/hero/`, `images/mision/`, `images/proyectos/`, `images/galeria/`
- [ ] Subí 3 imágenes en `images/hero/`
- [ ] Subí 1 imagen en `images/mision/`
- [ ] Subí 12 imágenes en `images/proyectos/` (4 x 3 proyectos)
- [ ] Subí fotos en `images/galeria/`
- [ ] Reemplacé el CSS de hero slides
- [ ] Reemplacé el SVG de misión con `<img>`
- [ ] Reemplacé imágenes principales de 3 proyectos
- [ ] Reemplacé miniaturas de 3 proyectos
- [ ] Reemplacé items de galería
- [ ] Guardé el archivo `web_botanica.html`

¡Listo! Abre el archivo en tu navegador para ver los cambios.
