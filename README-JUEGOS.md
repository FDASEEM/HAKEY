



### ✅ **Opción 1: Sistema Dinámico (RECOMENDADO)**



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
        

