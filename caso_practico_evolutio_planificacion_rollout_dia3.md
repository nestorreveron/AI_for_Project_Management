# Caso práctico Evolutio: planificación de rollout

## Slide 17 — Caso práctico Evolutio: planificación de rollout

Esta slide se puede usar como **caso práctico central del Día 3**. Aquí los alumnos dejan de hablar de IA en abstracto y la usan como Project Managers para analizar planificación, dependencias, riesgos, forecast y decisiones.

La lógica está alineada con buenas prácticas de gestión de proyectos: una WBS debe ayudar a definir entregables y estructurar el trabajo a gestionar, no limitarse a listar actividades sueltas. Además, la gestión de riesgos implica identificar, analizar y responder a riesgos durante el ciclo de vida del proyecto. En el uso de IA, la práctica **human-in-the-loop** es clave: la IA prepara, pero el PM valida, interpreta y decide.

---

## Explicación para leer en clase

Vamos a trabajar con un caso ficticio, pero muy cercano al tipo de proyectos tecnológicos que puede gestionar Evolutio.

Imaginemos que Evolutio debe planificar un **rollout tecnológico para un cliente enterprise**. Hay **12 intervenciones previstas**, **3 equipos técnicos compartidos**, **2 ventanas de cambio por semana**, información incompleta del cliente, **4 dependencias abiertas**, **3 issues activos** y un sponsor que pide un **forecast ejecutivo semanal**.

El reto del PM no es simplemente poner fechas en un cronograma. El reto es responder preguntas de gestión:

- ¿El plan es viable con solo dos ventanas de cambio por semana?
- ¿Qué dependencias pueden bloquear las intervenciones?
- ¿Qué información falta del cliente?
- ¿Qué riesgos impactan fecha, calidad, seguridad o experiencia del cliente?
- ¿Qué decisiones hay que escalar?
- ¿Qué escenario debemos comunicar al sponsor?

Aquí vamos a usar IA para preparar el análisis, pero no para delegar la responsabilidad. La IA nos ayuda a ordenar la información, detectar dependencias, identificar riesgos y preparar escenarios. El PM valida, prioriza y decide.

---

# Dinámica recomendada: 40 minutos

## Objetivo del ejercicio

Crear una **mini planificación asistida por IA** para el rollout, con foco en:

1. Dependencias críticas.
2. Riesgos principales.
3. Forecast con escenarios.
4. Decisiones para cliente, sponsor o PMO.
5. Recomendación ejecutiva del PM.

---

# Caso base para entregar a los alumnos

Puedes copiar esto y dárselo como contexto:

```text
Caso práctico: Planificación de rollout tecnológico — Evolutio

Evolutio debe planificar un rollout tecnológico para un cliente enterprise.

Datos del proyecto:
- 12 intervenciones planificadas.
- 3 equipos técnicos compartidos.
- 2 ventanas de cambio por semana.
- Información del cliente incompleta.
- 4 dependencias abiertas.
- 3 issues activos.
- Seguridad debe validar el uso de datos.
- La PMO requiere reporte semanal.
- El sponsor solicita forecast ejecutivo.

Supuestos iniciales:
- Las intervenciones deben ejecutarse en ventanas aprobadas por el cliente.
- Los equipos técnicos no están dedicados al 100%.
- Algunos datos del cliente todavía no están completos.
- Hay dependencias de aprobación, datos, seguridad y disponibilidad técnica.
- El proyecto debe mantener comunicación ejecutiva semanal.

Objetivo:
Preparar una revisión de planificación para determinar si el rollout puede mantenerse según el plan base o si requiere replanificación, escalamiento o priorización.
```

---

# Trabajo en equipos

Organiza grupos de **3 personas**.

## Roles sugeridos

### 1. PM líder

Guía el análisis, interpreta el resultado y decide qué se presenta.

### 2. Analista IA

Ejecuta el prompt, ajusta instrucciones y mejora la calidad de las respuestas.

### 3. Validador

Revisa supuestos, riesgos, owners, dependencias, calidad del resultado y posibles datos inventados.

Esto refuerza el concepto de **human-in-the-loop**:

> La IA prepara, pero el equipo valida.

---

# Actividad 1 — Detectar dependencias críticas

## Instrucción para los alumnos

Usen IA para identificar dependencias explícitas y ocultas del caso.

El objetivo es descubrir qué elementos pueden bloquear el avance del rollout aunque no aparezcan claramente en el cronograma.

---

## Prompt para compartir

```text
Actúa como Senior Project Manager en un proyecto tecnológico enterprise.

Analiza el siguiente caso de rollout tecnológico:

[pegar caso base]

Identifica dependencias explícitas y dependencias ocultas que podrían afectar fecha, calidad, coste, seguridad, operación o experiencia del cliente.

Clasifica cada dependencia por:
- Tipo: cliente, técnica, datos, seguridad, proveedor, aprobación, recursos o arquitectura.
- Impacto potencial.
- Urgencia: alta, media o baja.
- Owner sugerido.
- Pregunta de validación.
- Acción recomendada.

Restricciones:
- No inventes datos.
- Separa hechos confirmados de supuestos.
- Marca como supuesto todo lo que no esté confirmado.
- Indica qué información falta.
- Usa lenguaje claro para un Project Manager.

Entrega el resultado en una tabla con estas columnas:

Dependencia | Tipo | Evidencia | Impacto | Urgencia | Owner sugerido | Hecho o supuesto | Pregunta de validación | Acción recomendada
```

---

## Resultado esperado

Los alumnos deberían obtener algo parecido a esto:

| Dependencia | Tipo | Impacto | Acción PM |
|---|---|---|---|
| Confirmación de ventanas de cambio | Cliente | Puede retrasar intervenciones | Validar calendario con cliente |
| Datos incompletos del cliente | Datos | Puede afectar calidad del rollout | Solicitar dataset mínimo requerido |
| Validación de seguridad | Seguridad | Puede bloquear uso de datos | Escalar revisión con seguridad |
| Equipos técnicos compartidos | Recursos | Riesgo de solapamiento | Confirmar disponibilidad semanal |
| Aprobaciones pendientes | Aprobación | Puede bloquear ejecución | Definir responsable y fecha límite |

---

## Preguntas para discusión

- ¿Qué dependencia es más crítica?
- ¿Cuál depende directamente del cliente?
- ¿Cuál puede impactar seguridad o privacidad?
- ¿Cuál debería escalarse primero?
- ¿Qué dependencia no estaba explícita en el caso, pero aparece como supuesto razonable?

---

# Actividad 2 — Identificar riesgos del rollout

## Instrucción para los alumnos

Ahora usaremos las dependencias identificadas para crear un **registro inicial de riesgos**.

Aquí es importante diferenciar:

- **Riesgo:** algo que podría ocurrir.
- **Issue:** algo que ya está ocurriendo.

Ejemplo:

- Riesgo: “El cliente podría no confirmar las ventanas de cambio.”
- Issue: “Ya hay una ventana de cambio no confirmada para esta semana.”

---

## Prompt para compartir

```text
Actúa como Risk Manager de un proyecto tecnológico enterprise.

Con base en el caso de rollout de Evolutio y las dependencias identificadas, genera un registro inicial de riesgos.

Para cada riesgo incluye:
- Causa raíz.
- Evento de riesgo.
- Impacto.
- Probabilidad estimada: alta, media o baja.
- Impacto estimado: alto, medio o bajo.
- Nivel de riesgo resultante.
- Respuesta sugerida.
- Owner sugerido.
- Señales tempranas.
- Pregunta de validación.

Restricciones:
- No inventes datos.
- Diferencia riesgos de issues.
- Marca supuestos no confirmados.
- Usa lenguaje claro para PMO y sponsor.
- No generes alarmismo innecesario.
- Enfócate en riesgos que afecten fecha, calidad, seguridad, recursos o experiencia del cliente.

Entrega el resultado en una tabla.
```

---

## Resultado esperado

Ejemplos de riesgos esperados:

| Riesgo | Causa raíz | Impacto | Señal temprana |
|---|---|---|---|
| Retraso por ventanas no confirmadas | Dependencia del cliente | Impacto en fecha | Ventanas pendientes de aprobación |
| Baja calidad del reporting | Datos incompletos | Impacto en calidad | Información parcial o inconsistente |
| Sobrecarga de equipos técnicos | Recursos compartidos | Impacto en ejecución | Conflictos de disponibilidad |
| Bloqueo por validación de seguridad | Control pendiente | Impacto en cumplimiento | Revisión de seguridad no cerrada |
| Replanificación por cambios de alcance | Alcance no estabilizado | Impacto en coste y fecha | Solicitudes nuevas del cliente |

---

## Preguntas para discusión

- ¿Cuál es el riesgo más crítico?
- ¿Cuál debe convertirse en issue?
- ¿Qué riesgo requiere escalamiento?
- ¿Qué riesgo puede mitigarse con mejor planificación?
- ¿Qué riesgo depende de una decisión del cliente?

---

# Actividad 3 — Crear forecast con tres escenarios

## Instrucción para los alumnos

Ahora los equipos deben generar un forecast ejecutivo con tres escenarios:

### 1. Escenario optimista

Se resuelven las dependencias críticas y el plan puede mantenerse.

### 2. Escenario probable

Algunas dependencias se resuelven tarde y se requieren ajustes menores.

### 3. Escenario conservador

Persisten bloqueos, datos incompletos o aprobaciones pendientes, y se impacta el plan.

---

## Prompt para compartir

```text
Actúa como Senior Project Manager responsable de presentar forecast ejecutivo a sponsor y PMO.

Con base en el caso de rollout, las dependencias identificadas y los riesgos generados, crea un forecast con tres escenarios:

1. Optimista.
2. Probable.
3. Conservador.

Para cada escenario incluye:
- Supuestos clave.
- Impacto en fecha.
- Impacto en calidad.
- Impacto en recursos.
- Riesgos asociados.
- Decisión requerida.
- Recomendación del PM.
- Nivel de confianza: alto, medio o bajo.

Restricciones:
- No inventes fechas exactas.
- No ocultes riesgos relevantes.
- No generes alarmismo innecesario.
- Indica qué información falta para mejorar el forecast.
- Separa hechos confirmados de supuestos.
- Usa lenguaje ejecutivo para sponsor y PMO.

Entrega una tabla ejecutiva y luego un resumen de máximo 5 líneas para sponsor.
```

---

## Resultado esperado

| Escenario | Lectura PM | Decisión |
|---|---|---|
| Optimista | El rollout se mantiene si cliente confirma ventanas y datos | Mantener plan |
| Probable | Puede haber ajustes menores por dependencias abiertas | Replanificar parcialmente |
| Conservador | Riesgo alto de impacto en fecha si no se resuelven bloqueos | Escalar a sponsor |

---

## Ejemplo de resumen ejecutivo esperado

```text
El rollout mantiene viabilidad general, pero existen dependencias críticas asociadas a ventanas de cambio, datos del cliente y validación de seguridad. El escenario probable requiere replanificación parcial si las dependencias no se resuelven esta semana. Se recomienda escalar la confirmación de ventanas y priorizar la entrega de datos mínimos. El PM mantendrá seguimiento semanal con forecast actualizado. La decisión clave es confirmar si se mantiene el alcance completo o se prioriza una primera fase.
```

---

## Preguntas para discusión

- ¿Qué escenario es más realista?
- ¿Qué supuesto sostiene el escenario optimista?
- ¿Qué decisión mueve el proyecto del escenario conservador al probable?
- ¿Qué información falta para mejorar el forecast?
- ¿Cómo comunicaríamos esto sin generar alarma innecesaria?

---

# Actividad 4 — Preparar reunión de planificación

## Instrucción para los alumnos

Con las dependencias, riesgos y forecast, cada equipo debe preparar una **reunión de planificación de 45 minutos**.

El objetivo no es hacer una agenda genérica. El objetivo es que la reunión termine con:

- decisiones;
- responsables;
- fechas;
- riesgos priorizados;
- dependencias gestionadas;
- próximos pasos.

---

## Prompt para compartir

```text
Actúa como PM senior preparando una reunión de planificación de 45 minutos con cliente, equipos técnicos, PMO y sponsor.

Con base en el caso de rollout, dependencias, riesgos y forecast, crea una agenda de reunión.

La agenda debe incluir:
- Objetivo de la reunión.
- Participantes clave.
- Temas a revisar.
- Decisiones necesarias.
- Preguntas para el cliente.
- Riesgos críticos.
- Dependencias abiertas.
- Acciones esperadas.
- Cierre ejecutivo.

Restricciones:
- La reunión dura 45 minutos.
- Debe ser accionable.
- Debe evitar discusión genérica.
- Debe terminar con decisiones, owners y fechas.
- Usa lenguaje profesional y ejecutivo.
- No incluyas temas que no estén relacionados con planificación, riesgos, dependencias o forecast.

Entrega el resultado en formato agenda con tiempos.
```

---

## Resultado esperado

Ejemplo de agenda:

| Tiempo | Tema | Objetivo |
|---:|---|---|
| 5 min | Objetivo y estado general | Alinear contexto |
| 10 min | Dependencias abiertas | Validar bloqueos y owners |
| 10 min | Riesgos e impacto en cronograma | Priorizar riesgos críticos |
| 10 min | Forecast: optimista, probable, conservador | Revisar escenarios |
| 5 min | Decisiones requeridas | Confirmar decisiones clave |
| 5 min | Acciones, owners y fechas | Cerrar compromisos |

---

## Preguntas para discusión

- ¿Qué tema debe ir primero?
- ¿Qué decisión no puede salir sin owner?
- ¿Qué pregunta debe hacerse al cliente?
- ¿Qué riesgo se debe escalar?
- ¿Qué acción debe quedar documentada al final?

---

# Cierre del workshop — Conclusión ejecutiva

Al final, pide a cada grupo preparar una conclusión de máximo **5 líneas**.

## Prompt para conclusión ejecutiva

```text
Redacta una conclusión ejecutiva de máximo 5 líneas para sponsor y PMO.

Debe incluir:
- Estado general del rollout.
- Principal riesgo.
- Dependencia más crítica.
- Decisión requerida.
- Recomendación del PM.

Usa tono ejecutivo, claro y accionable.
No inventes información.
Separa hechos de supuestos cuando corresponda.
```

---

## Ejemplo de conclusión ejecutiva

```text
El rollout mantiene viabilidad general, pero existen dependencias críticas asociadas a ventanas de cambio, datos del cliente y validación de seguridad. El escenario probable requiere replanificación parcial si las dependencias no se resuelven esta semana. Se recomienda escalar la confirmación de ventanas y priorizar la entrega de datos mínimos. El PM mantendrá seguimiento semanal con forecast actualizado. La decisión clave es confirmar si se mantiene el alcance completo o se prioriza una primera fase.
```

---

# Checklist de validación para los alumnos

Antes de presentar, cada grupo debe validar:

- ¿Separaron hechos de supuestos?
- ¿Identificaron dependencias reales?
- ¿Asignaron owners sugeridos?
- ¿Incluyeron riesgos con señales tempranas?
- ¿Diferenciaron riesgos de issues?
- ¿El forecast tiene tres escenarios claros?
- ¿La recomendación es accionable?
- ¿Qué decisión debe tomar el cliente o sponsor?
- ¿Evitaron inventar información?
- ¿El lenguaje es ejecutivo y profesional?
- ¿La información sensible fue anonimizada?
- ¿El resultado se puede defender frente a cliente, sponsor o PMO?

---

# Estructura de presentación por equipo

Cada equipo puede presentar en **3 minutos**.

## 1. Lectura del caso

```text
Nuestro análisis parte de un rollout con 12 intervenciones, 3 equipos técnicos compartidos, 2 ventanas de cambio por semana, 4 dependencias abiertas y 3 issues activos.
```

## 2. Dependencia más crítica

```text
La dependencia más crítica identificada es la confirmación de ventanas de cambio por parte del cliente, porque puede impactar directamente la ejecución de las intervenciones.
```

## 3. Riesgo principal

```text
El principal riesgo es retraso del rollout por dependencias externas no resueltas, especialmente datos incompletos, aprobaciones pendientes y validación de seguridad.
```

## 4. Forecast

```text
El escenario probable indica necesidad de replanificación parcial si las dependencias no se resuelven en la próxima ventana de seguimiento.
```

## 5. Recomendación

```text
Recomendamos escalar la confirmación de ventanas, solicitar datos mínimos requeridos y cerrar validación de seguridad antes de comprometer nuevas fechas.
```

---

# Evaluación rápida del instructor

Puedes evaluar cada grupo con esta matriz:

| Criterio | Excelente | Aceptable | Mejorable |
|---|---|---|---|
| Dependencias | Claras, clasificadas y con owner | Identificadas, pero incompletas | Genéricas o sin owner |
| Riesgos | Tienen causa, impacto y señal temprana | Tienen impacto, pero poca causa | Son issues o están mal formulados |
| Forecast | Tres escenarios claros y defendibles | Escenarios presentes, pero poco diferenciados | Un solo escenario o sin supuestos |
| Recomendación | Ejecutiva y accionable | Clara, pero poco priorizada | Genérica |
| Validación | Separa hechos y supuestos | Algunos supuestos claros | Mezcla supuestos con hechos |
| Uso de IA | Buen prompt y revisión humana | Prompt útil, poca revisión | Resultado copiado sin validar |

---

# Frase para cerrar la actividad

> **El valor de la IA no está en generar una tabla bonita; está en ayudar al PM a convertir información dispersa en dependencias, riesgos, escenarios y decisiones accionables.**

---

# Fuentes de referencia

- PMI — Practice Standard for Work Breakdown Structures: https://www.pmi.org/standards/work-breakdown-structures-third-edition
- PMI — Work Breakdown Structure Basic Principles: https://www.pmi.org/learning/library/work-breakdown-structure-basic-principles-4883
- PMI — Human-in-the-Loop: What Project Managers Need to Know: https://www.pmi.org/blog/human-in-the-loop-what-project-managers-need-to-know
- PMI — Artificial Intelligence in Project Management: https://www.pmi.org/learning/ai-in-project-management
