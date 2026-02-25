# Proyectos C — PWA

## Archivos incluidos

```
proyectos-c-pwa/
├── index.html       ← App principal
├── manifest.json    ← Manifiesto PWA
├── sw.js            ← Service Worker (offline)
├── icon-192.svg     ← Icono app 192×192
├── icon-512.svg     ← Icono app 512×512
└── README.md        ← Este archivo
```

## Cómo instalar en el móvil

### Opción A — Hosting gratuito (recomendado)

1. Sube todos los archivos a **GitHub Pages**, **Netlify** o **Vercel**
2. Abre la URL en Chrome (Android) o Safari (iOS)
3. Android: aparecerá un banner automático "Instalar app"
4. iOS: pulsa el botón compartir → "Añadir a pantalla de inicio"

### Opción B — Servidor local para pruebas

```bash
# Con Python
python3 -m http.server 8080

# Con Node.js
npx serve .
```

Abre `http://localhost:8080` y desde ahí puedes probar el modo offline.

## Características PWA

- ✅ Funciona 100% offline una vez cargada por primera vez
- ✅ Instalable en pantalla de inicio (Android & iOS)
- ✅ Barra de estado adaptada al diseño oscuro
- ✅ Safe area para notch / barra de inicio del iPhone
- ✅ Vibración háptica al marcar tareas (Android)
- ✅ Banner de estado offline
- ✅ Progreso guardado en localStorage
- ✅ Responsive para móvil, tablet y escritorio

## Nota importante

La PWA **requiere HTTPS** para funcionar (el service worker no se activa en HTTP plano, excepto en localhost). Usa GitHub Pages o Netlify para tener HTTPS gratis.
