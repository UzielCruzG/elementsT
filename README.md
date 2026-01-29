# 🧪 ElementaQR - Tabla Periódica Interactiva

Una aplicación web progresiva (PWA) diseñada para la visualización educativa y técnica de los elementos químicos, accesible mediante códigos QR.

## 🎨 Características

### ✨ Funcionalidades Principales

- **Tabla Periódica Completa**: Visualización interactiva de 30 elementos químicos con datos científicos completos
- **Búsqueda Inteligente**: Busca por nombre, símbolo o número atómico
- **Filtros Dinámicos**: Filtra por categoría (metales alcalinos, gases nobles, etc.)
- **Modal Detallado**: Información técnica completa al hacer clic en cualquier elemento
- **Diseño Responsivo**: Funciona perfectamente en móviles, tablets y escritorio
- **Animaciones Fluidas**: Transiciones y efectos visuales científico-futuristas

### 📊 Información por Elemento

Cada elemento incluye:
- Identificación: Nombre, símbolo, número atómico
- Propiedades físicas: Masa atómica, densidad, puntos de fusión/ebullición
- Propiedades químicas: Electronegatividad, radio atómico, energía de ionización
- Estructura: Configuración electrónica, distribución por capas
- Historia: Año de descubrimiento y descubridor
- Aplicaciones: Usos principales en la industria y vida cotidiana
- Datos curiosos: Información interesante sobre el elemento
- Toxicidad y abundancia terrestre

## 🚀 Cómo Usar

### Opción 1: Abrir Localmente

1. Descarga el archivo `index.html`
2. Abre el archivo en tu navegador (Chrome, Firefox, Safari, Edge)
3. ¡Listo! No necesita instalación ni servidor

### Opción 2: Hospedar en Línea (Recomendado)

#### GitHub Pages (Gratis)
1. Crea un repositorio en GitHub
2. Sube el archivo `index.html`
3. Ve a Settings → Pages
4. Selecciona la rama main
5. Tu URL será: `https://usuario.github.io/repositorio`

#### Netlify (Gratis)
1. Arrastra el archivo `index.html` a [Netlify Drop](https://app.netlify.com/drop)
2. Netlify generará una URL automáticamente
3. Puedes personalizar el dominio en la configuración

#### Vercel (Gratis)
1. Instala Vercel CLI: `npm install -g vercel`
2. En la carpeta del proyecto ejecuta: `vercel`
3. Sigue las instrucciones

## 📱 Generar Código QR

Una vez que tengas tu URL en línea, genera un código QR:

### Opción 1: Herramientas Online
- [QR Code Generator](https://www.qr-code-generator.com/)
- [QRCode Monkey](https://www.qrcode-monkey.com/)
- [QR.io](https://qr.io/)

### Opción 2: Usando Python
```python
import qrcode

# Tu URL del proyecto
url = "https://tu-usuario.github.io/elementaqr"

# Generar QR
qr = qrcode.QRCode(version=1, box_size=10, border=5)
qr.add_data(url)
qr.make(fit=True)

img = qr.make_image(fill_color="black", back_color="white")
img.save("elementaqr_qr.png")
```

## 🎨 Personalización

### Cambiar Colores
Edita las variables CSS en el `<style>`:
```css
:root {
    --bg-primary: #0a0e27;
    --accent-cyan: #00f5ff;
    --accent-magenta: #ff00ff;
    /* ... más variables */
}
```

### Agregar Más Elementos
Edita el array `elementsData` en el JavaScript y agrega nuevos elementos siguiendo la estructura existente.

### Modificar Tipografías
Las fuentes actuales son:
- Display: 'Orbitron' (números y títulos)
- Cuerpo: 'Rajdhani' (texto general)

Cámbialas editando el `<link>` de Google Fonts y las referencias CSS.

## 🛠️ Tecnologías Utilizadas

- **React 18** (vía CDN)
- **Babel Standalone** (para JSX en el navegador)
- **CSS3** (Grid, Flexbox, Animaciones)
- **HTML5**
- **Google Fonts** (Orbitron, Rajdhani)

## 📋 Requisitos

- Navegador moderno (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- JavaScript habilitado
- No requiere Node.js ni instalación

## 🎯 Casos de Uso

- **Educación**: Material de apoyo para clases de química
- **Estudiantes**: Referencia rápida para estudiar
- **Laboratorios**: Información técnica accesible vía QR
- **Museos**: Exhibiciones interactivas
- **Presentaciones**: Complemento visual para exposiciones

## 🔮 Futuras Mejoras Posibles

- [ ] PWA completa (funcionamiento offline)
- [ ] Comparador de elementos (lado a lado)
- [ ] Modo oscuro/claro toggle
- [ ] Diagrama 3D de orbitales
- [ ] Exportar fichas a PDF
- [ ] Agregar isótopos
- [ ] Tabla periódica 3D interactiva
- [ ] Traducciones (inglés, francés, etc.)
- [ ] Gráficas de tendencias (radio atómico vs número)

## 📄 Licencia

Proyecto educativo de código abierto. Libre para uso personal y educativo.

## 👨‍💻 Autor

Creado con 💙 para aprender química de forma interactiva.

---

## 🐛 Reporte de Bugs

Si encuentras algún error o tienes sugerencias, por favor crea un issue en el repositorio.

## 🌟 Contribuciones

¡Las contribuciones son bienvenidas! Si quieres agregar más elementos o mejorar la aplicación, haz un fork y envía un pull request.

---

**¡Disfruta explorando los elementos químicos! 🧪✨**
