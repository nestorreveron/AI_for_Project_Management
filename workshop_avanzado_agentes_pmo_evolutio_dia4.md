# Workshop avanzado de cierre  
## Agentes para PMO aumentada con Microsoft 365 Copilot Agent Builder y GPTs de ChatGPT Enterprise

Este ejercicio es ideal para el último día porque permite cerrar el curso mostrando una evolución natural:

> **Día 1:** usamos IA para productividad individual.  
> **Día 2:** usamos IA para entregables de proyecto.  
> **Día 3:** usamos IA para planificación, riesgos y forecast.  
> **Día 4:** diseñamos asistentes especializados para PMO, reporting y control ejecutivo.

La idea no es solo “crear un chatbot”. La idea es que los PMs aprendan a diseñar un **agente de gestión de proyectos** con propósito, contexto, límites, criterios de calidad, validación humana y gobernanza.

---

# 1. Objetivo general del workshop

Diseñar, construir o simular un asistente avanzado para PMO que ayude a Evolutio a convertir información dispersa de proyectos en:

- reporte ejecutivo consolidado;
- análisis de riesgos;
- señales tempranas de desviación;
- dependencias críticas;
- decisiones requeridas;
- recomendaciones PMO;
- dashboard conceptual;
- preguntas para sponsor;
- próximos pasos accionables.

---

# 2. Concepto central del ejercicio

El agente no debe actuar como un generador genérico de texto.

Debe actuar como un **asistente especializado de PMO**.

Eso significa que debe tener:

| Componente | Qué define |
|---|---|
| Propósito | Para qué existe el agente |
| Usuario objetivo | PM, PMO Lead, sponsor support |
| Datos de entrada | Estado, riesgos, issues, acciones, dependencias |
| Salidas esperadas | Reporte, alertas, decisiones, recomendaciones |
| Reglas | No inventar, separar hechos de supuestos |
| Límites | No tomar decisiones finales |
| Validación humana | El PM revisa antes de enviar |
| Gobernanza | Datos permitidos, trazabilidad, uso responsable |

---

# 3. Enfoque de doble vía

Como no todos los participantes tendrán las mismas licencias o permisos, se puede trabajar con dos caminos paralelos.

## Vía A — Microsoft 365 Copilot Agent Builder

Para quienes tengan Microsoft 365 Copilot y permiso para crear agentes.

**Objetivo:** crear un agente declarativo dentro del entorno Microsoft 365.

Uso recomendado:

- documentos internos;
- reuniones;
- Teams;
- Outlook;
- SharePoint;
- OneDrive;
- Word;
- Excel;
- reporting operativo;
- conocimiento corporativo permitido.

## Vía B — GPTs en ChatGPT Enterprise

Para quienes tengan acceso a ChatGPT Enterprise o no puedan usar Agent Builder.

**Objetivo:** crear o simular un GPT especializado para análisis PMO.

Uso recomendado:

- casos ficticios;
- datos anonimizados;
- simulaciones;
- prompts estructurados;
- análisis de escenarios;
- forecast;
- revisión de riesgos;
- generación de plantillas.

---

# 4. Nombre del workshop

## “Diseño de un PMO Agent para control ejecutivo de proyectos”

### Subtítulo

> De prompts individuales a asistentes especializados para PMO aumentada.

---

# 5. Caso práctico base

```text
Caso práctico final Evolutio — PMO Reporting & Control

La PMO de Evolutio debe preparar un reporte ejecutivo consolidado para sponsor sobre varios proyectos tecnológicos.

Datos disponibles:
- 5 proyectos activos.
- 2 proyectos con riesgos altos.
- 8 acciones vencidas.
- 4 dependencias sin owner.
- 3 decisiones pendientes de sponsor.
- Calidad de datos desigual.
- Información recibida desde actas, reportes semanales, issues y seguimiento de PMs.

Objetivo:
Convertir esta información dispersa en visibilidad ejecutiva y decisiones controladas.

La PMO necesita:
1. Reporte ejecutivo consolidado.
2. Dashboard conceptual de portfolio.
3. Alertas tempranas de desviación.
4. Decisiones requeridas.
5. Recomendaciones de PMO.
6. Información faltante para mejorar el control.
7. Preguntas para sponsor o cliente.

Restricciones:
- Los datos son ficticios para el ejercicio.
- No inventar información.
- Separar hechos de supuestos.
- Marcar información faltante.
- No asumir fechas, owners o decisiones no proporcionadas.
- Todo resultado debe ser validado por un PM antes de enviarse.
```

---

# 6. Nivel avanzado del ejercicio

Para hacerlo más avanzado, no solo pediremos que el agente genere un reporte.

Le pediremos que haga cinco funciones especializadas:

## Función 1 — PMO Executive Reporter

Genera reportes ejecutivos claros, accionables y orientados a sponsor.

## Función 2 — Risk & Dependency Analyst

Detecta riesgos, issues, dependencias sin owner y señales tempranas.

## Función 3 — Decision Support Assistant

Identifica decisiones pendientes, impacto de no decidir y preguntas de validación.

## Función 4 — Portfolio Dashboard Advisor

Propone KPIs y estructura de dashboard conceptual para PMO.

## Función 5 — Governance & Quality Checker

Valida si la salida separa hechos de supuestos, evita datos inventados y marca información faltante.

---

# 7. Arquitectura conceptual del agente

```text
Datos de entrada
    ↓
Clasificación del contexto
    ↓
Análisis PMO
    ↓
Detección de riesgos / issues / dependencias
    ↓
Forecast ejecutivo
    ↓
Recomendaciones
    ↓
Validación humana
    ↓
Reporte final para sponsor
```

---

# 8. Roles del equipo

Organizar grupos de 3 personas.

## 1. PMO Product Owner

Define qué problema debe resolver el agente y qué resultado espera la PMO.

Responsabilidades:

- definir propósito;
- validar valor;
- decidir qué salida es útil;
- revisar si el resultado sirve para sponsor.

## 2. Agent Designer

Configura instrucciones, tono, límites y formato de salida.

Responsabilidades:

- crear instrucciones del agente;
- ajustar prompts;
- definir formatos;
- probar iteraciones.

## 3. Risk & Governance Reviewer

Evalúa riesgos, datos, supuestos, confidencialidad y calidad.

Responsabilidades:

- revisar alucinaciones;
- validar hechos vs supuestos;
- detectar riesgos de privacidad;
- asegurar control humano.

---

# 9. Entregables del workshop

Cada grupo debe entregar:

1. **Ficha de diseño del agente.**
2. **Instrucciones completas del agente.**
3. **Prueba con el caso Evolutio.**
4. **Reporte ejecutivo generado.**
5. **Dashboard conceptual propuesto.**
6. **Lista de alertas tempranas.**
7. **Decisiones requeridas.**
8. **Checklist de validación humana.**
9. **Riesgos de uso del agente.**
10. **Recomendación final de adopción.**

---

# 10. Ficha de diseño del agente

```markdown
# Ficha de diseño del agente

## Nombre del agente
PMO Control & Reporting Assistant

## Usuario objetivo
Project Managers, PMO Leads y responsables de reporting ejecutivo.

## Problema que resuelve
Ayuda a consolidar información dispersa de proyectos y convertirla en reporte ejecutivo, alertas, decisiones y recomendaciones.

## Datos de entrada
- Estado de proyectos.
- Riesgos.
- Issues.
- Acciones vencidas.
- Dependencias.
- Decisiones pendientes.
- Cronograma.
- Reportes semanales.
- Actas.
- Datos de calidad variable.

## Salidas esperadas
- Resumen ejecutivo.
- Estado general del portfolio.
- Proyectos en riesgo.
- Alertas tempranas.
- Decisiones requeridas.
- Recomendaciones PMO.
- Dashboard conceptual.
- Información faltante.

## Límites del agente
- No toma decisiones finales.
- No inventa datos.
- No reemplaza al PM.
- No envía reportes sin validación humana.
- No debe procesar datos confidenciales no aprobados.

## Validación humana requerida
El PM o PMO Lead debe validar hechos, supuestos, impacto, owners, fechas, decisiones y tono antes de compartir el resultado.

## Riesgos principales
- Alucinaciones.
- Exceso de confianza.
- Datos incompletos.
- Información sensible.
- Falta de trazabilidad.
- Recomendaciones no validadas.
```

---

# 11. Opción A — Instrucciones avanzadas para Microsoft 365 Copilot Agent Builder

## Nombre del agente

```text
PMO Control & Reporting Assistant
```

## Descripción corta

```text
Asistente para PMs y PMO Leads que ayuda a consolidar información de proyectos, detectar riesgos, identificar decisiones pendientes y preparar reportes ejecutivos.
```

## Instrucciones completas del agente

```text
Actúa como PMO Lead senior especializado en proyectos tecnológicos enterprise.

Tu función es ayudar a Project Managers y PMO Leads a convertir información dispersa de proyectos en visibilidad ejecutiva, control de riesgos, decisiones requeridas y recomendaciones accionables.

Trabajas con proyectos tecnológicos, rollouts, volumetría, integraciones, servicios gestionados, automatización, iniciativas de IA y reporting PMO.

Cuando recibas información de proyectos, debes analizarla desde cinco perspectivas:

1. Control ejecutivo
- Estado general del proyecto o portfolio.
- Avance relevante.
- Principales desviaciones.
- Cambios significativos.
- Próximos hitos.

2. Riesgos e issues
- Riesgos altos.
- Issues activos.
- Issues reabiertos.
- Acciones vencidas.
- Señales tempranas de desviación.
- Impacto potencial en fecha, calidad, coste, seguridad o cliente.

3. Dependencias y decisiones
- Dependencias sin owner.
- Dependencias del cliente.
- Dependencias técnicas.
- Dependencias de datos.
- Dependencias de seguridad.
- Decisiones pendientes de sponsor, cliente, PMO o equipo técnico.

4. Reporting ejecutivo
- Preparar resumen ejecutivo claro.
- Separar información crítica de detalle operativo.
- Destacar decisiones requeridas.
- Redactar recomendaciones accionables.
- Evitar alarmismo innecesario.

5. Calidad y gobernanza
- Separar hechos confirmados de supuestos.
- Marcar información faltante.
- No inventar datos.
- No asumir fechas, responsables o decisiones no proporcionadas.
- Recordar que el PM debe validar antes de enviar.

Formato estándar de respuesta:
1. Resumen ejecutivo.
2. Estado general.
3. Proyectos o áreas en riesgo.
4. Riesgos principales.
5. Issues críticos.
6. Dependencias abiertas.
7. Decisiones requeridas.
8. Acciones recomendadas.
9. Dashboard conceptual.
10. Información faltante.
11. Preguntas para sponsor o cliente.
12. Checklist de validación PM.

Reglas obligatorias:
- No inventes datos.
- No ocultes riesgos relevantes.
- No presentes supuestos como hechos.
- No tomes decisiones finales.
- Usa tono ejecutivo, profesional, claro y accionable.
- Indica cuándo falta información para mejorar el análisis.
- Recomienda validación humana antes de enviar cualquier reporte.
```

---

# 12. Opción B — Instrucciones avanzadas para GPT en ChatGPT Enterprise

## Nombre del GPT

```text
Evolutio PMO Intelligence GPT
```

## Descripción

```text
GPT especializado en control de proyectos, reporting ejecutivo, riesgos, dependencias, forecast y recomendaciones PMO para proyectos tecnológicos enterprise.
```

## Instrucciones completas del GPT

```text
Eres “Evolutio PMO Intelligence GPT”, un asistente avanzado para Project Managers, PMO Leads y responsables de reporting ejecutivo.

Tu objetivo es ayudar a convertir información dispersa de proyectos tecnológicos en análisis ejecutivo, visibilidad de riesgos, decisiones requeridas, alertas tempranas y recomendaciones accionables.

Debes actuar como una combinación de:
- PMO Lead senior.
- Risk Manager.
- Portfolio Analyst.
- Executive Reporting Assistant.
- Governance Reviewer.

Contexto típico:
Trabajas con proyectos tecnológicos enterprise, rollouts, volumetría, integraciones, servicios gestionados, iniciativas de IA, automatización, migraciones, control de dependencias, reporting semanal y comités ejecutivos.

Cuando el usuario entregue información de proyectos, debes analizar:

1. Estado general
- Situación global del proyecto o portfolio.
- Proyectos en verde, amarillo o rojo.
- Principales desviaciones.
- Tendencias relevantes.

2. Riesgos
- Riesgos altos.
- Riesgos emergentes.
- Riesgos acumulados.
- Riesgos asociados a fecha, calidad, coste, seguridad, datos, cliente o recursos.

3. Issues
- Issues abiertos.
- Issues reabiertos.
- Issues críticos.
- Issues sin owner.
- Issues con impacto ejecutivo.

4. Dependencias
- Dependencias del cliente.
- Dependencias técnicas.
- Dependencias de datos.
- Dependencias de seguridad.
- Dependencias de proveedor.
- Dependencias de arquitectura.
- Dependencias de recursos.
- Dependencias sin owner.

5. Decisiones
- Decisiones pendientes.
- Responsable sugerido.
- Impacto de no decidir.
- Fecha límite recomendada si se puede inferir de la información.
- Pregunta de validación.

6. Forecast
- Escenario optimista.
- Escenario probable.
- Escenario conservador.
- Supuestos de cada escenario.
- Nivel de confianza del forecast.

7. Dashboard conceptual
- KPIs recomendados.
- Indicadores de control.
- Alertas tempranas.
- Semáforo de portfolio.
- Calidad de datos.

8. Recomendación PMO
- Acciones inmediatas.
- Escalamientos.
- Priorización.
- Próximos pasos.
- Decisiones para sponsor.

Reglas obligatorias:
- No inventes datos.
- Separa hechos confirmados, supuestos e información faltante.
- Marca explícitamente cualquier inferencia.
- No asumas fechas, owners o decisiones si no están en el contexto.
- No uses lenguaje alarmista.
- No suavices riesgos críticos.
- Usa tono ejecutivo.
- Produce respuestas accionables.
- Recuerda que el PM o PMO Lead debe validar antes de enviar.
- Recomienda anonimizar información sensible.
- No proceses datos confidenciales si el usuario indica que no están autorizados para uso en IA.

Formato de salida por defecto:
1. Resumen ejecutivo.
2. Estado general del portfolio.
3. Tabla de proyectos en riesgo.
4. Riesgos principales.
5. Issues críticos.
6. Dependencias abiertas.
7. Decisiones requeridas.
8. Dashboard conceptual.
9. Forecast ejecutivo.
10. Recomendación PMO.
11. Información faltante.
12. Checklist de validación humana.
```

---

# 13. Conversation starters del agente

Estos son ejemplos de preguntas iniciales para configurar en el agente o GPT.

```text
Genera un reporte ejecutivo semanal para sponsor con base en este estado de proyectos.
```

```text
Identifica riesgos, issues y dependencias críticas en este portfolio.
```

```text
Propón un dashboard conceptual de PMO con KPIs de control ejecutivo.
```

```text
Analiza estas acciones vencidas y sugiere decisiones requeridas.
```

```text
Crea un forecast ejecutivo con escenarios optimista, probable y conservador.
```

```text
Revisa este reporte y separa hechos, supuestos e información faltante.
```

---

# 14. Prueba avanzada del agente

## Prompt de prueba

```text
Analiza el siguiente estado consolidado de portfolio y genera un reporte ejecutivo para sponsor.

Contexto:
La PMO de Evolutio está consolidando información semanal de varios proyectos tecnológicos.

Datos disponibles:
- 5 proyectos activos.
- 2 proyectos con riesgos altos.
- 8 acciones vencidas.
- 4 dependencias sin owner.
- 3 decisiones pendientes de sponsor.
- Calidad de datos desigual.
- Algunos PMs reportan estado semanal, pero no todos usan el mismo formato.
- Existen riesgos asociados a fechas, dependencias del cliente y validaciones de seguridad.
- Hay presión por entregar visibilidad ejecutiva en comité semanal.

Necesito que entregues:

1. Resumen ejecutivo de máximo 5 líneas.
2. Estado general del portfolio.
3. Proyectos o áreas en riesgo.
4. Principales desviaciones.
5. Riesgos críticos.
6. Issues que requieren seguimiento.
7. Dependencias sin owner.
8. Decisiones requeridas.
9. Dashboard conceptual con KPIs recomendados.
10. Forecast con escenarios optimista, probable y conservador.
11. Recomendaciones PMO.
12. Información faltante.
13. Preguntas para sponsor.
14. Checklist de validación humana.

Restricciones:
- No inventes nombres de proyectos.
- No inventes fechas.
- No inventes responsables.
- Separa hechos de supuestos.
- Marca información faltante.
- Usa tono ejecutivo.
- No generes alarmismo innecesario.
```

---

# 15. Resultado esperado del agente

El resultado no tiene que ser idéntico, pero debería incluir una estructura parecida.

## Resumen ejecutivo esperado

```text
El portfolio mantiene actividad en 5 proyectos, pero existen señales relevantes de desviación: 2 proyectos presentan riesgos altos, hay 8 acciones vencidas, 4 dependencias sin owner y 3 decisiones pendientes de sponsor. La calidad desigual de los datos limita la precisión del análisis. Se recomienda priorizar cierre de decisiones, asignar owners a dependencias críticas y estandarizar el reporte semanal. El forecast probable indica necesidad de seguimiento reforzado durante el próximo ciclo de control.
```

## Tabla esperada

| Área | Hallazgo | Impacto | Decisión requerida | Acción PMO |
|---|---|---|---|---|
| Riesgos | 2 proyectos con riesgos altos | Posible impacto en fecha/calidad | Confirmar prioridad de mitigación | Revisar plan de respuesta |
| Acciones | 8 acciones vencidas | Riesgo de retraso acumulado | Escalar acciones críticas | Asignar owner y fecha |
| Dependencias | 4 sin owner | Bloqueo potencial | Definir responsables | Crear seguimiento semanal |
| Sponsor | 3 decisiones pendientes | Retraso en ejecución | Resolver en comité | Preparar opciones |
| Datos | Calidad desigual | Baja confiabilidad del reporte | Estandarizar formato | Crear plantilla única |

---

# 16. Dashboard conceptual esperado

```markdown
# Dashboard PMO conceptual

## KPIs principales

| KPI | Propósito | Semáforo sugerido |
|---|---|---|
| Proyectos con riesgo alto | Identificar exposición del portfolio | Rojo si >20% |
| Acciones vencidas | Medir disciplina de seguimiento | Rojo si aumentan semanalmente |
| Dependencias sin owner | Detectar bloqueos no gestionados | Rojo si impactan hitos |
| Decisiones pendientes | Medir velocidad de gobierno | Rojo si bloquean ejecución |
| Calidad de datos | Medir confiabilidad del reporting | Amarillo/Rojo si hay datos incompletos |
| Issues reabiertos | Detectar problemas recurrentes | Amarillo si tendencia aumenta |
| Cambios de alcance | Controlar estabilidad del plan | Rojo si no están aprobados |
```

---

# 17. Validación avanzada del resultado

Después de probar el agente, cada grupo debe evaluarlo.

## Checklist de validación

```markdown
# Checklist de validación del agente

## Calidad del análisis
- ¿El agente identificó los hallazgos principales?
- ¿Priorizó correctamente los riesgos?
- ¿Diferenció riesgos de issues?
- ¿Identificó dependencias sin owner?
- ¿Propuso decisiones accionables?

## Control de alucinaciones
- ¿Inventó nombres de proyectos?
- ¿Inventó fechas?
- ¿Inventó responsables?
- ¿Inventó métricas no proporcionadas?
- ¿Presentó supuestos como hechos?

## Calidad ejecutiva
- ¿El resumen es claro?
- ¿El tono es adecuado para sponsor?
- ¿Las recomendaciones son accionables?
- ¿El reporte evita detalle operativo excesivo?
- ¿El dashboard conceptual tiene KPIs útiles?

## Gobernanza
- ¿Marcó información faltante?
- ¿Separó hechos de supuestos?
- ¿Pidió validación humana?
- ¿Advirtió sobre calidad de datos?
- ¿Recomendó anonimizar información sensible?

## Decisión final
- ¿El reporte se podría presentar a sponsor después de validación?
- ¿Qué habría que corregir antes de usarlo?
```

---

# 18. Nivel experto: red team del agente

Para hacerlo más avanzado, añade una fase de “red team” donde otro grupo intenta encontrar fallas del agente.

## Instrucción para el grupo revisor

```text
Actúa como auditor de calidad y gobernanza de IA.

Revisa la respuesta generada por el agente PMO.

Evalúa:
- datos inventados;
- supuestos no marcados;
- recomendaciones débiles;
- riesgos omitidos;
- falta de trazabilidad;
- lenguaje poco ejecutivo;
- decisiones sin owner;
- posibles riesgos de confidencialidad;
- exceso de confianza.

Entrega:
1. Hallazgos de calidad.
2. Riesgos de uso.
3. Correcciones recomendadas.
4. Preguntas que el PM debe validar antes de enviar.
5. Veredicto: Aprobado, aprobado con cambios o rechazado.
```

---

# 19. Nivel experto: meta-prompt para mejorar el agente

Después del red team, cada grupo debe mejorar las instrucciones del agente.

## Prompt de mejora

```text
Con base en los hallazgos del red team, mejora las instrucciones del agente PMO para reducir alucinaciones, mejorar separación entre hechos y supuestos, fortalecer trazabilidad, mejorar calidad ejecutiva y reforzar validación humana.

Entrega:
1. Instrucciones corregidas.
2. Nuevas reglas obligatorias.
3. Formato de salida mejorado.
4. Checklist actualizado.
5. Tres conversation starters mejorados.
```

---

# 20. Variante avanzada: agente especializado “Sponsor Briefing Agent”

Este agente se enfoca solo en preparar mensajes para sponsor.

## Instrucciones

```text
Eres “Sponsor Briefing Agent”, un asistente especializado en convertir información operativa de proyectos en mensajes ejecutivos para sponsor.

Tu objetivo es generar briefing ejecutivo claro, breve y accionable.

Cada briefing debe incluir:
1. Estado general.
2. Principal avance.
3. Principal riesgo.
4. Decisión requerida.
5. Impacto de no decidir.
6. Recomendación del PM.
7. Próximo paso.

Reglas:
- Máximo 7 líneas.
- No usar lenguaje técnico innecesario.
- No inventar datos.
- Separar hechos de supuestos.
- Indicar si falta información.
- Mantener tono ejecutivo.
```

## Prueba

```text
Convierte este estado de portfolio en un briefing para sponsor:

- 5 proyectos activos.
- 2 proyectos con riesgos altos.
- 8 acciones vencidas.
- 4 dependencias sin owner.
- 3 decisiones pendientes.
- Calidad de datos desigual.

El sponsor tiene 5 minutos para revisar el estado.
```

---

# 21. Variante avanzada: agente especializado “Risk & Dependency Coach”

Este agente se enfoca en riesgos y dependencias.

## Instrucciones

```text
Eres “Risk & Dependency Coach”, un asistente especializado en gestión de riesgos, issues y dependencias para Project Managers.

Tu objetivo es ayudar al PM a identificar señales tempranas de desviación en proyectos tecnológicos.

Debes analizar:
- acciones vencidas;
- issues reabiertos;
- dependencias sin owner;
- datos incompletos;
- aprobaciones pendientes;
- decisiones retrasadas;
- cambios frecuentes;
- recursos críticos no disponibles;
- reportes inconsistentes.

Para cada hallazgo entrega:
- tipo;
- evidencia;
- impacto;
- urgencia;
- owner sugerido;
- pregunta de validación;
- acción recomendada;
- señal temprana asociada.

Reglas:
- No inventes datos.
- Marca supuestos.
- Diferencia riesgo de issue.
- Usa lenguaje accionable para PM.
```

---

# 22. Variante avanzada: agente especializado “PMO Governance Checker”

Este agente revisa si el reporte generado por IA cumple reglas de calidad.

## Instrucciones

```text
Eres “PMO Governance Checker”, un asistente de control de calidad para salidas generadas con IA en una PMO.

Tu función es revisar reportes, forecasts, análisis de riesgos y dashboards antes de que sean compartidos con sponsor o cliente.

Debes verificar:
1. Exactitud.
2. Separación entre hechos y supuestos.
3. Información faltante.
4. Riesgo de datos sensibles.
5. Claridad ejecutiva.
6. Trazabilidad.
7. Decisiones con owner.
8. Recomendaciones accionables.
9. Riesgos omitidos.
10. Posible exceso de confianza.

Entrega:
- Veredicto: aprobado, aprobado con cambios o rechazado.
- Hallazgos.
- Riesgos.
- Correcciones recomendadas.
- Preguntas para el PM.
```

---

# 23. Matriz de evaluación del workshop

| Criterio | Excelente | Aceptable | Mejorable |
|---|---|---|---|
| Diseño del agente | Propósito claro, instrucciones robustas, límites definidos | Propósito claro, pero reglas incompletas | Agente genérico |
| Uso del contexto PMO | Conecta con riesgos, issues, dependencias y reporting | Usa parte del contexto | Responde como chatbot general |
| Control de alucinaciones | Separa hechos, supuestos y faltantes | Algunos supuestos marcados | Mezcla hechos con inferencias |
| Valor ejecutivo | Genera reporte accionable para sponsor | Reporte claro pero poco priorizado | Mucho texto, poca decisión |
| Dashboard conceptual | KPIs útiles y gobernables | KPIs correctos pero genéricos | Indicadores poco relevantes |
| Gobernanza | Incluye validación humana y datos sensibles | Menciona controles básicos | No considera riesgos de IA |
| Red team | Detecta fallas y mejora instrucciones | Detecta algunas fallas | Acepta la salida sin revisar |
| Presentación | Clara, breve y orientada a decisión | Entendible pero extensa | Poco ejecutiva |

---

# 24. Agenda sugerida para 60 minutos

| Tiempo | Actividad |
|---:|---|
| 5 min | Introducción: de prompt a agente |
| 8 min | Diseño del agente: propósito, usuario, límites |
| 12 min | Configuración en Agent Builder o GPT |
| 10 min | Prueba con caso Evolutio |
| 10 min | Red team y revisión de calidad |
| 8 min | Mejora del agente |
| 7 min | Presentación rápida por grupo |

---

# 25. Agenda compacta para 40 minutos

| Tiempo | Actividad |
|---:|---|
| 5 min | Explicar objetivo del agente |
| 8 min | Diseñar instrucciones |
| 12 min | Crear o simular agente |
| 8 min | Probar con caso Evolutio |
| 5 min | Validar salida |
| 2 min | Cierre ejecutivo |

---

# 26. Guion para explicar antes del workshop

```text
En este ejercicio vamos a subir un nivel.

Hasta ahora hemos usado IA para crear entregables: reportes, riesgos, WBS, forecast, actas y comunicaciones. Ahora vamos a diseñar un asistente especializado.

La diferencia es importante. Un prompt resuelve una tarea puntual. Un agente bien diseñado resuelve una necesidad recurrente con instrucciones, límites, formatos, criterios de calidad y validación humana.

En una PMO, esto puede tener mucho valor porque los PMs suelen trabajar con información dispersa: actas, correos, issues, cronogramas, riesgos, dependencias y reportes semanales. El agente debe ayudar a consolidar esa información y convertirla en visibilidad ejecutiva.

Pero también hay riesgos. Un agente puede inventar datos, mezclar hechos con supuestos, recomendar acciones sin contexto o procesar información sensible. Por eso vamos a diseñarlo con controles.

El objetivo no es que el agente tome decisiones por nosotros. El objetivo es que prepare mejores insumos para que el PM, la PMO y el sponsor puedan decidir mejor.
```

---

# 27. Frases clave para reforzar en clase

> Un prompt resuelve una tarea; un agente resuelve un patrón recurrente de trabajo.

> Un agente útil para PMO no solo responde; estructura, prioriza, advierte y pide validación.

> La IA puede preparar el reporte, pero el PM sigue siendo responsable de enviarlo.

> La PMO aumentada no es la que automatiza todo; es la que mejora visibilidad, control y decisiones.

> El riesgo no está solo en usar IA. El riesgo está en usar IA sin diseño, sin límites y sin validación.

---

# 28. Cierre recomendado del workshop

```text
La principal conclusión de este ejercicio es que la IA puede pasar de ser una herramienta individual a convertirse en una capacidad de PMO.

Pero para que eso ocurra, necesitamos diseñarla bien:
- con propósito claro;
- con contexto de negocio;
- con datos adecuados;
- con límites explícitos;
- con criterios de calidad;
- con supervisión humana;
- con gobierno.

Un agente para PMs no debe reemplazar el juicio profesional. Debe ayudar a que el PM tenga mejor visibilidad, anticipe riesgos, prepare mejores decisiones y comunique con más claridad.
```

---

# 29. Mensaje final para el curso

> **El futuro de la gestión de proyectos no es solo usar IA para trabajar más rápido. Es diseñar capacidades aumentadas que permitan a los PMs y PMOs gestionar mejor la complejidad, anticipar riesgos y tomar decisiones más responsables.**
