# 🚀 MayReplit - Proyecto Fácil

**Mantén tu Replit activo 24/7 súper fácil - ¡Solo edita un archivo y listo!**

**Creado por:** SoyMaycol ❤️  
**GitHub:** [SoySapo6](https://github.com/SoySapo6)

## ✨ ¿Qué es esto?

Un proyecto **súper simple** que usa el módulo `@soymaycol/mayreplit` para mantener tu Replit funcionando 24/7. **No necesitas saber programar**, solo editar un archivo de configuración.

## 🎯 Instalación Rápida

### 1️⃣ Descargar el proyecto
```bash
git clone https://github.com/SoySapo6/MayReplit.git
cd MayReplit
```

### 2️⃣ Instalar dependencias
```bash
npm install && npx playwright install --with-deps
```

### 3️⃣ Configurar (¡Solo esto tienes que hacer!)
Edita el archivo `config.js` con tus datos:

```javascript
export default {
  // 🔗 Pon la URL de tu Replit aquí
  replitUrl: 'https://replit.com/@tuusuario/TuProyecto',
  
  // 🍪 Pon la ruta de tus cookies aquí
  cookiesPath: './cookies.json',
  
  // ⏰ Cada cuánto tomar screenshots (5 minutos = 5 * 60 * 1000)
  screenshotInterval: 5 * 60 * 1000,
  
  // 👁️ Mostrar ventana del navegador o no
  headless: true,
  
  // 📊 Mostrar estadísticas cada minuto
  showStats: true
}
```

### 4️⃣ Obtener cookies de Replit
1. Ve a [Replit.com](https://replit.com) e inicia sesión
2. Presiona **F12** (herramientas de desarrollador)
3. Ve a **Application** → **Cookies** → **https://replit.com**
4. Exporta las cookies y guárdalas en `cookies.json`

**Formato del cookies.json:**
```json
[
  {
    "name": "connect.sid",
    "value": "tu-valor-aqui",
    "domain": ".replit.com",
    "path": "/",
    "expires": 1234567890,
    "httpOnly": true,
    "secure": true,
    "sameSite": "Lax"
  }
]
```

### 5️⃣ ¡Ejecutar!
```bash
npm start
```

¡Y ya está! Tu Replit estará activo 24/7 🎉

## 📋 Lo que hace automáticamente

- ✅ Abre tu Replit en segundo plano
- ✅ Toma screenshots cada X minutos para mantenerlo activo
- ✅ Maneja errores automáticamente
- ✅ Te muestra estadísticas en tiempo real
- ✅ Se cierra correctamente con Ctrl+C

## 🎛️ Configuraciones Disponibles

En `config.js` puedes cambiar:

| Opción | Descripción | Ejemplo |
|--------|-------------|---------|
| `replitUrl` | URL de tu Replit | `'https://replit.com/@usuario/proyecto'` |
| `cookiesPath` | Ruta de las cookies | `'./mis-cookies.json'` |
| `screenshotInterval` | Intervalo de screenshots | `3 * 60 * 1000` (3 min) |
| `headless` | Mostrar navegador | `false` (para ver la ventana) |
| `showStats` | Mostrar estadísticas | `false` (modo silencioso) |

## 🔧 Comandos Disponibles

```bash
# Iniciar el proyecto
npm start

# Lo mismo que start
npm run dev

# Reinstalar dependencias
npm run install-deps
```

## 📱 Ejemplo de Salida

```
╔══════════════════════════════════════════════════════════╗
║                     🚀 MayReplit v1.0                   ║
║                                                          ║
║              Mantén tu Replit activo 24/7                ║
║                Creado por SoyMaycol ❤️                  ║
╚══════════════════════════════════════════════════════════╝

✅ Archivo de cookies encontrado

⚙️  Configuración cargada:
   🔗 URL: https://replit.com/@usuario/proyecto
   🍪 Cookies: ./cookies.json
   📸 Screenshots cada: 5 minutos
   👁️  Modo headless: Sí

🚀 Iniciando MayReplit...
💡 Presiona Ctrl+C para detener
════════════════════════════════════════════════════════════

(⁠◍⁠•⁠ᴗ⁠•⁠◍⁠)⁠❤ ¡Ya estamos dentro del Replit!
📸 Screenshot inicial capturada
📊 Screenshot: 45.2 KB | 🕐 14:30:15
```

## 🆘 Solución de Problemas

### ❌ "Por favor configura tu URL de Replit"
- Edita `config.js` y pon tu URL real de Replit

### ❌ "No se encontró el archivo de cookies"
- Asegúrate de tener `cookies.json` con las cookies de Replit
- Verifica que la ruta en `cookiesPath` sea correcta

### ❌ Error al iniciar
- Verifica que tengas Node.js 16+ instalado
- Ejecuta `npm install` de nuevo
- Revisa que la URL de Replit sea correcta

## 🤝 Soporte

¿Problemas? ¡Aquí te ayudamos!

1. **GitHub Issues:** [Reportar problema](https://github.com/SoySapo6/MayReplit/issues)
2. **Revisa que todo esté configurado en `config.js`**
3. **Asegúrate de tener las cookies correctas**

## 📄 Licencia

MIT - Usa este proyecto como quieras pero siempre con creditos ❤️

---

**¡Hecho con ❤️ por SoyMaycol!**

*Si te ayuda este proyecto, dale una ⭐ en GitHub*
