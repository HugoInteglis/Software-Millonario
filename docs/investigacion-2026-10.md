# Investigación de oportunidades — octubre 2026

Cuatro líneas de búsqueda de necesidades reales:

1. Dolores en nichos B2B verticales.
2. Servicios caros que la IA abarata.
3. Demanda forzada por regulación.
4. Mercados fragmentados (conectar proveedores con clientes).

**Leyenda:** [D] = dato con fuente · [S] = suposición pendiente de validar.

## Patrones que se repiten en las cuatro líneas

- **Lo genérico con IA ya está saturado.** Vídeo, webs, reseñas, SDR y
  recepcionista son el primer sitio donde los grandes (Google, Meta, HubSpot)
  convierten el producto en una función más.
- **El hueco está en ayudar a la pyme a cobrar dinero que ya está a punto de
  ganar y está perdiendo:** presupuestos sin respuesta y licitaciones a las que
  no se presenta o que no gana.
- **Hay que elegir un vertical concreto y trabajar en español.** Varios modelos
  probados en EE. UU. no tienen equivalente bueno en español.
- **Evitar marketplaces de dos lados.** Para un fundador en solitario es mejor
  un SaaS que paga un solo lado.

## Finalista 1 — Reactivar presupuestos no aceptados (clínicas)

- **Cliente:** clínica dental o estética privada de 1 a 5 sillones. Decide el
  gerente o el propietario.
- **Dolor:**
  - Muchos tratamientos presupuestados nunca se agendan. Las cifras del sector
    hablan de un 40–60 % [S: dato genérico, no de España]
    ([Rework](https://resources.rework.com/es/libraries/dental-clinic-growth/treatment-plan-acceptance-rate)).
  - El seguimiento depende de la recepción, que cuesta 18–24 k€/año [D]
    ([Join](https://join.com/es/guias-de-puesto/recepcionista-clinico)).
- **Mercado:** más de 23.000 clínicas dentales en España [D]
  ([Redacción Médica](https://www.redaccionmedica.com/profesionales/20231005/los-dentistas-marcan-su-objetivo-para-atender-personas-sin-recursos/203527_0.html)).
- **Competencia:** AInora (recepción) y Wati (WhatsApp genérico). No se
  encontró un producto español dedicado a reactivar presupuestos integrado con
  Gesden o Clinic Cloud [S: verificar a fondo].
- **Producto:** secuencia de WhatsApp y llamada con IA sobre los presupuestos
  pendientes, oferta de financiación y panel de "euros recuperados".
- **Precio:** 249 €/mes, o 149 €/mes más un 3–5 % de lo recuperado.
- **Números:** ~37 clientes = 10 k USD de MRR; ~300 clientes = 1 M USD/año
  (1,3 % de las clínicas).
- **Expansión:** el mismo motor sirve para reformas, instalaciones y
  climatización (32 % de cierre con seguimiento frente a 11 % sin él
  [S: dato de blog]).
- **Riesgos:** que el software de gestión de la clínica lo incorpore; RGPD con
  datos de salud; agente de WhatsApp de Meta.
- **Validación (2 semanas, 0 €):** llamar a 30 clínicas y ofrecer un piloto
  manual (Hugo + WhatsApp + plantillas de IA) sobre sus presupuestos de los
  últimos 6 meses, cobrando el 5 % de lo recuperado.
  **Éxito:** 3 clínicas aceptan y se recuperan más de 5.000 €.

## Finalista 2 — Copiloto IA para preparar ofertas de licitación

Lo detectaron por separado dos de las cuatro líneas de investigación.

- **Cliente:** pyme proveedora del Estado (servicios, obra, limpieza,
  formación, suministros).
- **Dolor y mercado:**
  - Chile: Compra Ágil movió 787.211 procesos y 1.166 M USD en 2025 (+81,5 %);
    las empresas de menor tamaño se llevan el 82,9 % [D]
    ([ChileCompra](https://www.chilecompra.cl/2026/02/obras-publicas-y-salud-impulsan-dinamismo-de-las-compras-publicas-con-fuerte-retroceso-del-trato-directo/)).
    Hay 110.255 proveedores del Estado [D].
  - España: el 41 % de los contratos de 2024 tuvo un solo licitador [D]
    ([The Objective](https://theobjective.com/economia/2025-08-01/competencia-licitaciones-desploma-41-contratos-aspirante/)).
    En Madrid, el 65 % de los adjudicatarios son pymes [D].
- **Competencia:**
  - Las alertas están saturadas en España: más de 12 servicios entre 9 y
    345 €/mes [D]
    ([comparativa](https://jorpex.com/es/compare/alertas-licitaciones-comparativa/)).
  - Tendios (2 M€ levantados) cobra 600 € o el 1 % por oferta asistida [D]
    ([Forbes](https://forbes.es/economia/721760/tendios-cierra-una-ronda-de-inversion-de-dos-millones-para-mejorar-su-plataforma-y-consolidar-su-expansion/)).
  - En Chile: LicitaLAB y LicitAlertas.
- **Hueco:** casi todos ayudan a *encontrar* licitaciones; pocos ayudan a
  *ganarlas*. El producto sería redactar la memoria técnica puntuable por
  vertical, con revisión humana.
- **Precio:** 49–149 USD/mes (Chile) o 249–490 €/mes (España), más una tarifa
  por oferta preparada.
- **Ventajas:** los datos son públicos, así que no hay problema de huevo y
  gallina. Las adjudicaciones públicas sirven como lista perfecta para el
  outbound.
- **Riesgos:** que Tendios o LICAI amplíen hacia la redacción; churn de
  clientes que no ganan; cambios en los portales oficiales.
- **Validación (7–14 días, 0 €):** descargar adjudicatarios recientes y escribir
  a 50 ofreciendo preparar su próxima oferta (49 USD en Chile / 300 € en
  España), hecha a mano con Claude.
  **Éxito:** 5 pagos.

## Tercera opción — Accesibilidad web obligatoria (EAA) para tiendas online

- **Obligación:** desde el 28-6-2025 (Ley 11/2023). Las microempresas de
  servicios están exentas. Multas de hasta 1 M€. En Francia ya hay demandas
  contra Carrefour y Auchan [D]
  ([pinmeto](https://www.pinmeto.com/news/eu-accessibility-act-enforcement-french-courts-2026/)).
- **Mercado:** ~161.000 empresas con 10 o más asalariados [D]; de ellas, entre
  15 y 30 k venden online [S].
- **Hueco:** auditoría, corrección, declaración de accesibilidad y
  monitorización a precio cerrado y en español. Los overlays no cumplen y las
  consultoras son caras.
- **Precio:** 990 € de alta + 79 €/mes.
- **Encaje:** diseño web e IA. Se puede auditar cualquier tienda sin pedir
  permiso y enviar el informe en Loom.
- **Riesgos:** aún no hay sanciones públicas en España; parte del trabajo es
  servicio y no software.

## Otras señales a vigilar

- **Factura electrónica B2B (RD 238/2026, Orden HAC/1028/2026):**
  - Fechas: 6-10-2027 para empresas que facturan más de 8 M€ y 6-10-2028 para
    el resto.
  - El receptor debe comunicar el estado y el pago de cada factura.
  - Posible producto para gestorías, pero el pico de demanda llega en 2028 y
    Holded, Sage y A3 lo añadirán.
- **Verifactu:** Hacienda anuncia octubre de 2028, aún sin norma aprobada.
- **Registro horario digital:** sin aprobar.
- **Chile, Ley 21.719 de protección de datos:** entra en vigor el 1-12-2026,
  con un proyecto para aplazarla a 2027.
- **Choco en español:** convertir en pedidos los mensajes de WhatsApp que
  reciben los distribuidores. Validado en EE. UU. y Alemania; dolor sin
  verificar en España.

## Limitaciones de esta investigación

- No se pudo leer Reddit (las herramientas devuelven error).
- Varias cifras vienen de blogs de vendedores y están marcadas como [S].
- Ninguna idea se considera validada hasta que haya clientes que paguen en el
  experimento de validación.
