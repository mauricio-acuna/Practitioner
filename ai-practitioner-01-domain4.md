# Dominio de contenido 4: Pautas para una IA responsable

Fuente oficial: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/ai-practitioner-01-domain4.html  
Peso en el examen: 14% del contenido puntuado.

[Volver al indice](ai-practitioner-01.md)

## Que evalua este dominio

Este dominio comprueba que entiendas principios de IA responsable, riesgos legales y de confianza, caracteristicas de datos responsables y la importancia de modelos transparentes y explicables.

## Tareas del dominio

1. Explicar el desarrollo de sistemas de IA responsables.
2. Reconocer la importancia de modelos transparentes y explicables.

## 4.1 Sistemas de IA responsables

Caracteristicas clave:

| Caracteristica | Significado |
|---|---|
| Bias | Sesgo sistematico |
| Fairness | Trato equitativo entre grupos |
| Inclusividad | Considerar usuarios y casos diversos |
| Robustez | Comportamiento estable ante variaciones |
| Seguridad | Reducir dano y uso indebido |
| Veracidad | Respuestas correctas y fundamentadas |

## Herramientas y practicas

- Amazon Bedrock Guardrails: politicas, filtros y controles para GenAI.
- SageMaker Clarify: analisis de sesgo y explicabilidad.
- SageMaker Model Monitor: monitoreo de calidad y drift.
- Amazon A2I: revision humana.
- Auditorias humanas.
- Analisis por subgrupos.
- Revision de calidad de etiquetas.

## Seleccion responsable de modelos

Considera:

- Impacto ambiental.
- Sostenibilidad.
- Tamano del modelo frente a necesidad real.
- Costo energetico.
- Explicabilidad.
- Riesgo para usuarios.
- Cumplimiento legal.

## Riesgos legales y de confianza

- Reclamos de propiedad intelectual.
- Salidas sesgadas.
- Perdida de confianza del cliente.
- Riesgo para usuario final.
- Alucinaciones.
- Falta de explicabilidad.
- Uso de datos no autorizados.

## Caracteristicas de datasets responsables

- Inclusivos.
- Diversos.
- Curados.
- Balanceados cuando aplique.
- Representativos.
- Con calidad revisada.
- Con origen documentado.

## Bias y variance

| Concepto | Riesgo |
|---|---|
| Bias alto | El modelo simplifica demasiado y puede fallar sistematicamente |
| Variance alta | El modelo cambia demasiado ante nuevos datos |
| Overfitting | Memoriza entrenamiento y generaliza mal |
| Underfitting | Aprende poco incluso del entrenamiento |

## 4.2 Transparencia y explicabilidad

Un modelo transparente o explicable permite entender:

- Que datos usa.
- Como se evaluo.
- Para que sirve.
- Que limites tiene.
- Que riesgos presenta.
- Por que produce una decision o salida.

Herramientas:

- SageMaker Model Cards.
- SageMaker Clarify.
- Amazon Bedrock Model Evaluation.
- Modelos open source, cuando su licencia y datos son adecuados.
- Documentacion de datos y licencias.

## Tradeoffs

Puede existir tension entre:

- Rendimiento y explicabilidad.
- Seguridad y apertura.
- Tamano del modelo y costo.
- Automatizacion y control humano.

La respuesta correcta suele equilibrar valor de negocio, riesgo, explicabilidad y controles.

## Diseno centrado en humanos

Incluye:

- Informar cuando se usa IA.
- Dar mecanismos de feedback.
- Mostrar fuentes cuando aplique.
- Permitir revision humana en decisiones sensibles.
- Explicar limites.
- Diseñar para usuarios diversos.

## Senales de respuesta correcta

En preguntas de IA responsable, la opcion mas profesional suele:

- Analizar subgrupos, no solo promedio global.
- Documentar supuestos, datos, riesgos y limites.
- Mantener revision humana cuando el impacto es alto.
- Usar herramientas como Clarify, Model Monitor, Model Cards, A2I o Guardrails segun el caso.
- Equilibrar rendimiento, explicabilidad, seguridad y confianza.

## Errores comunes

- Pensar que precision alta elimina sesgo.
- No evaluar subgrupos.
- Omitir documentacion del modelo.
- Usar GenAI en decisiones sensibles sin revision.
- Ignorar sostenibilidad o impacto ambiental.

## Checklist profesional del dominio

- Puedo definir bias, fairness, inclusividad, robustez, seguridad y veracidad.
- Puedo explicar riesgos legales de GenAI.
- Puedo identificar caracteristicas de datasets responsables.
- Puedo explicar bias, variance, overfitting y underfitting.
- Puedo elegir herramientas AWS para sesgo, explicabilidad, monitoreo y revision humana.
- Puedo explicar transparencia, explicabilidad y diseno centrado en humanos.

## Ejercicios rapidos

1. Si un grupo demografico recibe peores resultados, revisa sesgo y fairness.
2. Para documentar proposito, datos y riesgos, usa Model Cards.
3. Para sesgo y explicabilidad, piensa en SageMaker Clarify.
4. Para decisiones de alto impacto, agrega revision humana.
5. Para bloquear contenido toxico, considera Bedrock Guardrails.
