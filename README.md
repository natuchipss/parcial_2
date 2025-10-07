# Manual de Videojuegos  
**Documento Ejecutivo**

---

### Curso:  
**Modelos y Documentación de Software**

### Profesor:  
**Ing. Hely Suárez Marín**

### Integrantes del equipo:  
- José David Cuberos  
- Natalia Salcedo  

### Fecha:  
**Noviembre 2025**

---

## 🧩 Resumen Ejecutivo

### Problema:
En el desarrollo de videojuegos, muchas veces la documentación es confusa o está incompleta. Es común que la información esté repartida en varios archivos o que no haya una guía visual que conecte todo el funcionamiento del juego.  
Esto provoca que los equipos de trabajo (diseñadores, programadores y testers) pierdan tiempo tratando de entender cómo está hecho el sistema o cómo se relacionan sus partes.

### Solución:
Nuestro proyecto propone la creación de un **Manual Digital de Videojuegos**, pensado como una guía visual y técnica dentro de la aplicación *Gaming Manual App*.  
Este manual no es una app terminada, sino un ejercicio de documentación en el que usamos **diagramas UML** para representar cómo funcionaría el sistema.  
El objetivo es mostrar, de manera clara y ordenada, tanto la estructura del videojuego (sus partes internas) como su comportamiento (cómo actúa y reacciona).

### Impacto:
Con este enfoque, se logra que cualquier persona del equipo —sin importar su rol o nivel técnico— pueda entender fácilmente cómo se organiza el videojuego.  
Además, los diagramas sirven como una referencia visual que mejora la comunicación, evita errores y facilita el aprendizaje de quienes se integran al proyecto.

### Conclusión:
El manual basado en UML se convierte en una herramienta que combina explicación, diseño y visualización, ayudando a que el proyecto sea más claro, ordenado y fácil de mantener en el futuro.

---

## 📘 Definición del Problema
Normalmente, los manuales de videojuegos se enfocan en describir botones, controles o imágenes, pero dejan de lado cómo está estructurado el sistema internamente.  
Esto genera confusiones al momento de desarrollar, ya que no hay una conexión clara entre la interfaz del jugador, las reglas del juego y la lógica que hay detrás.  
Por eso, en *Gaming Manual App* vimos la necesidad de crear un manual más completo, que no solo describa, sino que también muestre gráficamente cómo funciona todo.  
Para esto usamos **UML**, un lenguaje visual que nos permite representar tanto la parte técnica como las interacciones del jugador.

---

## 💡 Solución Propuesta
La solución fue desarrollar la documentación del manual digital, utilizando **diagramas UML** para explicar cómo estaría estructurado el videojuego y cómo se comportaría.  
Los diagramas se dividen en dos grandes grupos: **estáticos (la parte fija del sistema)** y **dinámicos (la parte que cambia y se mueve)**.

---

## 🧱 Diagramas Estáticos (Estructurales)

Los diagramas estáticos muestran cómo está formado el sistema, sus partes, jerarquías y relaciones internas. Es como ver el “esqueleto” del videojuego.

### 1. Diagrama de Clases
Muestra las partes principales del sistema, como **Jugador**, **Inventario**, **Misión**, **Enemigo**, **Nivel** y **Recompensa**.  
Ayuda a entender qué datos guarda cada clase y qué funciones cumple dentro del juego.

### 2. Diagrama de Componentes
Divide el sistema en módulos o secciones, por ejemplo:
- Gestión de Usuarios  
- Gestión del Juego  
- Gestión del Manual  

Cada módulo tiene una función clara dentro del proyecto.

### 3. Diagrama de Paquetes
Agrupa las clases en bloques más grandes, como **InterfazUsuario**, **LógicaDelJuego** y **Persistencia**.  
Esto permite visualizar cómo se organizan las partes y qué depende de qué.

### 4. Diagrama de Despliegue
Muestra cómo estaría distribuido el sistema físicamente, por ejemplo:
- Un cliente web (usuario)  
- Un servidor de aplicaciones  
- Una base de datos  

También se incluyen los archivos que formarían parte del sistema, como `ManualApp_UI.html` o `DB_Script.sql`.

### 5. Diagrama de Estructura Compuesta
Detalla la clase **Jugador**, mostrando lo que tiene dentro: **Inventario**, **Estadísticas**, **Perfil** y **ControlDeJuego**.  
Así se entiende cómo interactúan esas partes internas y qué funciones usa cada una.

### 6. Diagrama de Objetos
Muestra ejemplos reales de cómo se verían las clases cuando el juego está en uso.  
Por ejemplo:  
`jugador1: Jugador` con `nombre = "Ana"` y `nivel = 5`.  
Es una forma sencilla de ver cómo los datos del modelo se convierten en algo funcional.

---

## ⚙️ Diagramas Dinámicos (Comportamentales)

Los diagramas dinámicos muestran cómo se comporta el sistema mientras el jugador lo usa.  
Es decir, representan el movimiento, las acciones y las decisiones.

### 1. Diagrama de Casos de Uso
Describe las acciones principales que el jugador puede hacer: **iniciar sesión**, **jugar**, **guardar el progreso**, **comprar ítems**, etc.  
También muestra cómo se relacionan los actores (jugador, sistema, servidor).

### 2. Diagrama de Secuencia
Explica paso a paso cómo se comunican las partes del sistema cuando se realiza una acción, por ejemplo, **“iniciar una partida”** o **“guardar el progreso”**.

### 3. Diagrama de Comunicación
Representa esas mismas interacciones, pero de forma más visual, como una red que conecta los objetos que colaboran entre sí.

### 4. Diagrama de Estados
Muestra los diferentes estados del jugador, por ejemplo:  
**Inactivo → Jugando → Pausado → Finalizado**, y cómo pasa de uno a otro.

### 5. Diagrama de Actividades
Representa el flujo completo del juego, desde que el jugador entra hasta que termina, incluyendo decisiones como:  
- “¿Credenciales válidas?”  
- “¿Desea guardar el progreso?”

### 6. Diagrama de Tiempo
Indica la duración de ciertos procesos, como la carga de niveles o la sincronización de datos con el servidor.  
Permite analizar los tiempos y optimizar la experiencia del jugador.

---

---
