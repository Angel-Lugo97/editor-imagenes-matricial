## 👨‍💻 Información del Estudiante

- **Nombre:** [Angel Abraham Lugo Saenz]
- **Matrícula:** [SW2409052]
- **Grupo:** [B]
- **Cuatrimestre:** Primer Cuatrimestre
- **Carrera:** TSU en Desarrollo e Innovación de Software
- **Profesor:** Jorge Javier Pedrozo Romero

---

## 📋 Descripción del Proyecto

Este repositorio contiene mi solución a la práctica de **Fundamentos de Programación**, donde implemento funciones en JavaScript para resolver problemas de álgebra básica, preparándome para trabajar con operaciones matriciales más complejas.

## 🎯 Objetivos Alcanzados

- ✅ Dominar variables y tipos de datos en JavaScript
- ✅ Implementar estructuras condicionales
- ✅ Utilizar bucles y funciones
- ✅ Manipular arrays unidimensionales
- ✅ Trabajar con arrays bidimensionales (matrices)
- ✅ Aplicar control de versiones con Git y GitHub

---


## 📊 Progreso de Ejercicios

### Sección 1: Variables y Tipos de Datos (10 pts)
- [x] 1.1 Mi Información (2 pts) ✅
- [x] 1.2 Operaciones Básicas (3 pts) ✅
- [x] 1.3 Área de Rectángulo (2 pts) ✅
- [x] 1.4 Conversión Celsius a Fahrenheit (3 pts) ✅

**Puntos obtenidos: 10/10**

### Sección 2: Condicionales (15 pts)
- [x] 2.1 Par o Impar (3 pts) ✅
- [x] 2.2 Evaluar Nota (4 pts) ✅
- [x] 2.3 Mayor de Tres (4 pts) ✅
- [x] 2.4 Clasificar Edad (4 pts) ✅

**Puntos obtenidos: 15/15**

### Sección 3: Funciones y Bucles (20 pts)
- [x] 3.1 Factorial (5 pts) ✅
- [x] 3.2 Suma Hasta N (4 pts) ✅
- [x] 3.3 Tabla de Multiplicar (5 pts) ✅
- [x] 3.4 Números Pares (6 pts) ✅

**Puntos obtenidos: 20/20**

### Sección 4: Arrays (25 pts)
- [x] 4.1 Suma de Array (4 pts) ✅
- [x] 4.2 Promedio de Array (5 pts) ✅
- [x] 4.3 Encontrar Máximo (6 pts) ✅
- [x] 4.4 Filtrar Mayores (5 pts) ✅
- [x] 4.5 Invertir Array (5 pts) ✅

**Puntos obtenidos: 25/25**

### Sección 5: Arrays Bidimensionales - Matrices (30 pts)
- [x] 5.1 Crear Matriz (6 pts) ✅
- [x] 5.2 Suma de Matriz (6 pts) ✅
- [x] 5.3 Obtener Fila (5 pts) ✅
- [x] 5.4 Obtener Columna (7 pts) ✅
- [x] 5.5 Transponer Matriz (6 pts) ✅

**Puntos obtenidos: 30/30**

---

## 📈 Calificación Final

```
┌────────────────────────────────────────┐
│  REPORTE DE CALIFICACIÓN               │
├────────────────────────────────────────┤
│  Puntos obtenidos: 100/100             │
│  Porcentaje: 100%                      │
│  🎓 Calificación: A - Excelente        │
└────────────────────────────────────────┘
```

![Tests](https://github.com/Angel-Lugo97/editor-imagenes-matricial/actions/workflows/test.yml/badge.svg)




## 🚀 Instalación y Uso

### Prerrequisitos
- Node.js (versión 14 o superior)
- Git

### Clonar el repositorio
```bash
git clone https://github.com/TU-USUARIO/fundamentos-programacion-practica-1.git
cd fundamentos-programacion-practica-1
```

### Instalar dependencias
```bash
npm install
```

### Ejecutar tests
```bash
npm test
```

### Ejecutar tests en modo watch
```bash
npm run test:watch
```

### Ver cobertura de código
```bash
npm run test:coverage
```

---

## 📁 Estructura del Proyecto

```
fundamentos-programacion-practica-1/
│
├── ejercicios.js           # ⭐ Archivo principal con mis soluciones
├── ejercicios.test.js      # Tests automatizados (no modificar)
├── package.json            # Configuración del proyecto
├── README.md               # Este archivo
├── GUIA_ESTUDIANTES.md     # Guía de referencia
├── GUIA_INSTRUCTOR.md      # Guía del profesor
│
└── .github/
    └── workflows/
        └── test.yml        # Configuración de GitHub Actions
```

---

## 💡 Aprendizajes Clave

### Lo que más me costó
- **la investigacion para resolver los diferentes ejercicios**:

Validación de la estructura de los datos de entrada: Si la entrada no está bien estructurada (por ejemplo, si no es una matriz de objetos con propiedades r, g, b, y a), la función puede fallar. Manejar estos errores de forma adecuada o incluso verificar que la entrada tenga la forma correcta podría haber sido algo difícil de anticipar.

Manejo de matrices bidimensionales: Si la matriz de entrada no está claramente definida o si no tienes experiencia con matrices de dos dimensiones, podría haber sido un desafío comprender cómo iterar sobre ellas correctamente, asegurando que cada fila y columna se recorra adecuadamente para aplicar el filtro a cada píxel.
Asegurar el rango de valores para RGB: Las fórmulas para el filtro sepia podrían dar como resultado valores fuera del rango de 0 a 255. Asegurarte de que cada canal de color se mantenga dentro de este rango, usando Math.min() y Math.max(), puede ser confuso si no estás familiarizado con cómo se limitan estos valores en programación.
### Lo que más me gustó
- **Fue siempre la misma investigacion para solucionar los problemas planteados por el profesor**:

// 1. Convertir a escala de grises para simplificar el cálculo
const grises = []

for (let y = 0; y < alto; y++) {
  const filaGris = [];
  for (let x = 0; x < ancho; x++) {
    const p = matriz[y][x];
    // Aplicar fórmula estándar para conversión a gris
    const valorGris = Math.round(
      0.299 * p.r +
      0.587 * p.g +
      0.114 * p.b
    );
    filaGris.push(valorGris);
  }
  grises.push(filaGris);
}

Simplicidad y claridad: La conversión a escala de grises es un paso fundamental cuando se trabaja con imágenes en el contexto de procesamiento de bordes. Esta parte del código lo hace de manera clara y sencilla, utilizando la fórmula estándar (ponderada) que tiene en cuenta la percepción humana de los colores. No hay necesidad de complicarse con transformaciones innecesarias.

Uso de la fórmula estándar: La fórmula que se utiliza (0.299 * r + 0.587 * g + 0.114 * b) está basada en cómo los humanos perciben los colores, dando más peso al verde, luego al rojo y menos al azul. Esto asegura que la conversión a gris refleje de manera más precisa cómo veríamos una imagen en blanco y negro.

Manejo eficiente de la matriz: La función recorre la imagen pixel por pixel, creando una nueva matriz de grises, que es exactamente lo que se necesita para detectar bordes de forma efectiva. El uso de Math.round asegura que los valores de los píxeles sean enteros, lo cual es ideal para los siguientes cálculos.

### Técnicas aplicadas
- detectarBordes
- nversión a escala de grises ponderada (para simplificar el cálculo de bordes)
- Umbralización binaria (para marcar bordes según un umbral de diferencia)
- Manejo de los límites de la imagen (evitar errores al procesar píxeles en los bordes de la matriz)

---

## 🔧 Ejemplos de Código

### Función Favorita: Transponer Matriz
```javascript
function detectarBordes(matriz, umbral = 50) {
   // Obtener dimensiones de la imagen
  const alto = matriz.length;
  const ancho = matriz[0]?.length || 0;

  // 1. Convertir a escala de grises para simplificar el cálculo
  const grises = []

  for (let y = 0; y < alto; y++) {
    const filaGris = [];
    for (let x = 0; x < ancho; x++) {
      const p = matriz[y][x];
      // Aplicar fórmula estándar para conversión a gris
      const valorGris = Math.round(
        0.299 * p.r +
        0.587 * p.g +
        0.114 * p.b
      );
      filaGris.push(valorGris);
    }
    grises.push(filaGris);
  }

  // Crea la matriz resultado para almacenar los bordes detectados
  const resultado = [];

  // 2. Recorre cada píxel y compara con vecinos para detectar cambios bruscos
  for (let y = 0; y < alto; y++) {
    const filaResultado = [];

    for (let x = 0; x < ancho; x++) {
      // Obtiene el valor del pixel central
      const centro = grises[y][x];

      // Para la última fila / última columna no hay derecha o abajo:
      // los dejamos como negro (sin borde) para evitar errores de índice
      if (x === ancho - 1 || y === alto - 1) {
        filaResultado.push({ r: 0, g: 0, b: 0, a: 255 });
        continue;
      }

      // Obtener valores de los píxeles vecinos (derecha y abajo)
      const derecha = grises[y][x + 1];
      const abajo   = grises[y + 1][x];

      // Calcular diferencia máxima con sus vecinos derecha y abajo
      const difDerecha = Math.abs(centro - derecha);
      const difAbajo   = Math.abs(centro - abajo);
      const diferencia = Math.max(difDerecha, difAbajo);

      // Aplica umbral: si la diferencia es mayor al umbral, hay un borde
      const valor = diferencia > umbral ? 255 : 0;

      // Guarda píxel en blanco (borde) o negro (no borde)
      filaResultado.push({
        r: valor,
        g: valor,
        b: valor,
        a: 255 // Canal alpha (transparencia) se mantiene igual
      });
    }

    resultado.push(filaResultado);
  }

  // 3. Devuelve la imagen con bordes detectados
  return resultado;
}
```

**Por qué me gusta:** Demuestra cómo manipular estructuras bidimensionales de forma elegante.

---

## 📚 Recursos Utilizados

- [MDN Web Docs - JavaScript](https://developer.mozilla.org/es/docs/Web/JavaScript)
- [JavaScript.info](https://es.javascript.info/)
- [Stack Overflow](https://stackoverflow.com)
- Guía del estudiante incluida en el repositorio

---

## 🎯 Próximos Pasos

Este proyecto me prepara para:
- ✨ Operaciones matriciales avanzadas (multiplicación, determinantes)
- 🖼️ Desarrollo de editores de imágenes
- 🔐 Implementación de algoritmos de encriptación
- 📊 Creación de calculadoras científicas

---

## 📝 Historial de Commits
```bash
# Ver mi historial completo
git log --oneline --graph --decorate
```

**Commits destacados:**
- 8aa6dff feat: Ejercicios solucionados, empezando a llenar los datos del README
- e9d97d5 feat: Ejercicio 4.3 solucionado
- cecd8a7 feat: Ejercicio 4.2 solucionado
- 9526414 feat: Ejercicio 4.1 solucionado
- 7aa2154 feat: Ejercicio 3.3 solucionado
- 925af83 feat: Ejercicio 3.2 solucionado
- 65725d5 feat: Ejercicio 3.1 solucionado
- f9793a3 feat: Ejercicio 2.3 solucionado
- c00517b feat: Ejercicio 2.2 solucionado
- a459dae feat: Ejercicio 2.1 solucionado
- bb3ae32 feat: Ejercicio 1.4 solucionado
- f970198 feat: Ejercicio 1.3 solucionado
- 65d6189 feat: Ejercicio 1.2 solucionado
- c28b3c0 feat: Ejercicio 1.1 solucionado
- e58c3da feat: Cargar datos basicos
- 4c8c49a feat: prueba de funcionamiento



.
## 🤝 Agradecimientos

- **Profesor Jorge Javier Pedrozo Romero** por la estructura del curso y la práctica
- **Compañeros del Grupo [A/B/C]** por el apoyo mutuo
- **Tecnológico de Software** por la formación integral

---

## 📧 Contacto

- **Email Institucional:** [angel.lugo@tecdesoftware.edu.mx]
- **GitHub:** [@Angel-Lugo97](https://github.com/Angel-Lugo97)

---

## 📄 Licencia

Este proyecto es parte de las actividades académicas del **Tecnológico de Software** y está bajo la licencia MIT.

---

<div align="center">

**⭐ Si te gustó este proyecto, dale una estrella ⭐**

Hecho con 💙 por [Angel Abraham Lugo Saenz] - 2025

</div>
