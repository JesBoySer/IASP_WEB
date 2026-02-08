# Unidad 3.2 - Pensar Diferente para Resolver Problemas

| Tipo de Elemento | Identificador | Descripción |
| :--- | :--- | :--- |
| **Resultado de Aprendizaje (RA)** | **RA3** | Propone ideas innovadoras aplicando técnicas básicas de pensamiento creativo y resolución de problemas en contextos productivos. |
| **Criterio de Evaluación (CE)** | **b)** | Se han empleado habilidades básicas de análisis y resolución de problemas para identificar oportunidades de innovación en entornos empresariales del sector. |

---

## Introducción: La Creatividad como Herramienta

La innovación no es magia, es **creatividad aplicada**. En nuestro sector (Informática y Comunicaciones), esto significa utilizar métodos estructurados para generar nuevas ideas (**Pensamiento Divergente**) y, a su vez, utilizar métodos de análisis para desentrañar por qué fallan los sistemas o procesos (**Resolución de Problemas**).

**Ser creativo no es opcional; es una habilidad técnica que se entrena.**

![Presentación de la lección](../images/Unidad_3.2_Pensar_diferente_para_resolver_problemas.pdf) 
---

## 1. Técnicas de Pensamiento Creativo (Generación de Ideas)

Estas herramientas ayudan a generar un **gran volumen** de ideas, incluso las que parecen inusuales, antes de filtrarlas.

### 1.1 Lluvia de Ideas (*Brainstorming*)

| Concepto | Reglas Clave |
| :--- | :--- |
| Generar el **mayor número de ideas posibles** en un tiempo limitado. La **cantidad** es más importante que la **calidad** en esta fase inicial. | 1. **Cero Críticas:** No juzgar ni criticar las ideas. |
| | 2. **Libertad Total:** ¡Cualquier idea es válida! |
| | 3. **Construye:** Utiliza las ideas de otros para lanzar la tuya ("Sí, y además..."). |

> **Ejemplo Tech:** Un equipo busca la próxima función estrella de una app de mensajería: "Mensajes con realidad aumentada", "Modo silencio que solo permite la entrada de mensajes de emergencia", "Integración de un mini-juego P2P", etc.

### 1.2 SCAMPER (Un Check-List para la Innovación)

SCAMPER utiliza una serie de verbos de acción para forzar una perspectiva diferente sobre un producto o proceso existente.

| Verbo | Pregunta Clave | Ejemplo Aplicado a la Tecnología |
| :--- | :--- | :--- |
| **S**ustituir | ¿Qué podemos reemplazar? | Sustituir el login tradicional por **autenticación sin contraseña** (Magic Link). |
| **C**ombinar | ¿Qué podemos mezclar? | Combinar un servicio de **video streaming con la compra de productos** que aparecen en pantalla. |
| **A**daptar | ¿Qué podemos copiar de otros? | Adaptar la mecánica de **puntos/recompensas de los videojuegos** (gamificación) a una plataforma educativa. |
| **M**odificar | ¿Qué podemos cambiar (forma, tamaño, color)? | Modificar un servidor haciéndolo **modular y escalable** (*microservicios*). |
| **P**rop. Otros Usos | ¿Para qué más sirve? | Usar la **cámara de un móvil** (diseñada para fotos) para leer códigos QR o escanear documentos. |
| **E**liminar | ¿Qué podemos quitar o simplificar? | Eliminar la necesidad de tener la app instalada con el uso de **Web Apps Progresivas (PWA)**. |
| **R**eorganizar/Revertir | ¿Qué pasa si invertimos el proceso? | En lugar de que el usuario busque contenido, que el **contenido lo encuentre a él** (algoritmos de recomendación). |

### 1.3 Mapa Mental (*Mind Map*)

* **Concepto:** Representación gráfica y jerárquica de ideas. Empiezas con un concepto central y vas creando ramas con subtemas.
* **Utilidad:** Ideal para **estructurar la arquitectura** de un proyecto, planificar el contenido de una web, o visualizar la estructura de una base de datos.

> **Ejemplo Tech:**
> * **Concepto Central:** **"Rediseño de la Intranet del IES"**.
> * **Ramas Principales:** `Frontend (Diseño)`, `Backend (Servidor)`, `Base de Datos (SQL)`, `Seguridad`.
> * **Subramas de Backend:** `Lenguaje de programación (Python/Node)`, `Framework (Flask/Express)`, `API REST`.

---

## 2. Técnicas de Resolución de Problemas (Enfoque Analítico)

Una vez que algo falla, necesitamos herramientas para ir más allá de los síntomas y encontrar la **verdadera causa raíz** (**Pensamiento Convergente**).

### 2.1 Análisis de Causa Raíz (Diagrama de Ishikawa o Espina de Pescado)

* **Concepto:** Un diagrama visual que ayuda a clasificar las posibles causas de un problema (el *efecto*) en distintas categorías.

| Categorías Comunes (IT) | Lo que Incluyen |
| :--- | :--- |
| **Código** | Bugs, arquitectura deficiente, falta de pruebas. |
| **Infraestructura** | Servidores lentos, fallos de red, problemas de *Cloud Computing*. |
| **Procesos** | Flujo de trabajo confuso, falta de documentación, *deployment* manual. |
| **Personas** | Falta de formación, errores humanos, mala comunicación en el equipo. |

> **Ejemplo Tech:**
> * **Efecto:** "El servicio de autenticación se cae todos los lunes por la mañana".
> * **Causa Raíz (Podría ser):** Un proceso automático de limpieza de la base de datos (parte de **Procesos**) no está optimizado y satura el servidor (parte de **Infraestructura**) justo cuando la gente inicia sesión.

![ilustración](../images/Ishikawa.png)

### 2.2 Los 5 Porqués (*The 5 Whys*)

* **Concepto:** Preguntar "¿Por qué?" de forma repetida (cinco veces es la recomendación) sobre un problema hasta desenterrar la causa raíz.

> **Ejemplo Práctico:**

* **Problema:** La web se carga muy lenta.
* **1. ¿Por qué se carga lenta?** $\rightarrow$ Porque la consulta a la base de datos tarda 8 segundos.
* **2. ¿Por qué tarda 8 segundos?** $\rightarrow$ Porque la tabla principal tiene 50 millones de registros y no tiene un índice.
* **3. ¿Por qué no tiene un índice?** $\rightarrow$ Porque el desarrollador se olvidó de crearlo en la migración de la base de datos.
* **4. ¿Por qué se olvidó?** $\rightarrow$ Porque no hay una lista de verificación de *deployment* (despliegue).
* **5. ¿Por qué no hay una lista de verificación?** $\rightarrow$ Porque la empresa no tiene un **Proceso** de control de calidad estandarizado.

**Causa Raíz:** Falta de un proceso de QA y *deployment* estandarizado.

### 2.3 Matriz DAFO (SWOT Analysis)

* **Concepto:** Evalúa una idea, un producto o una empresa en sus factores **internos** (controlables) y **externos** (incontrolables).

| Factores | Internos (Controlables - Hoy) | Externos (Incontrolables - Mañana) |
| :--- | :--- | :--- |
| **Positivos** | **F**ortalezas (*Strengths*): Puntos fuertes de mi equipo/código/producto. | **O**portunidades (*Opportunities*): Tendencias del mercado, nuevas tecnologías, competencia débil. |
| **Negativos** | **D**ebilidades (*Weaknesses*): Puntos débiles (ej. falta de personal, tecnología obsoleta). | **A**menazas (*Threats*): Competencia fuerte, crisis económica, cambios regulatorios. |

> **Ejemplo Tech:**
> * **Fortaleza:** Tenemos un equipo de desarrolladores *full-stack* muy rápido.
> * **Oportunidad:** La IA generativa abre un nuevo nicho de mercado para la automatización.
> * **Debilidad:** Nuestra infraestructura de servidores es anticuada y costosa.
> * **Amenaza:** La Unión Europea acaba de aprobar una ley que exige más seguridad de datos.

---

## Ejemplo práctico (Siguiendo el Flujo)

Un problema de negocio nunca se resuelve solo con creatividad o solo con análisis; necesitas ambos:

1.  **Detectar y Analizar (Ishikawa / 5 Porqués):** Una empresa tiene una baja en las ventas online. El análisis encuentra la **Causa Raíz:** El formulario de registro del carrito es demasiado largo y pide datos irrelevantes.
2.  **Generar Soluciones (SCAMPER):** Ahora que el problema está *definido*, aplicamos SCAMPER al formulario:
    * **Eliminar:** Quitar los campos opcionales.
    * **Combinar:** Combinar el registro y el pago en una sola pantalla.
    * **Resultado:** Se introduce el "Checkout como invitado", eliminando el 70% de los datos solicitados. **Innovación exitosa.**

---

## Actividades Propuestas

### Actividad 1: Aplicar la técnica de los *5 porqués* (Individual)

**Tarea:** Piensa en un problema cotidiano del aula o del IES (ej. el Wi-Fi falla a menudo, hay mucha desorganización en un proyecto grupal).

**Proceso:** Aplica la cadena de los **5 Porqués** para encontrar la causa raíz y propón una solución real a ese problema de fondo.

### Actividad 2: Elaborar un *Mapa Mental* (En Grupos)

**Tarea:** Elaborar un **Mapa Mental** de posibles mejoras para la **cafetería del centro educativo** o para el **proceso de matrícula online** del IES.

**Proceso:**
1. Define el concepto central (Cafetería o Matrícula).
2. Crea al menos **cuatro ramas principales** (ej. Servicio, Tecnología, Productos, Diseño).
3. Desarrolla al menos **dos niveles de subramas** con ideas concretas.
