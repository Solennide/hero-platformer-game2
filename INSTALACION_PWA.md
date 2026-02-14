# 📱 Guía de Instalación - Hero Platformer PWA

## 🎯 ¿Qué es una PWA (Progressive Web App)?

Una PWA es una aplicación web que se comporta como una **app nativa**:

✅ Se instala en tu pantalla de inicio
✅ Funciona OFFLINE (sin internet)
✅ Pantalla completa (sin barra del navegador)
✅ Notificaciones (opcional)
✅ Acceso directo como cualquier app

## 📱 INSTALACIÓN EN IPHONE/IPAD

### Método 1: Desde Safari (Recomendado)

1. **Abre Safari** en tu iPhone/iPad
2. **Ve a tu sitio web** (ejemplo: https://tu-usuario.github.io/hero-platformer-pwa)
3. **Toca el botón de compartir** (📤) en la parte inferior
4. **Desplázate y selecciona** "Agregar a pantalla de inicio"
5. **Personaliza el nombre** (ejemplo: "Hero Game")
6. **Toca "Agregar"**

¡Listo! Ahora tienes un icono en tu pantalla de inicio.

### Método 2: Prompt Automático (iOS 16.4+)

Si usas iOS 16.4 o superior:

1. Abre el juego en Safari
2. Espera 3 segundos
3. Aparecerá un **mensaje verde** en la parte inferior
4. Toca **"Instalar"**
5. ¡Listo!

## 🤖 INSTALACIÓN EN ANDROID

### Opción 1: Chrome (Prompt Automático)

1. Abre **Chrome** en tu Android
2. Ve a tu sitio web
3. Espera 3 segundos
4. Aparecerá una **barra en la parte inferior** con "Agregar a pantalla de inicio"
5. Toca **"Agregar"**
6. Toca **"Instalar"**

### Opción 2: Menú Manual

1. Abre el juego en Chrome
2. Toca los **tres puntos** (⋮) arriba a la derecha
3. Selecciona **"Agregar a pantalla de inicio"** o **"Instalar app"**
4. Confirma tocando **"Agregar"**

## 💻 INSTALACIÓN EN ESCRITORIO

### Chrome/Edge (Windows/Mac/Linux)

1. Abre el juego en Chrome o Edge
2. Mira la **barra de direcciones** - verás un icono de instalación (+)
3. Haz clic en el icono
4. Click en **"Instalar"**

O alternativamente:
1. Click en los **tres puntos** (⋮) arriba a la derecha
2. Selecciona **"Instalar Hero Platformer Game"**
3. Confirma

## 🚀 PUBLICAR TU PWA EN INTERNET

### Opción 1: GitHub Pages (Gratis y Fácil)

```bash
# 1. Subir a GitHub
cd hero-platformer-pwa
git init
git add .
git commit -m "PWA Hero Platformer"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/hero-platformer-pwa.git
git push -u origin main

# 2. Activar GitHub Pages
# Ve a Settings > Pages
# Source: main branch
# Folder: / (root)
# Save
```

Tu PWA estará en: `https://TU-USUARIO.github.io/hero-platformer-pwa`

### Opción 2: Netlify (Super Rápido)

1. Ve a [netlify.com](https://netlify.com)
2. Arrastra la carpeta `hero-platformer-pwa` al navegador
3. ¡Listo! Obtendrás un link como `https://random-name.netlify.app`

### Opción 3: Vercel

```bash
# Instalar Vercel CLI
npm i -g vercel

# Deploy
cd hero-platformer-pwa
vercel
```

## 🧪 PROBAR LOCALMENTE

Si quieres probar antes de publicar:

```bash
# Opción 1: Python HTTP Server
cd hero-platformer-pwa
python3 -m http.server 8000

# Opción 2: Node.js
npx http-server

# Opción 3: PHP
php -S localhost:8000
```

Luego abre: `http://localhost:8000`

**IMPORTANTE:** Las PWAs requieren HTTPS en producción. En desarrollo puedes usar localhost.

## ✨ CARACTERÍSTICAS DE LA PWA

Una vez instalada, tu app puede:

### ✅ Funciona Offline
- Todos los recursos se guardan en caché
- Puedes jugar sin internet
- Se actualiza automáticamente cuando hay conexión

### ✅ Pantalla Completa
- Sin barra del navegador
- Experiencia inmersiva
- Controles táctiles optimizados

### ✅ Icono Personalizado
- Aparece en tu pantalla de inicio
- Icono del héroe con capa
- Se ve como una app real

### ✅ Actualización Automática
- Cuando publicas cambios, la app se actualiza sola
- Los usuarios obtienen la última versión

## 🔧 PERSONALIZACIÓN

### Cambiar el icono

Reemplaza los archivos en `icons/` con tus propias imágenes:
- `icon-72.png` hasta `icon-512.png`
- `apple-touch-icon.png`

### Cambiar el nombre

Edita `manifest.json`:
```json
{
  "name": "Tu Nombre de App",
  "short_name": "Tu App"
}
```

### Cambiar colores

En `manifest.json`:
```json
{
  "theme_color": "#00ff00",     // Color de la barra
  "background_color": "#1a1a2e"  // Color de fondo
}
```

## ❓ PROBLEMAS COMUNES

### "No aparece el prompt de instalación"

**Solución:**
- Asegúrate de estar en HTTPS (o localhost)
- Espera 3 segundos después de cargar la página
- Refresca la página (F5 o Cmd+R)

### "El icono no se ve bien"

**Solución:**
- Regenera los iconos con las dimensiones correctas
- Asegúrate de que sean PNG
- Limpia el caché del navegador

### "No funciona offline"

**Solución:**
- Verifica que el Service Worker esté registrado
- Abre DevTools > Application > Service Workers
- Debe aparecer "Activated and running"

### "Los cambios no se ven"

**Solución:**
- Desinstala la app
- Limpia el caché
- Vuelve a instalar

## 📊 VENTAJAS vs APP NATIVA

| Característica | PWA | App Nativa |
|----------------|-----|------------|
| Instalación | Instantánea | Descarga de tienda |
| Tamaño | ~1 MB | 50-200 MB |
| Actualizaciones | Automáticas | Manual |
| Desarrollo | Una vez | iOS + Android separado |
| Costo | Gratis | $99/año (Apple) |
| Distribución | Link web | App Store review |

## 🎉 ¡Felicidades!

Ahora tienes una PWA funcional que:
- 📱 Se instala como app nativa
- 🚀 Funciona offline
- 💯 Es 100% gratis
- 🌍 Se puede compartir con un link
- 📲 Compatible con iOS y Android

**¿Siguiente paso?**

Comparte tu juego:
```
https://TU-USUARIO.github.io/hero-platformer-pwa
```

¡Que lo disfruten! 🎮✨
