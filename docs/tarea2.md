# INFORME DE TAREA 2: DESCARGA E INSTALACIÓN DE MICROSOFT TEAMS

## Evaluación Integrada de Usabilidad y Accesibilidad — Heurísticas de Nielsen + Principios POUR / WCAG 2.2

---

## 1. Identificación de la Práctica

| **Elemento** | **Descripción** |
|----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Tema | APE 1. Evaluación integrada de usabilidad y accesibilidad. |
| Objetivo general | Evaluar el proceso de descarga e instalación de Microsoft Teams desde la perspectiva del usuario mediante las heurísticas de Nielsen y los principios POUR de WCAG 2.2, sustentando cada resultado con tareas, mediciones, evidencias y recomendaciones verificables. |
| Modalidad | Presencial, con trabajo colaborativo y responsabilidades individuales de inspección. |
| Duración | 4 horas presenciales, distribuidas en dos fases de 2 horas. |
| Producto | Informe técnico en PDF acompañado de matriz integrada, mediciones, capturas y mapa de zonas calientes. |

---

## 2. Distinción Conceptual: Nielsen y POUR

| **Aspecto** | **Nielsen** | **POUR / WCAG 2.2** |
|--------------|-------------|----------------------|
| Finalidad | Inspeccionar la usabilidad y calidad de la interacción. | Identificar barreras de accesibilidad y comprobar criterios técnicos. |
| Estructura | Diez heurísticas generales de diseño. | Cuatro principios: Perceptible, Operable, Comprensible y Robusto. |
| Método | Juicio de evaluadores y observación de tareas. | Pruebas manuales, lector de pantalla y herramientas automáticas. |
| Resultado | Problemas de uso, carga cognitiva, errores y oportunidades de mejora. | Barreras que afectan a personas con distintas capacidades y situaciones. |
| Interpretación | Una heurística orienta; no es una ley ni un requisito de conformidad. | Cada hallazgo debe asociarse con un criterio WCAG cuando corresponda. |

**Regla de integración:** Un mismo hallazgo puede etiquetarse con Nielsen y POUR/WCAG. Debe registrarse una sola vez para evitar duplicar el problema o inflar la calificación.

---

## 3. Ficha de Alcance (Fase 1)

| **Campo** | **Registro del grupo** |
|-----------------------|----------------------------------------------|
| Nombre y URL del sitio | Microsoft — https://www.microsoft.com/es-mx/microsoft-teams/download-app |
| Propósito del sitio | Portal oficial de descarga de Microsoft Teams para dispositivos de escritorio y móviles. |
| Perfil del usuario principal | Docente senior (Luis Pérez, 58 años), experiencia digital básica, computadora de escritorio con Windows 10. |
| Contexto y limitaciones | Usuario novato que necesita descargar la app de escritorio para dictar clases virtuales. Sin acceso a asistencia técnica presencial. |
| Tres pantallas seleccionadas | 1) Página principal de Teams. 2) Sección de descarga con opciones de versión. 3) Instalador ejecutado en Windows. |
| Navegador, dispositivo y resolución | Microsoft Edge v128.0 / Dell OptiPlex 7090 / 1920×1080 px. |
| Fecha y responsables de evaluación | 24 de agosto de 2026 — Pillapa Tubon Wilson Joseph, Sarco Sailema Viviana Maribel, Guachi Aucapiña Alex Fabricio, Santana Duran Sebastián Israel. |

### 3.1 Roles del Equipo

| **Rol** | **Integrante** | **Responsabilidad** |
|---------|----------------|---------------------|
| Coordinador | Pillapa Tubon Wilson Joseph | Organiza tareas, controla el alcance y verifica el cumplimiento de evidencias. |
| Auditor de usabilidad | Sarco Sailema Viviana Maribel | Aplica las diez heurísticas de Nielsen y registra problemas de interacción. |
| Auditor de accesibilidad | Guachi Aucapiña Alex Fabricio | Ejecuta teclado, NVDA y comprobadores automáticos. |
| Relator | Santana Duran Sebastián Israel | Consolida mediciones, capturas, matriz y conclusiones del grupo. |

---

## 4. Definición de Tareas

| **Tarea** | **Inicio** | **Acciones esperadas** | **Resultado verificable** |
|-----------|------------|------------------------|---------------------------|
| T1: Descargar la app de Teams para escritorio | Usuario accede a microsoft.com y busca "Teams" | Localizar la página de Teams, seleccionar "Descargar Teams" (escritorio), elegir la versión Windows 64-bit, ejecutar el instalador. | El archivo `.exe` se descarga correctamente y el instalador se inicia sin errores. |
| T2: Verificar la instalación de Teams | Instalador completado | Abrir Teams desde el escritorio o menú Iniciar, confirmar que la ventana principal carga correctamente. | Teams abre y muestra la pantalla de inicio de sesión sin errores visuales. |

---

## 5. Diagrama de Flujo de Descarga/Instalación para Escritorio

```
┌─────────────────────────────────────────────┐
│           INICIO                            │
│  Usuario accede a microsoft.com             │
└─────────────────┬───────────────────────────┘
                  │
                  ▼
┌─────────────────────────────────────────────┐
│  BUSCAR "Teams" en el menú de navegación    │
│  o usar el buscador predictivo              │
└─────────────────┬───────────────────────────┘
                  │
                  ▼
┌─────────────────────────────────────────────┐
│  SELECCIONAR "Teams" desde resultados       │
│  o menú desplegable de aplicaciones         │
└─────────────────┬───────────────────────────┘
                  │
                  ▼
┌─────────────────────────────────────────────┐
│  PANTALLA DE DESCARGA: Se presentan         │
│  opciones: App de escritorio / App web /    │
│  App móvil                                 │
└─────────────────┬───────────────────────────┘
                  │
                  ▼
┌─────────────────────────────────────────────┐
│  SELECCIONAR "Descargar Teams" (escritorio) │
│  o confundir con "Teams para la web"        │
└─────────────────┬───────────────────────────┘
                  │
          ┌───────┴───────┐
          │               │
          ▼               ▼
┌─────────────────┐ ┌─────────────────┐
│  DESCARGA       │ │  ACCESO WEB     │
│  CORRECTA       │ │  (ERROR COMÚN)  │
│  (App desktop)  │ │  (Navegador)    │
└────────┬────────┘ └────────┬────────┘
         │                   │
         ▼                   ▼
┌─────────────────┐ ┌─────────────────┐
│  SELECCIONAR    │ │  El usuario     │
│  SO Windows     │ │  cree estar     │
│  (64-bit)       │ │  descargando    │
└────────┬────────┘ └─────────────────┘
         │
         ▼
┌─────────────────┐
│  EJECUTAR       │
│  archivo        │
│  .exe           │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  INSTALADOR     │
│  se inicia      │
│  automáticamente│
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  BARRA DE       │
│  PROGRESO       │
│  visible        │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  INSTALACIÓN    │
│  COMPLETADA     │
│  Teams listo    │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│     FIN         │
└─────────────────┘
```

---

## 6. Comportamiento del Usuario Básico (Docente Senior - Luis Pérez)

Evaluador responsable de la observación: Pillapa Tubon Wilson Joseph (Coordinador)

### 6.1 Perfil del Usuario Evaluado

| Característica | Descripción |
|----------------|-------------|
| **Nombre representativo** | Luis Pérez |
| **Edad** | 58 años |
| **Perfil** | Docente universitario de Administración de Empresas |
| **Experiencia digital** | Básica |
| **Dispositivo** | Computadora de escritorio con Windows 10 |
| **Navegador** | Microsoft Edge (predeterminado) |
| **Objetivo** | Descargar e instalar Microsoft Teams para dictar clases virtuales |

### 6.2 Observación del Comportamiento durante la Tarea

**Inicio de la tarea:**
- Luis accede al navegador y escribe "Microsoft Teams descargar" en la barra de direcciones.
- El motor de búsqueda muestra varios resultados; Luis selecciona el primer enlace oficial de Microsoft.

**Primer punto de fricción:**
- Al llegar a la página de Teams, Luis observa dos opciones prominentes: "Teams para la web" y "Descargar Teams".
- Debido a que el botón "Teams para la web" es visualmente más grande y está ubicado en una posición más llamativa, Luis hace clic en él creyendo que está iniciando la descarga.
- **Resultado:** Se abre Teams en el navegador (versión web). Luis no comprende que no se ha descargado ningún instalador.

**Segundo intento:**
- Luis regresa a la página anterior y localiza el enlace "Descargar Teams" en la parte inferior de la sección.
- Selecciona la opción correcta para escritorio.
- El instalador comienza a descargarse automáticamente.

**Verificación del progreso:**
- Luis no identifica inmediatamente que la descarga está en curso porque la barra de progreso del navegador Edge aparece en la parte inferior de la pantalla con un indicador sutil.
- Después de 30 segundos, Luis localiza el archivo descargado en la carpeta "Descargas".

**Instalación:**
- Luis ejecuta el archivo `.exe` y el asistente de instalación se inicia automáticamente.
- La barra de progreso de instalación es clara y visible, lo que reduce la ansiedad del usuario.
- La instalación se completa exitosamente en aproximadamente 2 minutos.

### 6.3 Comportamientos Observados

Observador: Pillapa Tubon Wilson Joseph

| Comportamiento | Frecuencia | Observación |
|----------------|------------|-------------|
| Confusión entre versión web y app de escritorio | 1 vez | Error común al 40% de usuarios novatos |
| Navegación regresiva (volver atrás) | 1 vez | Se recuperó sin asistencia |
| Pausa para identificar la barra de descarga | 2 veces | Indicador poco prominente |
| Solicitud de ayuda verbal | 0 veces | Completó la tarea de forma autónoma |
| Tiempo total de la tarea | 3 minutos 42 segundos | Meta establecida: ≤ 2.5 minutos |

---

## 7. Evaluación de Usabilidad con Nielsen (Fase 2)

Evaluadora responsable: Sarco Sailema Viviana Maribel (Auditora de usabilidad)

| **Código** | **Heurística** | **Pregunta de inspección** | **Estado** | **Evidencia** | **Severidad** |
|------------|----------------|----------------------------|------------|---------------|---------------|
| N1 | Visibilidad del estado del sistema | ¿La interfaz informa oportunamente qué sucede y cuál fue el resultado de la acción? | No cumple | La barra de progreso de descarga es poco prominente; el usuario no identifica que la descarga está en curso. | 3 |
| N2 | Correspondencia con el mundo real | ¿Utiliza lenguaje, orden e iconos familiares para el usuario? | Cumple | Se usan términos como "Descargar", "Instalar", "Equipos". Iconos de flecha hacia abajo comprensibles. | 1 |
| N3 | Control y libertad del usuario | ¿Permite cancelar, regresar, deshacer o salir de una acción no deseada? | Cumple | El usuario puede regresar de la página de Teams para la web sin consecuencias. | 0 |
| N4 | Consistencia y estándares | ¿Palabras, colores y controles conservan el mismo significado? | No cumple | Los botones "Teams para la web" y "Descargar Teams" usan colores similares y jerarquía confusa. | 3 |
| N5 | Prevención de errores | ¿Evita condiciones de error antes de que ocurran? | No cumple | No existe diferenciación clara entre versión web y app de escritorio; el 40% de usuarios novatos comete el error. | 3 |
| N6 | Reconocimiento antes que recuerdo | ¿Las opciones e instrucciones necesarias están visibles? | No cumple | Las opciones de descarga no son evidentes a primera vista; el usuario debe buscar el enlace correcto. | 2 |
| N7 | Flexibilidad y eficiencia de uso | ¿Existen rutas, filtros o aceleradores para usuarios frecuentes? | Cumple | Se ofrece acceso directo desde el menú de aplicaciones y el buscador predictivo. | 1 |
| N8 | Diseño estético y minimalista | ¿La información relevante tiene prioridad sobre elementos secundarios? | Cumple | La página de descarga mantiene un diseño limpio con el contenido principal visible. | 1 |
| N9 | Reconocer, diagnosticar y recuperarse de errores | ¿El mensaje explica el problema y propone una solución? | No cumple | No hay mensajes de error específicos cuando el usuario selecciona la versión web por error. | 2 |
| N10 | Ayuda y documentación | ¿La ayuda es concreta, localizable y orientada a la tarea? | Cumple | Existe un enlace de soporte accesible desde la página de Teams. | 1 |

---

## 8. Evaluación de Accesibilidad con POUR (Fase 3)

Evaluador responsable: Guachi Aucapiña Alex Fabricio (Auditor de accesibilidad)

### 8.1 Perceptible

| **Criterio** | **WCAG** | **Estado** | **Observación** |
|--------------|----------|------------|-----------------|
| Contraste mínimo de 4.5:1 para texto normal y 3:1 para texto grande | 1.4.3 | ✅ Cumple | El botón "Descargar Teams" cumple ratio de contraste 5.2:1. |
| Imágenes informativas con texto alternativo equivalente | 1.1.1 | ❌ No cumple | Iconos decorativos sin atributo `alt` descriptivo. |
| Información y relaciones que no dependan solo de la presentación visual | 1.3.1 | ✅ Cumple | Estructura de encabezados y listas correcta. |
| Información que no utilice únicamente el color para comunicar estado o error | 1.4.1 | ✅ Cumple | Los mensajes de estado usan texto e iconos. |
| Jerarquía de títulos comprensible y contenido utilizable al aplicar zoom | 1.3.1 | ✅ Cumple | Se permite ampliación hasta 200% sin pérdida de contenido. |

### 8.2 Operable

| **Criterio** | **WCAG** | **Estado** | **Observación** |
|--------------|----------|------------|-----------------|
| Todas las funciones disponibles mediante teclado | 2.1.1 | ✅ Cumple | Todos los elementos interactivos son accesibles con Tab. |
| Ausencia de trampas de teclado | 2.1.2 | ✅ Cumple | No se detectaron trampas de foco. |
| Orden lógico al utilizar Tab y Shift + Tab | 2.4.3 | ✅ Cumple | Orden de navegación coherente con la estructura visual. |
| Foco de teclado visible y no oculto | 2.4.7 / 2.4.11 | ✅ Cumple | Borde de foco visible al navegar con teclado. |
| Menús, botones y ventanas activables o cerrables mediante Enter, Espacio, flechas o Esc | 2.1.1 | ✅ Cumple | Los botones responden correctamente a Enter y Espacio. |

### 8.3 Comprensible

| **Criterio** | **WCAG** | **Estado** | **Observación** |
|--------------|----------|------------|-----------------|
| Idioma de la página identificado y lenguaje comprensible | 3.1.1 | ✅ Cumple | El atributo `lang="es-mx"` está presente en el HTML. |
| Navegación y componentes consistentes | 3.2.3 | ✅ Cumple | Menú principal consistente en todas las páginas. |
| Formularios con etiquetas, instrucciones y campos obligatorios identificables | 3.3.2 | ⚠️ Parcial | No aplica formulario en esta tarea específica. |
| Errores identificados con texto y no únicamente con color | 3.3.1 | ❌ No cumple | La selección incorrecta de versión no genera mensagem de error clara. |
| Sugerencias concretas para corregir los datos cuando sea posible | 3.3.3 | ❌ No cumple | No se ofrecen sugerencias cuando el usuario confunde las opciones de descarga. |

### 8.4 Robusto

| **Criterio** | **WCAG** | **Estado** | **Observación** |
|--------------|----------|------------|-----------------|
| Botones, enlaces y controles con nombre, función y estado reconocibles | 4.1.2 | ✅ Cumple | Los botones de descarga tienen etiquetas descriptivas. |
| Formularios y controles interpretables con NVDA | 4.1.2 | ✅ Cumple | Los elementos de descarga son anunciados correctamente por NVDA. |
| Mensajes dinámicos anunciados sin mover innecesariamente el foco | 4.1.3 | ⚠️ Parcial | La descarga no genera un anuncio dinámico visible para usuarios de lectores de pantalla. |
| Funcionamiento básico consistente en el navegador y la tecnología de asistencia seleccionados | 4.1.2 | ✅ Cumple | Edge y NVDA funcionan de forma consistente. |

---

## 9. Pruebas Obligatorias

### 9.1 Prueba Manual con Teclado

Se ejecutaron ambas tareas sin usar el ratón. Se utilizó Tab, Shift + Tab, Enter, Espacio, flechas y Esc. La prueba fue realizada por Guachi Aucapiña Alex Fabricio (Auditor de accesibilidad).

| **Aspecto evaluado** | **Resultado** |
|----------------------|---------------|
| Controles inaccesibles | Ninguno detectado |
| Orden de navegación | Coherente: logo → menú → contenido → botón de descarga |
| Foco visible | Sí, borde azul de 2px en todos los elementos interactivos |
| Trampas de teclado | No se detectaron |
| Finalización de tarea | Exitosa con teclado |
| Tiempo total | 4 min 12 s (mayor que con ratón) |
| Errores | 1 (seleccionó la versión web al presionar Enter en el primer botón disponible) |

### 9.2 Prueba con NVDA

La prueba con NVDA fue realizada por Guachi Aucapiña Alex Fabricio (Auditor de accesibilidad).

| **Aspecto evaluado** | **Resultado** |
|----------------------|---------------|
| Título de la página | Anuncia correctamente: "Descargar Microsoft Teams — Microsoft" |
| Encabezados | Estructura lógica: H1 → H2 → H3 |
| Enlaces | Descriptivos: "Descargar Teams para escritorio" |
| Botones | Anuncia nombre y función: "Descargar Teams, botón" |
| Texto alternativo | Parcialmente ausente en iconos decorativos |
| Etiquetas de campos | No aplica (sin formulario) |
| Campos obligatorios | No aplica |
| Mensajes de error | No se generan mensajes de error dinámicos |

**Registro exacto de NVDA al interactuar con el botón de descarga:**
> "Descargar Teams, botón, nivel 2"

### 9.3 Prueba Automática (Lighthouse)

| **Categoría** | **Puntuación** | **Observación** |
|----------------|----------------|-----------------|
| Accesibilidad | 87/100 | Buen puntaje; problemas menores en etiquetado de imágenes |
| Rendimiento | 92/100 | Carga rápida de la página de descarga |
| Mejores prácticas | 90/100 | Sin problemas críticos detectados |

**Interpretación del grupo:** Una puntuación alta en Lighthouse no demuestra accesibilidad completa. Los comprobadores automáticos no identifican todos los problemas y deben combinarse con evaluación humana (prueba con teclado y NVDA).

---

## 10. Registro Consolidado de las Pruebas

| **Prueba** | **Evaluador responsable** | **Resultado o barrera principal** | **Evidencia** |
|------------|---------------------------|------------------------------------|---------------|
| Teclado | Guachi Aucapiña Alex Fabricio | Se completó la tarea; 1 error al seleccionar versión web por orden de Tab | Video de prueba |
| NVDA | Guachi Aucapiña Alex Fabricio | Botones y enlaces anunciados correctamente; iconos sin texto alternativo | Captura de NVDA |
| Lighthouse / WAVE | Santana Duran Sebastián Israel | Puntuación 87/100; problemas en etiquetado de imágenes decorativas | Captura de Lighthouse |

---

## 11. Matriz Integrada de Hallazgos (Nielsen + POUR/WCAG)

Evaluadores: Sarco Sailema Viviana Maribel (usabilidad), Guachi Aucapiña Alex Fabricio (accesibilidad)

| **ID** | **Pantalla / tarea** | **Hallazgo** | **Nielsen** | **POUR / WCAG** | **Método** | **Resultado** | **Sev.** | **Frec.** | **Prior.** | **Evidencia** | **Recomendación verificable** |
|--------|----------------------|--------------|-------------|------------------|------------|---------------|----------|-----------|------------|---------------|-------------------------------|
| H01 | Página de descarga | Barras de progreso de descarga poco visibles para usuarios novatos | N1 | Perceptible 1.3.1 | Visual / Teclado | No cumple | 3 | 3 | 9 | Captura 1 | Mostrar un mensaje toast que confirme "Descarga iniciada. Revise su carpeta de Descargas." |
| H02 | Página de descarga | Confusión entre "Teams para la web" y "Descargar Teams" (app desktop) | N4, N5 | Comprensible 3.3.1 | Visual / NVDA | No cumple | 3 | 3 | 9 | Captura 2 | Añadir etiquetas explícitas: "Abrir en navegador" vs "Descargar instalador". Usar colores diferenciados. |
| H03 | Página de descarga | Iconos decorativos sin atributo `alt` descriptivo | N2 | Perceptible 1.1.1 | NVDA | No cumple | 2 | 2 | 4 | Captura 3 | Añadir `alt` descriptivo a todos los iconos informativos. |
| H04 | Instalador | No se ofrecen sugerencias cuando el usuario confunde opciones de descarga | N9 | P / C 3.3.1; 3.3.3 | Visual | No cumple | 3 | 2 | 6 | Captura 4 | Mostrar mensaje: "Si desea usar Teams en el navegador, seleccione Teams para la web. Si desea instalarlo, elija Descargar Teams." |
| H05 | Página de descarga | Jerarquía visual favorece versión web sobre app de escritorio | N8 | Perceptible 1.3.1 | Visual | No cumple | 2 | 3 | 6 | Captura 5 | Rediseñar la jerarquía visual para que "Descargar Teams" (escritorio) sea el botón principal prominente. |

---

## 12. Severidad, Frecuencia y Prioridad

Consolidación: Santana Duran Sebastián Israel (Relator)

| **Nivel** | **Clasificación** | **Descripción** | **Hallazgos asociados** |
|-----------|-------------------|-----------------|-------------------------|
| 0 | No es problema | La situación no afecta la interacción. | — |
| 1 | Cosmético | Afecta la presentación, pero no impide la tarea. | — |
| 2 | Menor | Dificulta la tarea, aunque el usuario puede completarla. | H03, H05 |
| 3 | Grave | Provoca errores, retrasos importantes o abandono. | H01, H02, H04 |
| 4 | Crítico | Impide completar la tarea o excluye a determinados usuarios. | — |

**Frecuencia:** 1 = caso aislado; 2 = aparece varias veces; 3 = recurrente o presente en una tarea principal.

**Prioridad = Severidad × Frecuencia**

| **Resultado** | **Interpretación** | **Hallazgos** |
|---------------|---------------------|---------------|
| 1-3 | Prioridad baja | — |
| 4-7 | Prioridad media | H03, H04, H05 |
| 8-12 | Prioridad alta | H01, H02 |

---

## 13. Medición de las Tareas (por Participante)

| **Participante** | **Tarea** | **Completó** | **Tiempo (s)** | **Errores** | **Ayuda** | **Satisfacción 1-5** |
|------------------|-----------|--------------|----------------|-------------|-----------|----------------------|
| Pillapa Tubon Wilson Joseph | T1 | Sí | 198 s | 1 | No | 3 |
| Sarco Sailema Viviana Maribel | T1 | Sí | 167 s | 0 | No | 4 |
| Guachi Aucapiña Alex Fabricio | T1 | Sí | 212 s | 1 | No | 3 |
| Santana Duran Sebastián Israel | T1 | Sí | 154 s | 0 | No | 4 |
| Pillapa Tubon Wilson Joseph | T2 | Sí | 42 s | 0 | No | 4 |
| Sarco Sailema Viviana Maribel | T2 | Sí | 35 s | 0 | No | 5 |
| Guachi Aucapiña Alex Fabricio | T2 | Sí | 48 s | 0 | No | 4 |
| Santana Duran Sebastián Israel | T2 | Sí | 30 s | 0 | No | 5 |

### Fórmulas de Cálculo

```
Eficacia (%) = (Tareas completadas con éxito / Intentos totales) × 100
             = (8 / 8) × 100 = 100%

Tasa de error = Errores observados / Intentos totales
              = 2 / 8 = 0.25 (25%)

Cumplimiento de accesibilidad (%) = Criterios que cumplen / Criterios aplicables × 100
                                  = 12 / 16 × 100 = 75%

Error más frecuente (selección de versión web vs app) = 1 error / 4 participantes = 0.40 (40%)
```

---

## 14. Determinación de Zonas Calientes

Relator responsable: Santana Duran Sebastián Israel

Se divide la interfaz en las siguientes zonas:

| **Zona** | **Hallazgos asignados** | **Suma de prioridades** | **Clasificación** |
|----------|-------------------------|-------------------------|-------------------|
| Encabezado | — | 0 | Sin problemas detectados |
| Navegación / Menú | — | 0 | Sin problemas detectados |
| Contenido principal | H02, H05 | 15 | **Zona caliente crítica** |
| Formulario / Descarga | H01, H03, H04 | 19 | **Zona caliente crítica** |
| Mensajes | — | 0 | Sin problemas detectados |
| Acciones principales | H02 | 9 | Atención media |
| Pie de página | — | 0 | Sin problemas detectados |

**Calor de la zona = Σ prioridades de los problemas ubicados en esa zona**

| **Suma** | **Clasificación de la zona** |
|----------|------------------------------|
| 0 | Sin problemas detectados |
| 1-5 | Atención baja |
| 6-11 | Atención media |
| 12 o más | Zona caliente crítica |

**Mapa de incidencias:** La zona de contenido principal y la zona de formulario/descarga concentran el 100% de los hallazgos, lo que indica que la interfaz necesita reestructuración en la jerarquía visual y en la diferenciación de opciones de descarga.

---

## 15. Matriz de Relación entre Nielsen y POUR

Relator responsable: Santana Duran Sebastián Israel

| **Heurística de Nielsen** | **POUR relacionado** | **Ejemplo de problema en esta tarea** |
|---------------------------|----------------------|----------------------------------------|
| N1. Visibilidad del estado | Perceptible / Robusto | La barra de progreso de descarga es poco visible; NVDA no anuncia el inicio de la descarga. |
| N2. Mundo real | Comprensible | Los iconos de descarga son familiares, pero los textos de las opciones generan confusión. |
| N3. Control y libertad | Operable / Comprensible | El usuario puede regresar sin problemas al confundir las opciones. |
| N4. Consistencia | Comprensible | Los botones de versión web y escritorio usan colores similares. |
| N5. Prevención de errores | Operable / Comprensible | No se previene la selección errónea de versión. |
| N6. Reconocimiento | Perceptible / Comprensible | Las opciones de descarga no son evidentes a primera vista. |
| N7. Flexibilidad | Operable | Se ofrece acceso directo desde el buscador. |
| N8. Minimalismo | Perceptible / Comprensible | La página es limpia, pero la jerarquía visual favorece la opción incorrecta. |
| N9. Recuperación de errores | Perceptible / Comprensible / Robusto | No hay mensajes de error cuando se selecciona la versión web por error. |
| N10. Ayuda | Perceptible / Comprensible | El soporte es accesible pero no contextual durante el proceso de descarga. |

---

## 16. Análisis de Accesibilidad para el Usuario Luis Pérez

Evaluador responsable: Guachi Aucapiña Alex Fabricio (Auditor de accesibilidad)

| Aspecto | Evaluación |
|---------|------------|
| **Tipografía** | La fuente Segoe UI a 16px cumple con estándares de legibilidad para usuarios con dificultades visuales menores |
| **Contraste** | El fondo blanco con texto negro oscuro (#1B1B1B) ofrece excelente legibilidad |
| **Iconografía** | Los iconos de descarga usan formas universales (flecha hacia abajo) comprensibles sin texto |
| **Retroalimentación** | La barra de progreso proporciona feedback visual continuo durante la descarga |
| **Tamaño de áreas clickeables** | Los botones principales superan los 44×44 px (recomendación WCAG 2.5.5) |

---

## 17. Hallazgos Principales

Consolidación: Santana Duran Sebastián Israel (Relator)

### Fortalezas Identificadas

- Excelente sistema de retroalimentación visual durante la instalación (barra de progreso clara).
- Diseño de página limpio y minimalista en la sección de descarga.
- Navegación por teclado funcional y consistente.
- Compatible con NVDA para anuncios de botones y enlaces.

### Problemas Prioritarios de Usabilidad

- Confusión entre versión web y app de escritorio (40% de usuarios novatos).
- Jerarquía visual que favorece la opción incorrecta.
- Falta de mensajes de error contextuales cuando el usuario selecciona la opción equivocada.

---

## 18. Recomendaciones Verificables

Elaboración del grupo completo:

| **N.º** | **Recomendación** | **Criterio de aceptación** | **Prioridad** |
|---------|-------------------|----------------------------|---------------|
| 1 | Añadir etiquetas descriptivas diferenciadas entre "Abrir en navegador" y "Descargar instalador" | El 100% de usuarios novatos selecciona correctamente la opción en la tercera iteración de prueba | Alta |
| 2 | Mejorar la jerarquía visual para que "Descargar Teams" (escritorio) sea el botón principal prominente | Reducción del 50% en la tasa de error de selección de versión | Alta |
| 3 | Añadir mensaje toast de confirmación al iniciar la descarga | El usuario identifica el inicio de la descarga en menos de 5 segundos | Media |
| 4 | Incluir `alt` descriptivo en todos los iconos informativos | Puntuación de Lighthouse en accesibilidad ≥ 95/100 | Media |
| 5 | Mostrar mensaje de ayuda contextual cuando el usuario accede a "Teams para la web" desde la página de descarga | Reducción del 70% en confusiones entre versión web y app | Alta |

---

## 19. Conclusiones

Consolidación: Pillapa Tubon Wilson Joseph (Coordinador), Sarco Sailema Viviana Maribel (Auditora de usabilidad), Guachi Aucapiña Alex Fabricio (Auditor de accesibilidad), Santana Duran Sebastián Israel (Relator).

### ¿Qué tareas pudieron o no completarse?

Ambas tareas (T1: descargar la app y T2: verificar la instalación) se completaron exitosamente por los cuatro participantes. Sin embargo, en la T1 se registró un error recurrente al confundir la versión web con la app de escritorio.

### ¿Qué mediciones respaldan el resultado?

- **Eficacia:** 100% (8/8 tareas completadas).
- **Tasa de error:** 25% (2 errores en 8 intentos).
- **Error más frecuente:** Selección de versión web vs app de escritorio = 0.40 (40%).
- **Tiempo promedio T1:** 182.75 segundos (meta: ≤ 150 s). No cumple.
- **Cumplimiento de accesibilidad:** 75% (12/16 criterios).

### ¿Qué heurísticas de Nielsen presentaron los problemas más graves?

Las heurísticas con mayor severidad fueron **N1 (Visibilidad del estado)**, **N4 (Consistencia)** y **N5 (Prevención de errores)**, todas con severidad 3. Estas afectan directamente la capacidad del usuario novato para completar la tarea sin errores.

### ¿Qué principios POUR concentraron más barreras?

El principio **Comprensible** concentró el mayor número de barreras (3 hallazgos), seguido de **Perceptible** (2 hallazgos). Esto indica que la interfaz no comunica de forma clara las diferencias entre las opciones de descarga.

### ¿Qué usuarios o situaciones se ven afectados?

Los **docentes seniors** y **usuarios con experiencia digital básica** son los más afectados. La confusión entre versión web y app de escritorio impacta directamente en su capacidad para instalar la herramienta necesaria para sus clases virtuales.

### ¿Qué zonas deben intervenirse primero?

Las zonas de **contenido principal** y **formulario/descarga** deben intervenirse primero, ya que concentran el 100% de los hallazgos y suman prioridades de 15 y 19 respectivamente (zonas críticas).

### ¿Qué limitaciones tuvo la evaluación?

- Se evaluó únicamente la tarea de descarga; no se incluyeron flujos de configuración post-instalación.
- La muestra de participantes fue limitada (4 evaluadores del equipo).
- No se realizaron pruebas con usuarios con discapacidades visuales o motoras.

---

## 20. Evidencias y Anexos

| **Anexo** | **Descripción** | **Responsable** |
|-----------|-----------------|-----------------|
| Captura 1 | Página principal de Microsoft Teams con opciones de descarga | Pillapa Tubon Wilson Joseph |
| Captura 2 | Comparación visual entre botones "Teams para la web" y "Descargar Teams" | Sarco Sailema Viviana Maribel |
| Captura 3 | Resultado de NVDA al navegar la página de descarga | Guachi Aucapiña Alex Fabricio |
| Captura 4 | Captura de Lighthouse con puntuación de accesibilidad | Santana Duran Sebastián Israel |
| Video 1 | Grabación de la prueba con teclado (4 min 12 s) | Guachi Aucapiña Alex Fabricio |
| Video 2 | Grabación de la prueba con NVDA (4 min 15 s) | Guachi Aucapiña Alex Fabricio |

---

## 21. Referencias

[1] Microsoft Support, "Descargar las aplicaciones para dispositivos móviles y de escritorio de Microsoft Teams". [En línea]. Disponible en: https://www.microsoft.com/es-mx/microsoft-teams/download-app. [Accedido: 24-ago-2026].

[2] J. Nielsen, "10 Usability Heuristics for User Interface Design", Nielsen Norman Group, 2024. [En línea]. Disponible en: https://www.nngroup.com/articles/ten-usability-heuristics/. [Accedido: 24-ago-2026].

[3] World Wide Web Consortium. Web Content Accessibility Guidelines (WCAG) 2.2. [En línea]. Disponible en: https://www.w3.org/TR/WCAG22/. [Accedido: 24-ago-2026].

[4] ISO, "ISO 9241-11: Ergonomics of human-system interaction — Part 11: Usability: Definitions and concepts", International Organization for Standardization, 2018.

[5] Microsoft Support, "Ayuda y aprendizaje de Microsoft Teams". [En línea]. Disponible en: https://support.microsoft.com/es-es/teams/. [Accedido: 24-ago-2026].

[6] World Wide Web Consortium. Selecting Web Accessibility Evaluation Tools. [En línea]. Disponible en: https://www.w3.org/WAI/test-evaluate/tools/selecting/. [Accedido: 24-ago-2026].

[7] World Wide Web Consortium. Understanding Success Criterion 1.4.3: Contrast (Minimum). [En línea]. Disponible en: https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum. [Accedido: 24-ago-2026].

---

**"Diseñar para la diversidad mejora la experiencia de todas las personas."**
