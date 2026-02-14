# 🦸‍♂️ Hero Platformer - Progressive Web App (PWA)

## 📱 **¡Instálalo como APP en iPhone y Android!**

Esta es la versión **Progressive Web App (PWA)** del juego Hero Platformer. Se puede **instalar como una aplicación real** en tu dispositivo móvil sin necesidad de la App Store o Google Play.

![PWA Badge](https://img.shields.io/badge/PWA-Ready-brightgreen)
![iOS Compatible](https://img.shields.io/badge/iOS-Compatible-blue)
![Android Compatible](https://img.shields.io/badge/Android-Compatible-green)

## ✨ Características PWA

- 📲 **Se instala como app nativa** - Aparece en tu pantalla de inicio
- 🚫 **Sin navegador** - Pantalla completa, sin barras de Safari/Chrome
- 📡 **Funciona OFFLINE** - Juega sin conexión a internet
- 🔄 **Actualización automática** - Siempre tendrás la última versión
- ⚡ **Súper rápida** - Carga instantánea
- 💾 **Ocupa ~1MB** - Mucho menor que apps nativas
- 🆓 **100% Gratis** - No pagas App Store ni Google Play

## 🚀 Instalación Rápida

### En iPhone/iPad:

1. Abre Safari
2. Ve a: `https://TU-USUARIO.github.io/hero-platformer-pwa`
3. Toca 📤 (Compartir)
4. Selecciona "Agregar a pantalla de inicio"
5. ¡Listo! 🎮

### En Android:

1. Abre Chrome
2. Ve al link del juego
3. Toca "Agregar a pantalla de inicio" (aparece automáticamente)
4. ¡Listo! 🎮

**[📖 Guía completa de instalación](INSTALACION_PWA.md)**

## 📦 Contenido del Paquete

```
hero-platformer-pwa/
├── index.html              - El juego completo
├── manifest.json           - Configuración PWA
├── service-worker.js       - Cache y offline
├── icons/                  - Iconos de la app
│   ├── icon-72.png
│   ├── icon-96.png
│   ├── icon-128.png
│   ├── icon-144.png
│   ├── icon-152.png
│   ├── icon-192.png
│   ├── icon-384.png
│   ├── icon-512.png
│   └── apple-touch-icon.png
├── INSTALACION_PWA.md      - Guía de instalación
└── README.md               - Este archivo
```

## 🌍 Publicar tu PWA

### GitHub Pages (Recomendado):

```bash
git init
git add .
git commit -m "PWA Hero Platformer"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/hero-platformer-pwa.git
git push -u origin main

# Activar GitHub Pages en Settings > Pages
```

Tu PWA estará en: `https://TU-USUARIO.github.io/hero-platformer-pwa`

### Netlify (Más fácil):

1. Arrastra la carpeta a [netlify.com](https://netlify.com)
2. ¡Listo!

## 🎮 Controles

**Móvil:** Botones táctiles en pantalla (⬅️ ➡️ ⬆️)

**Teclado:** 
- A/← = Izquierda
- D/→ = Derecha
- W/↑/Espacio = Saltar

## 🔧 Personalización

### Cambiar nombre de la app:

Edita `manifest.json`:
```json
{
  "name": "Mi Juego Épico",
  "short_name": "Mi Juego"
}
```

### Cambiar iconos:

Reemplaza los archivos en `icons/` con tus propias imágenes.

### Cambiar colores:

En `manifest.json`:
```json
{
  "theme_color": "#FF0000",
  "background_color": "#000000"
}
```

## 🆚 PWA vs App Nativa

| | PWA | App Nativa |
|---|---|---|
| **Instalación** | Instantánea | Descarga tienda |
| **Tamaño** | ~1 MB | 50-200 MB |
| **Costo** | $0 | $99/año (Apple) |
| **Desarrollo** | HTML/JS | Swift/Kotlin |
| **Actualizar** | Auto | Manual |
| **Offline** | ✅ | ✅ |
| **Pantalla completa** | ✅ | ✅ |

## 🔒 Requisitos

- **HTTPS** requerido (excepto en localhost)
- Navegadores modernos:
  - iOS Safari 11.3+
  - Android Chrome 40+
  - Desktop Chrome/Edge 67+

## 💡 Cómo Funciona

1. **Service Worker** cachea todos los recursos
2. **Manifest.json** define la app (nombre, iconos, colores)
3. **Offline First** - funciona sin internet
4. **App Shell** - carga instantánea

## 🐛 Solución de Problemas

**No aparece prompt de instalación:**
- Usa HTTPS (o localhost)
- Espera 3 segundos
- Refresca la página

**No funciona offline:**
- Verifica Service Worker en DevTools
- Debe estar "Activated and running"

**Cambios no se ven:**
- Desinstala la app
- Limpia caché
- Reinstala

## 📚 Recursos

- [MDN: Progressive Web Apps](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps)
- [Google: PWA Checklist](https://web.dev/pwa-checklist/)
- [Apple: Configuring Web Applications](https://developer.apple.com/library/archive/documentation/AppleApplications/Reference/SafariWebContent/ConfiguringWebApplications/ConfiguringWebApplications.html)

## 🤝 Contribuir

¿Ideas para mejorar la PWA?

1. Fork el proyecto
2. Crea una rama (`git checkout -b feature/mejora`)
3. Commit (`git commit -m 'Mejora'`)
4. Push (`git push origin feature/mejora`)
5. Abre un Pull Request

## 📄 Licencia

MIT License - Libre para usar, modificar y distribuir.

## 👨‍💻 Autor

Tu Nombre - [@tu-twitter](https://twitter.com/tu-twitter)

## 🌟 Demo

**Prueba la PWA aquí:** [https://TU-USUARIO.github.io/hero-platformer-pwa](https://TU-USUARIO.github.io/hero-platformer-pwa)

---

⭐ Si te gusta, ¡dale una estrella en GitHub!

📱 **¡Descarga la app ahora y juega offline!**
