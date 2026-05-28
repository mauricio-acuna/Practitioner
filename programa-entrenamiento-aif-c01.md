# Programa de entrenamiento AWS Certified AI Practitioner AIF-C01

Version: 2026-05-27  
Objetivo: aprobar AWS Certified AI Practitioner (AIF-C01) con practica enfocada en el temario oficial, casos de uso y razonamiento de examen.  
Nota: las preguntas de practica son originales, no son preguntas oficiales de AWS.

## Fuentes oficiales de base

- Guia oficial del examen: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/ai-practitioner-01.html
- Pagina de la certificacion: https://aws.amazon.com/certification/certified-ai-practitioner/
- Servicios dentro del alcance: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/aif-01-in-scope-services.html

## Material complementario creado

- `ejercicios-explicados-por-dominio-aif-c01.md`: 50 ejercicios por dominio con respuesta, explicacion y descarte de distractores.
- `matriz-decision-aif-c01.md`: guia rapida para elegir tecnica, servicio y control segun pistas del enunciado.
- `simulador-2-aif-c01.md`: segundo simulador completo de 65 preguntas con respuestas explicadas.
- `tarjetas-memoria-aif-c01.md`: tarjetas pregunta/respuesta por dominio para repaso espaciado.

## Criterio de idioma

Todo el material esta redactado en castellano. Mantengo algunos terminos tecnicos en ingles cuando son los nombres habituales del examen o de la documentacion AWS, por ejemplo `prompt`, `RAG`, `fine-tuning`, `embedding`, `guardrails`, `batch`, `real-time` y nombres oficiales de servicios. Cuando aparecen, se explican en castellano.

## Ficha del examen

- Certificacion: AWS Certified AI Practitioner.
- Codigo: AIF-C01.
- Nivel: Foundational.
- Duracion: 90 minutos.
- Formato: 65 preguntas.
- Puntuadas: 50 preguntas.
- No puntuadas: 15 preguntas no identificadas.
- Puntaje minimo: 700 sobre 1000.
- Tipos: opcion multiple, respuesta multiple, orden y emparejamiento.
- Sin penalizacion por adivinar.
- Idiomas: incluye Espanol de Espana y Espanol Latinoamerica.
- Costo publicado por AWS: 100 USD, sujeto a region/impuestos/cambio.

Regla de tiempo: 90 minutos / 65 preguntas = 1 minuto 23 segundos por pregunta. En practica, usa esta rutina:

1. Primera pasada: responde lo claro en menos de 60 segundos.
2. Marca dudas: no te bloquees con preguntas largas.
3. Segunda pasada: resuelve marcadas por descarte.
4. Ultimos 5 minutos: revisa solo preguntas marcadas y respuestas multiples.

## Pesos oficiales y objetivo de practica

| Dominio | Peso | Preguntas puntuadas estimadas | Objetivo de practica |
|---|---:|---:|---|
| 1. Fundamentos de IA y ML | 20% | 10 | 80% minimo |
| 2. Fundamentos de GenAI | 24% | 12 | 85% recomendado |
| 3. Aplicaciones de modelos fundacionales | 28% | 14 | 85% recomendado |
| 4. IA responsable | 14% | 7 | 80% minimo |
| 5. Seguridad, cumplimiento y gobernanza | 14% | 7 | 80% minimo |

Prioridad real: domina primero Dominio 3 y Dominio 2. Juntos explican 52% del contenido puntuado.

## Metodo para aprobar

Usa este ciclo cada dia:

1. Recordar: 10 minutos sin mirar apuntes.
2. Estudiar: 35 a 45 minutos con el mapa del dominio.
3. Practicar: 20 a 30 preguntas o planteos.
4. Corregir: escribe por que la respuesta correcta gana.
5. Repetir fallos: al dia siguiente, empieza por tus errores.

No basta memorizar servicios. El examen suele preguntar "que conviene para este caso", no "que significa esta sigla". Entrena decisiones.

## Plan de 21 dias

### Semana 1: base de IA, ML y AWS

Dia 1: examenes, pesos, formato, servicios principales.  
Dia 2: IA vs ML vs deep learning vs GenAI vs agentic AI.  
Dia 3: tipos de datos, aprendizaje supervisado, no supervisado y refuerzo.  
Dia 4: clasificacion, regresion, clustering, forecasting, recomendaciones y deteccion de fraude.  
Dia 5: ciclo de vida ML: datos, entrenamiento, evaluacion, despliegue, monitoreo, reentrenamiento.  
Dia 6: servicios AWS basicos: S3, EC2, Lambda, IAM, Bedrock, SageMaker AI.  
Dia 7: mini simulador de 25 preguntas y correccion.

Meta de la semana: explicar cualquier caso de uso con tecnica + servicio + metrica.

### Semana 2: GenAI y modelos fundacionales

Dia 8: tokens, embeddings, chunking, vectores, transformers, FMs, LLMs, modelos multimodales y difusion.  
Dia 9: prompt engineering: zero-shot, one-shot, few-shot, plantillas, instrucciones, contexto y negativos.  
Dia 10: RAG, bases de conocimiento, bases vectoriales y grounding.  
Dia 11: seleccion de modelos: costo, latencia, modalidad, longitud, region, personalizacion, compliance.  
Dia 12: fine-tuning, instruction tuning, pre-training, continuous pre-training, distillation y RLHF.  
Dia 13: agentes: herramientas, memoria, MCP, orquestacion, Bedrock Agents, Bedrock AgentCore, Strands Agents.  
Dia 14: simulador de 40 preguntas y correccion.

Meta de la semana: decidir entre prompt, RAG, fine-tuning, modelo custom y agente.

### Semana 3: responsable, seguridad, gobernanza y simulacion

Dia 15: IA responsable: bias, fairness, inclusividad, robustez, seguridad, veracidad.  
Dia 16: transparencia, explicabilidad, Model Cards, SageMaker Clarify, Bedrock Model Evaluation.  
Dia 17: seguridad: IAM, cifrado, PrivateLink, Macie, KMS, Secrets Manager, Guardrails.  
Dia 18: cumplimiento y gobernanza: CloudTrail, CloudWatch, Config, Audit Manager, Artifact, Trusted Advisor.  
Dia 19: simulador completo de 65 preguntas con reloj.  
Dia 20: repaso de errores y tarjetas de memoria.  
Dia 21: simulador final. Si haces 80% o mas dos veces, agenda el examen.

Meta final: 80% global minimo y 75% minimo en cada dominio. Ideal: 85% global.

## Plan acelerado de 7 dias

Dia 1: ficha del examen + Dominio 1.  
Dia 2: Dominio 2 completo.  
Dia 3: Dominio 3 parte 1: seleccion de modelos, RAG y prompt engineering.  
Dia 4: Dominio 3 parte 2: fine-tuning, agentes y evaluacion.  
Dia 5: Dominio 4 + Dominio 5.  
Dia 6: simulador completo + correccion profunda.  
Dia 7: repaso de fallos + segundo simulador.

## Dominio 1: Fundamentos de IA y ML

### Debes saber explicar

- IA: sistemas que realizan tareas que parecen requerir inteligencia humana.
- ML: subcampo de IA donde los sistemas aprenden patrones desde datos.
- Deep learning: ML con redes neuronales profundas.
- GenAI: modelos que generan contenido nuevo: texto, imagen, audio, video, codigo.
- Agentic AI: sistemas que planifican, usan herramientas, mantienen contexto/memoria y ejecutan tareas de varios pasos.
- Modelo: artefacto entrenado que produce predicciones o generaciones.
- Algoritmo: metodo usado para entrenar o resolver una tarea.
- Entrenamiento: ajuste del modelo con datos.
- Inferencia: uso del modelo para generar predicciones/respuestas.
- Bias: sesgo sistematico en datos, modelo o resultado.
- Fairness: evaluacion de impacto equitativo entre grupos.
- Fit: ajuste del modelo; underfitting generaliza mal por simplicidad, overfitting memoriza entrenamiento.

### Tipos de aprendizaje

| Tipo | Cuando usarlo | Ejemplo |
|---|---|---|
| Supervisado | Datos etiquetados | predecir fraude: fraude/no fraude |
| No supervisado | Datos sin etiquetas | segmentar clientes por comportamiento |
| Refuerzo | Aprender acciones por recompensas | optimizar decisiones secuenciales |

### Tecnicas por caso

| Necesidad | Tecnica probable |
|---|---|
| Predecir numero | Regresion |
| Predecir categoria | Clasificacion |
| Agrupar sin etiquetas | Clustering |
| Predecir valores futuros en el tiempo | Forecasting |
| Encontrar rarezas | Anomaly detection |
| Recomendar productos | Sistemas de recomendacion |
| Extraer texto de documentos | OCR / document AI |
| Entender texto | NLP |
| Identificar objetos en imagen | Computer vision |

### Tipos de inferencia

- Batch: muchas predicciones juntas, no requiere respuesta inmediata.
- Real-time: baja latencia para usuarios/aplicaciones interactivas.
- Asincrona: trabajos largos o grandes, resultado posterior.
- Serverless: despliegue sin gestionar servidores, escala bajo demanda.

### Servicios AWS que suelen aparecer

- Amazon SageMaker AI: crear, entrenar, desplegar y operar modelos ML.
- Amazon Bedrock: construir aplicaciones GenAI con modelos fundacionales.
- Amazon Transcribe: audio a texto.
- Amazon Translate: traduccion.
- Amazon Comprehend: NLP, entidades, sentimiento, temas.
- Amazon Lex: chatbots/voz conversacional.
- Amazon Polly: texto a voz.
- Amazon Rekognition: vision artificial.
- Amazon Personalize: recomendaciones.
- Amazon Textract: extraer texto/datos de documentos.

### Errores tipicos

- Usar ML cuando el resultado debe ser exacto y determinista.
- Elegir GenAI para una clasificacion simple con datos tabulares y explicabilidad fuerte.
- Confundir entrenamiento con inferencia.
- Confundir regresion con clasificacion.
- Confundir embeddings con el texto original.

### Ejercicios con respuesta

1. Una empresa quiere predecir el importe de ventas del mes siguiente. Que tecnica conviene?  
Respuesta: forecasting o regresion sobre series temporales, segun el planteo. Si el foco es tiempo, forecasting.

2. Un banco tiene transacciones etiquetadas como fraude/no fraude. Que aprendizaje usa?  
Respuesta: supervisado, probablemente clasificacion binaria.

3. Marketing quiere descubrir grupos naturales de clientes sin etiquetas previas.  
Respuesta: aprendizaje no supervisado con clustering.

4. Un sistema debe convertir llamadas grabadas a texto. Que servicio AWS conviene?  
Respuesta: Amazon Transcribe.

5. Una app necesita leer facturas escaneadas y extraer campos.  
Respuesta: Amazon Textract.

## Dominio 2: Fundamentos de GenAI

### Conceptos clave

- Token: unidad de texto procesada por el modelo. Puede ser palabra, parte de palabra o simbolo.
- Chunking: dividir documentos en fragmentos para indexacion, RAG o procesamiento.
- Embedding: representacion numerica de significado.
- Vector: lista numerica que permite comparar similitud semantica.
- Foundation model: modelo grande preentrenado adaptable a multiples tareas.
- LLM: modelo fundacional enfocado en lenguaje.
- Modelo multimodal: trabaja con mas de una modalidad, como texto e imagen.
- Modelo de difusion: comun en generacion de imagenes.
- Prompt engineering: disenar instrucciones, contexto y ejemplos para guiar el modelo.
- Context engineering: preparar y administrar contexto, memoria, herramientas, politicas y datos que recibe el modelo.
- Agentic AI: modelos que pueden razonar sobre pasos, llamar herramientas y coordinar acciones.
- MCP: protocolo para conectar agentes con herramientas/sistemas externos de forma estandarizada.

### Capacidades de GenAI

- Resumir.
- Generar contenido.
- Asistir conversaciones.
- Traducir.
- Generar codigo.
- Responder sobre documentos con RAG.
- Automatizar atencion al cliente.
- Crear imagen, audio o video.
- Ayudar en busqueda semantica.

### Limitaciones y riesgos

- Hallucinations: respuestas plausibles pero falsas.
- No determinismo: puede variar entre ejecuciones.
- Latencia y costo por tokens.
- Riesgo de datos sensibles en prompts.
- Interpretabilidad limitada.
- Prompt injection, jailbreaking, poisoning.
- Sesgos y respuestas toxicas.

### Seleccion de modelo

Evalua:

- Modalidad: texto, imagen, audio, multimodal.
- Costo por token y volumen esperado.
- Latencia requerida.
- Longitud de entrada/salida.
- Region y disponibilidad.
- Privacidad y compliance.
- Necesidad de citar fuentes.
- Necesidad de personalizacion.
- Calidad contra tus metricas de negocio.
- Soporte de herramientas/agentes.

### Ciclo de vida FM

1. Seleccion de datos.
2. Seleccion de modelo.
3. Pre-training o uso de modelo preentrenado.
4. Fine-tuning si hace falta.
5. Evaluacion tecnica y humana.
6. Despliegue.
7. Observabilidad, feedback, seguridad y mejora continua.

### Servicios y tecnologias AWS

- Amazon Bedrock: acceso a modelos fundacionales, guardrails, agentes, knowledge bases, evaluacion.
- Amazon SageMaker AI: entrenamiento, despliegue y MLOps.
- SageMaker JumpStart: modelos y soluciones preconstruidas.
- Amazon Q: asistentes GenAI para productividad y trabajo con datos/codigo/negocio.
- Kiro: desarrollo asistido por IA.
- Strands Agents: construccion de agentes.
- Amazon Bedrock AgentCore: ejecutar, escalar y asegurar agentes.

### Ejercicios con respuesta

1. Un prompt largo se repite para miles de consultas. Que problema mirar primero?  
Respuesta: costo y latencia por tokens; considerar prompt caching, reducir contexto o RAG.

2. Un asistente debe responder usando documentos internos y citar fuentes.  
Respuesta: RAG con una base de conocimiento; en AWS, Amazon Bedrock Knowledge Bases.

3. El modelo inventa politicas internas. Que tecnica ayuda?  
Respuesta: grounding con RAG, validacion de salida, guardrails y evaluacion.

4. Se necesita generar imagenes de productos. Que tipo de modelo puede ser relevante?  
Respuesta: modelo multimodal o de difusion, segun capacidades.

5. Un agente debe consultar CRM y crear tickets. Que conceptos entran?  
Respuesta: herramientas, permisos, memoria/contexto, orquestacion, identidad, auditoria y posiblemente MCP.

## Dominio 3: Aplicaciones de modelos fundacionales

### Decidir entre prompt, RAG, fine-tuning y pre-training

| Situacion | Mejor primera opcion | Motivo |
|---|---|---|
| Mejorar formato, tono o estructura | Prompt engineering | Barato, rapido, reversible |
| Responder con datos privados o actualizados | RAG | Mantiene datos fuera del entrenamiento y permite citas |
| Enseñar estilo o tarea repetitiva especifica | Fine-tuning | Ajusta comportamiento del modelo |
| Crear capacidades de base nuevas con muchisimos datos | Pre-training | Costoso, raro para nivel practitioner |
| Reducir modelo grande a uno menor | Distillation | Costo/latencia menor |
| Tarea con varios pasos y sistemas externos | Agente | Usa herramientas y orquestacion |

### RAG en una frase

RAG recupera informacion relevante desde una fuente externa y la agrega al prompt para que el modelo responda con contexto actualizado o privado.

Componentes tipicos:

1. Documentos.
2. Chunking.
3. Embeddings.
4. Base vectorial.
5. Recuperacion por similitud.
6. Prompt con contexto recuperado.
7. Respuesta con citas/validacion.

AWS para embeddings/vector search:

- Amazon OpenSearch Service.
- Amazon Aurora.
- Amazon Neptune.
- Amazon RDS for PostgreSQL.
- Amazon Bedrock Knowledge Bases como capa administrada para RAG.

### Parametros de inferencia

- Temperature baja: respuestas mas consistentes y conservadoras.
- Temperature alta: mas diversidad/creatividad, tambien mas riesgo.
- Max output length: controla longitud/costo.
- Input length: contexto disponible, pero mas tokens implican mas costo/latencia.

### Prompt engineering

Tecnicas:

- Zero-shot: sin ejemplos.
- One-shot/single-shot: un ejemplo.
- Few-shot: varios ejemplos.
- Chain-of-thought: guiar razonamiento paso a paso; en producto, normalmente pedir una explicacion breve, no razonamiento interno extenso.
- Prompt templates: formato reutilizable.
- Negative prompts: indicar que evitar, comun en generacion visual y guardrails de salida.
- Prompt routing: dirigir solicitudes al modelo o flujo adecuado.
- Versionado y gestion de prompts: administrar cambios, pruebas, modelos, parametros y resultados; Amazon Bedrock Prompt Management aparece en la revision 1.1 del temario.

Buenas practicas:

- Rol + tarea + contexto + formato + restricciones.
- Ser especifico y conciso.
- Probar variantes.
- Separar datos de instrucciones.
- Validar salidas.
- Usar guardrails para politicas.

Riesgos:

- Prompt injection.
- Jailbreaking.
- Exposicion de datos.
- Poisoning de contexto.
- Dependencia excesiva de instrucciones en vez de controles reales.

### Evaluacion de FMs

Tecnica:

- Evaluacion humana.
- Benchmarks.
- Amazon Bedrock Model Evaluation.
- Evaluacion de RAG: relevancia de recuperacion, groundedness, citas, exactitud.
- Evaluacion de agentes: exito de tarea, llamadas correctas a herramientas, seguridad, costo, latencia.

Metricas:

- ROUGE: resumen, solapamiento con referencia.
- BLEU: traduccion, coincidencia con referencia.
- BERTScore: similitud semantica.
- LLM-as-a-judge: usar otro modelo para asistir en la evaluacion de salidas, sin tratarlo como verdad absoluta.
- Exactitud, precision, recall, F1 cuando aplique.
- Negocio: productividad, engagement, conversion, costo por usuario, ROI, satisfaccion, tasa de finalizacion de tarea y costo por interaccion.

### Ejercicios con respuesta

1. Tienes politicas internas que cambian semanalmente. Que evita reentrenar?  
Respuesta: RAG con documentos actualizados.

2. El bot debe crear una orden, consultar stock y enviar email.  
Respuesta: agente con herramientas, permisos y auditoria.

3. Quieres respuestas mas creativas para ideas de campanas.  
Respuesta: subir temperature, dentro de limites y con evaluacion.

4. Quieres respuestas consistentes para soporte regulado.  
Respuesta: temperature baja, RAG, guardrails, validacion y logs.

5. El modelo ya sabe el dominio, pero debe responder en estilo juridico interno.  
Respuesta: primero prompt/few-shot; si no basta y hay ejemplos de calidad, fine-tuning.

## Dominio 4: IA responsable

### Principios que debes dominar

- Bias: sesgo en datos o resultados.
- Fairness: tratamiento equitativo entre grupos.
- Inclusividad: considerar usuarios diversos.
- Robustez: comportamiento estable ante variaciones.
- Seguridad: evitar danos y usos indebidos.
- Veracidad: reducir falsedades y alucinaciones.
- Transparencia: informar uso, limites y fuentes.
- Explicabilidad: poder justificar decisiones.

### Herramientas AWS relevantes

- Amazon Bedrock Guardrails: politicas de seguridad, filtros, temas bloqueados, controles de salida.
- SageMaker Clarify: sesgo y explicabilidad.
- SageMaker Model Monitor: monitoreo de calidad/drift.
- SageMaker Model Cards: documentacion del modelo.
- Amazon Bedrock Model Evaluation: evaluar modelos fundacionales.
- Amazon A2I: revision humana.

### Riesgos legales y de confianza

- Infraccion de propiedad intelectual.
- Salidas sesgadas.
- Perdida de confianza del cliente.
- Riesgo para usuario final.
- Hallucinations.
- Datos no representativos.
- Falta de explicabilidad.

### Ejercicios con respuesta

1. Un modelo rechaza mas solicitudes de un grupo demografico. Que analizar?  
Respuesta: sesgo/fairness con analisis por subgrupos, datos balanceados y SageMaker Clarify.

2. Un caso de alto impacto requiere revision antes de decidir.  
Respuesta: human-in-the-loop con Amazon A2I o proceso equivalente.

3. La organizacion necesita documentar uso, datos, riesgos y evaluacion del modelo.  
Respuesta: SageMaker Model Cards.

4. Un chatbot produce lenguaje toxico.  
Respuesta: Amazon Bedrock Guardrails, filtros, evaluacion y monitoreo.

5. Un modelo muy preciso no se puede explicar y se usa para decisiones sensibles.  
Respuesta: existe tradeoff entre performance y explicabilidad; evaluar modelo mas interpretable o controles adicionales.

## Dominio 5: Seguridad, cumplimiento y gobernanza

### Seguridad para IA

Debes conectar IA con seguridad cloud clasica:

- IAM roles, policies y permisos minimos.
- Cifrado en reposo y en transito.
- AWS KMS para llaves.
- AWS Secrets Manager para secretos.
- Amazon Macie para datos sensibles en S3.
- AWS PrivateLink para conectividad privada.
- CloudTrail para auditoria.
- CloudWatch para logs/metricas.
- Guardrails para entradas/salidas de GenAI.
- Validacion de salida para reducir datos peligrosos o incorrectos.
- Data lineage y catalogacion para origen de datos.

### Riesgos de seguridad en GenAI

- Prompt injection: el usuario intenta cambiar instrucciones o exfiltrar datos.
- Data leakage: el modelo expone informacion sensible.
- Poisoning: datos/contexto malicioso contamina respuestas.
- Hallucination: salida falsa con apariencia de verdad.
- Toxicidad o contenido inseguro.
- Uso de herramientas sin permisos minimos.
- Logs con datos sensibles.

### Gobernanza y compliance

Servicios:

- AWS Config: evaluar configuraciones contra reglas.
- Amazon Inspector: vulnerabilidades.
- AWS Audit Manager: evidencias para auditorias.
- AWS Artifact: reportes/acuerdos de cumplimiento.
- AWS CloudTrail: registro de llamadas API.
- AWS Trusted Advisor: recomendaciones.
- Amazon CloudWatch: monitoreo y observabilidad.

Practicas:

- Politicas claras.
- Cadencia de revision.
- Retencion y residencia de datos.
- Data lifecycle.
- Logging y auditoria.
- Entrenamiento del equipo.
- Matriz de alcance de seguridad para IA generativa.
- Transparencia de uso de IA.

### Ejercicios con respuesta

1. El equipo necesita saber quien llamo a una API de AWS y cuando.  
Respuesta: AWS CloudTrail.

2. Se requiere evidencias para auditoria de cumplimiento.  
Respuesta: AWS Audit Manager y AWS Artifact, segun evidencia/reporte requerido.

3. Hay riesgo de datos personales en buckets S3.  
Respuesta: Amazon Macie.

4. El agente necesita acceder a herramientas externas. Que principio gobierna permisos?  
Respuesta: minimo privilegio con IAM/identidad del agente, politicas, logs y aprobaciones.

5. El sistema debe evitar respuestas no fundamentadas.  
Respuesta: RAG grounding, citas, confidence scoring, validacion de salida y guardrails.

## Tabla rapida de servicios AWS

| Servicio | Para que recordarlo en AIF-C01 |
|---|---|
| Amazon Bedrock | GenAI con FMs, agentes, knowledge bases, guardrails, evaluacion |
| Amazon Bedrock Knowledge Bases | RAG administrado |
| Amazon Bedrock Guardrails | Politicas de seguridad y control de contenido |
| Amazon Bedrock AgentCore | Ejecucion/seguridad/operacion de agentes |
| Amazon SageMaker AI | ML end-to-end: build, train, deploy, monitor |
| SageMaker JumpStart | Modelos/soluciones preentrenadas |
| SageMaker Clarify | Sesgo y explicabilidad |
| SageMaker Model Monitor | Monitoreo de modelos |
| SageMaker Model Cards | Documentacion de modelos |
| Amazon A2I | Revision humana |
| Amazon Comprehend | NLP administrado |
| Amazon Lex | Chatbots y voz conversacional |
| Amazon Polly | Texto a voz |
| Amazon Transcribe | Voz a texto |
| Amazon Translate | Traduccion |
| Amazon Rekognition | Vision artificial |
| Amazon Personalize | Recomendaciones |
| Amazon Textract | Extraccion de documentos |
| Amazon Kendra | Busqueda empresarial inteligente |
| Amazon Q | Asistente GenAI AWS/negocio/desarrollo |
| Amazon Nova | Familia de modelos fundacionales de AWS |
| Amazon OpenSearch Service | Busqueda, observabilidad y vector search |
| Amazon Aurora | Base relacional, puede soportar vectores segun configuracion |
| Amazon RDS for PostgreSQL | Relacional, vectores con extensiones como pgvector |
| Amazon Neptune | Grafo, util para relaciones/conocimiento |
| Amazon S3 | Almacenamiento de datos/documentos |
| AWS Glue | ETL/catalogo de datos |
| AWS Lake Formation | Gobernanza de data lake |
| AWS IAM | Identidad y permisos |
| AWS KMS | Llaves y cifrado |
| Amazon Macie | Descubrir datos sensibles |
| AWS PrivateLink | Acceso privado a servicios |
| AWS CloudTrail | Auditoria de llamadas API |
| Amazon CloudWatch | Logs, metricas, alarmas |
| AWS Config | Cumplimiento de configuracion |
| AWS Audit Manager | Evidencia de auditoria |
| AWS Artifact | Reportes/acuerdos de cumplimiento |
| Amazon Inspector | Vulnerabilidades |
| AWS Trusted Advisor | Recomendaciones de buenas practicas |
| AWS Budgets | Presupuestos |
| AWS Cost Explorer | Analisis de costos |

## Checklist completa de servicios dentro del alcance

No todos aparecen con la misma profundidad, pero conviene reconocerlos por categoria.

### Analitica

- AWS Data Exchange.
- Amazon EMR.
- AWS Glue.
- AWS Glue DataBrew.
- AWS Lake Formation.
- Amazon OpenSearch Service.
- Amazon Quick.
- Amazon Redshift.

### Gestion financiera en la nube

- AWS Budgets.
- AWS Cost Explorer.

### Computo

- Amazon EC2.
- AWS Lambda.

### Containers

- Amazon ECS.
- Amazon EKS.

### Database

- Amazon Aurora.
- Amazon DocumentDB.
- Amazon DynamoDB.
- Amazon ElastiCache.
- Amazon Neptune.
- Amazon RDS.

### Herramientas para desarrolladores

- Kiro.
- Strands Agents.
- Amazon Q.

### Machine Learning / Aprendizaje automatico

- Amazon A2I.
- Amazon Bedrock.
- Amazon Bedrock AgentCore.
- Amazon Comprehend.
- Amazon Kendra.
- Amazon Lex.
- Amazon Nova.
- Amazon Personalize.
- Amazon Polly.
- Amazon Rekognition.
- Amazon SageMaker AI.
- Amazon SageMaker JumpStart.
- Amazon Textract.
- Amazon Transcribe.
- Amazon Translate.
- AWS Transform.

### Administracion y gobernanza

- AWS CloudTrail.
- Amazon CloudWatch.
- AWS Config.
- AWS Trusted Advisor.
- AWS Well-Architected Tool.

### Redes y entrega de contenido

- Amazon CloudFront.
- Amazon VPC.

### Seguridad, identidad y cumplimiento

- AWS Artifact.
- AWS Audit Manager.
- AWS IAM.
- Amazon Inspector.
- AWS KMS.
- Amazon Macie.
- AWS Secrets Manager.

### Almacenamiento

- Amazon S3.
- Amazon S3 Glacier.

## Planteos integradores

### Planteo 1

Una empresa de soporte quiere un chatbot que responda preguntas sobre manuales internos. Los manuales cambian cada semana. La empresa necesita citas a fuentes.

Respuesta esperada:

- Usar RAG.
- En AWS: Amazon Bedrock Knowledge Bases.
- Guardar documentos en S3 y generar embeddings.
- Usar base vectorial administrada/compatible.
- Agregar citas y validacion de salida.
- No conviene fine-tuning como primera opcion porque los datos cambian seguido.

### Planteo 2

Una fintech quiere aprobar/rechazar solicitudes con datos tabulares historicos y necesita explicar decisiones a auditores.

Respuesta esperada:

- ML supervisado de clasificacion.
- SageMaker AI para entrenamiento/despliegue.
- SageMaker Clarify para sesgo/explicabilidad.
- Model Cards para documentacion.
- CloudTrail/CloudWatch para auditoria/observabilidad.
- GenAI no es la primera opcion si se requiere decision tabular explicable.

### Planteo 3

Marketing quiere generar ideas creativas de campanas y variantes de texto. La exactitud factual no es critica, pero se deben evitar marcas prohibidas.

Respuesta esperada:

- GenAI con Amazon Bedrock.
- Prompt templates y temperature moderada/alta.
- Guardrails o validacion para marcas prohibidas.
- Medir utilidad por conversion, engagement o feedback humano.

### Planteo 4

Una organizacion quiere que un agente consulte stock, cree tickets y actualice un CRM.

Respuesta esperada:

- Agentic AI.
- Herramientas con permisos minimos.
- Bedrock Agents/AgentCore o Strands Agents, segun arquitectura.
- Logs, auditoria, validacion y control humano si hay acciones sensibles.
- MCP puede ayudar a conectar agentes con sistemas externos de forma estandar.

### Planteo 5

Un modelo de resumen produce textos fluidos pero omite datos importantes.

Respuesta esperada:

- Evaluar con ROUGE si hay referencia, evaluacion humana y metricas de negocio.
- Mejorar prompt y contexto.
- Si resume documentos internos, usar RAG/grounding.
- Ajustar longitud maxima y validar salidas.

## Simulador AIF-C01: 65 preguntas

Instrucciones: responde en 90 minutos. En preguntas "elige dos" o "elige tres", debes seleccionar todas las correctas.

### Preguntas

1. Una solucion predice si un correo es spam o no spam a partir de correos etiquetados. Que tipo de aprendizaje usa?
   A. No supervisado  
   B. Supervisado  
   C. Refuerzo  
   D. Pre-training generativo

2. Una empresa quiere agrupar clientes sin categorias previas. Que tecnica corresponde?
   A. Clasificacion  
   B. Regresion  
   C. Clustering  
   D. Traduccion automatica

3. Cual es la diferencia mas correcta entre entrenamiento e inferencia?
   A. Entrenamiento usa el modelo; inferencia crea los datos  
   B. Entrenamiento ajusta el modelo; inferencia usa el modelo para responder  
   C. Entrenamiento siempre es serverless; inferencia siempre es batch  
   D. No hay diferencia en ML moderno

4. Un equipo quiere convertir audio de reuniones a texto. Que servicio AWS es mas adecuado?
   A. Amazon Polly  
   B. Amazon Transcribe  
   C. Amazon Translate  
   D. Amazon Rekognition

5. Una aplicacion debe generar voz a partir de texto. Que servicio conviene?
   A. Amazon Polly  
   B. Amazon Textract  
   C. Amazon Comprehend  
   D. Amazon Personalize

6. Una prediccion numerica como "importe esperado de compra" se modela normalmente como:
   A. Clasificacion  
   B. Regresion  
   C. Clustering  
   D. OCR

7. El overfitting ocurre cuando un modelo:
   A. No aprende suficientes patrones del entrenamiento  
   B. Memoriza demasiado el entrenamiento y generaliza mal  
   C. No usa datos etiquetados  
   D. Solo funciona con datos no estructurados

8. Que opcion representa datos no estructurados?
   A. Tabla de ventas con columnas fijas  
   B. Imagenes y correos de texto libre  
   C. Registro CSV con esquema rigido  
   D. Tabla relacional normalizada

9. Un sistema necesita procesar miles de predicciones durante la noche sin latencia interactiva. Que tipo de inferencia encaja mejor?
   A. Batch  
   B. Real-time  
   C. Manual  
   D. Prompt injection

10. Una empresa requiere resultado exacto y determinista basado en reglas fiscales simples. Que afirmacion es mejor?
   A. Usar siempre GenAI porque es mas moderno  
   B. Usar IA solo si no hay datos  
   C. Una solucion basada en reglas puede ser mas apropiada que ML  
   D. Fine-tuning siempre elimina errores

11. En GenAI, un token es:
   A. Una unidad de procesamiento de texto del modelo  
   B. Una politica IAM  
   C. Un bucket S3  
   D. Un reporte de compliance

12. Para busqueda semantica, los embeddings sirven para:
   A. Cifrar datos con KMS  
   B. Representar significado como vectores comparables  
   C. Crear roles IAM  
   D. Ejecutar contenedores

13. Que riesgo describe una respuesta plausible pero falsa de un LLM?
   A. Hallucination  
   B. Batch inference  
   C. Clustering  
   D. Data warehouse

14. El costo de inferencia de muchos servicios GenAI suele depender de:
   A. Numero de buckets creados  
   B. Tokens de entrada/salida y capacidad provisionada si aplica  
   C. Numero de usuarios IAM solamente  
   D. Cantidad de VPCs

15. Elige dos casos tipicos para GenAI.
   A. Resumen de documentos  
   B. Reemplazo de CloudTrail  
   C. Generacion de codigo  
   D. Asignacion de permisos IAM minimos  
   E. Configuracion de subredes

16. Un modelo multimodal puede:
   A. Trabajar con mas de una modalidad como texto e imagen  
   B. Solo procesar numeros tabulares  
   C. Evitar toda alucinacion  
   D. Reemplazar cifrado

17. Que concepto se refiere a dividir documentos en fragmentos antes de indexarlos para RAG?
   A. Chunking  
   B. Distillation  
   C. IAM policy  
   D. Temperature

18. En una aplicacion agentic AI, el uso de herramientas significa:
   A. Que el agente puede llamar sistemas externos o funciones para completar tareas  
   B. Que el modelo no requiere permisos  
   C. Que no se necesitan logs  
   D. Que el entrenamiento es obligatorio

19. Que describe mejor MCP en el contexto de agentes?
   A. Un metodo de cifrado de S3  
   B. Un protocolo para conectar agentes con herramientas/sistemas externos  
   C. Un benchmark de traduccion  
   D. Un tipo de base relacional

20. El no determinismo en GenAI significa que:
   A. El modelo siempre devuelve la misma salida exacta  
   B. El modelo puede variar respuestas entre ejecuciones  
   C. El modelo no usa tokens  
   D. El modelo solo trabaja en batch

21. Una empresa necesita menor barrera de entrada para probar FMs sin administrar infraestructura de entrenamiento. Que servicio es mas directo?
   A. Amazon Bedrock  
   B. Amazon EC2 Auto Scaling solamente  
   C. AWS Artifact  
   D. Amazon Macie

22. Elige dos factores clave al seleccionar un modelo fundacional.
   A. Latencia requerida  
   B. Color del logo del proveedor  
   C. Modalidad de entrada/salida  
   D. Numero de zonas horarias del equipo  
   E. Nombre del bucket

23. Una base de conocimiento para responder con datos internos actualizados se implementa normalmente con:
   A. RAG  
   B. Solo temperature alta  
   C. AWS Budgets  
   D. Amazon Polly

24. Que servicio de AWS se asocia directamente con Knowledge Bases para RAG?
   A. Amazon Bedrock  
   B. Amazon Inspector  
   C. AWS Artifact  
   D. Amazon CloudFront

25. Elige dos almacenes/servicios que pueden ayudar a almacenar o buscar embeddings.
   A. Amazon OpenSearch Service  
   B. AWS IAM  
   C. Amazon Aurora  
   D. AWS Budgets  
   E. Amazon Polly

26. Una temperature mas baja suele producir:
   A. Respuestas mas consistentes  
   B. Respuestas mas aleatorias  
   C. Mas permisos IAM  
   D. Menos necesidad de datos

27. Few-shot prompting significa:
   A. Dar varios ejemplos en el prompt  
   B. Entrenar desde cero  
   C. Cifrar salida  
   D. Crear una VPC

28. Cual es el mejor primer paso para cambiar el formato de respuesta de un LLM?
   A. Prompt engineering  
   B. Pre-training desde cero  
   C. Comprar mas dominios DNS  
   D. Desactivar logs

29. Una empresa tiene ejemplos de alta calidad y quiere adaptar estilo/tarea del modelo despues de probar prompts. Que tecnica puede considerar?
   A. Fine-tuning  
   B. Clustering  
   C. CloudTrail  
   D. OCR

30. Pre-training de un FM suele ser:
   A. Barato y rapido para cualquier empresa  
   B. Costoso y usado para crear capacidades base con grandes datos  
   C. Igual que cambiar un prompt  
   D. Un servicio de auditoria

31. Para evaluar traduccion con referencia, que metrica podria aparecer?
   A. BLEU  
   B. KMS  
   C. VPC  
   D. IAM

32. Para evaluar resumen con referencia, que metrica podria aparecer?
   A. ROUGE  
   B. S3 Glacier  
   C. Inspector  
   D. PrivateLink

33. Un agente debe completar una tarea de varios pasos. Que capacidad es mas relevante?
   A. Orquestacion y uso de herramientas  
   B. Solo batch inference  
   C. Solo datos no estructurados  
   D. Solo cifrado de disco

34. Prompt injection es:
   A. Un ataque que intenta manipular instrucciones o contexto del modelo  
   B. Un algoritmo de clustering  
   C. Un formato de imagen  
   D. Una metrica de resumen

35. Ordena un flujo RAG basico:
   A. Generar embeddings e indexar  
   B. Responder con contexto recuperado  
   C. Dividir documentos en chunks  
   D. Recuperar chunks relevantes para la consulta

36. Cual es una razon para usar prompt caching?
   A. Reducir costo/latencia de contexto repetido  
   B. Eliminar necesidad de IAM  
   C. Convertir audio a texto  
   D. Hacer auditorias de compliance

37. SageMaker Clarify se asocia principalmente con:
   A. Sesgo y explicabilidad  
   B. Presupuestos  
   C. CDN  
   D. Texto a voz

38. Una Model Card ayuda a:
   A. Documentar proposito, datos, riesgos y evaluacion de un modelo  
   B. Traducir texto  
   C. Crear redes VPC  
   D. Reemplazar CloudTrail

39. Amazon Bedrock Guardrails se usa para:
   A. Controlar politicas de contenido y seguridad en apps GenAI  
   B. Generar facturas  
   C. Administrar certificados SSL solamente  
   D. Crear tablas SQL

40. Elige dos caracteristicas de IA responsable.
   A. Fairness  
   B. Robustez  
   C. Mas tokens siempre  
   D. Sin logs nunca  
   E. Ignorar subgrupos

41. Un dataset de entrenamiento debe ser:
   A. Representativo, diverso y curado  
   B. Siempre pequeno  
   C. Siempre sin etiquetas  
   D. Sin revisar por temas de calidad

42. Para decisiones de alto impacto, un mecanismo recomendable es:
   A. Revision humana  
   B. Desactivar auditoria  
   C. Aumentar temperature al maximo  
   D. Evitar explicaciones

43. Que expresa mejor el tradeoff entre seguridad y transparencia?
   A. A veces un modelo mas interpretable puede rendir menos, y un modelo mas potente puede ser menos explicable  
   B. La transparencia elimina toda necesidad de seguridad  
   C. La seguridad solo aplica a redes, no a IA  
   D. Ningun modelo puede explicarse

44. Que servicio registra llamadas API para auditoria?
   A. AWS CloudTrail  
   B. Amazon Polly  
   C. Amazon Translate  
   D. Amazon Personalize

45. Para detectar datos sensibles en S3, usa:
   A. Amazon Macie  
   B. Amazon Lex  
   C. Amazon Rekognition  
   D. Amazon Neptune

46. El principio de minimo privilegio se implementa principalmente con:
   A. IAM roles, policies y permisos adecuados  
   B. Temperature alta  
   C. BLEU  
   D. Chunking

47. Para gestionar llaves de cifrado, AWS ofrece:
   A. AWS KMS  
   B. Amazon Comprehend  
   C. Amazon Polly  
   D. SageMaker Clarify

48. AWS Artifact se usa para:
   A. Acceder a reportes/acuerdos de cumplimiento  
   B. Entrenar embeddings  
   C. Generar voz  
   D. Crear prompts

49. Elige dos controles para reducir data leakage en GenAI.
   A. Filtrado/validacion de salida  
   B. Permisos minimos y control de acceso a datos  
   C. Publicar prompts con secretos  
   D. Desactivar logging de auditoria siempre  
   E. Usar temperature maxima

50. Que practica ayuda a demostrar origen de datos?
   A. Data lineage y catalogacion  
   B. Usar nombres cortos de variables  
   C. Aumentar max tokens  
   D. Desactivar metadatos

51. Una empresa quiere recomendaciones personalizadas de productos. Que servicio AWS es mas directo?
   A. Amazon Personalize  
   B. Amazon Transcribe  
   C. AWS Artifact  
   D. Amazon Macie

52. Una empresa quiere detectar objetos inapropiados en imagenes. Que servicio puede aplicar?
   A. Amazon Rekognition  
   B. AWS Budgets  
   C. Amazon Translate  
   D. AWS Config

53. Un equipo necesita controlar gasto de pruebas GenAI. Que servicios ayudan?
   A. AWS Budgets y AWS Cost Explorer  
   B. Amazon Polly y Textract  
   C. Amazon Lex y Rekognition  
   D. AWS Artifact y Transcribe

54. El modelo responde bien, pero la app no sabe si cumple objetivos de negocio. Que debes medir?
   A. ROI, productividad, engagement, conversion o satisfaccion, segun caso  
   B. Solo numero de parametros del modelo  
   C. Solo color de interfaz  
   D. Solo cantidad de prompts escritos

55. Una empresa necesita extraer entidades y sentimiento de texto. Que servicio conviene?
   A. Amazon Comprehend  
   B. Amazon Polly  
   C. Amazon Inspector  
   D. AWS KMS

56. Para evaluar configuraciones contra reglas de cumplimiento en AWS:
   A. AWS Config  
   B. Amazon Translate  
   C. Amazon Nova  
   D. Amazon Personalize

57. Una app GenAI regulada requiere conectividad privada a servicios sin exponer trafico a internet publico. Que tecnologia puede ayudar?
   A. AWS PrivateLink  
   B. ROUGE  
   C. Amazon Polly  
   D. Few-shot prompting

58. Un chatbot en atencion al cliente debe hablar con usuarios por voz y texto. Que servicio historico de AWS para bots conversacionales es relevante?
   A. Amazon Lex  
   B. Amazon S3 Glacier  
   C. AWS Audit Manager  
   D. Amazon EMR

59. Que opcion combina mejor exactitud factual y datos privados en respuestas GenAI?
   A. RAG + citas + validacion  
   B. Temperature maxima sin fuentes  
   C. Solo modelo base sin contexto  
   D. Desactivar guardrails

60. Que afirmacion sobre modelo de responsabilidad compartida es correcta?
   A. AWS y el cliente comparten responsabilidades; AWS protege la nube y el cliente configura/protege lo que usa  
   B. AWS siempre es responsable de todos los prompts del cliente  
   C. El cliente nunca configura IAM  
   D. No aplica a soluciones de IA

61. Para vulnerabilidades en cargas de trabajo, que servicio del alcance puede ayudar?
   A. Amazon Inspector  
   B. Amazon Polly  
   C. Amazon Translate  
   D. Amazon Textract

62. Una organizacion quiere buscar en documentos empresariales con capacidades inteligentes. Que servicio puede aparecer?
   A. Amazon Kendra  
   B. AWS Budgets  
   C. Amazon EC2 solamente  
   D. AWS Artifact

63. Que opcion describe mejor BERTScore?
   A. Metrica de similitud semantica para evaluar texto generado  
   B. Servicio de cifrado  
   C. Tipo de permiso IAM  
   D. Formato de imagen

64. Elige tres practicas de gobernanza para IA.
   A. Politicas y revision periodica  
   B. Retencion/residencia de datos definida  
   C. Entrenamiento del equipo  
   D. Secretos dentro del prompt  
   E. Sin trazabilidad de decisiones

65. Antes del examen, cual es la mejor senal de preparacion?
   A. Dos simuladores cronometrados con 80-85% y revision de errores  
   B. Leer solo nombres de servicios una vez  
   C. Memorizar siglas sin casos de uso  
   D. Evitar preguntas de respuesta multiple

### Respuestas y explicaciones

1. B. Datos etiquetados implican aprendizaje supervisado.
2. C. Clustering agrupa sin etiquetas.
3. B. Entrenamiento ajusta; inferencia usa.
4. B. Transcribe convierte audio a texto.
5. A. Polly convierte texto a voz.
6. B. Regresion predice valores numericos.
7. B. Overfitting memoriza y generaliza mal.
8. B. Imagenes y texto libre son no estructurados.
9. A. Batch encaja con procesamiento masivo no interactivo.
10. C. Si el resultado debe ser determinista, reglas pueden ganar.
11. A. Token es unidad de texto/procesamiento.
12. B. Embeddings representan significado en vectores.
13. A. Hallucination es salida falsa plausible.
14. B. GenAI suele cobrarse por tokens/capacidad.
15. A y C. Resumen y codigo son casos tipicos GenAI.
16. A. Multimodal combina modalidades.
17. A. Chunking divide documentos.
18. A. Herramientas permiten actuar fuera del modelo.
19. B. MCP conecta agentes con herramientas/sistemas.
20. B. No determinismo implica variacion posible.
21. A. Bedrock da acceso administrado a FMs.
22. A y C. Latencia y modalidad son criterios reales.
23. A. RAG combina recuperacion y generacion.
24. A. Knowledge Bases pertenece a Amazon Bedrock.
25. A y C. OpenSearch y Aurora pueden soportar busqueda/vector.
26. A. Baja temperature da salidas mas consistentes.
27. A. Few-shot incluye varios ejemplos.
28. A. Cambios de formato se intentan primero con prompt.
29. A. Fine-tuning adapta comportamiento con ejemplos.
30. B. Pre-training es costoso y base.
31. A. BLEU se asocia a traduccion.
32. A. ROUGE se asocia a resumen.
33. A. Agentes orquestan pasos y herramientas.
34. A. Prompt injection manipula instrucciones/contexto.
35. Orden correcto: C, A, D, B. Primero chunks, luego embeddings/index, recuperar, responder.
36. A. Prompt caching reduce repeticion de tokens/costo/latencia.
37. A. Clarify: sesgo y explicabilidad.
38. A. Model Cards documentan modelos.
39. A. Guardrails controla seguridad/contenido.
40. A y B. Fairness y robustez son principios.
41. A. Datos representativos/diversos/curados reducen riesgo.
42. A. Human-in-the-loop reduce riesgo en alto impacto.
43. A. Existe tradeoff entre interpretabilidad, seguridad y performance.
44. A. CloudTrail registra llamadas API.
45. A. Macie detecta datos sensibles en S3.
46. A. Minimo privilegio se implementa con IAM.
47. A. KMS gestiona llaves.
48. A. Artifact da reportes/acuerdos de cumplimiento.
49. A y B. Validacion y control de acceso reducen fuga.
50. A. Lineage/catalogacion documentan origen.
51. A. Personalize es para recomendaciones.
52. A. Rekognition trabaja con imagen/video.
53. A. Budgets y Cost Explorer ayudan con gasto.
54. A. Hay que medir metricas de negocio.
55. A. Comprehend analiza texto.
56. A. Config evalua configuraciones.
57. A. PrivateLink da conectividad privada.
58. A. Lex es para bots conversacionales.
59. A. RAG con citas/validacion mejora grounding.
60. A. Modelo compartido: AWS de la nube, cliente en la nube.
61. A. Inspector ayuda con vulnerabilidades.
62. A. Kendra es busqueda empresarial inteligente.
63. A. BERTScore evalua similitud semantica.
64. A, B y C. Politicas, datos y entrenamiento son gobernanza.
65. A. Simuladores cronometrados con revision son la mejor senal.

## Tarjetas de memoria rapida

- Clasificacion: categoria.
- Regresion: numero.
- Clustering: grupos sin etiquetas.
- Forecasting: futuro en serie temporal.
- Transcribe: voz a texto.
- Polly: texto a voz.
- Translate: traduccion.
- Comprehend: NLP administrado.
- Rekognition: imagen/video.
- Textract: documentos.
- Personalize: recomendaciones.
- Bedrock: GenAI con FMs.
- SageMaker AI: ML end-to-end.
- Clarify: sesgo/explicabilidad.
- Model Monitor: monitoreo de modelos.
- Model Cards: documentacion.
- A2I: revision humana.
- Guardrails: politicas de GenAI.
- Knowledge Bases: RAG en Bedrock.
- Embedding: significado como vector.
- Chunking: dividir documentos.
- RAG: recuperar + generar.
- Fine-tuning: adaptar modelo con ejemplos.
- Pre-training: entrenar base.
- Distillation: modelo menor imita a mayor.
- Temperature alta: creatividad/variacion.
- Temperature baja: consistencia.
- ROUGE: resumen.
- BLEU: traduccion.
- BERTScore: similitud semantica.
- CloudTrail: auditoria API.
- CloudWatch: logs/metricas.
- Config: configuracion/compliance.
- Audit Manager: evidencia de auditoria.
- Artifact: reportes/acuerdos.
- Macie: datos sensibles.
- KMS: llaves.
- IAM: permisos.
- PrivateLink: conectividad privada.
- Inspector: vulnerabilidades.

## Checklist de dia anterior

- Hice al menos 2 simuladores cronometrados.
- Revise todas las respuestas multiples falladas.
- Puedo explicar RAG vs fine-tuning vs prompt engineering.
- Puedo elegir servicios AWS por caso de uso.
- Puedo explicar bias, fairness, transparencia y guardrails.
- Puedo explicar IAM, CloudTrail, Macie, KMS, Config, Artifact y Audit Manager.
- Tengo claro que no hay penalizacion por adivinar.
- Se que debo marcar dudas y avanzar.

## Plantilla para corregir errores

Usa esta tabla despues de cada simulador:

| Pregunta | Dominio | Mi respuesta | Correcta | Por que falle | Regla para no repetir |
|---|---|---|---|---|---|
| | | | | | |

Ejemplo:

| Pregunta | Dominio | Mi respuesta | Correcta | Por que falle | Regla para no repetir |
|---|---|---|---|---|---|
| 25 | 3 | IAM | OpenSearch/Aurora | Confundi permisos con vector search | Embeddings viven en bases/vector search, no en IAM |

## Regla final de examen

Cuando dudes, pregunta:

1. Es IA clasica/ML, GenAI, RAG, agente o seguridad?
2. El caso requiere prediccion, generacion, recuperacion, accion o gobernanza?
3. Hay datos etiquetados, datos privados, necesidad de citas, baja latencia, compliance o explicabilidad?
4. Que opcion resuelve el requisito con menos complejidad y mas control?

La respuesta correcta suele ser la que satisface el caso de negocio, reduce riesgo y usa el servicio administrado mas adecuado.
