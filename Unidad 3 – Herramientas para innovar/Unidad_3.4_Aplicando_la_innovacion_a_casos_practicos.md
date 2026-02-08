# Unidad 3.4 - Aplicando la Innovación a Casos Prácticos

## Objetivo de la Unidad (RA3)

**RA3. Propone ideas innovadoras aplicando técnicas básicas de pensamiento creativo y resolución de problemas en contextos productivos.**

| Tipo de Elemento | Identificador | Descripción |
| --- | --- | --- |
| **Resultado de Aprendizaje** | **RA3** | Propone ideas innovadoras aplicando técnicas básicas de pensamiento creativo y resolución de problemas en contextos productivos. |
| **Criterios de Evaluación** | **d)**<br> **e)** | Se ha valorado la viabilidad económica de forma sencilla y se ha presentado un plan de implementación básico<br>Se ha presentado un plan de implementación básico para una idea innovadora. |

---

## Introducción: El Reto de la Viabilidad

En el mundo del desarrollo de software y la administración de sistemas, una idea excelente y un cronograma bien trazado (visto en la Unidad 3.3) no son suficientes. El éxito real depende de dos factores críticos:

1. **¿Es rentable o sostenible?** (Viabilidad Económica).
2. **¿Cómo lo vamos a construir paso a paso?** (Plan de Implementación).

Como técnicos, debemos entender que la innovación no solo es "que funcione", sino que sea eficiente en el uso de los recursos .

---

## 1. Viabilidad Económica: El Lado Humano y Técnico del Dinero

En informática, la viabilidad no siempre significa "vender un producto". Si desarrollamos una herramienta interna, la viabilidad se mide en **ahorro de tiempo y recursos**.

### 1.1 Estimación de Costes de Desarrollo

Para saber cuánto cuesta nuestra idea, debemos desglosar tres categorías:

* **Costes de Personal (Talento):** Es el gasto principal. Se calcula multiplicando las horas estimadas de trabajo por el coste/hora del técnico.
* *Ejemplo:* Si 2 alumnos dedican 40 horas a configurar un sistema de copias de seguridad a 15€/hora (precio ficticio de junior), el coste de personal es de **1.200 €**.


* **Infraestructura y Materiales:** Licencias de software, suscripciones a APIs, hardware (Raspberry Pi, servidores, almacenamiento) y servicios Cloud (AWS, Azure).
* **Costes Operativos (Mantenimiento):** ¿Cuánto cuesta mantener el sistema encendido y actualizado cada mes?

### 1.2 Retorno de la Inversión (Ingresos vs. Ahorros)

¿Cómo recuperamos lo invertido?

* **Modelos Directos:** SaaS (suscripciones), licencias de pago único o publicidad.
* **Modelos Indirectos (Ahorro):** Si automatizamos el inventario del IES, y el responsable de TIC ahorra 5 horas semanales, ese tiempo es dinero que la institución gana en eficiencia.

> **La Regla de Oro:** Si el coste de mantenimiento y desarrollo supera el beneficio (económico o de tiempo) en un plazo razonable, el proyecto debe ser rediseñado o pivotado.

---

## 2. Plan de Implementación: La Hoja de Ruta de Ejecución

El plan de implementación es el "manual de instrucciones" para que el equipo de IT sepa qué hacer cada semana. Utilizaremos un enfoque basado en fases lógicas de ingeniería de software.

### 2.1 Fases del Ciclo de Vida del Proyecto

1. **Fase de Descubrimiento y Diseño (UX/Arquitectura):** Antes de teclear código, definimos cómo se verá la interfaz y qué base de datos usaremos.
2. **Desarrollo del Core (MVP):** Construcción de las funciones mínimas que hacen que la idea funcione.
3. **QA y Testing (Control de Calidad):** Fase crítica de depuración de *bugs*, pruebas de carga y auditoría de seguridad de red.
4. **Despliegue (Rollout):** Paso a producción y formación a los usuarios finales.

### 2.2 Roles y Responsabilidades en el Equipo

Para que un proyecto en el IES funcione, cada miembro debe conocer su "mochila":

* **Product Owner / Scrum Master:** Gestiona que se cumplan los plazos y elimina bloqueos.
* **Full-stack / Backend Developer:** Se encarga de la lógica, el servidor y los datos.
* **SysAdmin / DevOps:** Configura la infraestructura, contenedores (Docker) y seguridad.

---

## Caso Práctico: App de Gestión de Incidencias para el Centro

Imagina que queremos implementar un sistema de tickets para que los profesores reporten fallos en los ordenadores de las aulas del **IES Vía de la Plata**.

| Concepto | Detalle de Implementación |
| --- | --- |
| **Viabilidad Económica** | Coste de servidor (10€/mes) + 100h de desarrollo. Ahorro estimado: 4h/semana de gestión manual. |
| **MVP** | Formulario simple de reporte y panel de administración para el técnico. |
| **Fase Crítica** | **Testing:** Comprobar que el sistema aguanta 50 peticiones simultáneas desde diferentes subredes del centro. |
| **Responsable** | Alumno A (Frontend), Alumno B (Base de Datos), Alumno C (Seguridad/Redes). |

---
