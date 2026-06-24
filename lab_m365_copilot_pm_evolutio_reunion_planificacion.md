# Lab práctico — Microsoft 365 Copilot para PMs de Evolutio

## Preparación de reunión de planificación y seguimiento de rollout

### Curso
**AI for Project Management — Día 3**  
**Tema:** IA para planificación, dependencias, cronogramas, forecast y toma de decisiones.

---

# 1. Propósito del lab

Este ejercicio está diseñado para Project Managers de Evolutio que ya trabajan con herramientas del ecosistema Microsoft 365 y quieren usar **Microsoft 365 Copilot** para mejorar su preparación antes de reuniones de planificación, seguimiento o comité.

El objetivo no es usar IA para reemplazar el criterio del PM, sino para ayudar a:

- consolidar información dispersa;
- preparar reuniones más efectivas;
- identificar acciones pendientes;
- detectar riesgos y dependencias;
- preparar mensajes ejecutivos;
- mejorar el seguimiento de decisiones;
- reducir ambigüedad antes de reunirse con cliente, sponsor o equipos técnicos.

**Mensaje central del lab:**

> Microsoft 365 Copilot ayuda al PM a trabajar mejor sobre el contexto corporativo; el PM sigue siendo responsable de validar, priorizar, decidir y comunicar.

---

# 2. Herramienta principal

## Microsoft 365 Copilot

Usaremos Microsoft 365 Copilot porque el ejercicio se enfoca en información típica del día a día de un PM:

- reuniones de Teams;
- correos de Outlook;
- documentos de Word;
- presentaciones de PowerPoint;
- archivos de Excel;
- documentos almacenados en SharePoint o OneDrive;
- notas y minutas;
- acciones pendientes;
- decisiones tomadas;
- reportes de seguimiento.

Microsoft 365 Copilot es especialmente útil cuando necesitamos trabajar con información que ya existe dentro del entorno Microsoft 365 de la organización.

---

# 3. Caso práctico del lab

## Caso: reunión de planificación de rollout tecnológico

Evolutio está gestionando un rollout tecnológico para un cliente enterprise.

El PM debe preparar una reunión de planificación y seguimiento con:

- cliente;
- equipos técnicos;
- PMO;
- sponsor;
- equipo de seguridad;
- posibles proveedores.

## Contexto ficticio del proyecto

```text
Proyecto: Rollout tecnológico enterprise

Situación actual:
- Hay 12 intervenciones planificadas.
- Existen 3 equipos técnicos compartidos.
- Solo hay 2 ventanas de cambio disponibles por semana.
- La información del cliente está parcialmente incompleta.
- Hay 4 dependencias abiertas.
- Hay 3 issues activos.
- Seguridad debe validar el uso de ciertos datos.
- La PMO solicita un reporte semanal.
- El sponsor quiere un forecast ejecutivo.

Reto del PM:
Preparar una reunión de planificación de 45 minutos que permita revisar estado, dependencias, riesgos, decisiones pendientes y próximos pasos.
```

---

# 4. Objetivos del ejercicio

Al finalizar el lab, cada grupo deberá producir:

1. Una agenda ejecutiva de reunión.
2. Un resumen de estado del proyecto.
3. Una lista de acciones pendientes.
4. Una lista de decisiones tomadas y decisiones pendientes.
5. Una matriz simple de dependencias y riesgos.
6. Un correo ejecutivo de seguimiento.
7. Un checklist de validación humana antes de enviar el resultado.

---

# 5. Duración sugerida

**Duración total:** 45 a 60 minutos

| Fase | Tiempo sugerido |
|---|---:|
| Introducción del caso | 5 min |
| Preparación de contexto en Copilot | 10 min |
| Generación de agenda y resumen | 10 min |
| Identificación de acciones, riesgos y decisiones | 15 min |
| Redacción de correo ejecutivo | 10 min |
| Discusión y cierre | 10 min |

---

# 6. Organización de equipos

Trabajar en grupos de **3 personas**.

## Roles sugeridos

### 1. PM líder

Responsable de interpretar el resultado, decidir qué se usa y preparar la conclusión.

### 2. Operador de Copilot

Responsable de ejecutar los prompts en Microsoft 365 Copilot, ajustar instrucciones y refinar la salida.

### 3. Validador de calidad

Responsable de revisar:

- si Copilot inventó información;
- si hay supuestos no validados;
- si las acciones tienen responsable;
- si las decisiones están claras;
- si el lenguaje es adecuado para cliente o sponsor.

---

# 7. Preparación previa del instructor

Antes de ejecutar el lab, el instructor puede preparar tres documentos ficticios para que los alumnos los usen en Microsoft 365 Copilot.

## Documento 1 — Acta de reunión anterior

```text
Acta de reunión — Seguimiento rollout tecnológico

Fecha: 20 de junio
Participantes: PM Evolutio, equipo técnico, representante cliente, seguridad, PMO

Puntos discutidos:
- El cliente aún no ha entregado la lista completa de sedes/intervenciones.
- Se mantienen 12 intervenciones planificadas.
- Hay disponibilidad limitada de ventanas de cambio: 2 por semana.
- Seguridad solicita revisar el uso de datos antes de iniciar pruebas.
- El equipo técnico indica que comparte recursos con otros proyectos.
- Se identifican 3 issues activos relacionados con datos incompletos, accesos pendientes y validación de entorno.

Decisiones tomadas:
- Mantener el plan base hasta nueva revisión.
- Solicitar al cliente confirmación de ventanas para las próximas dos semanas.
- Preparar forecast para sponsor.

Acciones:
- Cliente debe enviar información faltante de sedes antes del viernes.
- Seguridad debe confirmar criterios de validación de datos.
- PM debe preparar agenda de reunión de planificación.
- Equipo técnico debe confirmar disponibilidad de recursos.
```

---

## Documento 2 — Lista de issues

```text
Issues activos del proyecto

Issue 1: Datos incompletos del cliente
Descripción: falta información de varias sedes/intervenciones.
Impacto: puede afectar planificación y calidad del rollout.
Estado: abierto.
Owner sugerido: cliente.

Issue 2: Accesos técnicos pendientes
Descripción: algunos accesos necesarios para validación no están habilitados.
Impacto: puede retrasar pruebas técnicas.
Estado: abierto.
Owner sugerido: equipo técnico y cliente.

Issue 3: Validación de seguridad pendiente
Descripción: seguridad debe validar el uso de ciertos datos antes de avanzar.
Impacto: puede bloquear actividades de prueba y reporting.
Estado: abierto.
Owner sugerido: seguridad.
```

---

## Documento 3 — Cronograma resumido

```text
Cronograma resumido del rollout

Semana 1:
- Validar información del cliente.
- Confirmar ventanas de cambio.
- Revisar accesos técnicos.

Semana 2:
- Ejecutar primeras intervenciones.
- Validar resultados iniciales.
- Preparar reporte PMO.

Semana 3:
- Continuar intervenciones.
- Revisar riesgos y dependencias.
- Preparar forecast para sponsor.

Semana 4:
- Cerrar intervenciones principales.
- Consolidar lecciones aprendidas.
- Preparar informe final.
```

---

# 8. Lab 1 — Preparar contexto con Microsoft 365 Copilot

## Objetivo

Usar Copilot para consolidar la información disponible antes de preparar la reunión.

## Instrucción para alumnos

En Microsoft 365 Copilot, usen los documentos disponibles del proyecto o peguen el contexto ficticio proporcionado por el instructor.

## Prompt sugerido

```text
Actúa como asistente de Project Manager.

Con base en la información disponible del proyecto de rollout tecnológico, resume el estado actual del proyecto.

Identifica:
1. Estado general.
2. Puntos abiertos.
3. Acciones pendientes.
4. Decisiones tomadas.
5. Decisiones pendientes.
6. Riesgos visibles.
7. Dependencias críticas.
8. Información faltante.

No inventes datos.
Separa hechos confirmados de supuestos.
Usa lenguaje claro y profesional.
```

## Resultado esperado

Copilot debería producir un resumen estructurado como este:

| Categoría | Resultado esperado |
|---|---|
| Estado general | Rollout en planificación con dependencias abiertas |
| Acciones pendientes | Cliente debe enviar datos; seguridad debe validar; equipo técnico debe confirmar recursos |
| Decisiones tomadas | Mantener plan base hasta nueva revisión |
| Decisiones pendientes | Confirmar ventanas, validar datos, aprobar forecast |
| Riesgos visibles | Datos incompletos, accesos pendientes, seguridad no validada |
| Información faltante | Detalle completo de sedes, calendario confirmado, disponibilidad de recursos |

## Preguntas para discusión

- ¿Copilot distinguió hechos de supuestos?
- ¿Identificó correctamente las acciones pendientes?
- ¿Faltó algún riesgo importante?
- ¿El resumen es útil para preparar una reunión real?

---

# 9. Lab 2 — Crear agenda de reunión de planificación

## Objetivo

Generar una agenda accionable para una reunión de 45 minutos.

## Prompt sugerido

```text
Actúa como Senior Project Manager.

Con base en el estado del proyecto, prepara una agenda para una reunión de planificación de 45 minutos con cliente, PMO, equipos técnicos, seguridad y sponsor.

La agenda debe incluir:
- objetivo de la reunión;
- participantes clave;
- temas a revisar;
- decisiones necesarias;
- preguntas para el cliente;
- riesgos a discutir;
- dependencias abiertas;
- acciones esperadas;
- cierre con owners y fechas.

Restricciones:
- La reunión no debe ser genérica.
- Debe enfocarse en decisiones y desbloqueos.
- Debe cerrar con acciones claras.
- No inventes información.

Entrega la agenda en formato de tabla con tiempo, tema, objetivo y resultado esperado.
```

## Resultado esperado

| Tiempo | Tema | Objetivo | Resultado esperado |
|---:|---|---|---|
| 5 min | Estado general | Alinear contexto | Todos entienden situación actual |
| 10 min | Dependencias abiertas | Revisar bloqueos | Dependencias priorizadas |
| 10 min | Riesgos principales | Evaluar impacto | Riesgos con acción definida |
| 10 min | Forecast | Revisar escenarios | Escenario probable validado |
| 5 min | Decisiones | Confirmar decisiones necesarias | Decisiones asignadas |
| 5 min | Cierre | Owners y fechas | Próximos pasos claros |

## Preguntas para discusión

- ¿La agenda ayuda a tomar decisiones?
- ¿Hay temas innecesarios?
- ¿Faltan participantes clave?
- ¿La reunión termina con owners y fechas?

---

# 10. Lab 3 — Extraer acciones pendientes y decisiones

## Objetivo

Usar Copilot para separar acciones, decisiones y temas abiertos.

## Prompt sugerido

```text
Analiza la información del proyecto y genera una tabla con:

1. Acciones pendientes.
2. Responsable sugerido.
3. Fecha objetivo si aparece en la información.
4. Impacto si no se completa.
5. Estado: abierto, en progreso o pendiente de validación.
6. Pregunta de seguimiento.

Luego genera otra tabla con:

1. Decisiones tomadas.
2. Decisiones pendientes.
3. Quién debe decidir.
4. Información necesaria para decidir.
5. Impacto si la decisión se retrasa.

No inventes responsables ni fechas.
Si algo no está confirmado, márcalo como supuesto o información faltante.
```

## Resultado esperado — Acciones

| Acción | Responsable sugerido | Fecha objetivo | Impacto si no se completa | Estado | Pregunta de seguimiento |
|---|---|---|---|---|---|
| Enviar información faltante de sedes | Cliente | Viernes | Retraso en planificación | Abierto | ¿Qué sedes faltan? |
| Confirmar criterios de seguridad | Seguridad | No indicada | Bloqueo de pruebas | Abierto | ¿Qué criterios aplican? |
| Confirmar disponibilidad técnica | Equipo técnico | No indicada | Riesgo de solapamiento | Abierto | ¿Qué recursos están disponibles? |

## Resultado esperado — Decisiones

| Decisión | Estado | Responsable sugerido | Información necesaria | Impacto si se retrasa |
|---|---|---|---|---|
| Mantener plan base | Tomada | PM / PMO | Seguimiento semanal | Bajo |
| Confirmar ventanas próximas | Pendiente | Cliente | Calendario de ventanas | Alto |
| Validar uso de datos | Pendiente | Seguridad | Criterios de seguridad | Alto |

## Preguntas para discusión

- ¿Qué acción es más urgente?
- ¿Qué decisión debe escalarse?
- ¿Hay responsables inventados?
- ¿Qué información falta para cerrar decisiones?

---

# 11. Lab 4 — Generar matriz de riesgos y dependencias

## Objetivo

Convertir información de reuniones, issues y cronograma en una matriz simple de riesgos y dependencias.

## Prompt sugerido

```text
Con base en la información del proyecto, genera una matriz de riesgos y dependencias para el PM.

Primero identifica dependencias críticas:
- dependencia;
- tipo: cliente, técnica, datos, seguridad, recursos, aprobación o proveedor;
- impacto;
- urgencia;
- owner sugerido;
- pregunta de validación;
- acción recomendada.

Luego identifica riesgos:
- riesgo;
- causa;
- impacto;
- probabilidad estimada: alta, media o baja;
- nivel de riesgo: alto, medio o bajo;
- señal temprana;
- respuesta sugerida.

Restricciones:
- No inventes información.
- Diferencia riesgos de issues.
- Marca supuestos.
- Usa lenguaje ejecutivo y accionable.
```

## Resultado esperado — Dependencias

| Dependencia | Tipo | Impacto | Urgencia | Owner sugerido | Acción recomendada |
|---|---|---|---|---|---|
| Confirmación de ventanas | Cliente | Impacto en fecha | Alta | Cliente | Validar calendario |
| Datos completos de sedes | Datos | Impacto en calidad | Alta | Cliente | Solicitar información mínima |
| Validación de seguridad | Seguridad | Bloqueo de pruebas | Alta | Seguridad | Escalar criterios |
| Disponibilidad técnica | Recursos | Riesgo de solapamiento | Media | Equipo técnico | Confirmar capacidad |

## Resultado esperado — Riesgos

| Riesgo | Causa | Impacto | Probabilidad | Nivel | Señal temprana | Respuesta |
|---|---|---|---|---|---|---|
| Retraso de rollout | Ventanas no confirmadas | Fecha | Media | Alto | Calendario no validado | Escalar confirmación |
| Baja calidad de planificación | Datos incompletos | Calidad | Alta | Alto | Faltan sedes | Solicitar datos mínimos |
| Bloqueo por seguridad | Validación pendiente | Fecha / cumplimiento | Media | Alto | Criterios no definidos | Reunión con seguridad |

## Preguntas para discusión

- ¿Qué dependencia tiene mayor impacto?
- ¿Qué riesgo debe escalarse primero?
- ¿Qué riesgo es realmente un issue?
- ¿Qué respuesta es más adecuada: mitigar, transferir, aceptar o escalar?

---

# 12. Lab 5 — Preparar correo ejecutivo de seguimiento

## Objetivo

Transformar la información del proyecto en un correo claro, ejecutivo y accionable.

## Prompt sugerido

```text
Actúa como Project Manager senior.

Redacta un correo ejecutivo de seguimiento para cliente, sponsor y PMO.

El correo debe incluir:
- estado general del rollout;
- principales avances;
- dependencias abiertas;
- riesgos principales;
- decisiones requeridas;
- acciones con owner;
- próximos pasos.

Tono:
- profesional;
- claro;
- ejecutivo;
- sin alarmismo innecesario;
- orientado a decisiones.

Restricciones:
- No inventes información.
- No incluyas datos sensibles.
- Marca como pendiente lo que no esté confirmado.
- No culpes al cliente ni a equipos internos.
- Mantén el correo breve.
```

## Resultado esperado

```text
Asunto: Seguimiento rollout tecnológico — dependencias, riesgos y próximos pasos

Hola equipo,

Compartimos el estado actualizado del rollout tecnológico. El proyecto mantiene el plan base en revisión, aunque existen dependencias críticas que deben cerrarse para proteger la planificación de las próximas intervenciones.

Principales puntos abiertos:
- Confirmación de ventanas de cambio por parte del cliente.
- Entrega de información faltante de sedes/intervenciones.
- Validación de criterios de seguridad para el uso de datos.
- Confirmación de disponibilidad de equipos técnicos compartidos.

Riesgos principales:
- Posible impacto en fechas si las ventanas no se confirman oportunamente.
- Riesgo de baja calidad de planificación si los datos del cliente permanecen incompletos.
- Posible bloqueo de pruebas si la validación de seguridad no se completa.

Decisiones requeridas:
- Confirmar calendario de ventanas para las próximas dos semanas.
- Validar información mínima necesaria para continuar.
- Confirmar si se mantiene el plan base o si se requiere replanificación parcial.

Próximos pasos:
- Cliente confirma información pendiente.
- Seguridad valida criterios de uso de datos.
- Equipo técnico confirma disponibilidad.
- PM actualiza forecast ejecutivo para la PMO y sponsor.

Gracias,
[Nombre del PM]
```

## Preguntas para discusión

- ¿El correo es claro para sponsor?
- ¿Evita lenguaje acusatorio?
- ¿Incluye decisiones concretas?
- ¿Se entiende qué debe pasar después?

---

# 13. Lab 6 — Validación humana del resultado

## Objetivo

Revisar el contenido generado por Copilot antes de usarlo en un contexto real.

## Checklist de validación

Antes de enviar cualquier resultado generado con IA, el PM debe revisar:

- ¿El resultado está basado en información real?
- ¿Hay datos inventados?
- ¿Se separaron hechos de supuestos?
- ¿Las acciones tienen owner?
- ¿Las decisiones pendientes están claras?
- ¿Los riesgos están correctamente formulados?
- ¿Se diferencian riesgos de issues?
- ¿El tono es adecuado para cliente o sponsor?
- ¿Hay información confidencial que deba eliminarse?
- ¿El correo o reporte puede defenderse en comité?

## Prompt de validación

```text
Revisa el siguiente resultado como PM senior antes de enviarlo a cliente, sponsor o PMO.

Evalúa:
1. Claridad.
2. Precisión.
3. Riesgo de información inventada.
4. Supuestos no validados.
5. Datos sensibles.
6. Tono ejecutivo.
7. Acciones sin owner.
8. Decisiones poco claras.
9. Riesgos mal formulados.
10. Mejoras recomendadas.

Entrega una tabla con:
- Hallazgo.
- Impacto.
- Corrección recomendada.
```

---

# 14. Entregable final del grupo

Cada equipo debe entregar o presentar:

1. Agenda de reunión.
2. Top 5 dependencias.
3. Top 5 riesgos.
4. Tabla de decisiones pendientes.
5. Correo ejecutivo de seguimiento.
6. Checklist de validación aplicado.

---

# 15. Presentación rápida por equipo

Cada grupo tendrá **3 minutos** para presentar:

## 1. Estado del proyecto

```text
El rollout mantiene viabilidad general, pero existen dependencias abiertas que pueden afectar la planificación de las próximas intervenciones.
```

## 2. Dependencia más crítica

```text
La dependencia más crítica es la confirmación de ventanas de cambio por parte del cliente, porque condiciona la ejecución de las intervenciones planificadas.
```

## 3. Riesgo principal

```text
El principal riesgo es impacto en fecha y calidad si la información del cliente y la validación de seguridad no se completan a tiempo.
```

## 4. Decisión requerida

```text
La decisión clave es confirmar si se mantiene el plan base o si se requiere replanificación parcial.
```

## 5. Recomendación

```text
Recomendamos cerrar las dependencias críticas antes de comprometer nuevas fechas y mantener un forecast ejecutivo semanal para sponsor y PMO.
```

---

# 16. Matriz de evaluación del instructor

| Criterio | Excelente | Aceptable | Mejorable |
|---|---|---|---|
| Uso de Copilot | Prompts claros, iteración y validación | Uso básico con resultado útil | Copia directa sin revisión |
| Agenda | Orientada a decisiones | Tiene estructura, pero poca priorización | Genérica |
| Dependencias | Claras, clasificadas y accionables | Identificadas, pero incompletas | Confusas o sin owner |
| Riesgos | Bien formulados con causa e impacto | Riesgos útiles, pero poco priorizados | Mezcla riesgos con issues |
| Correo ejecutivo | Claro, breve y accionable | Correcto, pero poco ejecutivo | Largo o ambiguo |
| Validación humana | Detecta supuestos y datos sensibles | Revisión parcial | Sin revisión crítica |

---

# 17. Variantes del ejercicio

## Variante 1 — Usando Teams

Si los alumnos tienen acceso a una reunión grabada o transcrita:

```text
Resume esta reunión e identifica decisiones, acciones, riesgos, bloqueos y preguntas pendientes para la próxima reunión de planificación.
```

## Variante 2 — Usando Outlook

Si tienen correos del proyecto:

```text
Resume los correos recientes relacionados con este proyecto. Identifica acuerdos, acciones pendientes, riesgos, decisiones y temas que requieren seguimiento.
```

## Variante 3 — Usando Word

Si tienen actas o documentos del proyecto:

```text
Analiza este documento y extrae información útil para preparar una reunión de planificación: alcance, entregables, dependencias, riesgos, decisiones y datos faltantes.
```

## Variante 4 — Usando Excel

Si tienen lista de tareas o issues:

```text
Analiza esta tabla e identifica tareas vencidas, acciones sin owner, dependencias abiertas, riesgos de fecha y prioridades para seguimiento.
```

---

# 18. Reglas de seguridad para el lab

Antes de usar Copilot o cualquier herramienta de IA, recordar:

- No pegar información confidencial en herramientas no aprobadas.
- No compartir datos personales innecesarios.
- No incluir credenciales, IPs, contratos, precios o información sensible.
- No usar datos reales del cliente si no están autorizados.
- Anonimizar nombres, sistemas y datos sensibles cuando sea necesario.
- Validar siempre la salida antes de enviarla.
- No asumir que una respuesta bien redactada es automáticamente correcta.

---

# 19. Cierre del lab

## Mensaje final para los alumnos

> El valor de Microsoft 365 Copilot para un PM no está solo en resumir reuniones o redactar correos. El verdadero valor está en convertir información dispersa en acciones, riesgos, decisiones y conversaciones mejor preparadas.

## Frase de cierre

> Copilot prepara el contexto; el PM dirige la conversación y asume la responsabilidad de la decisión.
