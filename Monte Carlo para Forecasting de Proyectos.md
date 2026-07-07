# Workshop: Monte Carlo para Forecasting de Proyectos

## Objetivo

Comprender cómo la simulación Monte Carlo ayuda a un Project Manager a dejar de pensar en una única fecha de entrega y comenzar a tomar decisiones basadas en probabilidades.

---

# Escenario

Eres el Project Manager de un programa de migración de infraestructura hacia Azure para un banco internacional.

El patrocinador solicita confirmar si el programa podrá finalizar antes del **30 de septiembre**.

Sin embargo, existen múltiples incertidumbres relacionadas con aprobaciones, proveedores, redes y validaciones de seguridad.

Tu trabajo consiste en utilizar IA para estimar la probabilidad de cumplir la fecha objetivo y proponer acciones de mitigación.

---

# Información del Proyecto

## Fecha objetivo

30 de septiembre

---

## Actividades

| ID | Actividad | Optimista | Más Probable | Pesimista |
|----|-------------------------------|-----------|--------------|------------|
| A | Assessment de infraestructura | 4 | 6 | 10 |
| B | Diseño de arquitectura Azure | 5 | 8 | 14 |
| C | Configuración Landing Zone | 6 | 10 | 18 |
| D | Configuración de Firewalls | 3 | 6 | 12 |
| E | Migración de aplicaciones | 8 | 14 | 25 |
| F | Validaciones de Seguridad | 4 | 7 | 15 |
| G | Pruebas Integrales | 5 | 9 | 16 |
| H | Go-Live | 2 | 3 | 5 |

---

## Dependencias

A → B → C

C → D

D → E

E → F

F → G

G → H

---

# Riesgos conocidos

## Riesgo 1

Aprobación del Firewall

Probabilidad:
40%

Impacto:

+5 días

---

## Riesgo 2

Retraso del proveedor Cloud

Probabilidad:

30%

Impacto:

+7 días

---

## Riesgo 3

Hallazgos críticos de Ciberseguridad

Probabilidad:

20%

Impacto:

+10 días

---

## Riesgo 4

Cambios de alcance solicitados por negocio

Probabilidad:

25%

Impacto:

+8 días

---

# Restricciones

• No pueden agregarse más ingenieros.

• El presupuesto no puede aumentar.

• El Go-Live debe realizarse antes del cierre fiscal.

---

# Tarea

Realiza una simulación Monte Carlo utilizando 10 000 iteraciones.

Asume distribución triangular para cada actividad utilizando los tres puntos estimados.

Considera además la ocurrencia probabilística de los riesgos descritos.

---

# Entregables

## 1. Forecast del cronograma

Indicar:

- Duración promedio del proyecto
- Duración mínima observada
- Duración máxima observada

---

## 2. Percentiles

Calcular:

P50

P70

P80

P90

P95

---

## 3. Probabilidad de cumplir

Calcular la probabilidad de terminar:

- Antes del 30 de septiembre
- Antes del 5 de octubre
- Antes del 15 de octubre

---

## 4. Tornado de riesgos

Identificar cuáles actividades generan mayor variabilidad.

Ordenarlas de mayor a menor impacto.

---

## 5. Riesgos dominantes

Determinar cuáles riesgos afectan más la fecha final.

Explicar por qué.

---

## 6. Recomendaciones

Proponer al menos cinco acciones para aumentar la probabilidad de éxito.

Por ejemplo:

- dividir actividades

- ejecutar tareas en paralelo

- reducir dependencias

- adelantar aprobaciones

- aumentar buffers

- modificar secuencia

---

## 7. Executive Summary

Preparar un resumen ejecutivo dirigido al Steering Committee.

Debe responder:

¿Cuál es la probabilidad real de cumplir la fecha?

¿Cuál es el principal riesgo?

¿Qué decisión recomienda tomar?

¿Qué nivel de confianza tiene la recomendación?

---

# Preguntas para discusión

1.

¿Por qué una fecha única genera falsa precisión?

---

2.

¿Por qué un P70 suele ser una mejor fecha para negociar con el cliente que un P50?

---

3.

¿Qué actividad convendría acelerar para obtener el mayor beneficio?

---

4.

¿Qué pasaría si agregáramos dos ingenieros adicionales?

---

5.

¿Reducir una actividad crítica dos días tiene más impacto que reducir una actividad no crítica cinco días?

¿Por qué?

---

6.

¿Qué decisión tomarías si el cliente exige una confianza del 90%?

---

# Bonus

Ahora modifica el escenario.

Supón que:

• El riesgo del Firewall desaparece.

• La Migración baja su tiempo más probable de 14 a 10 días.

• Las pruebas se automatizan reduciendo un 30% su duración.

Vuelve a ejecutar la simulación.

Compara ambos escenarios.

¿En cuánto aumentó la probabilidad de cumplir la fecha?

¿Qué aprendiste?
