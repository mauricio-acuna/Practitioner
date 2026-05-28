# Tarjetas de memoria AIF-C01

Uso: tapa la respuesta, contesta en voz alta y marca las falladas. Repite las falladas al dia siguiente.

## Dominio 1: IA y ML

| Frente | Reverso |
|---|---|
| Que es IA? | Sistemas que realizan tareas asociadas a inteligencia humana. |
| Que es ML? | Subcampo de IA donde los sistemas aprenden patrones desde datos. |
| Que es deep learning? | ML basado en redes neuronales profundas. |
| Que es GenAI? | IA que genera contenido nuevo como texto, imagen, audio, video o codigo. |
| Que es agentic AI? | IA que planifica, usa herramientas, mantiene contexto/memoria y ejecuta tareas de varios pasos. |
| Clasificacion predice... | Una categoria o clase. |
| Regresion predice... | Un valor numerico. |
| Clustering sirve para... | Agrupar datos sin etiquetas previas. |
| Forecasting sirve para... | Predecir valores futuros en una serie temporal. |
| Aprendizaje supervisado usa... | Datos etiquetados. |
| Aprendizaje no supervisado usa... | Datos sin etiquetas. |
| Aprendizaje por refuerzo optimiza... | Acciones mediante recompensas. |
| Entrenamiento significa... | Ajustar un modelo con datos. |
| Inferencia significa... | Usar un modelo entrenado para responder o predecir. |
| Overfitting significa... | El modelo memoriza entrenamiento y generaliza mal. |
| Underfitting significa... | El modelo es demasiado simple y aprende poco. |
| Inferencia por lotes, o batch inference, es mejor cuando... | Se procesan muchas predicciones sin respuesta inmediata. |
| Inferencia en tiempo real, o real-time inference, es mejor cuando... | El usuario o sistema necesita baja latencia. |
| Inferencia sin servidor, o serverless inference, aporta... | Escalado bajo demanda sin administrar servidores. |
| Amazon Transcribe sirve para... | Voz/audio a texto. |
| Amazon Polly sirve para... | Texto a voz. |
| Amazon Translate sirve para... | Traduccion automatica. |
| Amazon Comprehend sirve para... | NLP: entidades, sentimiento, temas, texto. |
| Amazon Lex sirve para... | Bots conversacionales por voz/texto. |
| Amazon Rekognition sirve para... | Analisis de imagen y video. |
| Amazon Textract sirve para... | Extraer texto y datos de documentos. |
| Amazon Personalize sirve para... | Recomendaciones personalizadas. |
| Cuando NO usar IA/ML? | Cuando reglas simples deterministicas resuelven mejor, o costo/riesgo supera beneficio. |

## Dominio 2: GenAI

| Frente | Reverso |
|---|---|
| Token es... | Unidad de texto/procesamiento del modelo. |
| Embedding es... | Representacion numerica del significado. |
| Vector database permite... | Buscar similitud semantica entre embeddings. |
| Chunking es... | Dividir documentos en fragmentos. |
| Foundation model es... | Modelo grande preentrenado adaptable a varias tareas. |
| LLM es... | Modelo fundacional orientado a lenguaje. |
| Modelo multimodal trabaja con... | Mas de una modalidad, como texto e imagen. |
| Modelo de difusion se asocia con... | Generacion de imagenes. |
| Ingenieria de prompts, o prompt engineering, busca... | Guiar mejor al modelo con instrucciones, contexto y ejemplos. |
| Context engineering incluye... | Gestion de contexto, memoria, herramientas, politicas y datos. |
| Hallucination es... | Respuesta plausible pero falsa. |
| No determinismo significa... | La salida puede variar entre ejecuciones. |
| GenAI sirve muy bien para... | Resumen, asistentes, generacion de contenido/codigo, busqueda semantica. |
| GenAI es riesgosa para... | Decisiones criticas sin validacion, datos sensibles, respuestas factuales sin fuentes. |
| Costo GenAI suele depender de... | Tokens de entrada/salida, throughput, region, modelo y personalizacion. |
| Amazon Bedrock sirve para... | Crear aplicaciones GenAI con modelos fundacionales, agentes, bases de conocimiento, guardrails y evaluacion. |
| SageMaker JumpStart aporta... | Modelos y soluciones preconstruidas como punto de partida. |
| Amazon Q se asocia con... | Asistentes generativos para productividad, desarrollo y negocio. |
| Strands Agents se asocia con... | Construccion de agentes. |
| Bedrock AgentCore se asocia con... | Ejecucion, identidad, politicas y operacion de agentes. |

## Dominio 3: Aplicaciones de modelos fundacionales

| Frente | Reverso |
|---|---|
| RAG significa... | Generacion aumentada por recuperacion: recuperar informacion y agregarla al prompt. |
| RAG es mejor cuando... | Datos son privados, actualizados o requieren citas. |
| Fine-tuning es mejor cuando... | Hay ejemplos de calidad para adaptar estilo/tarea/comportamiento. |
| Ingenieria de prompts es mejor cuando... | Solo hay que mejorar formato, instrucciones, tono o estructura. |
| Pre-training es mejor cuando... | Se necesitan capacidades base nuevas con muchisimos datos y alto costo. |
| Distillation busca... | Que un modelo menor imite a uno mayor para bajar costo/latencia. |
| Continuous pre-training busca... | Ampliar/adaptar conocimiento base con datos de dominio. |
| RLHF significa... | Aprendizaje por refuerzo a partir de retroalimentacion humana. |
| Temperature baja produce... | Salidas mas consistentes y conservadoras. |
| Temperature alta produce... | Mas creatividad y variacion, con mas riesgo. |
| Zero-shot es... | Prompt sin ejemplos. |
| Single-shot/one-shot es... | Prompt con un ejemplo. |
| Few-shot es... | Prompt con varios ejemplos. |
| Negative prompt indica... | Que evitar. |
| Prompt injection intenta... | Manipular instrucciones/contexto para saltar controles o extraer datos. |
| Jailbreaking intenta... | Forzar al modelo a ignorar restricciones. |
| Prompt poisoning es... | Contaminar contexto/datos recuperados con instrucciones maliciosas. |
| Versionar prompts sirve para... | Comparar calidad, auditar cambios, revertir versiones y controlar comportamiento. |
| Amazon Bedrock Prompt Management se asocia con... | Gestion y versionado de prompts. |
| Amazon Bedrock Knowledge Bases sirve para... | Implementar RAG administrado. |
| OpenSearch/Aurora/Neptune/RDS PostgreSQL aparecen para... | Almacenar/buscar embeddings o soportar vector search. |
| ROUGE evalua... | Resumen contra referencia. |
| BLEU evalua... | Traduccion contra referencia. |
| BERTScore evalua... | Similitud semantica de texto generado. |
| LLM-as-a-judge es... | Evaluacion asistida por otro modelo; util, pero no verdad absoluta. |
| Bedrock Model Evaluation sirve para... | Evaluar modelos fundacionales. |
| Exito de agentes se mide por... | Cumplimiento de tarea, herramientas correctas, costo, latencia y seguridad. |

## Dominio 4: IA responsable

| Frente | Reverso |
|---|---|
| Bias es... | Sesgo sistematico en datos, modelo o resultados. |
| Fairness busca... | Tratamiento equitativo entre grupos. |
| Inclusividad en datos significa... | Representar diversidad de usuarios/casos. |
| Robustez significa... | Comportamiento estable ante variaciones o entradas inesperadas. |
| Veracidad busca... | Reducir falsedades y respuestas no fundamentadas. |
| Transparencia significa... | Comunicar uso, limites, fuentes y razones de decision. |
| Explicabilidad significa... | Poder entender o justificar por que el modelo produjo una salida. |
| SageMaker Clarify sirve para... | Sesgo y explicabilidad. |
| SageMaker Model Cards sirve para... | Documentar proposito, datos, riesgos y evaluacion del modelo. |
| SageMaker Model Monitor sirve para... | Monitorear calidad/drift en produccion. |
| Amazon A2I sirve para... | Revision humana. |
| Bedrock Guardrails sirve para... | Politicas de contenido, temas bloqueados y controles de seguridad. |
| Riesgos legales de GenAI incluyen... | IP, sesgos, alucinaciones, perdida de confianza y riesgo al usuario. |
| Dataset responsable debe ser... | Curado, representativo, diverso y balanceado cuando aplique. |

## Dominio 5: Seguridad, cumplimiento y gobernanza

| Frente | Reverso |
|---|---|
| IAM sirve para... | Identidad, roles, politicas y permisos minimos. |
| AWS KMS sirve para... | Gestion de llaves y cifrado. |
| AWS Secrets Manager sirve para... | Guardar y rotar secretos. |
| Amazon Macie sirve para... | Descubrir datos sensibles, especialmente en S3. |
| AWS PrivateLink sirve para... | Conectividad privada a servicios sin internet publico. |
| AWS CloudTrail sirve para... | Auditar llamadas API. |
| Amazon CloudWatch sirve para... | Logs, metricas y alarmas. |
| AWS Config sirve para... | Evaluar configuraciones contra reglas. |
| Amazon Inspector sirve para... | Gestion/deteccion de vulnerabilidades. |
| AWS Audit Manager sirve para... | Recopilar evidencias de auditoria. |
| AWS Artifact sirve para... | Reportes y acuerdos de cumplimiento. |
| AWS Trusted Advisor sirve para... | Recomendaciones de buenas practicas. |
| Data lineage significa... | Trazabilidad del origen y transformacion de datos. |
| Data residency significa... | Donde se almacenan/procesan datos segun region/requisitos. |
| Validacion de salida, u output validation, sirve para... | Reducir respuestas inseguras, falsas o con datos sensibles. |
| Confidence scoring ayuda a... | Estimar confianza para decidir validacion/revision. |
| Minimo privilegio significa... | Dar solo permisos necesarios para la tarea. |
| Modelo de responsabilidad compartida significa... | AWS protege la nube; el cliente configura y protege lo que usa en la nube. |
| Matriz de alcance de seguridad para IA generativa ayuda a... | Clasificar alcance/riesgo de soluciones GenAI y aplicar controles. |

## Como repetir

1. Repasa todas las tarjetas una vez.
2. Marca falladas con una X.
3. Repite solo falladas hasta contestarlas sin mirar.
4. Al dia siguiente, repite las falladas otra vez.
5. Antes del examen, haz una pasada completa cronometrada de 30 minutos.
