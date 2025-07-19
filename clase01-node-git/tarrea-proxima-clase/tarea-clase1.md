# 🏠 TAREA PARA PRÓXIMA CLASE

**Tiempo estimado:** 1-2 horas  
**Fecha entrega:** Próxima clase (antes de comenzar)

---

## 📋 PARTE 1: COMPLETAR SETUP (OBLIGATORIO)

### **✅ Verificar que tienes:**
- [ ] **Repositorio GitHub** creado y clonado
- [ ] **Tipo de API elegido** (Blog/Restaurante/E-learning/E-commerce)
- [ ] **Archivo server.js** ejecutándose sin errores
- [ ] **README.md** actualizado con tu información
- [ ] **Primer commit** realizado exitosamente

### **🧪 Comandos que deben funcionar:**
```bash
# En la carpeta de tu proyecto
node server.js
node server.js tu-nombre

# Git funcionando
git status
git log --oneline
```

---

## 💻 PARTE 2: EJERCICIOS DE JAVASCRIPT (PRÁCTICA)

**Crear estos archivos en tu repositorio personal:**

### **Ejercicio 1: practica-arrays.js**
```javascript
// practica-arrays.js
const frutas = ['manzana', 'banana', 'naranja', 'uva', 'kiwi'];

console.log('🍎 Ejercicio Arrays:');

// TODO: Usar forEach para mostrar cada fruta
frutas.forEach(fruta => {
    // Completar aquí
});

// TODO: Usar filter para frutas que tengan más de 5 letras
const frutasLargas = frutas.filter(fruta => {
    // Completar aquí
});
console.log('Frutas largas:', frutasLargas);

// TODO: Usar map para convertir todas a mayúsculas
const frutasMayusculas = frutas.map(fruta => {
    // Completar aquí
});
console.log('En mayúsculas:', frutasMayusculas);

// TODO: Usar find para encontrar 'banana'
const encontrarBanana = frutas.find(fruta => {
    // Completar aquí
});
console.log('Encontré:', encontrarBanana);
```

### **Ejercicio 2: practica-objetos.js**
```javascript
// practica-objetos.js
const usuario = {
    nombre: 'Ana',
    edad: 25,
    email: 'ana@gmail.com',
    activo: true
};

console.log('👤 Ejercicio Objetos:');

// TODO: Usar destructuring para extraer nombre y email
// const { nombre, email } = ...

// TODO: Agregar una nueva propiedad 'telefono'
// usuario.telefono = ...

// TODO: Crear función que valide si el usuario es mayor de edad
function esMayorDeEdad(usuario) {
    // Completar aquí
}

// TODO: Mostrar info completa con template literals
// console.log(`Información: ...`);
console.log('¿Es mayor de edad?', esMayorDeEdad(usuario));
```

### **Ejercicio 3: practica-funciones.js**
```javascript
// practica-funciones.js
console.log('⚡ Ejercicio Funciones:');

// TODO: Crear función tradicional que sume dos números
function sumar(a, b) {
    // Completar aquí
}

// TODO: Crear arrow function que calcule el área de un círculo
const areaCirculo = (radio) => {
    // Completar aquí (π × radio²)
};

// TODO: Crear función que reciba un array y devuelva el mayor
const encontrarMayor = (numeros) => {
    // Completar aquí
};

// TODO: Crear función con valores por defecto
function saludar(nombre = 'Usuario') {
    // Completar aquí
}

// Probar todas las funciones
console.log('Suma 5 + 3:', sumar(5, 3));
console.log('Área círculo radio 5:', areaCirculo(5));
console.log('Mayor de [2,8,3,1]:', encontrarMayor([2, 8, 3, 1]));
console.log(saludar('Luis'));
```

---

## 📖 LECTURA RECOMENDADA

- [NPM Básico](https://docs.npmjs.com/getting-started) - 15 minutos
- [Módulos Node.js](https://nodejs.org/docs/latest/api/modules.html) - Solo introducción

---

## ✅ CHECKLIST ANTES DE LA PRÓXIMA CLASE

- [ ] Repositorio funcionando correctamente
- [ ] Ejercicio 1 (arrays) completado
- [ ] Ejercicio 2 (objetos) completado  
- [ ] Ejercicio 3 (funciones) completado
- [ ] Dudas anotadas para preguntarlas en clase

---

## 🆘 ¿NECESITAS AYUDA?

**Si algo no funciona:**
- Revisa que Node.js esté instalado: `node --version`
- Verifica que estés en la carpeta correcta
- Lee los mensajes de error cuidadosamente
- Anota las dudas para la próxima clase

**Recuerda:** Es normal que algunos ejercicios sean desafiantes. ¡Lo importante es intentarlo y aprender en el proceso!

---

## 🎯 PRÓXIMA CLASE: Node.js Fundamentos

**Veremos:**
- NPM y package.json
- Módulos built-in (fs, path)
- Crear y usar módulos propios
- Trabajar con archivos JSON

¡Nos vemos en la próxima clase! 🚀