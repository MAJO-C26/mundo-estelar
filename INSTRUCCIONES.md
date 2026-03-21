# ⚡ VICKY.EXE — Guía de instalación en Netlify

## Estructura de archivos que necesitas subir:

```
vicky-app/
├── index.html          ← La app completa
├── manifest.json       ← Configuración PWA
├── service-worker.js   ← Para que funcione offline
├── netlify.toml        ← Configuración de Netlify
└── icons/
    ├── icon-192.png    ← Tu ícono (192x192 px)
    └── icon-512.png    ← Tu ícono (512x512 px)
```

---

## PASO 1 — Prepara los íconos

Toma el ícono que diseñaste y exporta 2 versiones:
- `icon-192.png` → 192 × 192 píxeles
- `icon-512.png` → 512 × 512 píxeles

Ponlos dentro de la carpeta `icons/`

---

## PASO 2 — Crea cuenta en Netlify (si no tienes)

1. Ve a **netlify.com**
2. Clic en "Sign up"
3. Regístrate con Google o correo — es gratis

---

## PASO 3 — Sube la app (método fácil, sin código)

1. Entra a **app.netlify.com**
2. En el panel principal verás una zona que dice:
   **"Want to deploy a new site without connecting to Git? Drag and drop your site output folder here"**
3. Arrastra toda la carpeta `vicky-app/` a esa zona
4. ¡Listo! Netlify te dará una URL como `https://nombre-aleatorio.netlify.app`

---

## PASO 4 — Cambia el nombre del sitio (opcional)

1. Ve a **Site configuration → Site details → Change site name**
2. Ponle algo como `vicky-exe` → quedará como `https://vicky-exe.netlify.app`

---

## PASO 5 — Instalar como app en el teléfono

### Android (Chrome):
1. Abre la URL en Chrome
2. Aparecerá un banner abajo que dice "Instalar app" → toca "Instalar"
3. Si no aparece: menú (⋮) → "Añadir a pantalla de inicio"

### iPhone (Safari):
1. Abre la URL en Safari (importante: no Chrome)
2. Toca el botón de compartir (□↑)
3. Desplázate y toca "Añadir a pantalla de inicio"
4. Ponle el nombre "VICKY.EXE" → "Añadir"

---

## ✅ Ya está instalada como app

- Funciona sin internet (offline) gracias al service worker
- Guarda todos los datos en el teléfono de Vicky
- Se ve como app nativa, sin barra del navegador
- El ícono aparece en la pantalla de inicio

---

## 🔄 Cómo actualizar la app en el futuro

Si quieres hacer cambios:
1. Edita el `index.html`
2. En Netlify → tu sitio → Deploys → arrastra la carpeta nueva
3. La app se actualiza automáticamente

---

**PIN de admin: 2601** (guárdalo bien 🔐)
