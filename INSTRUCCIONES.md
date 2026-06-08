# 📖 INSTRUCCIONES — Portafolio Maleja Acevedo

## Archivos incluidos
```
maleja_portfolio/
├── index.html       → Página de inicio (con nombre, foto y botones)
├── portafolio.html  → Todo el contenido de tu portafolio
├── redes.html       → Links de Instagram y TikTok
├── contacto.html    → Botón de WhatsApp
└── styles.css       → Todos los estilos y colores
```

---

## ✏️ Cómo personalizar

### 1. Agregar tu foto (página de inicio)
Abre `index.html` y busca esta parte:
```html
<div class="photo-circle">
  <div class="photo-placeholder">
    <span>Tu Foto Aquí</span>
    ...
  </div>
</div>
```
Reemplázala con:
```html
<div class="photo-circle">
  <img src="mi-foto.jpg" alt="Maleja Acevedo" style="width:100%;height:100%;object-fit:cover;">
</div>
```
📌 Guarda tu foto en la misma carpeta y ponle el mismo nombre que escribiste en `src`.

---

### 2. Agregar tu video de presentación (portafolio)
Abre `portafolio.html` y busca el div `video-placeholder`. Reemplázalo con:

**Opción A — Video local (un archivo .mp4 en la misma carpeta):**
```html
<video controls style="width:100%;border-radius:14px;max-height:420px;">
  <source src="mi-video.mp4" type="video/mp4">
</video>
```

**Opción B — Video de YouTube:**
```html
<iframe
  src="https://www.youtube.com/embed/TU_ID_DE_VIDEO"
  style="width:100%;aspect-ratio:9/16;border-radius:14px;border:none;max-height:420px;"
  allowfullscreen>
</iframe>
```
(El ID de YouTube es lo que va después de `v=` en el link)

**Opción C — Video de Instagram/TikTok:**
Usa el código de "Insertar" (Embed) que te da la propia plataforma y pégalo en lugar del bloque.

---

### 3. Agregar tu foto de certificado (portafolio)
Busca en `portafolio.html` el bloque `cert-placeholder` y reemplaza el contenido por:
```html
<img src="certificado.jpg" alt="Certificado" style="width:100%;border-radius:14px;max-width:500px;">
```

---

### 4. Agregar casos de éxito y comentarios
En `portafolio.html`, cada `media-card` es un espacio. Puedes reemplazarlos con:

**Video:**
```html
<div class="media-card">
  <video controls style="width:100%;border-radius:12px;">
    <source src="caso1.mp4" type="video/mp4">
  </video>
</div>
```

**Imagen de comentario (screenshot):**
```html
<div class="media-card">
  <img src="comentario1.jpg" alt="Comentario cliente" style="width:100%;border-radius:12px;">
</div>
```

---

### 5. Agregar métricas
Mismo proceso: reemplaza los bloques `metric-card` con capturas de pantalla de tus estadísticas.

---

### 6. Agregar logos de marcas
En `portafolio.html`, reemplaza cada `brand-card` con:
```html
<div class="brand-card" style="background:white;padding:16px;border-radius:12px;">
  <img src="logo-marca.png" alt="Nombre Marca" style="width:100%;object-fit:contain;max-height:80px;">
</div>
```

---

### 7. Tu link de Instagram
Abre `redes.html` y reemplaza las dos apariciones de `TU_USUARIO_AQUI` con tu usuario real:
- En el `href`: `https://www.instagram.com/maleja.acevedo`
- En el texto del botón: `@maleja.acevedo`

---

### 8. Tu link de TikTok
Igual que Instagram, misma sección `redes.html`.

---

### 9. Tu número de WhatsApp
Abre `contacto.html` y reemplaza:
```
57TUNUMERODETELEFONO
```
Con tu número completo con código de país, sin espacios ni signos. Ejemplo:
```
573001234567
```

---

## 🌐 Cómo subir a internet (GRATIS)

### Opción 1 — Netlify (la más fácil, recomendada)
1. Ve a [https://netlify.com](https://netlify.com)
2. Crea una cuenta gratis (puedes entrar con Google)
3. En tu panel, busca la zona que dice **"Drag & Drop"** o **"Deploy manually"**
4. Arrastra toda la carpeta `maleja_portfolio` a esa zona
5. ¡Listo! En segundos te dan un link como `https://maleja-acevedo.netlify.app`
6. En Settings > Domain puedes personalizar el nombre del subdominio gratis

### Opción 2 — GitHub Pages
1. Crea cuenta en [https://github.com](https://github.com)
2. Crea un repositorio nuevo (botón verde "New")
3. Sube todos los archivos de la carpeta
4. Ve a Settings > Pages > Source: Main branch
5. Tu sitio queda en `https://TU-USUARIO.github.io/NOMBRE-REPO`

### Opción 3 — Tiiny.host (la más rápida, sin registro)
1. Ve a [https://tiiny.host](https://tiiny.host)
2. Comprime la carpeta en un ZIP
3. Arrástralo a la página
4. Te da un link inmediatamente (gratis por 24h, con cuenta gratis por más tiempo)

---

## 🎨 Cambiar colores
Si algún día quieres cambiar la paleta, todos los colores están en las primeras líneas de `styles.css`:
```css
:root {
  --cream:    #FFF3EB;   /* fondo principal */
  --sand:     #F7E1D2;   /* fondo secciones */
  --blush:    #E9B79A;   /* bordes y detalles */
  --terracota:#C76E4E;   /* color principal */
  --dark-terra:#7A3E2E;  /* títulos y oscuro */
}
```

---

¡Mucho éxito con tu portafolio! 🌟
