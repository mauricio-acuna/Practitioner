# Dominio de contenido 1: Aspectos basicos de la IA y el ML

Fuente oficial: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/ai-practitioner-01-domain1.html  
Peso en el examen: 20% del contenido puntuado.

[Volver al indice](ai-practitioner-01.md)

## Que evalua este dominio

Este dominio comprueba que puedas explicar conceptos basicos de inteligencia artificial, machine learning y aprendizaje profundo, reconocer casos de uso practicos y describir el ciclo de vida de desarrollo de soluciones IA/ML.

## Tareas del dominio

1. Explicar conceptos y terminologia basica de IA.
2. Identificar casos de uso practicos para IA.
3. Describir el ciclo de vida de desarrollo IA/ML.

## 1.1 Conceptos basicos

Debes poder definir:

- IA: sistemas que realizan tareas asociadas a inteligencia humana.
- ML: subcampo de IA donde los sistemas aprenden patrones desde datos.
- Deep learning: aprendizaje automatico basado en redes neuronales profundas.
- Redes neuronales: modelos inspirados en capas de unidades conectadas que aprenden patrones.
- NLP: procesamiento de lenguaje natural.
- Computer vision: analisis de imagenes y video.
- Modelo: artefacto que produce predicciones o respuestas.
- Algoritmo: metodo usado para entrenar o resolver una tarea.
- Entrenamiento: ajuste del modelo con datos.
- Inferencia: uso del modelo entrenado para predecir o responder.
- Bias: sesgo sistematico en datos, modelo o resultados.
- Fairness: evaluacion de trato equitativo entre grupos.
- Fit: nivel de ajuste del modelo a los datos.
- LLM: modelo grande de lenguaje.
- GenAI: IA que genera contenido nuevo.
- Agentic AI: sistemas que planifican, usan herramientas y ejecutan tareas de varios pasos.

## Relaciones importantes

| Concepto | Como recordarlo |
|---|---|
| IA | Campo amplio |
| ML | IA que aprende desde datos |
| Deep learning | ML con redes neuronales profundas |
| GenAI | Genera contenido nuevo |
| Agentic AI | Usa modelos, herramientas, memoria y orquestacion |

## Tipos de inferencia

| Tipo | Cuando conviene |
|---|---|
| Batch / por lotes | Muchas predicciones sin urgencia |
| Real-time / tiempo real | Respuesta inmediata o baja latencia |
| Asincrona | Trabajos largos cuyo resultado puede llegar despues |
| Serverless / sin servidor | Escalado bajo demanda sin gestionar servidores |

## Tipos de datos

- Etiquetados: tienen respuesta conocida, utiles para aprendizaje supervisado.
- No etiquetados: no tienen respuesta previa, utiles para clustering o exploracion.
- Tabulares: filas y columnas.
- Series temporales: datos ordenados por tiempo.
- Imagen, texto y audio: normalmente no estructurados.
- Estructurados: esquema definido.
- No estructurados: texto libre, imagenes, audio, video.

## Tipos de aprendizaje

| Tipo | Entrada | Salida tipica |
|---|---|---|
| Supervisado | Datos etiquetados | Clasificacion o regresion |
| No supervisado | Datos sin etiquetas | Clustering, patrones ocultos |
| Refuerzo | Estados, acciones y recompensas | Politicas de decision |

## 1.2 Casos de uso practicos

IA/ML puede aportar valor cuando necesitas:

- Escalar decisiones.
- Automatizar procesos repetitivos.
- Asistir a personas con recomendaciones o analisis.
- Detectar patrones dificiles de codificar con reglas.
- Trabajar con texto, imagen, audio o grandes volumenes de datos.

IA/ML puede no ser apropiado cuando:

- La regla es simple y deterministica.
- Se necesita una salida exacta y auditable sin incertidumbre.
- No hay datos suficientes o de calidad.
- El costo y el riesgo superan el valor esperado.
- El requisito de explicabilidad es incompatible con el modelo elegido.

## Tecnicas por caso

| Caso | Tecnica |
|---|---|
| Predecir categoria | Clasificacion |
| Predecir numero | Regresion |
| Agrupar sin etiquetas | Clustering |
| Detectar anomalias | Deteccion de anomalias |
| Predecir futuro por tiempo | Forecasting |
| Recomendar productos | Sistemas de recomendacion |
| Leer documentos | OCR / document AI |
| Analizar texto | NLP |
| Analizar imagen/video | Vision artificial |

## Servicios AWS que debes reconocer

| Servicio | Uso principal |
|---|---|
| Amazon SageMaker AI | Crear, entrenar, desplegar y operar modelos ML |
| Amazon Bedrock | Crear aplicaciones GenAI con modelos fundacionales |
| Amazon Q | Asistente generativo |
| Amazon Quick | Servicio incluido por AWS dentro del alcance oficial en la categoria de analitica |
| Kiro | Herramienta de desarrollo asistida |
| Amazon Transcribe | Voz a texto |
| Amazon Translate | Traduccion |
| Amazon Comprehend | NLP, entidades, sentimiento |
| Amazon Lex | Bots conversacionales |
| Amazon Polly | Texto a voz |

## 1.3 Ciclo de vida IA/ML

Etapas tipicas:

1. Definir problema de negocio.
2. Recolectar y preparar datos.
3. Seleccionar tecnica o modelo.
4. Entrenar o configurar.
5. Evaluar con metricas tecnicas y de negocio.
6. Desplegar.
7. Monitorear.
8. Reentrenar o ajustar cuando cambian datos/requisitos.

## MLOps basico

MLOps busca que el trabajo de ML sea repetible, escalable y listo para produccion. Incluye:

- Experimentacion controlada.
- Versionado de datos/modelos/configuraciones.
- Procesos repetibles.
- Monitoreo de rendimiento.
- Deteccion de drift.
- Reentrenamiento.
- Gestion de deuda tecnica.

## Metricas

| Metrica | Para que sirve |
|---|---|
| Accuracy | Proporcion global de aciertos |
| Precision | De los positivos predichos, cuantos eran correctos |
| Recall | De los positivos reales, cuantos encontro |
| F1 | Balance entre precision y recall |
| ROI | Retorno de inversion |
| Coste por usuario | Evaluacion economica |
| Feedback del cliente | Valor percibido |

## Errores comunes

- Confundir clasificacion con regresion.
- Usar GenAI para un problema tabular simple y regulado.
- Confundir entrenamiento con inferencia.
- Elegir IA cuando una regla deterministica basta.
- Olvidar metricas de negocio.
- Confundir metricas tecnicas buenas con valor real para el negocio.

## Checklist profesional del dominio

- Puedo diferenciar IA, ML, deep learning, GenAI y agentic AI.
- Puedo explicar aprendizaje supervisado, no supervisado y por refuerzo.
- Puedo elegir clasificacion, regresion, clustering o forecasting por caso.
- Puedo decidir cuando no usar IA.
- Puedo mapear servicios administrados de AWS a casos de uso.
- Puedo describir un pipeline IA/ML y conceptos basicos de MLOps.
- Puedo explicar accuracy, precision, recall, F1 y metricas de negocio.

## Ejercicios rapidos

1. Una prediccion de "fraude/no fraude" con etiquetas historicas es clasificacion supervisada.
2. Una prediccion de importe de venta es regresion.
3. Agrupar clientes sin categorias previas es clustering.
4. Convertir audio a texto usa Amazon Transcribe.
5. Si el resultado debe ser exacto por regla fija, una regla deterministica puede ser mejor que IA.
