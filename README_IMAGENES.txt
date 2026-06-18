╔══════════════════════════════════════════════════════════════════════════════╗
║                                                                              ║
║                    PERSONALIZA TU WEB CON IMÁGENES REALES                   ║
║                                                                              ║
║              Guía Completa para Reemplazar Placeholders de Imágenes         ║
║                                                                              ║
╚══════════════════════════════════════════════════════════════════════════════╝


📖 LEE ESTO PRIMERO
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Tu proyecto web está listo para agregar imágenes reales. 

Tienes 4 opciones de cómo aprender a hacerlo:

1. QUICK_REFERENCE.txt      ← Resumen RÁPIDO (1 página, lo esencial)
2. REEMPLAZAR_EXACTAMENTE.md ← Guía PASO A PASO (muy detallada)
3. LINEAS_EXACTAS.txt        ← Números de LÍNEA específicos del HTML
4. Este README               ← Explicación general


🚀 EMPEZAR RÁPIDO (5 minutos)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

1. Lee: QUICK_REFERENCE.txt

2. Crea estas carpetas en tu proyecto:
   • images/hero/
   • images/mision/
   • images/proyectos/
   • images/galeria/

3. Prepara 28 imágenes con los nombres exactos:
   • 3 imágenes del slider hero
   • 1 foto de perfil de misión
   • 12 imágenes de proyectos (4 por proyecto)
   • 6 imágenes de galería

4. Abre web_botanica.html con tu editor de texto

5. Usa Buscar y Reemplazar (Ctrl+H):
   • Busca el código VIEJO
   • Reemplaza con el código NUEVO
   • Guarda (Ctrl+S)

6. ¡Listo! Abre en navegador


📊 LISTA DE ARCHIVOS A CREAR
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Total: 28 imágenes distribuidas en 4 carpetas


CARPETA: images/hero/
────────────────────
✓ hero-slide-1.jpg        (1920x1080) - Slide 1 del slider
✓ hero-slide-2.jpg        (1920x1080) - Slide 2 del slider
✓ hero-slide-3.jpg        (1920x1080) - Slide 3 del slider


CARPETA: images/mision/
───────────────────────
✓ emiliano-perfil.jpg     (600x750)   - Foto del perfil


CARPETA: images/proyectos/
──────────────────────────
✓ proyecto-1-principal.jpg  (800x600)  - Imagen grande Proyecto 1
✓ proyecto-1-thumb-1.jpg    (52x40)    - Miniatura 1
✓ proyecto-1-thumb-2.jpg    (52x40)    - Miniatura 2
✓ proyecto-1-thumb-3.jpg    (52x40)    - Miniatura 3
✓ proyecto-1-thumb-4.jpg    (52x40)    - Miniatura 4

✓ proyecto-2-principal.jpg  (800x600)  - Imagen grande Proyecto 2
✓ proyecto-2-thumb-1.jpg    (52x40)    - Miniatura 1
✓ proyecto-2-thumb-2.jpg    (52x40)    - Miniatura 2
✓ proyecto-2-thumb-3.jpg    (52x40)    - Miniatura 3
✓ proyecto-2-thumb-4.jpg    (52x40)    - Miniatura 4

✓ proyecto-3-principal.jpg  (800x600)  - Imagen grande Proyecto 3
✓ proyecto-3-thumb-1.jpg    (52x40)    - Miniatura 1
✓ proyecto-3-thumb-2.jpg    (52x40)    - Miniatura 2
✓ proyecto-3-thumb-3.jpg    (52x40)    - Miniatura 3
✓ proyecto-3-thumb-4.jpg    (52x40)    - Miniatura 4


CARPETA: images/galeria/
────────────────────────
✓ galeria-1.jpg           (variable) - Foto galería 1
✓ galeria-2.jpg           (variable) - Foto galería 2
✓ galeria-3.jpg           (variable) - Foto galería 3
✓ galeria-4.jpg           (variable) - Foto galería 4
✓ galeria-5.jpg           (variable) - Foto galería 5
✓ galeria-6.jpg           (variable) - Foto galería 6


💡 TIPS IMPORTANTES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✓ Optimiza las imágenes primero en: https://tinypng.com
  • Las imágenes grandes deben ser < 500 KB
  • Las miniaturas < 50 KB

✓ Nombra los archivos exactamente como se indica (sin espacios)

✓ Todas las rutas deben ser: images/carpeta/archivo.jpg

✓ No uses MAYÚSCULAS en nombres de archivos (salvo extensión)

✓ Guarda el HTML después de cambios (Ctrl+S)

✓ Abre en navegador y verifica cada sección


⚠️ SI ALGO NO FUNCIONA
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Problema: La imagen no aparece

Solución:
1. Verifica que el archivo existe en la carpeta correcta
2. Comprueba que el nombre es exactamente igual (sin espacios)
3. Verifica que usaste la ruta correcta: images/carpeta/archivo.jpg
4. Abre la consola del navegador (F12) y busca errores 404
5. Limpia el caché del navegador (Ctrl+Shift+Del)


📝 CHEAT SHEET - COPY & PASTE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Formato para imágenes de fondo:
────────────────────────────────
background-image: url('images/carpeta/archivo.jpg');
background-size: cover;
background-position: center;


Formato para imágenes (<img>):
──────────────────────────────
<img src="images/carpeta/archivo.jpg" 
     alt="Descripción de la imagen"
     style="width: 100%; height: 100%; object-fit: cover;">


📚 DOCUMENTACIÓN INCLUIDA
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

En tu proyecto encontrarás:

📄 QUICK_REFERENCE.txt
   → Resumen visual de 1 página con todo lo que necesitas
   → Usa esto si tienes prisa

📄 REEMPLAZAR_EXACTAMENTE.md
   → Guía detallada paso a paso
   → Incluye ejemplos de código
   → Usa esto si quieres entender todo

📄 LINEAS_EXACTAS.txt
   → Números de línea específicos donde buscar
   → Usa esto si tienes dudas de dónde está cada cosa

📄 ESTRUCTURA_ARCHIVOS.txt
   → Listado completo de archivos

📄 Este README
   → Visión general y tips


🎯 PRÓXIMOS PASOS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

1. Lee QUICK_REFERENCE.txt (5 minutos)
2. Crea las carpetas de imágenes
3. Prepara 28 imágenes
4. Abre web_botanica.html
5. Busca y reemplaza siguiendo la guía
6. Guarda
7. Verifica en navegador
8. ¡Listo!


Si tienes dudas, revisa los archivos de documentación incluidos.

¡Buena suerte! 🌿

════════════════════════════════════════════════════════════════════════════════
