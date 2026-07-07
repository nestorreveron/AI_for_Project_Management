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


-----------------------------------------------------------

Actúa como un analista experto en Project Risk Analysis, Monte Carlo Simulation y Project Forecasting para una PMO enterprise.

Contexto:
Soy el Project Manager de un programa de migración de infraestructura hacia Azure para un banco internacional. El sponsor quiere saber si el proyecto podrá finalizar antes del 30 de septiembre.

Quiero que realices una simulación Monte Carlo conceptual con 10 000 iteraciones para estimar la duración probable del proyecto, la probabilidad de cumplir la fecha objetivo y los principales drivers de riesgo.

Datos del proyecto:

Fecha objetivo:
30 de septiembre

Actividades:

A. Assessment de infraestructura
- Optimista: 4 días
- Más probable: 6 días
- Pesimista: 10 días

B. Diseño de arquitectura Azure
- Optimista: 5 días
- Más probable: 8 días
- Pesimista: 14 días

C. Configuración Landing Zone
- Optimista: 6 días
- Más probable: 10 días
- Pesimista: 18 días

D. Configuración de Firewalls
- Optimista: 3 días
- Más probable: 6 días
- Pesimista: 12 días

E. Migración de aplicaciones
- Optimista: 8 días
- Más probable: 14 días
- Pesimista: 25 días

F. Validaciones de Seguridad
- Optimista: 4 días
- Más probable: 7 días
- Pesimista: 15 días

G. Pruebas Integrales
- Optimista: 5 días
- Más probable: 9 días
- Pesimista: 16 días

H. Go-Live
- Optimista: 2 días
- Más probable: 3 días
- Pesimista: 5 días

Dependencias:
A → B → C → D → E → F → G → H

Riesgos adicionales:

Riesgo 1: Aprobación del Firewall
- Probabilidad: 40%
- Impacto si ocurre: +5 días

Riesgo 2: Retraso del proveedor Cloud
- Probabilidad: 30%
- Impacto si ocurre: +7 días

Riesgo 3: Hallazgos críticos de Ciberseguridad
- Probabilidad: 20%
- Impacto si ocurre: +10 días

Riesgo 4: Cambios de alcance solicitados por negocio
- Probabilidad: 25%
- Impacto si ocurre: +8 días

Restricciones:
- No se pueden agregar más ingenieros.
- El presupuesto no puede aumentar.
- El Go-Live debe realizarse antes del cierre fiscal.

Instrucciones para la simulación:

1. Usa distribución triangular para cada actividad, tomando como parámetros los valores optimista, más probable y pesimista.
2. Simula conceptualmente 10 000 ejecuciones del proyecto.
3. Incorpora los riesgos adicionales como eventos probabilísticos independientes.
4. Calcula la duración total del proyecto para cada simulación.
5. No inventes datos adicionales fuera del escenario. Si necesitas asumir algo, indícalo claramente.

Entrega el análisis en este formato:

1. Supuestos utilizados
- Explica cómo se modelaron las actividades.
- Explica cómo se modelaron los riesgos.
- Explica cualquier limitación del análisis.

2. Resultados principales
- Duración promedio estimada.
- Duración mínima simulada.
- Duración máxima simulada.
- Rango más probable de duración.

3. Percentiles
Entrega una tabla con:
- P50
- P70
- P80
- P90
- P95

Explica qué significa cada percentil en lenguaje ejecutivo.

4. Probabilidad de cumplir fechas
Calcula la probabilidad aproximada de terminar:
- Antes del 30 de septiembre.
- Antes del 5 de octubre.
- Antes del 15 de octubre.

5. Histograma textual
Muestra una distribución textual de resultados por rangos de duración.

Ejemplo:
- 45–50 días: ####
- 51–55 días: ########
- 56–60 días: ############

6. Tornado de sensibilidad
Identifica qué actividades generan mayor variabilidad en la fecha final.

Ordena de mayor a menor impacto:
- Actividad
- Motivo del impacto
- Recomendación de mitigación

7. Riesgos dominantes
Identifica cuáles riesgos adicionales tienen mayor efecto sobre la fecha final:
- Aprobación del Firewall
- Retraso proveedor Cloud
- Hallazgos críticos de Ciberseguridad
- Cambios de alcance

Explica por qué.

8. Recomendaciones para mejorar la probabilidad de éxito
Propón al menos cinco acciones concretas para aumentar la probabilidad de cumplir la fecha objetivo.

Ejemplos:
- Adelantar aprobaciones de firewall.
- Ejecutar validaciones de seguridad en paralelo.
- Reducir incertidumbre en migración.
- Congelar alcance.
- Crear buffer ejecutivo.
- Dividir pruebas integrales por oleadas.
- Aumentar frecuencia de seguimiento de riesgos.

9. Recomendación Go / Conditional Go / No-Go
Con base en los resultados, recomienda una decisión:
- Go
- Conditional Go
- No-Go
- Escalar al Steering Committee

Justifica la recomendación.

10. Executive Summary
Prepara un resumen ejecutivo de máximo 250 palabras para el Steering Committee.

Debe responder:
- ¿Cuál es la probabilidad real de cumplir la fecha?
- ¿Cuál es el principal driver de riesgo?
- ¿Qué decisión recomiendas?
- ¿Qué acciones deben aprobarse esta semana?
- ¿Qué nivel de confianza tiene la recomendación?

11. Preguntas para discusión en clase
Genera cinco preguntas para que los participantes reflexionen sobre cómo usar Monte Carlo en proyectos reales de PMO.
