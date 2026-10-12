# Notas del presentador — IA Generativa Tierragrande
Comité Directivo · 20 min · 15 diapositivas (13 de arco + 2 de apéndice)

Tono: ejecutivo y sobrio. Un punto por diapositiva. El texto en pantalla es una señal, no un guion.

---

## 1 · Portada y la petición (todos)
- **Punto:** encuadrar la decisión desde el minuto cero — sin suspenso en una junta.
- **Dí:** "Hoy pedimos aprobar el Año 1 con dos casos internos, y avalar el camino al asistente de compras en el Año 2. En 6 meses verán algo que pueden tocar."
- **Objeción esperada:** ninguna aún; es orientación.

## 2 · El problema (Ricardo / CEO)
- **Punto:** la madurez en datos ya existe; falta convertirla en IA.
- **Número a defender:** 15 personas, cero experiencia LLM (del caso).
- **Objeción:** "¿No deberíamos ir más rápido?" → el cuello de botella es capacidad, no fundaciones; lo abordamos en slides 9 y 12.

## 3 · Costo de inacción (Ricardo / Patricia)
- **Punto:** no actuar también cuesta.
- **Números a defender:** 2,8 días de primera respuesta · 60.000 PQR/año · competidor lanzó hace 2 meses (todos del caso).
- **Cita de Ricardo** en pantalla — úsala para validar la urgencia, luego gíra a "pero por el camino de menor riesgo".
- **Objeción:** "El shadow AI es tu dato, no del caso" → es cita textual de Patricia; está documentado.

## 4 · El cambio (Ricardo / Andrés)
- **Punto:** la plataforma está lista; falta la capa de IA gobernada. La Ley 1581 obliga a gobernar antes de ir al cliente.
- **Objeción (Andrés):** "¿Y si se adelanta un caso con datos personales?" → por diseño, Año 1 no usa datos personales (slide 8).

## 5 · La propuesta (todos)
- **Punto:** el giro problema → plan. Léelo como la frase que un miembro de junta repetiría en el pasillo.
- **Defender:** el "todavía no" al asistente de compras NO es un "no" — es secuencia de riesgo (desarrollado en slide 12).
- **Objeción (Ricardo):** "Quiero el asistente de compras ya" → slide 12 muestra que el Año 1 ES el camino a eso, con menos riesgo.

## 6 · Cómo funciona — arquitectura (Patricia / Andrés)
- **Punto:** una plataforma común sobre Databricks; cero infra nueva que un equipo pequeño tendría que operar.
- **Defender:** gateway agnóstico = anti-lock-in; conocimiento dentro de Unity Catalog = menos superficie Ley 1581.
- **Objeción (Patricia):** "¿Se puede con lo que tenemos?" → sí; reutiliza Databricks + Power BI que el equipo ya domina.

## 7 · Cómo funciona cada caso (Patricia / Andrés)
- **Punto:** cada flujo responde con cita a la fuente (Caso 1) y con humano en el lazo (Caso 2).
- **Defender:** Caso 1 tiene guardrail de entrada (PII) y de salida (groundedness + cita); Caso 2 no publica nada sin aprobación del redactor + mide con A/B.
- **Objeción (Andrés):** "¿Y la trazabilidad?" → MLflow Tracing + Inference Tables + Unity Catalog (auditoría/linaje) en ambos diagramas.

## 8 · Riesgo y gobierno (Andrés / Patricia)
- **Punto:** cero alucinaciones por diseño.
- **Números a defender:** groundedness mínimo 95% como compuerta go/no-go · 0 datos personales en Año 1 · PII filtrado desde el día 1.
- **Cita de Andrés** en pantalla + "el CDO aprueba el go-live" le entrega el control explícito.
- **Objeción (Andrés):** "¿Quién garantiza el 95%?" → golden set validado por expertos + revisión humana + LLM-as-judge calibrado; se versiona en Databricks.

## 9 · Costo y lock-in (Patricia / Finanzas)
- **Punto:** USD 200k todo incluido; el talento es el 60% porque la capacidad es la restricción crítica.
- **Números a defender:** desglose exacto del Bloque 5 del informe. Run-rate Año 2: 25–50k modelos + 15–20k licencias.
- **Cita implícita de Patricia:** responde sus 3 preguntas — costos (gasto por caso + caché), lock-in (cambio en el gateway), quién opera (1 senior + MLOps + 2 internos).
- **Objeción:** "¿Y si los salarios suben?" → la contratación #2 es la primera variable de ajuste (nota del informe); 3,5% de contingencia.

## 10 · ROI y repago (Ricardo / Finanzas)
- **Punto:** el Año 1 se paga solo incluso en el escenario conservador.
- **Números a defender:** Caso 2 ventas incrementales 100–300k/año (uplift 1–3%); Caso 1 50–75k/año; inversión 200k.
- **IMPORTANTE:** son estimaciones de orden de magnitud (supuesto S8). Reportamos ventas incrementales, no margen (riesgo declarado). El ROI real se mide en F1–F2.
- **Objeción (Finanzas):** "Tu ROI es optimista" → por eso mostramos el rango conservador y la base de cada supuesto (apéndice slide 13).

## 11 · Hito visible 6 meses (Ricardo / todos)
- **Punto:** en 6 meses, algo tangible con números REALES, no proyectados.
- **Defender:** demo en vivo + primeros resultados del A/B (medidos) + costo mensual real + plataforma ya construida.
- **Cierra la cita de Ricardo** de la slide 3 ("algo que puedan tocar en 6 meses").

## 12 · Hoja de ruta (todos)
- **Punto:** ganar confianza en Año 1, monetizar de cara al cliente en Año 2.
- **Defender:** decir "no" con un plan — el asistente de compras (#4) está parqueado en F3 con condición de revisión (hito mes 6).
- **Objeción (Ricardo):** "¿Por qué no antes?" → #4 es cara al cliente (máximo riesgo), toca datos de fidelidad (consentimiento), y "no hay cifras propias de impacto" → imposible sustentar ROI hoy.

## 13 · La decisión (Ricardo)
- **Punto:** un solo "sí" claro. Restablece el ask de la slide 1.
- **Dí:** "Pedimos aprobar el Año 1, avalar el plan al Año 2 condicionado al hito de 6 meses, y arrancar F0 ya."
- **No cierres en falso** ("sigamos hablando"). Pide el sí.

## Apéndices (backup Q&A)
- **14 · Supuestos S1–S14:** si retan una cifra, ve directo al supuesto y su base. Cada uno es trazable o pendiente de validación en F0.
- **15 · Mapa de objeciones:** una referencia rápida de qué slide responde a cada directivo. Úsalo si una objeción llega fuera de secuencia.

---

### Si el reloj aprieta (fusiones permitidas por la skill)
1. Fusiona 7 → 6 (los 4 diagramas en una sola "Cómo funciona").
2. Fusiona 11 → 12.
3. **Nunca** quites la slide 8 (riesgo/gobierno) con Andrés en la sala.
