# 📦 CLASE 2 - Node.js Fundamentos (NPM + Módulos + JSON)

## 🎯 OBJETIVOS DE LA CLASE
Al final de esta clase podrás:
- ✅ Crear y configurar package.json con npm init
- ✅ Usar módulos built-in de Node.js (fs)
- ✅ Leer y escribir archivos
- ✅ Trabajar con JSON para datos estructurados
- ✅ Tener datos JSON listos para Express

---

## 📚 MATERIALES DE LA CLASE

### **🖼️ Slides:**
- **Slide 1:** NPM y package.json
- **Slide 2:** Módulos built-in (fs)  
- **Slide 3:** Trabajar con JSON

### **💻 Ejercicios:**
- **Ejercicio 1:** Crear package.json personalizado
- **Ejercicio 2:** Tu primer archivo con fs
- **Ejercicio 3:** Tu primer archivo JSON

### **🏠 Tarea:**
- Preparar datos JSON para Express (Clase 3)

---

## 🔧 HERRAMIENTAS NECESARIAS

### **Verificar antes de empezar:**
```bash
# Node.js funcionando
node --version    # v18.0.0 o superior
npm --version     # 9.0.0 o superior

# Git configurado
git config user.name
git config user.email

# Proyecto personal configurado
ls mi-api-[tipo]/  # Tu carpeta de proyecto
```

---

## 📋 FLUJO DE LA CLASE

### **1. NPM y package.json (55 min)**
- **Qué es NPM:** Gestor de paquetes de Node.js
- **Demo:** `npm init -y` paso a paso
- **Ejercicio:** Crear tu package.json personalizado
- **Resultado:** Scripts npm funcionando

### **2. Módulos built-in (50 min)**
- **Sistema de módulos:** `require()` y `module.exports`
- **Demo 1:** Escribir archivos con `fs.writeFileSync()`
- **Demo 2:** Leer archivos con `fs.readFileSync()`
- **Ejercicio:** Crear y leer tu archivo personalizado
- **Resultado:** Archivos funcionando con try/catch

### **3. Trabajar con JSON (35 min)**
- **Qué es JSON:** Datos estructurados para APIs
- **Demo:** `JSON.parse()` y `JSON.stringify()`
- **Ejercicio:** Crear archivo JSON para tu API
- **Resultado:** Base de datos temporal lista

---

## 🎯 LO QUE LOGRARÁS HOY

### **Al final de la clase tendrás:**
```
mi-api-[tipo]/
├── package.json              ← Con scripts funcionando
├── server.js                 ← Mostrando info del proyecto
├── crear-datos.js            ← Creando archivo JSON
├── leer-datos.js             ← Leyendo archivo JSON
├── [posts/menu/cursos/productos].json  ← Con tus datos
└── README.md                 ← Documentación básica
```

### **Scripts npm operativos:**
```bash
npm start           # Ver info del proyecto
node crear-datos.js # Crear archivo JSON
node leer-datos.js  # Ver datos JSON
```

---

## 📊 DATOS ESPECÍFICOS POR PROYECTO

### **📝 Si tienes API Blog:**
- **Archivo:** `posts.json`
- **Estructura:** id, titulo, contenido, autor, fecha

### **🍽️ Si tienes API Restaurante:**
- **Archivo:** `menu.json`
- **Estructura:** id, nombre, precio, categoria, disponible

### **📚 Si tienes API E-learning:**
- **Archivo:** `cursos.json`
- **Estructura:** id, titulo, instructor, duracion, precio

### **🛍️ Si tienes API E-commerce:**
- **Archivo:** `productos.json`
- **Estructura:** id, nombre, precio, stock, disponible

---

## 🚨 IMPORTANTE: QUÉ NO HAREMOS HOY

- ❌ Express (llega en Clase 3)
- ❌ Servidores HTTP (llega en Clase 3)
- ❌ npm install de paquetes externos
- ❌ Base de datos reales (MySQL llega en Clase 8)
- ❌ APIs REST (llegan en Clase 3)

---

## 🆘 AYUDA DURANTE LA CLASE

### **❌ Problemas comunes:**

**"npm no se reconoce como comando"**
- Verificar instalación Node.js
- Reiniciar terminal

**"Cannot find module"**
- Verificar que escribiste bien `require('fs')`
- fs viene incluido en Node.js

**"JSON malformado"**
- Verificar comillas dobles en claves
- Usar `JSON.stringify(datos, null, 2)`

**"ENOENT: no such file"**
- Ejecutar crear-datos.js primero
- Verificar nombres exactos de archivos

### **✅ Cómo pedir ayuda:**
1. Compartir pantalla con tu código
2. Mostrar el error exacto en terminal
3. Decir qué estabas intentando hacer

---

## 🏠 TAREA PARA CASA

### **📝 Completar después de clase:**
1. **Agregar más datos:** Expandir a 5 registros en tu JSON
2. **Actualizar README:** Documentar tu proyecto
3. **Verificar funcionamiento:** Todo debe funcionar para Clase 3

### **🎯 Preparación para Clase 3:**
- Express usará tus archivos JSON como "base de datos"
- Crearemos rutas: `GET /posts`, `GET /posts/1`
- Tu archivo JSON será la base de tu API REST

---

## 🔄 CONEXIÓN CON EL CURSO

### **De dónde venimos (Clase 1):**
- ✅ Node.js instalado y funcionando
- ✅ Proyecto personal configurado
- ✅ Git y repositorios configurados

### **A dónde vamos (Clase 3):**
- 🎯 Express y primer servidor HTTP
- 🎯 Rutas REST usando datos JSON
- 🎯 Postman para testing de APIs

---

## 💡 TIPS PARA EL ÉXITO

### **✅ Durante la clase:**
- Seguir las demos paso a paso
- Escribir tu propio código (no copy-paste)
- Preguntar inmediatamente si algo no funciona
- Probar cada ejercicio antes de continuar

### **✅ Al escribir código:**
- Usar nombres descriptivos para variables
- Agregar console.log() para verificar funcionamiento
- Usar try/catch para manejar errores
- Guardar archivos antes de ejecutar

---

## 🚀 ¡EMPEZAMOS!

**¡Bienvenido a los fundamentos de Node.js!** 

Al final de esta clase tendrás:
- 📦 NPM dominado
- 📁 Sistema de archivos funcionando  
- 📊 Datos JSON estructurados
- 🎯 Base sólida para Express

**¡Tu API está tomando forma!** 💪