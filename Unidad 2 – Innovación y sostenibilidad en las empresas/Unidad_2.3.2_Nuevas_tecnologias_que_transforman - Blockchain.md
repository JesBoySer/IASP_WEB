# Unidad 2.3 - Nuevas Tecnologías que Transforman -  Blockchain – La Tecnología de la Confianza

| Tipo | Código | Descripción Detallada |
| :--- | :--- | :--- |
| **Resultado de Aprendizaje (RA)** | RA2 | Reconoce la importancia de la innovación como motor de crecimiento y desarrollo sostenible en los sectores productivos, y su impacto en la gestión empresarial y la transformación digital de las organizaciones. |
| **Criterio de Evaluación (CE)** | d) | Se han identificado tecnologías emergentes y tendencias innovadoras que están transformando los sectores productivos y su potencial impacto en las empresas. |

---

# Introducción Histórica: ¿Por qué nace Blockchain?

Imagina que quieres enviar dinero a un amigo. Tradicionalmente, necesitas un **intermediario** (un banco) para verificar que tienes el dinero y registrar la transacción. Este modelo centralizado tiene un problema: si el banco falla o es atacado, todo el sistema de confianza colapsa.

**Blockchain** nace en 2008, con la creación de **Bitcoin**, como una solución radical a este problema. Su objetivo: permitir transacciones y registros de datos de forma **segura, transparente y sin necesidad de una autoridad central** (un banco, un gobierno o una empresa).

---

## 1. ¿Qué es Blockchain? El Concepto Clave

**Blockchain** (Cadena de Bloques) es, simplemente, una **base de datos distribuida e inmutable**.

1.  **Cadena (Chain):** La información se agrupa en **bloques**. Cuando un bloque se llena, se añade al bloque anterior, formando una cadena.
2.  **Bloques (Blocks):** Cada bloque contiene un registro de datos (transacciones, contratos, información) y dos identificadores clave:
    * El **Hash** de su contenido (su huella digital).
    * El **Hash** del bloque inmediatamente anterior.
3.  **Inmutable:** Como cada bloque está **encadenado criptográficamente** al anterior, si alguien intenta modificar un dato en el bloque 3, el *hash* de ese bloque cambia. Automáticamente, el bloque 4 (que depende del *hash* correcto del 3) y todos los siguientes se vuelven inválidos. Es imposible cambiar el pasado sin que toda la red lo detecte.
4.  **Distribuida (Descentralizada):** La cadena no se guarda en un solo servidor (como el de un banco). Se copia en miles de ordenadores alrededor del mundo (llamados **nodos**). Si hackeas un ordenador, los otros miles demuestran que tu versión es falsa.

---

## 2. El Funcionamiento Clave: Minería y Consenso

Para que un nuevo bloque se añada a la cadena, debe pasar por un proceso de **validación** conocido como **consenso**. En Bitcoin, este consenso se llama **Prueba de Trabajo** (*Proof of Work*), y el proceso para lograrlo es la **Minería**.

### Explicación Detallada: ¿Qué es Minar un Bloque?

**Minar un bloque no es crear criptomonedas, es validar y asegurar la información de un bloque.**

| Concepto | Explicación | Ejemplo Práctico (Criptomoneda) |
| :--- | :--- | :--- |
| **El Desafío Criptográfico** | Para que un bloque sea válido, su *hash* debe cumplir una condición muy difícil: debe empezar, por ejemplo, con cuatro ceros consecutivos (**0000**...). | El sistema pide a los mineros encontrar un *hash* que valide las últimas transacciones de Bitcoin. |
| **El Nonce** | El *hash* de un bloque depende de sus datos. Como los datos son fijos, el minero debe encontrar un número aleatorio, llamado **Nonce**, que, al añadirse a los datos del bloque, produce el *hash* que cumple la condición. | El ordenador de un minero prueba millones de *nonces* por segundo hasta que uno de ellos genera el *hash* que empieza por **0000**... |
| **El Consenso** | El primer minero que encuentra el *nonce* lo comunica al resto de la red. Si el 51% de los nodos (ordenadores) comprueba que el *hash* es correcto, el bloque se acepta y se añade a la cadena. | El bloque se adjunta a la cadena de Bitcoin, y todas las copias de la cadena en el mundo se actualizan. |
| **La Recompensa** | El minero ganador recibe una recompensa (monedas recién creadas y las tarifas de las transacciones). | El minero recibe una cantidad de Bitcoin por asegurar la red (la **emisión** de la criptomoneda). |

Este proceso garantiza que se necesita un enorme poder de cálculo (energía y tiempo) para añadir un bloque. Por lo tanto, intentar modificar un bloque pasado (y tener que *reminar* todos los bloques posteriores) es **económicamente inviable**. La minería es la innovación que asegura la red.

---

## 3. Aplicaciones de Blockchain más allá de las Criptomonedas

La innovación de Blockchain va mucho más allá del dinero digital. Su utilidad principal es eliminar la necesidad de un intermediario en cualquier registro.

| Área de Aplicación | Innovación que Aporta | Ejemplo Tecnológico |
| :--- | :--- | :--- |
| **Cadena de Suministro** | **Trazabilidad Inmutable:** El origen y la ruta de un producto se registran sin posibilidad de fraude. | Empresas de logística como **Maersk** (en colaboración con $IBM$) usan $Blockchain$ para rastrear contenedores. |
| **Gestión de Identidad** | **Identidad Digital Soberana:** El individuo controla sus propios datos y decide con quién compartirlos. | Proyectos que buscan reemplazar documentos de identidad centralizados con credenciales verificables. |
| **Contratos Inteligentes ($Smart$ $Contracts$)** | **Automatización Legal:** Contratos digitales que se ejecutan automáticamente cuando se cumplen condiciones predefinidas, sin abogados ni notarios. | Un contrato que libera el pago a un proveedor cuando el $IoT$ registra que la mercancía ha llegado. |
| **Votaciones Digitales** | **Transparencia y Seguridad:** Garantía de que un voto es único y no puede ser alterado o eliminado. | Proyectos piloto de votación electrónica. |

---

## 🛠️ Práctica Creativa 1: El Juego de la Confianza Descentralizada (Desarrollo Completo)

**Herramienta Online:** [Blockchain Demo de Anders Brownworth](https://andersbrownworth.com/blockchain/blockchain)

### **Fase A: El Bloque y la Minería (La Prueba de Trabajo)**

| Paso | Tarea del Alumno | Observación Clave |
| :--- | :--- | :--- |
| **1: Datos Fijos** | En la pestaña 'Block', introducir un dato de la empresa (ej: "Inventario: 100 PCs"). El *Hash* se ve en rojo. | El *hash* es la huella digital que certifica la información. |
| **2: Minería (MINE)** | Pulsar **MINE**. El sistema buscará el *Nonce* correcto. El *hash* se vuelve verde. | El sistema gasta energía (tiempo de cálculo) para **validar** el bloque y hacerlo seguro. |

### **Fase B: La Cadena y la Inmutabilidad (Prevención del Fraude)**

| Paso | Tarea del Alumno | Observación Clave |
| :--- | :--- | :--- |
| **3: Creación de la Cadena** | Cambiar a la pestaña **'Chain'** y añadir 3 bloques. Cada bloque contiene información crucial (ej: "Licencia ID 123"). | Cada bloque incluye el *Hash* del bloque anterior, creando un enlace criptográfico. |
| **4: El Intento de Fraude** | Volver al **Bloque 2** y modificar ligeramente el dato (ej: cambiar "ID 123" por "ID 500"). | El Bloque 2 se vuelve **ROJO**, y **todos los bloques posteriores** también se vuelven **ROJOS**. |
| **5: Conclusión de la Inmutabilidad** | Observar la ruptura de la cadena. | El fraude es detectable automáticamente porque rompe todos los eslabones posteriores.

### **Fase C: Descentralización y Consenso de la Mayoría**

| Paso | Tarea del Alumno | Observación Clave de la Corrección |
| :--- | :--- | :--- |
| **6: La Red Distribuida** | Cambiar a la pestaña **'Distributed'**. Asegurarse de que los 4 nodos tienen la misma cadena válida (todos verdes). | La base de datos está replicada en todos los ordenadores (nodos). |
| **7: El Fraude en un Nodo Único** | En el **Nodo 3**, modificar el dato del Bloque 2 (SIN minar). | El Nodo 3 se pone **ROJO**, mientras que los Nodos 1, 2 y 4 permanecen **VERDES** (la versión correcta). |
| **8: La Solución del Consenso** | Pulsar **MINE** en el Nodo 3 (el nodo fraudulento). | El nodo alterado se **sincroniza automáticamente** con la cadena más larga y válida (la de la mayoría) y sus bloques vuelven a ser verdes con los datos correctos. |

### **Pregunta Guía de Innovación para el Debate**

> Si pudierais usar *Blockchain* para garantizar la autenticidad y el origen de un componente crítico de *hardware* (como un microchip o una licencia de *software*) desde que sale del fabricante hasta que llega al cliente, ¿cómo cambiaría esto el modelo de negocio de una empresa como HP o Dell?
