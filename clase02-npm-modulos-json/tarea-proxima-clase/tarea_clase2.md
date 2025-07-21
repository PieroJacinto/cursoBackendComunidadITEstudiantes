# 🏠 TAREA CLASE 2 → CLASE 3

## 🎯 OBJETIVO
Aplicar lo aprendido a tu proyecto personal y tener datos JSON listos para Express.

---

## 📋 TAREA SIMPLE (20 minutos total)

### **PASO 1: Verificar que todo funciona (5 min)**

**✅ Revisar que tienes estos archivos funcionando:**
- `package.json` con scripts
- `server.js` que muestra info del proyecto  
- Archivo JSON con datos de tu API

```bash
# Probar que todo funciona:
npm start
node crear-datos.js
node leer-datos.js
```

---

### **PASO 2: Agregar más datos a tu JSON (10 min)**

**📝 Editar tu archivo `crear-datos.js` para agregar MÁS datos:**

#### **📝 Blog - agregar hasta 5 posts:**
```javascript
const posts = [
    { id: 1, titulo: "Mi primer post", contenido: "Hola mundo!", fecha: "2025-07-19" },
    { id: 2, titulo: "Aprendiendo Node.js", contenido: "JSON es increíble", fecha: "2025-07-20" },
    { id: 3, titulo: "Creando mi API", contenido: "Pronto tendré Express", fecha: "2025-07-21" },
    { id: 4, titulo: "Backend con Node.js", contenido: "Cada día aprendo más", fecha: "2025-07-22" },
    { id: 5, titulo: "Mi blog crece", contenido: "¡Ya tengo 5 posts!", fecha: "2025-07-23" }
];
```

#### **🍽️ Restaurante - agregar hasta 5 platos:**
```javascript
const menu = [
    { id: 1, nombre: "Pizza Margherita", precio: 1200, categoria: "principales" },
    { id: 2, nombre: "Ensalada César", precio: 900, categoria: "ensaladas" },
    { id: 3, nombre: "Pasta Bolognesa", precio: 1100, categoria: "principales" },
    { id: 4, nombre: "Tiramisu", precio: 650, categoria: "postres" },
    { id: 5, nombre: "Agua mineral", precio: 200, categoria: "bebidas" }
];
```

#### **📚 E-learning - agregar hasta 5 cursos:**
```javascript
const cursos = [
    { id: 1, titulo: "Node.js Básico", instructor: "Ana", duracion: "4 semanas", precio: 15000 },
    { id: 2, titulo: "React Avanzado", instructor: "Luis", duracion: "6 semanas", precio: 20000 },
    { id: 3, titulo: "MySQL desde cero", instructor: "María", duracion: "3 semanas", precio: 12000 },
    { id: 4, titulo: "Express y APIs", instructor: "Carlos", duracion: "5 semanas", precio: 18000 },
    { id: 5, titulo: "Deploy en producción", instructor: "Sofia", duracion: "2 semanas", precio: 10000 }
];
```

#### **🛍️ E-commerce - agregar hasta 5 productos:**
```javascript
const productos = [
    { id: 1, nombre: "Auriculares Bluetooth", precio: 8500, stock: 15, categoria: "tecnología" },
    { id: 2, nombre: "Mouse Gamer", precio: 4200, stock: 8, categoria: "tecnología" },
    { id: 3, nombre: "Teclado Mecánico", precio: 12000, stock: 5, categoria: "tecnología" },
    { id: 4, nombre: "Monitor 24 pulgadas", precio: 35000, stock: 3, categoria: "tecnología" },
    { id: 5, nombre: "Webcam HD", precio: 6500, stock: 12, categoria: "tecnología" }
];
```

**🔄 Ejecutar:** `node crear-datos.js` para actualizar tu archivo JSON

---

### **PASO 3: Actualizar README.md (5 min)**

**📝 Editar tu `README.md`:**

```markdown
# Mi API [Blog/Restaurante/E-learning/E-commerce]

## Descripción
API para [descripción de tu proyecto en 1 línea]

## Cómo usar
```bash
# Ver información del proyecto
npm start

# Crear datos
node crear-datos.js

# Ver datos  
node leer-datos.js
```

## Datos
- Archivo: [posts/menu/cursos/productos].json
- Total: 5 registros
- Listo para usar con Express en Clase 3

## Próximo paso
Crear rutas REST con Express.
```

---

## 🎯 VERIFICACIÓN FINAL

### **✅ Debes tener:**
- [ ] 5 registros en tu archivo JSON
- [ ] `npm start` funciona
- [ ] `node leer-datos.js` muestra 5 elementos
- [ ] README.md actualizado

### **📂 Estructura final:**
```
mi-api-[tipo]/
├── package.json
├── server.js  
├── crear-datos.js          ← Con 5 registros
├── leer-datos.js
├── posts.json              ← Con 5 posts (Blog)
├── menu.json               ← Con 5 platos (Restaurante)  
├── cursos.json             ← Con 5 cursos (E-learning)
├── productos.json          ← Con 5 productos (E-commerce)
└── README.md               ← Actualizado
```

---

## 🚀 PARA CLASE 3

**En la próxima clase usaremos estos 5 registros para crear:**
- `GET /posts` → devuelve los 5 posts
- `GET /posts/1` → devuelve el post con ID 1
- `GET /posts/2` → devuelve el post con ID 2

**¡Tu archivo JSON será la base de datos de tu API!** 🎉

---

## 🆘 Si algo no funciona

1. Ejecutar `node crear-datos.js` de nuevo
2. Verificar que el archivo JSON tiene 5 registros
3. Probar `npm start` y `node leer-datos.js`

**¡Con esto estás 100% listo para Express!** 🚀