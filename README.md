# 🧮 Calculadora Multifuncional en PSeInt

> Sistema completo de calculadora desarrollado en PSeInt con funcionalidades extendidas de cálculo, geometría, estadística y sucesiones matemáticas.

---

## 📋 Tabla de Contenidos

- [Descripción](#-descripción)
- [Características](#-características)
- [Instalación](#-instalación)
- [Uso](#-uso)
- [Arquitectura](#-arquitectura)
- [Módulos](#️-módulos)
- [Capturas de Pantalla](#-capturas-de-pantalla)
- [Dificultades Encontradas](#-dificultades-encontradas)
- [Contribuciones](#-contribuciones)
- [Autores](#-autores)
- [Licencia](#-licencia)

---

## 📖 Descripción

### ¿Qué hicimos?

Desarrollamos una **calculadora multifuncional completa** en PSeInt que integra cuatro módulos principales:

1. **Operaciones Básicas**: Suma, resta, multiplicación y división con validación de errores
2. **Cálculos Geométricos**: Áreas, perímetros, diámetros y radios de figuras geométricas
3. **Estadística Básica**: Cálculo de media, mediana y moda de conjuntos de datos
4. **Sucesión de Fibonacci**: Generador matemáticamente correcto de la sucesión de Fibonacci

### ¿Para qué lo hicimos?

Este proyecto fue diseñado con los siguientes propósitos:

- **Académico**: Demostrar dominio en programación estructurada y pseudocódigo
- **Práctico**: Crear una herramienta funcional para cálculos matemáticos diversos
- **Profesional**: Aplicar buenas prácticas de documentación y control de versiones
- **Educativo**: Servir como referencia para futuros desarrolladores y estudiantes

### ¿Cómo lo hicimos?

Implementamos una **arquitectura modular** con las siguientes características técnicas:

#### 🎯 Principios de Diseño

- **Modularidad**: Cada funcionalidad está encapsulada en subprocesos independientes
- **Reutilización**: Funciones auxiliares compartidas entre módulos
- **Validación**: Control de errores en todas las entradas de usuario
- **Usabilidad**: Interfaz intuitiva con menús claros y navegación fluida

#### 🛠️ Técnicas Implementadas

- Estructuras de control (Mientras, Para, Segun)
- Subprocesos y funciones parametrizadas
- Arrays para manejo de datos estadísticos
- Algoritmo de ordenamiento burbuja para estadística
- Algoritmos matemáticos precisos (área de círculo con π, Fibonacci real)

---

## ✨ Características

### Funcionalidades Principales

#### 1️⃣ **Operaciones Básicas**
- ✅ Suma de dos números
- ✅ Resta de dos números
- ✅ Multiplicación de dos números
- ✅ División con protección contra división por cero

#### 2️⃣ **Cálculos Geométricos**

| Figura | Cálculos Disponibles |
|--------|---------------------|
| **Círculo** | Área, Radio, Diámetro |
| **Cuadrado** | Área, Perímetro |
| **Triángulo** | Área (base × altura) |
| **Trapecio** | Área (bases + altura) |

#### 3️⃣ **Estadística Básica**
- 📊 **Media aritmética** (promedio)
- 📈 **Mediana** (valor central)
- 📉 **Moda** (valor más frecuente)
- 🔢 Soporta hasta 100 números
- 🔄 Ordenamiento automático de datos

#### 4️⃣ **Sucesión de Fibonacci**
- ✅ Generación matemáticamente correcta
- ✅ Inicio desde cualquier número de Fibonacci válido
- ✅ Advertencias si el número no pertenece a la sucesión
- ✅ Generación configurable (1-50 términos)

### Características Técnicas

- 🛡️ **Validación de entradas**: Previene errores de usuario
- 🔄 **Navegación cíclica**: Permite múltiples operaciones sin reiniciar
- 🎨 **Interfaz visual**: Menús con formato ASCII art
- 📝 **Código comentado**: Documentación inline completa
- ⚡ **Eficiente**: Algoritmos optimizados

---

## 💾 Instalación

### Requisitos Previos

- **PSeInt** versión 20190822 o superior
- Sistema operativo: Windows, Linux o macOS
- 10 MB de espacio en disco

### Pasos de Instalación

1. **Descargar PSeInt**
   ```
   https://pseint.sourceforge.net/
   ```

2. **Clonar el repositorio**
   ```bash
   git clone https://github.com/tuusuario/calculadora-pseint.git
   cd calculadora-pseint
   ```

3. **Abrir el archivo**
   - Iniciar PSeInt
   - Archivo → Abrir
   - Seleccionar `CalculadoraMultifuncional.psc`

4. **Ejecutar**
   - Presionar F9 o clic en "Ejecutar"

---

## 🚀 Uso

### Inicio Rápido

1. Ejecutar el programa
2. Seleccionar una opción del menú principal (1-5)
3. Seguir las instrucciones en pantalla
4. Los resultados se mostrarán automáticamente

### Ejemplos de Uso

#### Ejemplo 1: Operación Básica (División)
```
 === OPERACIONES BÁSICAS ===
Ingrese el primer número: 
5
Ingrese el segundo número: 
4
Suma: 9
Resta: 1
Multiplicación: 20
División: 1.25

```

#### Ejemplo 2: Cálculo Geométrico (Círculo)
```
Menú Principal → 2 (Cálculos Geométricos)
Submenu → 1 (Círculo)
Radio: 5
Resultados:
  - Área: 78.5
  - Diámetro: 10
  - Radio: 5
```

#### Ejemplo 3: Estadística
```
Menú Principal → 3 (Estadística Básica)
Cantidad de números: 5
Números: 10, 20, 20, 30, 40
Resultados:
  - Media: 24
  - Mediana: 20
  - Moda: 20 (aparece 2 veces)
```

#### Ejemplo 4: Fibonacci
```
Menú Principal → 4 (Sucesión de Fibonacci)
Número inicial: 5
Términos a generar: 7
Resultados:
  Término 1: 5
  Término 2: 5
  Término 3: 10
  Término 4: 15
  Término 5: 25
  Término 6: 40
  Término 7: 6
  ...
```

---

## 🏗️ Arquitectura

### Estructura del Código

```
CalculadoraMultifuncional.psc
│
├── Algoritmo Principal
│   ├── Bucle principal con menú
│   └── Control de flujo general
│
├── Módulo 1: Operaciones Básicas
│   ├── MostrarMenuPrincipal()
│   └── MenuOperacionesBasicas()
│       ├── Suma
│       ├── Resta
│       ├── Multiplicación
│       └── División (con validación)
│
├── Módulo 2: Cálculos Geométricos
│   ├── MenuCalculosGeometricos()
│   ├── CalcularCirculo()
│   ├── CalcularCuadrado()
│   ├── CalcularTriangulo()
│   └── CalcularTrapecio()
│
├── Módulo 3: Estadística
│   └── MenuEstadistica()
│       ├── Captura de datos
│       ├── Ordenamiento (Burbuja)
│       ├── Cálculo de Media
│       ├── Cálculo de Mediana
│       └── Cálculo de Moda
│
└── Módulo 4: Fibonacci
    └── GenerarFibonacci()
        ├── Validación de entrada
        ├── Búsqueda en sucesión
        └── Generación de términos
```

### Diagrama de Flujo Principal

```
[INICIO]
   ↓
[Mostrar Menú Principal]
   ↓
[Leer Opción del Usuario]
   ↓
   ├─→ Opción 1: [Operaciones Básicas] → [Ejecutar] → [¿Continuar?]
   ├─→ Opción 2: [Cálculos Geométricos] → [Ejecutar] → [¿Continuar?]
   ├─→ Opción 3: [Estadística] → [Ejecutar] → [¿Continuar?]
   ├─→ Opción 4: [Fibonacci] → [Ejecutar] → [¿Continuar?]
   └─→ Opción 5: [Salir] → [FIN]
```

---

## 🛠️ Módulos

### Módulo 1: Operaciones Básicas

**Propósito**: Realizar cálculos aritméticos fundamentales con validación de errores.

**Funciones**:
- Suma de dos números reales
- Resta de dos números reales
- Multiplicación de dos números reales
- División con protección contra división por cero

**Validaciones**:
- ✅ Verifica divisor ≠ 0
- ✅ Soporta números decimales
- ✅ Manejo de números negativos

---

### Módulo 2: Cálculos Geométricos

**Propósito**: Calcular propiedades de figuras geométricas básicas.

**Fórmulas Implementadas**:

| Figura | Fórmula del Área | Extras |
|--------|-----------------|--------|
| Círculo | A = π × r² | Diámetro = 2r |
| Cuadrado | A = l² | Perímetro = 4l |
| Triángulo | A = (b × h) / 2 | - |
| Trapecio | A = [(B + b) × h] / 2 | - |

**Validaciones**:
- ✅ Todas las medidas deben ser > 0
- ✅ Uso de π con 11 decimales de precisión
- ✅ Resultados formateados con claridad

---

### Módulo 3: Estadística Básica

**Propósito**: Analizar conjuntos de datos numéricos.

**Algoritmos Implementados**:

#### Media (Promedio)
```
Media = Σ(xi) / n
Donde: xi = cada valor, n = cantidad de valores
```

#### Mediana
```
Si n es par: Mediana = (valor[n/2] + valor[n/2+1]) / 2
Si n es impar: Mediana = valor[(n+1)/2]
*Requiere datos ordenados
```

#### Moda
```
Moda = Valor con mayor frecuencia
*Si todos son únicos, no hay moda
```

**Características**:
- Ordenamiento automático (algoritmo burbuja)
- Soporta 2-100 números
- Identifica si no hay moda
- Muestra frecuencia de la moda

---

### Módulo 4: Sucesión de Fibonacci

**Propósito**: Generar términos de la sucesión real de Fibonacci.

**Algoritmo**:
```
F(0) = 0
F(1) = 1
F(n) = F(n-1) + F(n-2)  para n ≥ 2
```

**Características Especiales**:
- ✅ No inventa números: sigue la lógica matemática estricta

**Validaciones**:
- ✅ Número inicial ≥ 0
- ✅ Cantidad de términos entre 1-50

---

## 📸 Capturas de Pantalla

### Menú Principal
```
╔════════════════════════════════════════════════╗
║    CALCULADORA MULTIFUNCIONAL - PSEINT         ║
╠════════════════════════════════════════════════╣
║  1. Operaciones Básicas                        ║
║  2. Cálculos Geométricos                       ║
║  3. Estadística Básica                         ║
║  4. Sucesión de Fibonacci                      ║
║  5. Salir                                      ║
╚════════════════════════════════════════════════╝
```

### Ejemplo de Salida - Estadística
```
════════════════ RESULTADOS ESTADÍSTICOS ════════════════
Cantidad de números: 7
Media (Promedio):    28.5714
Mediana:             25
Moda:                30 (aparece 2 veces)
═══════════════════════════════════════════════════════
```

---

## 🚧 Dificultades Encontradas

### 1. **Cálculo de la Moda con Datos No Repetidos**

**Problema**: 
Inicialmente, el algoritmo siempre mostraba un valor como moda, incluso cuando todos los números eran únicos.

**Solución**:
Implementamos una verificación de `maxFrecuencia`. Si la frecuencia máxima es 1, significa que todos los valores aparecen solo una vez, por lo que no hay moda estadísticamente significativa.

```pseint
Si maxFrecuencia > 1 Entonces
    Escribir "Moda: ", moda
SiNo
    Escribir "No hay moda (todos los valores son únicos)"
FinSi
```

**Lección Aprendida**: Es fundamental validar casos extremos en algoritmos estadísticos.

---

### 2. **Validación de Números en Sucesión de Fibonacci**

**Problema**:
El requerimiento especificaba que SOLO se deben mostrar números que pertenecen a la sucesión REAL de Fibonacci. Un usuario podría ingresar cualquier número (ej: 7, 100).

**Solución**:
Implementamos un algoritmo que:
1. Genera la sucesión de Fibonacci hasta encontrar o superar el número ingresado
2. Verifica si el número ingresado coincide exactamente con un término de Fibonacci
3. Si no coincide, advierte al usuario y comienza desde el siguiente número válido

```pseint
Mientras fib2 < numInicial Hacer
    fibSiguiente <- fib1 + fib2
    fib1 <- fib2
    fib2 <- fibSiguiente
FinMientras

Si fib2 = numInicial Entonces
    // Número válido encontrado
SiNo
    Escribir "ADVERTENCIA: No pertenece a Fibonacci"
    Escribir "Se comenzará desde: ", fib2
FinSi
```

**Lección Aprendida**: La validación matemática rigurosa es esencial para cumplir especificaciones precisas.

---

### 3. **Limitaciones de Arrays en PSeInt**

**Problema**:
PSeInt no permite arrays dinámicos, lo que limitaba el módulo de estadística.

**Solución**:
- Definimos un array de tamaño fijo máximo (100 elementos)
- Implementamos validación para que el usuario no pueda ingresar más de 100 números
- Usamos una variable `n` para controlar cuántos elementos del array están realmente en uso

```pseint
Dimension numeros[100]
Repetir
    Leer n
    Si n < 2 O n > 100 Entonces
        Escribir "ERROR: Debe ingresar entre 2 y 100 números"
    FinSi
Hasta Que n >= 2 Y n <= 100
```

**Lección Aprendida**: Las limitaciones del lenguaje requieren soluciones creativas que no comprometan la funcionalidad.

---

### 4. **Precisión de π (Pi)**

**Problema**:
El cálculo del área de círculos requería precisión en el valor de π.

**Solución**:
Definimos π con 11 decimales de precisión:
```pseint
PI <- 3.14159265359
```

**Alternativas Consideradas**:
- Usar π = 3.14 (rechazado por baja precisión)
- Usar π = 22/7 (rechazado por ser menos preciso que 3.14159...)

**Lección Aprendida**: La precisión numérica impacta directamente la calidad de los resultados.

---

### 5. **División por Cero**

**Problema**:
La división sin validación causaba errores de ejecución.

**Solución**:
Validación explícita antes de realizar la operación:
```pseint
Si num2 = 0 Entonces
    Escribir "ERROR: No se puede dividir entre cero"
SiNo
    resultado <- num1 / num2
FinSi
```

**Lección Aprendida**: Siempre anticipar y prevenir errores matemáticos comunes.

---

### 6. **Ordenamiento de Datos para Mediana**

**Problema**:
El cálculo de la mediana requiere datos ordenados, pero PSeInt no tiene funciones de ordenamiento integradas.

**Solución**:
Implementamos el algoritmo de **ordenamiento burbuja** (Bubble Sort):

```pseint
Para i <- 1 Hasta n-1 Con Paso 1 Hacer
    Para j <- 1 Hasta n-i Con Paso 1 Hacer
        Si numeros[j] > numeros[j+1] Entonces
            temp <- numeros[j]
            numeros[j] <- numeros[j+1]
            numeros[j+1] <- temp
        FinSi
    FinPara
FinPara
```

**Por qué Burbuja**:
- Simple de implementar
- Suficientemente eficiente para n ≤ 100
- Fácil de entender y mantener

**Lección Aprendida**: A veces los algoritmos "básicos" son la mejor solución para el contexto.

---

### 7. **Experiencia de Usuario en Validaciones**

**Problema**:
Validaciones muy estrictas frustraban al usuario sin dar feedback claro.

**Solución**:
- Mensajes de error descriptivos
- Bucles `Repetir-Hasta` que permiten reintentar
- Indicación de rangos válidos en los prompts

```pseint
Repetir
    Escribir "¿Cuántos números desea ingresar? (2-100): "
    Leer n
    Si n < 2 O n > 100 Entonces
        Escribir "ERROR: Debe ingresar entre 2 y 100 números"
    FinSi
Hasta Que n >= 2 Y n <= 100
```

**Lección Aprendida**: La usabilidad es tan importante como la funcionalidad.

---

## 📊 Mejoras Futuras

- [ ] Soporte para más figuras geométricas (pentágono, hexágono)
- [ ] Cálculo de desviación estándar y varianza
- [ ] Historial de operaciones realizadas
- [ ] Exportación de resultados a archivo de texto
- [ ] Modo científico con funciones trigonométricas
- [ ] Calculadora de matrices

---

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Para contribuir:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/NuevaFuncionalidad`)
3. Commit tus cambios (`git commit -m 'Agrega nueva funcionalidad'`)
4. Push a la rama (`git push origin feature/NuevaFuncionalidad`)
5. Abre un Pull Request

### Guía de Estilo

- Comentar cada subproceso con su propósito
- Usar nombres descriptivos para variables
- Validar todas las entradas de usuario
- Mantener consistencia en formato de menús

---

## 👥 Autores

**-Loredo Villanueva Paola Jocelyn**
**-Olalde Campos Schoenstatt**
**-Olvera Hernandez Maria Guadalupe**
**-Perez Mendoza Roxana**
- GitHub: [@tuusuario](https://github.com/sxhoenstatt23)
- Email: 024000641@upsrj.edu.mx

**Proyecto**: Optativa 1
**Institución**: Universidad Politécnica de Santa Rosa Jauregui
**Fecha**: 13 Noviembre 2025

---

## 📄 Licencia

Este proyecto está bajo la Licencia MIT

---

## 🙏 Agradecimientos

- A PSeInt por proporcionar una herramienta educativa excelente
- A la comunidad de GitHub por las mejores prácticas

---

## 📞 Soporte

Si encuentras algún bug o tienes sugerencias:
1. Crea un nuevo Issue si es necesario
2. Describe el problema con el mayor detalle posible

---

**⭐ Si este proyecto te fue útil, considera darle una estrella en GitHub**

---

*Desarrollado con 💙 en PSeInt*
