# PROYECTO: EdiFix IES – Gestión de Incidencias
**Módulo:** Innovación Aplicada al Sector Productivo  
**Equipo:** Lucía Martínez, Jorge Sanz y Raúl Cobo  
**Estado:** Prototipo Funcional (MVP)

---

## 1. RESUMEN EJECUTIVO
EdiFix IES es una solución digital diseñada para centralizar y agilizar el reporte de averías e incidencias técnicas en el entorno educativo. Actualmente, los avisos en el centro se gestionan de forma analógica (papel o comunicación verbal), lo que provoca duplicidad de reportes y falta de trazabilidad. Nuestra aplicación permite a cualquier miembro de la comunidad educativa notificar un desperfecto en menos de 10 segundos, adjuntando evidencias visuales y permitiendo al equipo de mantenimiento gestionar las tareas en tiempo real desde un panel de control dedicado.

---

## 2. FASE DE EMPATÍA Y REQUISITOS (DESIGN THINKING)
### 2.1. Toma de Requisitos (Trabajo de Campo)
Se han realizado **5 entrevistas semiestructuradas** (conserje, 2 profesores y 2 alumnos).

* **Hallazgo 1 (Saturación):** El personal de mantenimiento recibe el mismo aviso varias veces, lo que genera pérdida de tiempo.
* **Hallazgo 2 (Incertidumbre):** Los profesores no saben si su aviso ha sido leído o si se está trabajando en él.
* **Hallazgo 3 (Falta de datos):** Muchas incidencias se reportan sin ubicación exacta (ej: "el enchufe del aula de informática", sin especificar cuál de ellas).

### 2.2. Mapa de Empatía (Perfil: Responsable de Mantenimiento)
| ¿Qué PIENSA y SIENTE? | ¿Qué VE? |
| :--- | :--- |
| Le preocupa olvidar una avería urgente. Siente que su trabajo es caótico por falta de orden. | Ve un tablón lleno de post-its y gente parándole constantemente por los pasillos. |
| **¿Qué OYE?** | **¿Qué DICE y HACE?** |
| Oye quejas de: "Llevo tres días con la persiana rota". | Dice: "Pónmelo por escrito o no me acuerdo". Hace rondas con una libreta apuntando todo. |

---

## 3. DEFINICIÓN Y ESTRUCTURA 
### 3.1. Definición del Problema (POV)
> **"El personal de mantenimiento necesita un sistema de tickets centralizado y visual porque la comunicación fragmentada actual causa retrasos críticos en las reparaciones."**

### 3.2. Mapa Mental de la Solución

* **Módulo Usuario:** Login ➡️ Formulario (Aula, Tipo de avería, Foto) ➡️ Historial de mis reportes.
* **Módulo Admin:** Dashboard con lista de espera ➡️ Cambio de estado (Pendiente / En Proceso / Resuelto).
* **Notificaciones:** Alerta vía email al usuario cuando se cierra el ticket.

---

## 4. ANÁLISIS ESTRATÉGICO (MATRIZ DAFO) 

| MATRIZ DAFO | ORIGEN INTERNO (Equipo) | ORIGEN EXTERNO (Entorno/IES) |
| :--- | :--- | :--- |
| **POSITIVO** | **FORTALEZAS:** <br> Dominio de MySQL y PHP. Conocimiento profundo de la infraestructura del centro. | **OPORTUNIDADES:** <br> El IES busca la certificación de "Centro Digital". Disponibilidad de servidores en el centro. |
| **NEGATIVO** | **DEBILIDADES:** <br> Falta de experiencia en diseño de interfaces (UI/UX). Tiempo de desarrollo limitado a 8 semanas. | **AMENAZAS:** <br> Posible baja adopción por parte del personal menos familiarizado con la tecnología. |

---

## 5. DESARROLLO DEL PRODUCTO (MVP) 
### 5.1. Definición del Producto Mínimo Viable
Para la validación inicial, la App incluirá:
1.  **Formulario de reporte:** Selección de aula (desplegable) y descripción.
2.  **Carga de imagen:** API de cámara para adjuntar evidencia visual.
3.  **Gestión de estados:** El administrador puede marcar una avería como "Finalizada".

### 5.2. Métrica de Éxito (KPI)
* **Objetivo:** Conseguir que el **100% de las incidencias del Pabellón A** se reporten digitalmente durante la semana de pruebas.

---

## 6. PLANIFICACIÓN Y CRONOGRAMA 
### 6.1. Recursos Técnicos
* **Infraestructura:** Servidor Apache local (XAMPP/Debian).
* **Tecnologías:** PHP 8, MariaDB para la base de datos y Bootstrap para el diseño responsivo.

### 6.2. Hitos del Proyecto
| Hito | Descripción | Fecha |
| :--- | :--- | :--- |
| **1. Diseño** | Creación del esquema de base de datos y wireframes. | 15 de Febrero |
| **2. Desarrollo** | Implementación del sistema de envío y almacenamiento de tickets. | 10 de Marzo |
| **3. Cierre** | Pruebas beta con el personal de conserjería y corrección de bugs. | 25 de Marzo |