# 💻 EJERCICIO: Tu primer archivo JSON

## ⏱️ TIEMPO: 10 minutos

## 🎯 OBJETIVO
Crear archivo JSON con datos para tu tipo de API usando lo que aprendimos de fs y JSON.

---

## 📋 INSTRUCCIONES

### **PASO 1: Crear archivo crear-datos.js (6 minutos)**

**📄 Crear archivo:** `crear-datos.js`

**🎯 Tu tarea:** Escribir código que cree un archivo JSON con **3 registros** según tu tipo de API:

#### **📝 Si tienes API Blog, crear array con:**
- 3 posts con: `id`, `titulo`, `contenido`, `autor`, `fecha`

#### **🍽️ Si tienes API Restaurante, crear array con:**
- 3 platos con: `id`, `nombre`, `precio`, `categoria`, `disponible`

#### **📚 Si tienes API E-learning, crear array con:**
- 3 cursos con: `id`, `titulo`, `instructor`, `duracion`, `precio`

#### **🛍️ Si tienes API E-commerce, crear array con:**
- 3 productos con: `id`, `nombre`, `precio`, `stock`, `disponible`

**🔧 Lo que DEBES usar en tu código:**
- `const fs = require('fs')` para importar sistema de archivos
- `fs.writeFileSync()` para escribir el archivo  
- `JSON.stringify()` para convertir array a texto JSON
- Parámetro `null, 2` en stringify para formato bonito
- `console.log()` para confirmar que se creó

---

### **PASO 2: Ejecutar y verificar (1 minuto)**

```bash
node crear-datos.js
```

**✅ Debes ver:** Mensaje de confirmación y archivo JSON creado

---

### **PASO 3: Crear archivo leer-datos.js (3 minutos)**

**📄 Crear archivo:** `leer-datos.js`

**🎯 Tu tarea:** Escribir código que lea y muestre tus datos JSON

**🔧 Lo que DEBES usar en tu código:**
- `const fs = require('fs')` para importar sistema de archivos
- `try/catch` para manejar errores
- `fs.readFileSync()` para leer el archivo
- `JSON.parse()` para convertir texto a array
- `forEach()` para mostrar cada registro

---

## 🎯 VERIFICACIÓN FINAL

### **✅ Si hiciste todo bien:**
- ✅ `node crear-datos.js` → crea archivo JSON
- ✅ `node leer-datos.js` → muestra tus 3 registros
- ✅ Archivo JSON tiene formato bonito (indentado)
- ✅ Datos son específicos para TU tipo de API

---

## 🆘 AYUDA

**❌ Si no sabes cómo empezar:**
1. Mira los ejemplos del profesor de fs y JSON
2. Combina lo que aprendiste en las demos
3. Pregunta al profesor si te bloqueas

**❌ Si el JSON no se ve bonito:**
- Usar `JSON.stringify(datos, null, 2)` ← el `2` es importante

**❌ Si no puedes leer el archivo:**
- Verificar que el nombre del archivo sea exacto
- Ejecutar crear-datos.js primero

---

## 🚀 OBJETIVO

**Al final tendrás:**
- Archivo JSON con TUS datos
- Experiencia escribiendo código fs + JSON
- Base de datos para Express en Clase 3

**¡Es TU código, no copy-paste!** 💪