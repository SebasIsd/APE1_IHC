# 📊 Auditoría de Usabilidad y Accesibilidad Web: Microsoft.com

Proyecto de evaluación heurística de usabilidad y cumplimiento de estándares de accesibilidad WCAG 2.1 (Principios POUR) sobre el ecosistema web de Microsoft, correspondiente a la asignatura de Interacción Humano-Computador.

---

## 👥 Equipo de Trabajo y Distribución de Tareas

| Integrante | Rol / Tarea Evaluada |
| :--- | :--- |
| **Viviana Sarco** | **Tarea 1:** Encontrar información para activar o adquirir una suscripción |
| **Alex Guachi** | **Tarea 2:** Descargar e instalar una aplicación oficial (Microsoft Teams) |
| **Sebastián Santana** | **Tarea 3:** Recuperar la contraseña organizacional (SSPR)<br>**Tarea 5:** Localizar el centro de soporte técnico y ayuda interactiva |
| **Wilson Pillapa** | **Tarea 4:** Consultar e inspeccionar el historial de facturación/compras |

---

## 📈 Resumen General de Métricas Operacionales

* **Efectividad Global:** `100 %` (15/15 ejecuciones completadas)
* **Tasa de Error Operacional:** `40 %` (6 errores registrados en total)
* **Satisfacción Promedio (SEQ/SUS):** `4.33 / 5`
* **Puntuación Google Lighthouse (Accesibilidad):** `100 / 100`
* **Puntuación WAVE (AIM Score):** `9.9 / 10`

---

## 🧩 Matriz Integrada de Hallazgos (Nielsen + POUR / WCAG)

| ID | Pantalla / tarea | Hallazgo | Nielsen | POUR / WCAG | Método | Resultado | Sev. | Frec. | Prior. | Evidencia | Recomendación verificable |
| :---: | :--- | :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :--- |
| **H01** | Página Principal (Home) / T1 | Exceso de banners promocionales y saturación visual de productos. | N8 | Perceptible 1.4.8 | Visual / WAVE | No cumple | 2 | 3 | 6 | [Ver imagen](./docs/img/captura1.png) | Redistribuir componentes visuales usando espacios en blanco y jerarquías claras. |
| **H02** | Portal Licencias / T1 | Denominaciones comerciales (E3, E5, F3) poco intuitivas para usuarios novatos. | N2 | Comprensible 3.1.3 | WAVE | Parcial | 2 | 3 | 6 | [Ver imagen](./docs/img/captura1.png) | Reestructurar la arquitectura de información eliminando la jerga técnica. |
| **H03** | Descarga Teams / T2 | Confusión entre el botón "Usar en navegador" y el botón de descarga del ejecutable. | N5 | Comprensible 3.3.2 | LightHouse | Parcial | 2 | 2 | 4 | [Ver imagen](./docs/img/captura2.png) | Diferenciar visualmente la opción de descarga ejecutable frente al acceso web. |
| **H04** | Recuperación SSPR / T3 | Mensajes de error técnicos que despliegan códigos opacos (HTTP 401 / MS-Auth). | N9 | Comprensible 3.3.1 | LightHouse | No cumple | 3 | 2 | 6 | [Ver imagen](./docs/img/image-2.png) | Implementar mensajes descriptivos en lenguaje natural orientados a la acción. |
| **H05** | Facturación / T4 | Ruta de navegación extensa y confusión entre "Suscripciones" y "Pagos". | N4 | Operable 2.4.5 | Visual / WAVE | Parcial | 2 | 2 | 4 | [Ver imagen](./docs/img/captura3.png) | Simplificar los pasos en los flujos principales y consolidar accesos directos. |
| **H06** | Centro Soporte / T5 | Desvío inicial de los usuarios usando la barra de búsqueda global en lugar de la de soporte. | N10 | Operable 2.4.6 | Visual / Teclado | Parcial | 2 | 2 | 4 | [Ver imagen](./docs/img/image-3.png) | Unificar el motor de búsqueda global con sugerencias automáticas de ayuda. |

---

## ♿ Resumen de Evidencias de Accesibilidad

### 1. Evaluaciones Automáticas

#### 🌊 Herramienta WAVE
Se comprobó la ausencia de errores críticos de accesibilidad y contraste de color, con un uso correcto de etiquetas semánticas y atributos ARIA.

<img width="1899" height="882" alt="image" src="https://github.com/user-attachments/assets/96c1e29e-0987-4d74-9f31-a75bb5896793" />


#### ⚡ Herramienta Google Lighthouse
Puntuación perfecta de accesibilidad alcanzada en las pruebas de auditoría automatizada.

<img width="961" height="669" alt="image" src="https://github.com/user-attachments/assets/a4c32632-ad19-4959-872e-17053edabfda" />

---

### 2. Evaluaciones Manuales

#### ⌨️ Navegación por Teclado
Se verificó que los flujos de las 5 tareas son operables sin ratón mediante el uso de `Tab`, `Shift + Tab` y `Enter`, manteniendo el foco visible en todo momento.

(aqui pon la captura o gif de la navegacion por teclado o asi)

#### 🗣️ Lector de Pantalla (NVDA)
Prueba realizada con software de asistencia para validar la lectura fluida de encabezados, formularios y botones dinámicos.

<img width="1735" height="791" alt="image" src="https://github.com/user-attachments/assets/c1ecec20-e006-46e9-b6fe-203a8e7a0609" />


---

## 📁 Estructura del Repositorio

* `README.md`: Resumen ejecutivo del proyecto y matriz integrada de hallazgos.
* `docs/Tarea1.md`: Documentación detallada del flujo de licencias (Viviana Sarco).
* `docs/Tarea2.md`: Documentación del flujo de descarga de software (Alex Guachi).
* `docs/Tarea3.md`: Documentación del restablecimiento autónomo de clave (Sebastián Santana).
* `docs/Tarea4.md`: Documentación de la consulta de facturas y pagos (Wilson Pillapa).
* `docs/Tarea5.md`: Documentación del módulo de ayuda interactiva (Sebastián Santana).
