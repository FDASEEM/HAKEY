# 🎮 HAKEY - Sistema de Gestión de Juegos

## 📋 Cómo Agregar Nuevos Juegos

### ✅ **Opción 1: Sistema Dinámico (RECOMENDADO)**

Ya tienes implementado un sistema dinámico que funciona con una sola página. Aquí te explico cómo agregar nuevos juegos:

#### 1. **Editar el archivo `games.json`**
```json
{
  "nuevo-juego-id": {
    "title": "Nombre del Juego",
    "price": "$XX.XX USD",
    "developer": "Nombre del Desarrollador",
    "genre": "Género1, Género2, Género3",
    "description": "Descripción detallada del juego...",
    "duration": "XX horas (historia principal)",
    "languages": "Español, Inglés, Francés",
    "images": [
      "ruta/imagen1.jpg",
      "ruta/imagen2.jpg",
      "ruta/imagen3.jpg"
    ],
    "minRequirements": [
      "Sistema: Windows 10",
      "Procesador: Intel Core i5-XXXX",
      "Memoria: X GB RAM",
      "Gráficos: NVIDIA GeForce GTX XXX",
      "DirectX: Versión XX",
      "Almacenamiento: XX GB disponibles"
    ],
    "recRequirements": [
      "Sistema: Windows 10",
      "Procesador: Intel Core i7-XXXX",
      "Memoria: XX GB RAM",
      "Gráficos: NVIDIA GeForce GTX XXX",
      "DirectX: Versión XX",
      "Almacenamiento: XX GB disponibles"
    ]
  }
}
```

#### 2. **Agregar la tarjeta en `index.html`**
```html
<a href="game.html?id=nuevo-juego-id" class="juego-card">
    <img src="ruta/imagen-principal.jpg" alt="Nombre del Juego">
    <span>Nombre del Juego</span>
</a>
```

#### 3. **¡Listo!** 
El juego aparecerá automáticamente en la página principal y tendrá su propia página de detalles.

---

## 🔧 **Otras Opciones Disponibles**

### **Opción 2: Páginas Estáticas Individuales**
Si prefieres tener un HTML por cada juego:

1. Copia `juego.html` y renómbralo (ej: `cyberpunk.html`)
2. Cambia el contenido estático dentro del HTML
3. Actualiza los enlaces en `index.html`

### **Opción 3: Sistema con Base de Datos**
Para proyectos más grandes, podrías usar:
- **Backend**: Node.js + Express + MongoDB/MySQL
- **Frontend**: React/Vue.js
- **API**: Para gestionar juegos dinámicamente

---

## 📁 **Estructura de Archivos Actual**

```
HAKEY-1/
├── index.html          # Página principal con tarjetas de juegos
├── game.html           # Página dinámica de detalles del juego
├── games.json          # Base de datos de juegos
├── juego.html          # Página estática original (puedes eliminarla)
├── login.html          # Página de login
├── registro.html       # Página de registro
├── cart.html           # Página del carrito
├── style.css           # Estilos CSS
└── assets/
    └── img/            # Imágenes de juegos
```

---

## 🎯 **Ventajas del Sistema Dinámico**

✅ **Una sola página** para todos los juegos  
✅ **Fácil mantenimiento** - solo editar `games.json`  
✅ **Consistencia visual** - mismo diseño para todos  
✅ **Escalable** - agregar juegos sin crear archivos nuevos  
✅ **SEO friendly** - URLs con parámetros  
✅ **Carga rápida** - solo carga datos necesarios  

---

## 🚀 **Próximos Pasos Recomendados**

1. **Agregar más juegos** editando `games.json`
2. **Mejorar imágenes** - usar URLs reales de juegos
3. **Añadir funcionalidad de carrito** real
4. **Implementar sistema de búsqueda**
5. **Agregar filtros por género/precio**
6. **Sistema de usuarios y reviews**

---

## 💡 **Tips para Agregar Juegos**

- **ID único**: Usa nombres descriptivos sin espacios (ej: `elden-ring`)
- **Imágenes**: Usa imágenes de alta calidad (800x400px recomendado)
- **Descripción**: Sé descriptivo pero conciso
- **Requisitos**: Sé específico con las especificaciones técnicas
- **Precios**: Mantén formato consistente (`$XX.XX USD`)

¡Tu sistema está listo para escalar! 🎮✨
