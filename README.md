# 🔐 NexusPortal — Login Page

Una página de inicio de sesión **moderna, interactiva y completamente responsiva**, construida con HTML, CSS y JavaScript vanilla. Diseñada para impresionar desde el primer vistazo.

---

## ✨ Características

- 🎨 **Diseño glassmorphism** con fondo animado de blobs y partículas en canvas
- 🌐 **Google Sign-In (OAuth 2.0)** integrado mediante Google Identity Services (GIS)
- ✅ **Validación en tiempo real** de email y contraseña con estados visuales
- 🔔 **Sistema de toasts** para notificaciones no intrusivas
- 👁️ **Toggle de contraseña** visible / oculta
- 💫 **Micro-animaciones** — ripple en el botón, tilt en botones sociales, shake en errores
- 🏆 **Overlay de éxito** animado con SVG al autenticarse
- 📱 **Totalmente responsivo** (mobile-first, breakpoints en 900px y 480px)
- ♿ **Accesibilidad** — atributos `aria-label`, roles ARIA, navegación por teclado

---

## 📁 Estructura

```
login-page/
├── index.html   # Estructura semántica de la página
├── style.css    # Estilos con variables CSS, animaciones y media queries
└── script.js    # Lógica: partículas, validación, Google OAuth, toasts, efectos
```

---

## 🚀 Uso

### Sin configuración
Abre `index.html` directamente en tu navegador. La página es funcional como demo sin ningún backend.

### Con Google Sign-In real
1. Ve a [Google Cloud Console → Credenciales](https://console.cloud.google.com/apis/credentials)
2. Crea un **OAuth 2.0 Client ID** de tipo *Aplicación web*
3. Añade tu dominio en **Orígenes autorizados** (ej. `http://localhost`)
4. Haz clic en el botón **Google** de la página y pega tu Client ID en el modal que aparece
5. El ID se guarda en `localStorage` para sesiones futuras

---

## 🛠️ Tecnologías

| Tecnología | Uso |
|---|---|
| HTML5 semántico | Estructura accesible |
| CSS3 (Vanilla) | Variables, animaciones, glassmorphism, grid |
| JavaScript ES2020+ | Partículas, validación, OAuth, async/await |
| Google Identity Services | Autenticación con Google |
| Google Fonts — Inter | Tipografía moderna |

---

## 🎨 Paleta de colores

| Variable | Valor | Uso |
|---|---|---|
| `--primary` | `#6c63ff` | Color principal |
| `--primary-light` | `#a78bfa` | Acentos, gradientes |
| `--accent` | `#f0abfc` | Gradiente del título |
| `--bg` | `#0a0a1a` | Fondo oscuro |
| `--success` | `#10b981` | Validación correcta |
| `--error` | `#f87171` | Errores de validación |

---

## 📸 Vista previa

> Panel izquierdo con brand + features animadas · Panel derecho con tarjeta glassmorphism · Partículas interconectadas en fondo

---

## 📝 Notas

- El botón de **GitHub** muestra un aviso informativo: el flujo OAuth de GitHub requiere un servidor backend para el intercambio de tokens.
- El formulario de email/contraseña simula un login con un delay de 1.8s y overlay de éxito. Conecta tu propio backend modificando el listener `submit` en `script.js`.

---

## 📄 Licencia

MIT — libre para uso personal y comercial.
