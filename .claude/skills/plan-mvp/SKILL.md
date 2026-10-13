---
name: plan-mvp
description: Convierte una idea validada en un plan de MVP ejecutable - alcance mínimo, modelo de precios, arquitectura, tareas por semana y plan de lanzamiento. Úsala cuando una idea ya está validada y toca empezar a construir.
---

# Plan de MVP

Idea: $ARGUMENTS

Genera el plan y guárdalo en `docs/mvp.md` con estas secciones:

1. **Propuesta de valor** en una frase: "Ayudamos a [cliente] a [resultado]
   sin [dolor actual]".
2. **Cliente ideal (ICP)**: rol, tipo de empresa, dónde se reúne online.
3. **Alcance del MVP**: máximo 3–5 funciones. Lista aparte de lo que queda
   **fuera** explícitamente.
4. **Precios**: planes, precio, prueba gratuita o no, y por qué. Incluye el
   cálculo de cuántos clientes hacen falta para 10k USD de MRR.
5. **Arquitectura**: según el stack por defecto de `CLAUDE.md`; modelo de
   datos principal y servicios externos.
6. **Plan semana a semana** (2–4 semanas) con tareas pequeñas y verificables.
   La semana 1 ya incluye auth y pagos funcionando.
7. **Analítica**: eventos a medir (registro, activación, pago, cancelación) y
   definición de "usuario activado".
8. **Lanzamiento**: canales para los primeros 100 usuarios, con acciones
   concretas (dónde publicar, a quién escribir, qué contenido crear).
9. **Riesgos principales** y cómo mitigarlos.

Después, pregunta si empezar a construir la semana 1 y, si la respuesta es sí,
inicializa el proyecto.
