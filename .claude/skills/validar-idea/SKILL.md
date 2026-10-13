---
name: validar-idea
description: Evalúa una idea de software con una puntuación objetiva (dolor, disposición a pagar, mercado, competencia, distribución, viabilidad) y da un veredicto. Úsala cuando el usuario proponga una idea nueva de producto o quiera comparar varias.
---

# Validar idea de software

Idea a evaluar: $ARGUMENTS

## Pasos

1. Si falta información clave (quién es el cliente, qué problema resuelve),
   haz como máximo 3 preguntas concretas antes de seguir.
2. Lanza el subagente `estratega-negocio` para investigar competencia, precios
   y canales de la idea.
3. Puntúa cada criterio de 1 a 5 y justifica en una línea:

| Criterio | Qué mide |
|---|---|
| Dolor | ¿Es un problema caro, frecuente y urgente? |
| Disposición a pagar | ¿El cliente ya gasta dinero o tiempo en resolverlo? |
| Tamaño del nicho | ¿Hay suficientes clientes para llegar a 1M USD/año? |
| Competencia | ¿Hay hueco claro? (mercado con competidores que cobran = buena señal) |
| Distribución | ¿Sabemos exactamente dónde encontrar a los primeros 100 clientes? |
| Viabilidad técnica | ¿Se puede lanzar un MVP de pago en ≤ 4 semanas? |
| Defensibilidad | ¿Datos, integraciones, comunidad o costes de cambio? |

4. Calcula el total (máx. 35):
   - **≥ 26** → Adelante: pasa a `/plan-mvp`.
   - **18–25** → Pivotar: propone 2–3 variantes que mejoren los criterios débiles.
   - **< 18** → Descartar: explica por qué y sugiere ideas cercanas más prometedoras.
5. Propón el **experimento de validación más barato** (landing con lista de
   espera y precio, 10 entrevistas, preventa, etc.) con un criterio de éxito
   numérico.
6. Añade la idea, su puntuación y el veredicto a `docs/ideas.md`.
