
# Workshop Avanzado: Digital Twin para PMO y Decision Intelligence

**Curso:** AI for Project Management II  
**Audiencia:** Project Managers, PMO Leads, Service Managers, Delivery Managers y líderes de transformación  
**Contexto:** Evolutio / Evolution — Servicios gestionados, proyectos cloud, operación SOC/NOC, SLAs y clientes enterprise  
**Duración sugerida:** 45–60 minutos  
**Formato:** Trabajo en grupos + simulación con IA + presentación ejecutiva  

---

## 1. Objetivo del workshop

Diseñar un **Digital Twin de PMO** capaz de simular decisiones antes de ejecutarlas, con foco en:

- Reasignación de recursos críticos.
- Riesgo de incumplimiento de SLA.
- Priorización de clientes y servicios.
- Impacto en cronograma, capacidad y operación.
- Governance, trazabilidad y accountability.

El objetivo no es construir técnicamente un Digital Twin completo, sino entender cómo un PM Senior puede usar este concepto para mejorar decisiones ejecutivas.

---

## 2. Concepto base

Un **Digital Twin** es una representación digital dinámica de un sistema real que se actualiza con datos operativos y permite observar, diagnosticar, predecir, simular y optimizar decisiones.

En una PMO, el “sistema real” no es una máquina física. Es el ecosistema de proyectos, personas, tickets, SLAs, clientes, riesgos, dependencias y decisiones.

Por eso, un Digital Twin de PMO puede responder preguntas como:

- ¿Qué ocurre si movemos tres ingenieros de un cliente a otro?
- ¿Qué SLA queda en riesgo si retrasamos una ventana de cambio?
- ¿Qué proyecto se impacta si un proveedor se retrasa cinco días?
- ¿Qué cliente debe priorizarse si tenemos capacidad limitada?
- ¿Qué escenario reduce más riesgo con menor impacto en el portafolio?

---

## 3. Diferencia entre Dashboard, Forecast y Digital Twin

| Capacidad | Pregunta que responde | Ejemplo |
|---|---|---|
| Dashboard | ¿Qué pasó o qué está pasando? | Tickets abiertos, avance del proyecto, SLA actual |
| Forecast | ¿Qué podría pasar? | Probabilidad de incumplimiento de SLA en 10 días |
| Digital Twin | ¿Qué pasaría si tomamos una decisión? | Simular mover recursos, cambiar prioridad o retrasar go-live |

**Idea clave:**  
Un dashboard informa.  
Un forecast anticipa.  
Un Digital Twin permite probar decisiones antes de ejecutarlas.

---

## 4. Caso de estudio

Evolutio gestiona servicios cloud y ciberseguridad para varios clientes enterprise.

Durante una semana crítica, el **Cliente B** reporta una brecha de ciberseguridad que requiere atención urgente. El equipo propone reasignar ingenieros de ciberseguridad desde el **Cliente A**, pero esa decisión podría afectar SLAs, backlog y satisfacción del cliente.

La PMO debe decidir entre tres escenarios:

1. Mover 3 ingenieros del Cliente A al Cliente B por 3 días.
2. Mover 2 ingenieros y contratar soporte externo temporal.
3. No mover recursos y mantener la asignación actual.

---

## 5. Datos ficticios del entorno

### 5.1 Clientes

| Cliente | Tipo | Criticidad | SLA contractual | Penalidad por incumplimiento |
|---|---|---:|---:|---:|
| Cliente A | Cloud Managed Services | Alta | 99.5% | Media |
| Cliente B | Cybersecurity Managed Services | Crítica | 99.9% | Alta |
| Cliente C | Cloud Migration Program | Media | 98.5% | Baja |

---

### 5.2 Estado actual de capacidad

| Equipo | Capacidad semanal total | Capacidad comprometida | Capacidad libre |
|---|---:|---:|---:|
| Cloud Engineering | 400 h | 340 h | 60 h |
| Cybersecurity | 300 h | 285 h | 15 h |
| SOC/NOC | 500 h | 430 h | 70 h |
| PMO | 160 h | 130 h | 30 h |

---

### 5.3 Ingenieros disponibles

| Recurso | Skill principal | Cliente actual | Utilización | Puede reasignarse |
|---|---|---|---:|---|
| Engineer 1 | Cybersecurity Senior | Cliente A | 90% | Sí |
| Engineer 2 | Cybersecurity Senior | Cliente A | 85% | Sí |
| Engineer 3 | Cybersecurity Mid | Cliente A | 80% | Sí |
| Engineer 4 | SOC Analyst | Cliente B | 95% | No |
| Engineer 5 | Cloud Security | Cliente C | 75% | Parcial |

---

### 5.4 Estado de tickets

| Cliente | P1 abiertos | P2 abiertos | P3 abiertos | Tendencia 7 días |
|---|---:|---:|---:|---|
| Cliente A | 1 | 6 | 18 | Estable |
| Cliente B | 4 | 9 | 22 | En aumento |
| Cliente C | 0 | 3 | 15 | Estable |

---

### 5.5 Riesgo inicial

| Cliente | Riesgo actual de SLA | Riesgo reputacional | Riesgo operativo |
|---|---:|---:|---:|
| Cliente A | 15% | Medio | Medio |
| Cliente B | 80% | Alto | Crítico |
| Cliente C | 10% | Bajo | Bajo |

---

## 6. Escenarios a simular

### Escenario 1 — Mover 3 ingenieros

| Variable | Resultado estimado |
|---|---:|
| Riesgo SLA Cliente B | Baja de 80% a 35% |
| Riesgo SLA Cliente A | Sube de 15% a 42% |
| Costo adicional | 0% |
| Riesgo reputacional Cliente B | Baja significativamente |
| Riesgo reputacional Cliente A | Sube moderadamente |
| Complejidad operativa | Alta |

---

### Escenario 2 — Mover 2 ingenieros + soporte externo

| Variable | Resultado estimado |
|---|---:|
| Riesgo SLA Cliente B | Baja de 80% a 45% |
| Riesgo SLA Cliente A | Sube de 15% a 25% |
| Costo adicional | 12% |
| Riesgo reputacional Cliente B | Baja |
| Riesgo reputacional Cliente A | Bajo-moderado |
| Complejidad operativa | Media |

---

### Escenario 3 — No mover recursos

| Variable | Resultado estimado |
|---|---:|
| Riesgo SLA Cliente B | Se mantiene en 80% |
| Riesgo SLA Cliente A | Se mantiene en 15% |
| Costo adicional | 0% |
| Riesgo reputacional Cliente B | Muy alto |
| Riesgo reputacional Cliente A | Bajo |
| Complejidad operativa | Baja |

---

## 7. Modelo de scoring del Digital Twin

Cada grupo debe evaluar los tres escenarios usando esta fórmula:

```text
Score total =
(Reducción de riesgo Cliente B x 30%) +
(Protección SLA Cliente A x 20%) +
(Impacto reputacional x 20%) +
(Factibilidad operativa x 15%) +
(Control de costo x 10%) +
(Gobernanza y trazabilidad x 5%)
```

Escala sugerida:

| Puntuación | Interpretación |
|---:|---|
| 1 | Muy débil |
| 2 | Débil |
| 3 | Aceptable |
| 4 | Fuerte |
| 5 | Muy fuerte |

---

## 8. Tabla de trabajo para los grupos

| Criterio | Peso | Escenario 1 | Escenario 2 | Escenario 3 |
|---|---:|---:|---:|---:|
| Reducción de riesgo Cliente B | 30% |  |  |  |
| Protección SLA Cliente A | 20% |  |  |  |
| Impacto reputacional | 20% |  |  |  |
| Factibilidad operativa | 15% |  |  |  |
| Control de costo | 10% |  |  |  |
| Gobernanza y trazabilidad | 5% |  |  |  |
| **Score total** | **100%** |  |  |  |

---

## 9. Decisión ejecutiva esperada

Cada grupo debe recomendar una de estas decisiones:

- **Go:** ejecutar el escenario propuesto inmediatamente.
- **Conditional Go:** ejecutar con condiciones, controles y aprobaciones.
- **No-Go:** no ejecutar hasta tener datos o controles adicionales.
- **Escalar:** llevar la decisión al Sponsor, Service Owner o AI Governance Board.

---

## 10. Preguntas guía

1. ¿Qué escenario reduce más el riesgo crítico?
2. ¿Qué escenario protege mejor el portafolio completo?
3. ¿Cuál es el costo de no actuar?
4. ¿Cuál es el costo de actuar demasiado agresivamente?
5. ¿Qué datos faltan para decidir con más confianza?
6. ¿Quién debe aprobar la decisión?
7. ¿Qué evidencia debe quedar registrada?
8. ¿Qué control evitaría una decisión automatizada incorrecta?

---

## 11. Prompt para usar con IA

```text
Actúa como PMO Digital Twin Advisor para una empresa de servicios gestionados.

Debes evaluar tres escenarios de reasignación de recursos entre clientes enterprise.

Contexto:
Cliente B tiene una brecha crítica de ciberseguridad.
Cliente A tiene servicios cloud gestionados con SLA contractual.
La PMO debe decidir si reasigna ingenieros del Cliente A al Cliente B.

Datos:
Cliente A:
- Riesgo SLA actual: 15%
- Riesgo reputacional: medio
- Penalidad contractual: media

Cliente B:
- Riesgo SLA actual: 80%
- Riesgo reputacional: alto
- Penalidad contractual: alta
- Brecha crítica de seguridad activa

Escenario 1:
Mover 3 ingenieros del Cliente A al Cliente B por 3 días.
- Riesgo SLA Cliente B baja a 35%
- Riesgo SLA Cliente A sube a 42%
- Costo adicional: 0%
- Complejidad operativa: alta

Escenario 2:
Mover 2 ingenieros y contratar soporte externo temporal.
- Riesgo SLA Cliente B baja a 45%
- Riesgo SLA Cliente A sube a 25%
- Costo adicional: 12%
- Complejidad operativa: media

Escenario 3:
No mover recursos.
- Riesgo SLA Cliente B se mantiene en 80%
- Riesgo SLA Cliente A se mantiene en 15%
- Costo adicional: 0%
- Complejidad operativa: baja

Evalúa los escenarios usando estos criterios:
- Reducción de riesgo Cliente B
- Protección SLA Cliente A
- Impacto reputacional
- Factibilidad operativa
- Control de costo
- Gobernanza y trazabilidad

Entrega:
1. Tabla comparativa.
2. Recomendación ejecutiva.
3. Decisión sugerida: Go, Conditional Go, No-Go o Escalar.
4. Principales riesgos.
5. Controles de gobernanza requeridos.
6. Evidencia que debe conservarse.
7. Mensaje ejecutivo para el sponsor en máximo 200 palabras.
```

---

## 12. Prompt avanzado: diseño del Digital Twin

```text
Actúa como AI Solution Architect y PMO Transformation Lead.

Diseña un Digital Twin de PMO para una empresa de servicios gestionados.

El Digital Twin debe permitir simular:
- Reasignación de recursos.
- Riesgo de incumplimiento de SLA.
- Impacto en clientes.
- Capacidad disponible.
- Priorización de incidentes.
- Impacto financiero.
- Escenarios Go/No-Go.

Incluye:
1. Fuentes de datos necesarias.
2. Modelo conceptual.
3. Variables principales.
4. Reglas de simulación.
5. Métricas de salida.
6. Controles de gobernanza.
7. Roles y responsabilidades.
8. Riesgos del modelo.
9. Roadmap de implementación en 90 días.
10. Primer piloto recomendado.
```

---

## 13. Governance checklist

Antes de ejecutar una recomendación del Digital Twin, la PMO debe validar:

| Control | Pregunta |
|---|---|
| Fuentes autorizadas | ¿Los datos vienen de sistemas oficiales? |
| Calidad de datos | ¿Los datos están actualizados y completos? |
| Supuestos visibles | ¿El modelo muestra sus supuestos? |
| Human-in-the-loop | ¿Un responsable humano aprueba la decisión? |
| Trazabilidad | ¿Queda registro de escenario, recomendación y decisión? |
| Impacto | ¿Se evaluó el impacto en clientes y SLAs? |
| Riesgo | ¿Se documentaron riesgos residuales? |
| Auditoría | ¿La decisión puede explicarse posteriormente? |

---

## 14. Conexión con frameworks

| Framework | Aplicación en el Digital Twin |
|---|---|
| PMBOK | Riesgos, recursos, stakeholders, valor y gobernanza |
| PMI-CPMAI | Business understanding, data understanding, model evaluation y operationalization |
| ISO/IEC 42001 | Sistema de gestión de IA, roles, controles y mejora continua |
| ISO/IEC 23894 | Gestión de riesgos de IA, datos, modelo y operación |
| ISO/IEC 42005 | Evaluación de impacto en clientes, usuarios y servicios |
| NIST AI RMF | Govern, Map, Measure, Manage |
| ISO/IEC 38507 | Supervisión ejecutiva y accountability del uso de IA |

---

## 15. Entregable final del grupo

Cada grupo debe presentar en 5 minutos:

1. Escenario recomendado.
2. Justificación basada en datos.
3. Score comparativo.
4. Riesgos residuales.
5. Controles de gobernanza.
6. Decisión ejecutiva.
7. Mensaje al sponsor.

---

## 16. Guía para el instructor

### Resultado esperado

El escenario más balanceado probablemente será el **Escenario 2: mover 2 ingenieros + soporte externo**.

Razón:
- Reduce significativamente el riesgo del Cliente B.
- No dispara demasiado el riesgo del Cliente A.
- Tiene costo adicional, pero controlado.
- Es más defendible desde una perspectiva de portafolio.
- Facilita una decisión de tipo **Conditional Go**.

### Decisión recomendada

**Conditional Go**

Condiciones:
- Aprobación del Service Owner.
- Notificación al Cliente A si existe impacto potencial.
- Revisión diaria de SLA durante 72 horas.
- Registro de decisión en la PMO.
- Criterio de reversión si el riesgo del Cliente A supera 35%.
- Cierre post-incidente y lecciones aprendidas.

---

## 17. Executive Summary de ejemplo

La opción recomendada es ejecutar el Escenario 2: mover dos ingenieros de ciberseguridad al Cliente B y complementar con soporte externo temporal. Esta alternativa reduce el riesgo crítico del Cliente B de 80% a 45%, limitando el impacto sobre el SLA del Cliente A a 25%. Aunque implica un costo adicional del 12%, ofrece el mejor equilibrio entre protección del cliente crítico, continuidad operativa y riesgo reputacional.

La decisión debe aprobarse como Conditional Go, con monitoreo diario de SLA, trazabilidad de la decisión, aprobación del Service Owner y criterio de reversión si el riesgo del Cliente A supera el umbral definido. Esta opción no elimina todos los riesgos, pero ofrece una respuesta proporcionada, gobernada y defendible ante el sponsor.

---

## 18. Pregunta final de reflexión

Cuando una PMO enfrenta una crisis en un cliente estratégico, ¿decide por urgencia o simula el impacto completo sobre el portafolio antes de mover recursos críticos?

---

## 19. Bonus challenge

Modificar el escenario:

- El Cliente B exige respuesta en 24 horas.
- El Cliente A amenaza con penalidad si su SLA cae bajo 99.5%.
- El soporte externo solo está disponible en 48 horas.
- El equipo SOC/NOC puede aportar 1 recurso adicional durante 2 días.

Preguntas:
1. ¿Cambia la recomendación?
2. ¿Qué nuevo escenario propondrías?
3. ¿Qué condición de gobernanza se vuelve más crítica?
4. ¿Qué decisión debe escalarse al sponsor?
