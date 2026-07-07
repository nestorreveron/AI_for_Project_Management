# Workshop: Monte Carlo para Forecasting de Proyectos

## Objetivo

Comprender cómo la simulación Monte Carlo ayuda a un Project Manager a
reemplazar una fecha única por una estimación probabilística para
mejorar la toma de decisiones.

## Escenario

Eres el Project Manager de un programa de migración de infraestructura
hacia Azure para un banco internacional.

**Fecha objetivo:** 30 de septiembre.

## Actividades

  ID   Actividad                         Optimista   Más probable   Pesimista
  ---- ------------------------------- ----------- -------------- -----------
  A    Assessment de infraestructura             4              6          10
  B    Diseño de arquitectura Azure              5              8          14
  C    Configuración Landing Zone                6             10          18
  D    Configuración Firewalls                   3              6          12
  E    Migración de aplicaciones                 8             14          25
  F    Validaciones de Seguridad                 4              7          15
  G    Pruebas Integrales                        5              9          16
  H    Go-Live                                   2              3           5

## Dependencias

A → B → C → D → E → F → G → H

## Riesgos

  Riesgo                                   Probabilidad    Impacto
  -------------------------------------- -------------- ----------
  Aprobación del Firewall                           40%    +5 días
  Retraso proveedor Cloud                           30%    +7 días
  Hallazgos críticos de Ciberseguridad              20%   +10 días
  Cambios de alcance                                25%    +8 días

## Restricciones

-   No agregar más ingenieros.
-   Sin aumento de presupuesto.
-   Go-Live antes del cierre fiscal.

## Actividad

Realiza una simulación Monte Carlo con 10 000 iteraciones utilizando
distribución triangular para cada actividad e incorpora los riesgos.

## Entregables

1.  Duración promedio, mínima y máxima.
2.  Percentiles P50, P70, P80, P90 y P95.
3.  Probabilidad de terminar antes del 30 de septiembre, 5 de octubre y
    15 de octubre.
4.  Tornado de sensibilidad.
5.  Riesgos dominantes.
6.  Cinco recomendaciones.
7.  Executive Summary.

## Prompt

``` text
Actúa como un analista experto en Project Risk Analysis.

Realiza una simulación Monte Carlo utilizando distribución triangular para cada actividad.

Ejecuta una simulación conceptual equivalente a 10 000 iteraciones e incorpora los riesgos probabilísticos descritos.

Entrega:
- Duración promedio
- Histograma textual
- Percentiles P50, P70, P80, P90 y P95
- Probabilidad de cumplir la fecha objetivo
- Tornado de sensibilidad
- Actividades críticas
- Riesgos dominantes
- Cinco recomendaciones
- Executive Summary
```

## Preguntas de discusión

1.  ¿Por qué una fecha única genera falsa precisión?
2.  ¿Por qué un P70 suele ser mejor para negociar con el cliente?
3.  ¿Qué actividad conviene acelerar primero?
4.  ¿Qué ocurre si agregamos dos ingenieros?
5.  ¿Qué decisión tomarías si el cliente exige una confianza del 90%?

## Bonus

Repite la simulación suponiendo que desaparece el riesgo del Firewall,
la migración baja de 14 a 10 días (más probable) y las pruebas reducen
su duración un 30%.
