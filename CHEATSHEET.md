# CHEATSHEET - Guía Rápida de Reemplazo

## 🎯 Lo que necesitas hacer (resumido)

**1. Coloca 28+ imágenes en las carpetas correspondientes**
**2. Reemplaza el código CSS y HTML con URLs a tus imágenes**
**3. Guarda y abre en navegador**

---

## 📁 Estructura de carpetas (YA CREADA)

```
proyecto/
├── images/
│   ├── hero/        ← 3 imágenes
│   ├── mision/      ← 1 imagen
│   ├── proyectos/   ← 12 imágenes
│   └── galeria/     ← 6+ imágenes
└── web_botanica.html
```

---

## 🖼️ Imágenes que necesitas

| Ubicación | Archivo | Cantidad | Tamaño aprox |
|-----------|---------|----------|-------------|
| Hero | `slide-1.jpg`, `slide-2.jpg`, `slide-3.jpg` | 3 | 1920x1080 |
| Misión | `emiliano.jpg` | 1 | 600x750 |
| Proyectos | `proyecto-{1,2,3}-main.jpg` | 3 | 1200x800 |
| Proyectos | `proyecto-{1,2,3}-thumb-{1,2,3}.jpg` | 9 | 200x150 |
| Galería | `foto-1.jpg` ... `foto-N.jpg` | 6+ | 800x600+ |

---

## 🔧 Reemplazos de Código

### HERO (líneas 244-252)

```diff
- .hero-slide:nth-child(1) {
-   background: linear-gradient(135deg, #0d3b1f 0%, ...);
- }

+ .hero-slide:nth-child(1) {
+   background-image: url('images/hero/slide-1.jpg');
+ }

- .hero-slide:nth-child(2) {
-   background: linear-gradient(135deg, #1a2e10 0%, ...);
- }

+ .hero-slide:nth-child(2) {
+   background-image: url('images/hero/slide-2.jpg');
+ }

- .hero-slide:nth-child(3) {
-   background: linear-gradient(135deg, #2c1a0e 0%, ...);
- }

+ .hero-slide:nth-child(3) {
+   background-image: url('images/hero/slide-3.jpg');
+ }
```

---

### MISIÓN (líneas 1218-1233)

```diff
- <div class="mision-photo-inner">
-   <svg viewBox="0 0 300 380">...</svg>
- </div>

+ <div class="mision-photo-inner">
+   <img src="images/mision/emiliano.jpg" alt="Emiliano Vargas" 
+        style="width:100%; height:100%; object-fit:cover;">
+ </div>
```

---

### PROYECTO 1 - Imagen Principal (línea 1307)

```diff
- <div class="proyecto-visual-bg" 
-      style="background: linear-gradient(135deg,#1a5c35 0%,...);"> 

+ <div class="proyecto-visual-bg" 
+      style="background-image: url('images/proyectos/proyecto-1-main.jpg'); 
+              background-size: cover; background-position: center;">
```

---

### PROYECTO 1 - Miniaturas (líneas 1318-1320)

```diff
- <div class="gallery-thumb">
-   <div class="gallery-thumb-inner"></div>
- </div>

+ <div class="gallery-thumb">
+   <div class="gallery-thumb-inner" 
+        style="background-image: url('images/proyectos/proyecto-1-thumb-1.jpg'); 
+                background-size: cover; background-position: center;"></div>
+ </div>

- <div class="gallery-thumb">
-   <div class="gallery-thumb-inner"></div>
- </div>

+ <div class="gallery-thumb">
+   <div class="gallery-thumb-inner" 
+        style="background-image: url('images/proyectos/proyecto-1-thumb-2.jpg'); 
+                background-size: cover; background-position: center;"></div>
+ </div>

- <div class="gallery-thumb">
-   <div class="gallery-thumb-inner"></div>
- </div>

+ <div class="gallery-thumb">
+   <div class="gallery-thumb-inner" 
+        style="background-image: url('images/proyectos/proyecto-1-thumb-3.jpg'); 
+                background-size: cover; background-position: center;"></div>
+ </div>
```

---

### PROYECTO 2 - Imagen Principal (línea 1381)

```diff
- background: linear-gradient(135deg,#2d5a1e 0%,...);

+ background-image: url('images/proyectos/proyecto-2-main.jpg'); 
+ background-size: cover; 
+ background-position: center;
```

**Miniaturas:** Igual que Proyecto 1, pero con `proyecto-2-thumb-{1,2,3}.jpg`

---

### PROYECTO 3 - Imagen Principal (línea 1454)

```diff
- background: linear-gradient(135deg,#5c3a1e 0%,...);

+ background-image: url('images/proyectos/proyecto-3-main.jpg'); 
+ background-size: cover; 
+ background-position: center;
```

**Miniaturas:** Igual que Proyecto 1, pero con `proyecto-3-thumb-{1,2,3}.jpg`

---

### GALERÍA (línea ~1730+)

```diff
- <div class="galeria-item"></div>
- <div class="galeria-item"></div>
- <div class="galeria-item"></div>

+ <div class="galeria-item" style="background-image: url('images/galeria/foto-1.jpg'); background-size: cover; background-position: center;"></div>
+ <div class="galeria-item" style="background-image: url('images/galeria/foto-2.jpg'); background-size: cover; background-position: center;"></div>
+ <div class="galeria-item" style="background-image: url('images/galeria/foto-3.jpg'); background-size: cover; background-position: center;"></div>
+ <div class="galeria-item" style="background-image: url('images/galeria/foto-4.jpg'); background-size: cover; background-position: center;"></div>
+ <div class="galeria-item" style="background-image: url('images/galeria/foto-5.jpg'); background-size: cover; background-position: center;"></div>
+ <div class="galeria-item" style="background-image: url('images/galeria/foto-6.jpg'); background-size: cover; background-position: center;"></div>
```

---

## 🔍 Búsquedas rápidas (Ctrl+F en tu editor)

| Qué buscar | Para encontrar |
|-----------|---|
| `.hero-slide:nth-child(1)` | Hero slides |
| `.mision-photo-inner` | Foto misión |
| `Consolidación de la Amazonía` | Proyecto 1 |
| `Bosque Andino de Cusco` | Proyecto 2 |
| `galeria-item` | Galería |

---

## ⚡ Patrón General

**Todos los reemplazos siguen este patrón:**

```html
<!-- DE: -->
<div style="background: linear-gradient(...)">

<!-- A: -->
<div style="background-image: url('images/carpeta/archivo.jpg'); background-size: cover; background-position: center;">
```

**O en CSS:**

```css
/* DE: */
.elemento {
  background: linear-gradient(...);
}

/* A: */
.elemento {
  background-image: url('images/carpeta/archivo.jpg');
}
```

---

## 📝 Archivo de documentación completa

Para explicación detallada, lee:
- **GUIA_IMAGENES.md** - Explicación paso a paso
- **EJEMPLOS_CODIGO.md** - Ejemplos completos de código
- **ESTRUCTURA_ARCHIVOS.txt** - Estructura y nombres de archivos

---

## ✅ Checklist de Finalización

```
☐ Imágenes preparadas (28+)
☐ Carpetas creadas (hero, mision, proyectos, galeria)
☐ Imágenes copiadas a carpetas
☐ web_botanica.html abierto en editor
☐ Reemplazos de Hero completados
☐ Reemplazo de Misión completado
☐ Reemplazos de Proyectos completados
☐ Reemplazo de Galería completado
☐ Archivo guardado
☐ Abierto en navegador y verificado
```

---

## 🎬 Inicio Rápido

1. **Lee:** `GUIA_IMAGENES.md`
2. **Prepara:** 28+ imágenes con nombres correctos
3. **Copia:** Imágenes a carpetas `images/`
4. **Abre:** `web_botanica.html` en tu editor
5. **Busca:** Usa Ctrl+F para encontrar qué cambiar
6. **Reemplaza:** Usa ejemplos de `EJEMPLOS_CODIGO.md`
7. **Guarda:** El archivo HTML
8. **Verifica:** Abre en navegador

---

## 🚀 ¡Listo!

Sigue estos pasos y tus imágenes aparecerán en el sitio. 🌿
