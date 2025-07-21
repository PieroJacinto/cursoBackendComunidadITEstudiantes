# 💻 EJERCICIO: Crear tu package.json personalizado

## ⏱️ TIEMPO: 15 minutos

## 🎯 OBJETIVO
Crear y configurar package.json para tu proyecto personal de API, con scripts básicos y información correcta.

---

## 📋 INSTRUCCIONES PASO A PASO

### **PASO 1: Navegar a tu proyecto personal (2 min)**

```bash
# Ir a la carpeta de tu proyecto
cd mi-api-blog
# o
cd mi-api-restaurante  
# o
cd mi-api-elearning
# o
cd mi-api-ecommerce

# Verificar que estás en el lugar correcto
pwd
```

---

### **PASO 2: Crear package.json automáticamente (3 min)**

```bash
# Crear package.json con valores por defecto
npm init -y
```

**✅ Verificación:** Debe aparecer un archivo `package.json` en tu carpeta.

---

### **PASO 3: Personalizar tu package.json (8 min)**

**📝 Abrir package.json en VS Code y editarlo:**

#### **📝 Para API Blog:**
```json
{
  "name": "mi-api-blog",
  "version": "1.0.0",
  "description": "API REST para blog personal con Node.js",
  "main": "server.js",
  "scripts": {
    "start": "node server.js",
    "dev": "node server.js"
  },
  "keywords": ["blog", "api", "nodejs"],
  "author": "Tu Nombre <tu.email@ejemplo.com>",
  "license": "MIT"
}
```

#### **🍽️ Para API Restaurante:**
```json
{
  "name": "mi-api-restaurante",
  "version": "1.0.0",
  "description": "API REST para gestión de restaurante",
  "main": "server.js",
  "scripts": {
    "start": "node server.js",
    "dev": "node server.js"
  },
  "keywords": ["restaurante", "api", "nodejs"],
  "author": "Tu Nombre <tu.email@ejemplo.com>",
  "license": "MIT"
}
```

#### **📚 Para API E-learning:**
```json
{
  "name": "mi-api-elearning",
  "version": "1.0.0",
  "description": "API REST para plataforma de cursos online",
  "main": "server.js",
  "scripts": {
    "start": "node server.js",
    "dev": "node server.js"
  },
  "keywords": ["elearning", "api", "nodejs"],
  "author": "Tu Nombre <tu.email@ejemplo.com>",
  "license": "MIT"
}
```

#### **🛍️ Para API E-commerce:**
```json
{
  "name": "mi-api-ecommerce",
  "version": "1.0.0",
  "description": "API REST para tienda online",
  "main": "server.js",
  "scripts": {
    "start": "node server.js",
    "dev": "node server.js"
  },
  "keywords": ["ecommerce", "api", "nodejs"],
  "author": "Tu Nombre <tu.email@ejemplo.com>",
  "license": "MIT"
}
```

**🔧 Cambios importantes:**
- ✅ Cambiar `"main"` de `"index.js"` a `"server.js"`
- ✅ Agregar script `"start"`
- ✅ Personalizar `"description"` 
- ✅ Poner tu nombre real en `"author"`
- ✅ Agregar `"keywords"` relacionadas con tu API

---

### **PASO 4: Crear server.js básico (2 min)**

**📄 Crear archivo `server.js`:**

```javascript
// server.js
console.log('🚀 Iniciando servidor...');

const packageInfo = require('./package.json');

console.log('📦 Proyecto:', packageInfo.name);
console.log('📝 Descripción:', packageInfo.description);
console.log('⚡ Versión:', packageInfo.version);

console.log('✅ ¡Todo configurado correctamente!');
```

---

## 🧪 PASO 5: Probar que funciona (1 min)

```bash
# Probar script start
npm start
```

**✅ Salida esperada:**
```
🚀 Iniciando servidor...
📦 Proyecto: mi-api-blog
📝 Descripción: API REST para blog personal con Node.js
⚡ Versión: 1.0.0
✅ ¡Todo configurado correctamente!
```

---

## 🎯 VERIFICACIÓN FINAL

### **✅ Debes tener:**
- [ ] Archivo `package.json` con tu información personal
- [ ] Archivo `server.js` funcionando
- [ ] `npm start` muestra información correcta de tu proyecto
- [ ] Scripts básicos configurados

### **📂 Estructura final:**
```
mi-api-[tipo]/
├── package.json          ← Configurado con tu info
├── server.js            ← Archivo principal
└── README.md            ← Del proyecto anterior
```

---

## 🚀 SIGUIENTE PASO

Una vez que tengas esto funcionando, estarás listo para la siguiente sección: **Módulos Built-in (fs)** donde aprenderemos a leer y escribir archivos.