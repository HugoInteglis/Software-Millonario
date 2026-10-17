# Concepto: recuperar presupuestos no aceptados en clínicas

> Borrador de trabajo (17-10-2026). Nada de esto está validado con clientes.
> [S] = suposición pendiente de comprobar.

## Qué es, en una frase

Un sistema que hace seguimiento a cada paciente que recibió un presupuesto y
no lo aceptó. Responde sus dudas, le ofrece facilidades de pago y avisa a la
clínica cuando el paciente está listo para agendar. Todo se mide en euros (o
quetzales) recuperados.

## Por qué el paciente no acepta (lo que el seguimiento debe resolver)

| Motivo | Respuesta del sistema |
|---|---|
| Precio / "no me lo puedo permitir ahora" | Financiación, pago por fases (España) o enganche más cuotas / Visacuotas (Guatemala) [S] |
| Miedo o dudas sobre el tratamiento | Contenido explicativo, casos de antes y después, respuesta a preguntas frecuentes |
| "Me lo pienso" / falta de tiempo | Recordatorio en el momento adecuado y facilidad para agendar |
| Está comparando con otra clínica | Recordar el valor (garantía, materiales, el doctor) sin entrar en guerra de precios |
| Simple olvido | Un mensaje a tiempo |

## Cómo funciona

1. **Entrada de presupuestos.**
   - v0: la clínica sube un Excel o CSV exportado de su software de gestión.
   - Más adelante: integración con el software de gestión de la clínica
     (Gesden, Clinic Cloud, Dentalink, etc. [S]).
2. **Secuencia automática por WhatsApp.** Por ejemplo:
   - Día 2: "¿te quedó alguna duda?".
   - Día 7: opciones de pago.
   - Día 21: caso similar.
   - Día 45: último recordatorio.

   Los mensajes son plantillas aprobadas por Meta y personalizadas con el
   tratamiento y el nombre del doctor.
3. **La IA lee las respuestas y las clasifica:**
   - "Quiere cita" → aviso inmediato a la coordinadora.
   - "Duda" → la IA responde con la información aprobada por la clínica.
   - "Precio" → envía las opciones de financiación.
   - "No interesado" → se detiene la secuencia.
   - Cualquier pregunta clínica → pasa siempre a una persona.
4. **La coordinadora cierra.** El producto no la sustituye: le da una lista
   priorizada de "pacientes calientes" para que llame o agende.
5. **Panel de resultados:**
   - Presupuestos en seguimiento.
   - Tasa de respuesta.
   - Citas generadas.
   - Tratamientos aceptados.
   - **€ recuperados**, comparados con un **grupo de control**.

## El grupo de control

Se reserva un 10–20 % de los presupuestos sin seguimiento automático. La
diferencia de aceptación entre los dos grupos es la recuperación real, no una
estimación.

Esto sirve para tres cosas:

- **Vender:** "en tu clínica, el seguimiento subió la aceptación del X % al Y %".
- **Cobrar con justicia** si el precio va ligado a resultados.
- **Retener al cliente:** es difícil darse de baja de algo que demuestra su
  rentabilidad cada mes.

## Fases

| Fase | Qué es | Cuándo se pasa a la siguiente |
|---|---|---|
| **0. Piloto manual** | Hugo con WhatsApp Business, plantillas redactadas con Claude y una hoja de cálculo. Sin código. | 3 clínicas pagando y más de 5.000 € recuperados |
| **1. MVP (2–4 semanas)** | Importación de Excel, secuencias, API de WhatsApp, clasificación con IA, panel con grupo de control, cobro | 20 clínicas de pago |
| **2. Escala** | Integraciones con los softwares de gestión, enlaces de financiación, llamadas con IA (solo si hay consentimiento y demanda), Guatemala | — |

## Diferencias por país

| | España | Guatemala |
|---|---|---|
| Vocabulario | presupuesto, coordinadora | cotización, asistente |
| Pago del tratamiento | financiación al consumo, pago por fases | enganche más cuotas, cuotas con tarjeta [S] |
| Precio del producto | 149–249 €/mes | 79–99 USD/mes |
| Datos de pacientes | RGPD: datos de salud (art. 9). La clínica es responsable del tratamiento y nosotros encargados. | Sin ley general todavía; se aplica el mismo estándar |
| Cobro a la clínica | Stripe en EUR | Stripe desde la entidad española, en USD |

## Cuestiones legales a resolver antes de escalar

- **Consentimiento del paciente** para recibir seguimiento por WhatsApp. Lo
  más limpio: una casilla o frase al entregar el presupuesto. Validar con un
  abogado de protección de datos sanitarios.
- **Llamadas automatizadas:** la Ley General de Telecomunicaciones limita las
  llamadas comerciales no solicitadas. Por eso las llamadas con IA quedan
  fuera del MVP.
- **Contrato de encargado de tratamiento** con cada clínica.
- **Calidad del número en WhatsApp:** si muchos pacientes bloquean o
  denuncian, Meta limita el número. Frecuencia baja y opción clara de
  "no quiero más mensajes".

## Costes unitarios estimados (por clínica y mes)

- **WhatsApp:** unos 100 presupuestos × 4 mensajes ≈ 400 plantillas, entre
  10 y 25 € según la tarifa de Meta [S].
- **IA:** menos de 5 € [S].
- **Margen bruto:** más del 85 % a 149–249 €/mes.

## Ejemplo de retorno para la venta (hipotético)

- La clínica tiene 60 presupuestos pendientes al mes con un ticket medio de
  1.500 € [S].
- Si se recuperan 4 → 6.000 € facturados, frente a 249 € de cuota.

## Riesgos principales

1. Que los softwares de gestión añadan esta función.
2. Pacientes molestos, que dañen la imagen de la clínica.
3. Disputas sobre qué recuperación se debe al producto (lo mitiga el grupo de
   control).
4. Resistencia de la coordinadora si siente que la sustituyen. Por eso el
   producto se presenta como su herramienta, no como su reemplazo.
