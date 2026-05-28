# Matriz de decision AIF-C01

Version: 2026-05-28  
Objetivo: decidir rapido la respuesta probable ante preguntas de AWS Certified AI Practitioner AIF-C01.

## Fuentes de referencia

- Guia oficial AIF-C01: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/ai-practitioner-01.html
- Servicios dentro del alcance: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/aif-01-in-scope-services.html
- Revisiones: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/aif-01-revisions.html

## Regla maestra

Lee el enunciado y busca primero el objetivo real:

1. Prediccion o clasificacion con datos historicos: ML clasico.
2. Generacion, resumen, conversacion o codigo: GenAI.
3. Responder con documentos privados, actualizados o con citas: RAG.
4. Cambiar formato, tono o instrucciones: prompt engineering.
5. Adaptar estilo o tarea con ejemplos: fine-tuning.
6. Ejecutar pasos en sistemas externos: agentes.
7. Controlar riesgo, permisos, auditoria o datos sensibles: seguridad/gobernanza.
8. Sesgo, explicabilidad o impacto humano: IA responsable.

## Matriz rapida por pista del enunciado

| Si el enunciado dice... | Piensa primero en... | Por que |
|---|---|---|
| Categoria, aprobado/rechazado, fraude/no fraude | Clasificacion | El resultado es una clase |
| Importe, cantidad, precio, score numerico | Regresion | El resultado es un numero |
| Futuro, demanda, ventas por fecha | Forecasting | Hay componente temporal |
| Grupos naturales, segmentos sin etiquetas | Clustering | No hay etiquetas previas |
| Recomendaciones personalizadas | Amazon Personalize | Servicio administrado para recomendaciones |
| Audio a texto | Amazon Transcribe | Transcripcion |
| Texto a voz | Amazon Polly | Sintesis de voz |
| Traduccion | Amazon Translate | Traduccion automatica |
| Entidades, sentimiento, texto | Amazon Comprehend | NLP administrado |
| Chatbot conversacional historico | Amazon Lex | Bots de voz/texto |
| Imagenes o video | Amazon Rekognition | Vision artificial |
| Facturas, formularios, tablas en PDF | Amazon Textract | Extraccion documental |
| Modelos fundacionales administrados | Amazon Bedrock | GenAI con FMs |
| Entrenar/desplegar ML end-to-end | Amazon SageMaker AI | Plataforma ML |
| Modelos preconstruidos | SageMaker JumpStart | Arranque rapido |
| Busqueda empresarial | Amazon Kendra | Busqueda inteligente |
| Datos sensibles en S3 | Amazon Macie | Descubrimiento de datos sensibles |
| Llaves de cifrado | AWS KMS | Gestion de claves |
| Secretos | AWS Secrets Manager | Gestion de secretos |
| Quien llamo una API | AWS CloudTrail | Auditoria API |
| Logs, metricas, alarmas | Amazon CloudWatch | Observabilidad |
| Configuracion contra reglas | AWS Config | Compliance de configuracion |
| Vulnerabilidades | Amazon Inspector | Inspeccion de vulnerabilidades |
| Evidencias de auditoria | AWS Audit Manager | Evidencias |
| Reportes/acuerdos de compliance | AWS Artifact | Documentos de cumplimiento |

## ML clasico frente a GenAI

| Necesidad | Mejor opcion habitual |
|---|---|
| Decision tabular explicable | ML clasico |
| Prediccion con etiquetas historicas | ML supervisado |
| Agrupar sin etiquetas | ML no supervisado |
| Generar texto o resumen | GenAI |
| Conversar con lenguaje natural | GenAI |
| Crear codigo | GenAI |
| Crear imagen | Modelo multimodal o de difusion |
| Reglas exactas y simples | Reglas deterministicas, no IA |

Senal de distractor: si una regla fija resuelve el problema con exactitud, no elijas un modelo complejo solo porque suena moderno.

## RAG, prompt engineering, fine-tuning, pre-training y agentes

| Situacion | Respuesta mas probable | Descarte tipico |
|---|---|---|
| Datos internos cambian con frecuencia | RAG | Fine-tuning queda desactualizado |
| Necesito citar fuentes | RAG | Prompt solo no garantiza fuentes |
| El modelo inventa politicas | RAG + grounding + validacion | Subir temperature empeora |
| Solo quiero JSON, tabla o tono formal | Prompt engineering | Pre-training es excesivo |
| Hay ejemplos buenos de estilo/tarea | Fine-tuning | RAG no cambia estilo por si solo |
| Quiero crear capacidades base nuevas | Pre-training | Muy costoso, raro en practitioner |
| Quiero modelo mas pequeno/barato | Distillation | No es prompt engineering |
| Debe consultar CRM y crear ticket | Agente con herramientas | RAG solo responde, no ejecuta |
| Debe planificar pasos | Agente | Clasificacion no basta |

## Flujo RAG correcto

Orden mental:

1. Documentos.
2. Chunking.
3. Embeddings.
4. Base vectorial.
5. Recuperacion.
6. Prompt con contexto.
7. Respuesta con citas o validacion.

Errores frecuentes:

- Recuperar antes de indexar.
- Elegir fine-tuning para documentos que cambian cada semana.
- Olvidar evaluar calidad de recuperacion.
- No validar salida cuando el caso es sensible.

## Parametros de inferencia

| Requisito | Ajuste |
|---|---|
| Consistencia | Temperature baja |
| Creatividad | Temperature mas alta |
| Menor costo | Reducir tokens/contexto/salida, cache de prompt, modelo mas pequeno |
| Menor latencia | Menos tokens, modelo adecuado, capacidad provisionada si aplica |
| Respuesta mas corta | Max output length menor |
| Mas contexto | Mayor input/context window, con cuidado por costo |

Regla: temperature alta no arregla exactitud. Para exactitud factual usa fuentes, RAG, validacion y evaluacion.

## Agentes

Elige agentes cuando el enunciado incluya:

- Varios pasos.
- Herramientas externas.
- Crear, actualizar o cancelar registros.
- Consultar sistemas.
- Memoria.
- Orquestacion.
- MCP.
- Multiagente.

Controles obligatorios:

- IAM o identidad con permisos minimos.
- Politicas de herramientas.
- Logs.
- Auditoria.
- Validacion de salida.
- Aprobacion humana para acciones sensibles.

Servicios/conceptos:

- Amazon Bedrock Agents.
- Amazon Bedrock AgentCore.
- AgentCore Identity.
- Strands Agents.
- MCP.

## IA responsable

| Pista | Respuesta probable |
|---|---|
| Grupo demografico perjudicado | Bias / fairness |
| Necesito explicar una decision | Explicabilidad |
| Documentar proposito, datos y riesgos | SageMaker Model Cards |
| Analizar sesgo | SageMaker Clarify |
| Monitorear drift o calidad | SageMaker Model Monitor |
| Decision de alto impacto | Human-in-the-loop / Amazon A2I |
| Bloquear contenido toxico | Bedrock Guardrails |
| Usuarios diversos | Inclusividad |
| Respuesta falsa plausible | Alucinacion / veracidad |

Distractor frecuente: alta precision global no elimina sesgo. Siempre revisa subgrupos.

## Seguridad y gobernanza

| Pista | Servicio/control |
|---|---|
| Permisos minimos | IAM |
| Cifrado | AWS KMS |
| Secretos | Secrets Manager |
| Datos sensibles en S3 | Macie |
| Trafico privado | PrivateLink |
| Llamadas API | CloudTrail |
| Logs y metricas | CloudWatch |
| Configuraciones | Config |
| Vulnerabilidades | Inspector |
| Evidencia de auditoria | Audit Manager |
| Reportes de cumplimiento | Artifact |
| Recomendaciones AWS | Trusted Advisor |
| Presupuestos | AWS Budgets |
| Analisis de costos | Cost Explorer |

## Riesgos GenAI y respuesta esperada

| Riesgo | Control |
|---|---|
| Prompt injection | Separar instrucciones/datos, guardrails, validacion |
| Data leakage | Minimo privilegio, filtrado de salida, no poner secretos en prompts |
| Poisoning de contexto | Curacion de fuentes, validacion, controles de ingesta |
| Alucinaciones | RAG grounding, citas, validacion, confidence scoring |
| Contenido toxico | Bedrock Guardrails |
| Acciones peligrosas de agente | Aprobacion humana, permisos minimos, logs |

## Evaluacion

| Caso | Metrica o enfoque |
|---|---|
| Clasificacion | Accuracy, precision, recall, F1 |
| Resumen | ROUGE |
| Traduccion | BLEU |
| Similitud semantica | BERTScore |
| Evaluacion asistida por modelo | LLM-as-a-judge |
| RAG | Relevancia, groundedness, citas, exactitud |
| Agentes | Tarea completada, herramientas correctas, coste, latencia, seguridad |
| Negocio | ROI, conversion, productividad, satisfaccion, costo por interaccion |

LLM-as-a-judge es util como apoyo, pero no es garantia absoluta. Para casos sensibles combina evaluacion humana, benchmarks y pruebas de negocio.

## Preguntas de seleccion multiple

Cuando diga "elige dos" o "elige tres":

- Cuenta cuantas respuestas pide.
- Busca requisitos independientes.
- No selecciones opciones redundantes si una no aporta.
- Desconfia de opciones absolutas: "siempre", "nunca", "garantiza".
- En seguridad, suele haber una combinacion de permisos, cifrado, logs, validacion o guardrails.

Ejemplo mental:

Pregunta: "Reducir fuga de datos en un agente GenAI".  
Buenas respuestas: permisos minimos + validacion/filtrado de salida.  
Malas respuestas: temperature maxima + secretos en prompt.

## Preguntas de orden

Patrones frecuentes:

RAG:

1. Dividir documentos.
2. Crear embeddings.
3. Indexar.
4. Recuperar.
5. Generar respuesta.

ML:

1. Definir problema.
2. Recolectar/preparar datos.
3. Entrenar.
4. Evaluar.
5. Desplegar.
6. Monitorear.

Gobernanza:

1. Definir politica.
2. Catalogar y controlar datos.
3. Implementar controles.
4. Monitorear/auditar.
5. Revisar y mejorar.

## Distractores tipicos

- Usar pre-training para un cambio de formato.
- Usar fine-tuning para documentos actualizados.
- Usar IAM para busqueda vectorial.
- Usar CloudWatch cuando preguntan "quien llamo una API" y no logs generales.
- Usar CloudTrail cuando preguntan metricas y alarmas.
- Usar KMS para detectar datos sensibles.
- Usar Macie para gestionar llaves.
- Usar GenAI cuando una regla deterministica basta.
- Usar RAG cuando la tarea requiere ejecutar acciones reales.

## Mini simulacion de decision

### Caso 1

Un asistente debe responder preguntas sobre politicas internas que cambian mensualmente y mostrar fuentes.

Respuesta: RAG con Knowledge Bases, embeddings, base vectorial, citas y validacion.

### Caso 2

Un banco predice si una transaccion es fraude usando historico etiquetado.

Respuesta: clasificacion supervisada, probablemente con SageMaker AI si se construye en AWS.

### Caso 3

Un modelo debe redactar respuestas en el estilo de la empresa y hay miles de ejemplos aprobados.

Respuesta: primero prompt/few-shot; si no basta, fine-tuning.

### Caso 4

Un agente debe consultar stock, crear pedido y enviar confirmacion.

Respuesta: agente con herramientas, permisos minimos, logs, validacion y posible aprobacion humana.

### Caso 5

Auditoria pregunta que usuario llamo a una API y cuando.

Respuesta: AWS CloudTrail.

## Ultima regla antes de marcar

Antes de elegir, pregunta:

1. La opcion resuelve el requisito principal?
2. Es el servicio correcto para ese tipo de dato?
3. Reduce el riesgo mencionado?
4. Es mas simple que las alternativas?
5. Esta dentro del alcance del examen?

Si una opcion suena potente pero no responde al requisito exacto, es distractor.
