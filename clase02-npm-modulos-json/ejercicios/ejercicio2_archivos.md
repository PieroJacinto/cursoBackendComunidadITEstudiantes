# 💻 EJERCICIO: Tu primer archivo personalizado

## ⏱️ TIEMPO: 10 minutos

## 🎯 OBJETIVO
Crear y leer tu propio archivo con información personalizada, aplicando fs.writeFileSync() y fs.readFileSync() con manejo de errores.

---

## 📋 INSTRUCCIONES PASO A PASO

### **PASO 1: Crear archivo mi-info.js (3 minutos)**

**📄 Crear archivo:** `mi-info.js` con este contenido (personalízalo con TU información):

```javascript
// mi-info.js
const fs = require('fs');

// 🎯 PERSONALIZA CON TUS DATOS:
const miInfo = `
=== MI INFORMACIÓN ===
Nombre: [TU NOMBRE AQUÍ]
Proyecto: API [Blog/Restaurante/E-learning/E-commerce]
Fecha: ${new Date().toLocaleDateString()}

=== TÉCNICO ===
Node.js: ${process.version}
Plataforma: ${process.platform}

¡Aprendiendo Node.js! 🚀
`;

// Escribir archivo
fs.writeFileSync('mi-informacion.txt', miInfo, 'utf8');
console.log('✅ Archivo creado: mi-informacion.txt');
```

**🔧 IMPORTANTE:** Reemplaza los datos entre [ ] con tu información real:
- Tu nombre completo
- Tipo de API que elegiste
- Tu ciudad y país

---

### **PASO 2: Ejecutar y verificar (1 minuto)**

```bash
# Ejecutar el archivo
node mi-info.js
```

**✅ Salida esperada:**
```
✅ Archivo creado: mi-informacion.txt
```

**📂 Verificación:** Debe aparecer el archivo `mi-informacion.txt` en tu carpeta.

---

### **PASO 3: Crear archivo mostrar-info.js (4 minutos)**

**📄 Crear archivo:** `mostrar-info.js` para leer tu información:

```javascript
// mostrar-info.js
const fs = require('fs');

try {
    // Leer archivo
    const info = fs.readFileSync('mi-informacion.txt', 'utf8');
    
    console.log('📄 MI INFORMACIÓN:');
    console.log(info);
    console.log('✅ ¡Leído correctamente!');
    
} catch (error) {
    console.log('❌ Error: No se pudo leer el archivo');
    console.log('💡 Solución: Ejecutar primero "node mi-info.js"');
}
```

---

### **PASO 4: Probar la lectura (1 minuto)**

```bash
# Leer tu información
node mostrar-info.js
```

**✅ Salida esperada:**
```
📄 MI INFORMACIÓN:

=== MI INFORMACIÓN ===
Nombre: Juan Pérez
Proyecto: API Blog
Fecha: 7/19/2025

=== TÉCNICO ===
Node.js: v18.17.0
Plataforma: win32

¡Aprendiendo Node.js! 🚀

✅ ¡Leído correctamente!
```

---

### **PASO 5: Probar manejo de errores (1 minuto)**

**🧪 Experiment opcional:** Para ver cómo funciona el try/catch:

1. **Renombrar** el archivo `informacion-personal.txt` a `respaldo.txt`
2. **Ejecutar:** `node mostrar-info.js`
3. **Ver** el mensaje de error
4. **Renombrar** de vuelta a `informacion-personal.txt`
5. **Ejecutar** otra vez `node mostrar-info.js`

---

## 🎯 VERIFICACIÓN FINAL

### **✅ Debes tener:**
- [ ] Archivo `mi-info.js` con tu información personalizada
- [ ] Archivo `mostrar-info.js` que lee y muestra estadísticas
- [ ] Archivo `informacion-personal.txt` generado automáticamente
- [ ] `node mi-info.js` crea el archivo correctamente
- [ ] `node mostrar-info.js` lee y muestra tu información
- [ ] Tu nombre y datos reales (no los [ ] de ejemplo)

### **📂 Estructura final:**
```
mi-api-[tipo]/
├── package.json
├── server.js
├── mi-info.js                    ← Nuevo
├── mostrar-info.js              ← Nuevo
├── informacion-personal.txt     ← Generado automáticamente
└── README.md
```

---

## 🆘 PROBLEMAS COMUNES

### **❌ Error: "Cannot find module 'fs'"**
**Solución:** fs viene incluido en Node.js, verifica que estás usando Node.js v16+

### **❌ Error: "ENOENT: no such file or directory"**  
**Solución:** 
1. Ejecutar primero `node mi-info.js`
2. Verificar que se creó `informacion-personal.txt`
3. Después ejecutar `node mostrar-info.js`

### **❌ Mi archivo muestra [ ] en vez de mi información**
**Solución:** Editar `mi-info.js` y reemplazar todos los textos entre [ ] con tu información real

### **❌ El archivo se creó pero está vacío**
**Solución:** Verificar que no hay errores en la sintaxis de mi-info.js

---

## 🎯 CONCEPTOS QUE PRACTICASTE

### **✅ Aprendiste:**
- ✅ **fs.writeFileSync()** - Escribir archivos
- ✅ **fs.readFileSync()** - Leer archivos  
- ✅ **try/catch** - Manejar errores elegantemente
- ✅ **Template literals** - Crear contenido dinámico con ${}
- ✅ **process.version, process.platform** - Información del sistema
- ✅ **Verificación de contenido** - .includes(), .length, .split()

---

## 🚀 SIGUIENTE PASO

¡Felicitaciones! Ya sabes trabajar con archivos en Node.js. 

**Próxima sección:** Aprenderemos a trabajar con **archivos JSON** para guardar datos estructurados como posts, menú, productos o cursos para tu API.

---

## 💡 BONUS (si terminas rápido)

Crea un archivo adicional para tu tipo de API:

### **📝 Para Blog:**
```javascript
// crear-post-demo.js
const fs = require('fs');

const post = `TÍTULO: Mi primer post
AUTOR: [Tu nombre]
FECHA: ${new Date().toLocaleDateString()}
CONTENIDO: Este es mi primer post de prueba para mi blog API.
¡Pronto podré crear posts desde mi API con Express!`;

fs.writeFileSync('mi-primer-post.txt', post, 'utf8');
console.log('📝 Post de demo creado!');
```

### **🍽️ Para Restaurante:**
```javascript
// crear-menu-demo.js  
const fs = require('fs');

const menu = `🍽️ MENÚ DEL DÍA
Restaurante: [Nombre de tu restaurante]
Fecha: ${new Date().toLocaleDateString()}

ENTRADAS:
- Empanadas de carne - $500
- Provoleta - $600

PRINCIPALES:  
- Milanesa con papas - $1200
- Pasta con tuco - $900

¡Pronto podré gestionar el menú desde mi API!`;

fs.writeFileSync('menu-demo.txt', menu, 'utf8');
console.log('🍽️ Menú de demo creado!');
```

**Ejecutar:** `node crear-post-demo.js` o `node crear-menu-demo.js`