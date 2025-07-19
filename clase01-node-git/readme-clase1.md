# 📚 CLASE 1 - Repaso JS/Git + Intro Node.js + Setup Proyecto API

## 🎯 OBJETIVO DE LA CLASE
Repasar fundamentos de JavaScript y Git, aprender Node.js básico y configurar tu proyecto personal de API.

**Duración:** 3 horas

---

## 📋 LO QUE VAS A LOGRAR HOY

- ✅ **Repasar JavaScript** y Git esenciales para backend
- ✅ **Entender Node.js** y ejecutar tu primer script
- ✅ **Elegir tu tipo de API** personal (Blog, Restaurante, E-learning o E-commerce)
- ✅ **Configurar tu repositorio** GitHub personal
- ✅ **Crear tu primer script** Node.js funcionando

---

## 🛠️ HERRAMIENTAS NECESARIAS

Verificar que tienes todo instalado:

```bash
# Verificar Node.js (debe ser v18 o superior)
node --version

# Verificar NPM
npm --version

# Verificar Git
git --version

# Verificar VS Code
code --version
```

**¿Algo no funciona?** Pregunta en chat para resolverlo rápidamente.

---

## 📚 REPASO RÁPIDO

### **JavaScript Básico**
- Variables: `const` y `let` (NO usar `var`)
- Condicionales: `if/else` con `===`
- Bucles: `for`, `forEach`
- Funciones: tradicionales vs arrow functions

### **Git Workflow**
- `git add .` - Agregar cambios
- `git commit -m "mensaje"` - Guardar cambios
- `git push` - Subir a GitHub
- `git pull` - Bajar cambios

---

## ⚡ INTRODUCCIÓN A NODE.JS

### **¿Qué es Node.js?**
JavaScript que corre **fuera del navegador** en tu computadora.

### **Diferencias clave:**
- **Navegador:** DOM, window, alert()
- **Node.js:** archivos, process, console.log()

### **Tu primer script Node.js:**
```javascript
// archivo: saludo.js
console.log('¡Hola desde Node.js!');

const args = process.argv.slice(2);
const nombre = args[0];

console.log(`Hola ${nombre}!`);
```

**Ejecutar:**
```bash
node saludo.js Ana
```

---

## 🎯 ELIGE TU PROYECTO API

**Vas a elegir UNA de estas 4 opciones:**

### 📝 **Blog Personal**
- Posts, categorías, comentarios
- **Usuarios:** autores, lectores, admins
- **Ideal para:** escritores, bloggers

### 🍽️ **Restaurante**
- Menú, pedidos, gestión
- **Usuarios:** clientes, staff, admins  
- **Ideal para:** emprendedores, foodies

### 📚 **E-learning**
- Cursos, lecciones, inscripciones
- **Usuarios:** estudiantes, instructores, admins
- **Ideal para:** educadores, estudiantes

### 🛍️ **E-commerce**
- Productos, carrito, pedidos
- **Usuarios:** clientes, vendedores, admins
- **Ideal para:** interesados en comercio digital

**Al final del curso tendrás:**
- 🔐 Sistema de autenticación completo
- 📊 API REST con todas las operaciones CRUD
- 🗄️ Base de datos MySQL con relaciones
- 🚀 Deploy gratuito con URL pública

---

## 💻 SETUP DE TU PROYECTO PERSONAL

### **Paso 1: Crear repositorio en GitHub**
1. Ir a github.com
2. Click "New Repository"
3. Nombre: `mi-api-[tu-eleccion]`
   - `mi-api-blog`
   - `mi-api-restaurante`
   - `mi-api-elearning` 
   - `mi-api-ecommerce`
4. ✅ **Marcar "Add a README file"**
5. ✅ **Marcar "Add .gitignore: Node"**
6. Click "Create repository"

### **Paso 2: Clonar a tu computadora**
```bash
# Clonar (cambiar por tu URL)
git clone https://github.com/tu-usuario/mi-api-blog.git

# Entrar a la carpeta
cd mi-api-blog

# Verificar
git status
```

### **Paso 3: Crear tu primer script**
Crear archivo `server.js`:

```javascript
// server.js
console.log('🚀 Hola! Soy tu API personal');
console.log('📅 Fecha:', new Date().toLocaleDateString());

const args = process.argv.slice(2);

if (args.length === 0) {
    console.log('💡 Prueba: node server.js tu-nombre');
} else {
    const nombre = args[0];
    console.log(`👋 Hola ${nombre}! Tu API está funcionando`);
}

console.log('✅ Script ejecutado correctamente');
```

**Probar:**
```bash
node server.js
node server.js Ana
```

### **Paso 4: Primer commit**
```bash
# Agregar archivos
git add .

# Hacer commit
git commit -m "Clase 1: Setup inicial + primer script Node.js"

# Subir a GitHub
git push origin main
```

### **Paso 5: Documentar tu proyecto**
Actualizar `README.md`:

```markdown
# Mi API [TIPO] - Curso Backend ComuIT

## 📋 Información del Proyecto
- **Tipo:** [Blog/Restaurante/E-learning/E-commerce] 
- **Autor:** [Tu Nombre]
- **Fecha inicio:** [Fecha de hoy]

## 🎯 Objetivo
Crear una API completa con autenticación durante el curso

## 📚 Progreso
- [x] **Clase 1:** Setup inicial + Node.js básico
- [ ] **Clase 2:** NPM y módulos
- [ ] **Clase 3:** Express básico

## 🧪 Comandos
```bash
# Ejecutar script
node server.js

# Probar con nombre
node server.js Ana
```

## 📝 Notas
[Aquí anota lo que aprendas cada clase]
```

---

## ✅ CHECKLIST FINAL

Antes de terminar, verifica que tienes:

- [ ] Node.js funcionando (`node --version`)
- [ ] Repositorio GitHub creado y clonado
- [ ] Archivo `server.js` ejecutándose sin errores
- [ ] Tipo de API elegido y documentado
- [ ] Primer commit realizado (`git log`)
- [ ] README.md actualizado con tu información

---

## 🏠 TAREA PARA PRÓXIMA CLASE

- 📖 **Leer** documentación básica de NPM
- 💭 **Pensar** en funcionalidades específicas para tu API
- 🔄 **Practicar** comandos: `node server.js`
- 📝 **Documentar** tus ideas en README.md

---

## 🆘 AYUDA

**¿Algo no funciona?**
- Pregunta en chat con captura del error
- Comparte pantalla si necesitas ayuda
- Verifica que Node.js y Git estén bien instalados

---

## 🚀 PRÓXIMA CLASE

**Clase 2: Node.js Fundamentos**
- NPM y package.json
- Módulos built-in (fs, path)
- Crear y usar módulos propios
- Trabajar con archivos JSON

**¡Preparado para crear tu API completa!** 🎯