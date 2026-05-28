# Dominio de contenido 3: Aplicaciones de los modelos fundacionales

Fuente oficial: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/ai-practitioner-01-domain3.html  
Peso en el examen: 28% del contenido puntuado.

[Volver al indice](ai-practitioner-01.md)

## Que evalua este dominio

Este es el dominio con mas peso. Evalua si puedes disenar aplicaciones con modelos fundacionales, elegir tecnicas de prompts, entender entrenamiento/personalizacion y evaluar rendimiento de FMs.

## Tareas del dominio

1. Describir consideraciones de diseno para aplicaciones que usan FMs.
2. Elegir tecnicas efectivas de prompt engineering.
3. Describir entrenamiento y fine-tuning de FMs.
4. Describir metodos para evaluar FMs.

## 3.1 Diseno de aplicaciones con FMs

Al elegir un modelo preentrenado, considera:

- Costo.
- Modalidad.
- Latencia.
- Idiomas.
- Tamano del modelo.
- Complejidad.
- Personalizacion.
- Longitud de entrada y salida.
- Cache de prompt.
- Disponibilidad regional.
- Requisitos de compliance.

## Parametros de inferencia

| Parametro | Efecto |
|---|---|
| Temperature baja | Mas consistencia, menos creatividad |
| Temperature alta | Mas diversidad, mas riesgo |
| Longitud de entrada | Mas contexto, mas costo/latencia |
| Longitud de salida | Controla detalle, costo y latencia |

## RAG

RAG significa generacion aumentada por recuperacion. Recupera informacion externa y la agrega al contexto del modelo.

Usa RAG cuando:

- Los datos cambian con frecuencia.
- Necesitas citas o fuentes.
- La informacion es privada.
- No quieres reentrenar el modelo.
- Debes reducir alucinaciones mediante grounding.

En AWS, Amazon Bedrock Knowledge Bases es una opcion central para RAG.

## Vector databases y embeddings

Servicios dentro del alcance que pueden aparecer para almacenar o buscar embeddings:

- Amazon OpenSearch Service.
- Amazon Aurora.
- Amazon Neptune.
- Amazon RDS for PostgreSQL.

## Personalizacion de FMs

| Necesidad | Tecnica preferida |
|---|---|
| Mejorar instrucciones/formato | Prompt engineering |
| Usar datos privados/actualizados | RAG |
| Adaptar estilo o tarea con ejemplos | Fine-tuning |
| Ampliar conocimiento de base | Continuous pre-training |
| Crear capacidades desde cero | Pre-training |
| Reducir costo/latencia | Distillation |

## Agentes

Los agentes son utiles para tareas de varios pasos:

- Consultar sistemas.
- Llamar herramientas.
- Mantener memoria.
- Decidir pasos.
- Coordinar flujos.
- Ejecutar acciones.

Controles importantes:

- Permisos minimos.
- Validacion de herramientas.
- Logs.
- Auditoria.
- Aprobacion humana para acciones sensibles.

## 3.2 Prompt engineering

Elementos de un buen prompt:

- Rol.
- Tarea.
- Contexto.
- Instrucciones.
- Formato esperado.
- Restricciones.
- Ejemplos.

Tecnicas:

- Zero-shot: sin ejemplos.
- Single-shot / one-shot: un ejemplo.
- Few-shot: varios ejemplos.
- Chain-of-thought: guiar razonamiento paso a paso, cuando aplique.
- Prompt templates: plantillas reutilizables.
- Negative prompts: indicar que evitar.
- Prompt routing: dirigir solicitudes al modelo o flujo correcto.

## Versionado y gestion de prompts

La version 1.1 del temario agrega gestion y versionado de prompts. Para examen, recuerda:

- Un prompt es parte del comportamiento de la aplicacion y debe tratarse como artefacto versionado.
- Conviene registrar version, objetivo, modelo usado, parametros, dataset de prueba y resultado.
- Amazon Bedrock Prompt Management aparece como referencia para administrar prompts.
- Versionar prompts permite comparar calidad, revertir cambios y auditar por que cambio una salida.
- No sustituyas controles reales por prompts: los prompts ayudan, pero seguridad, permisos y validacion deben existir fuera del texto.

Buenas practicas:

- Ser especifico y conciso.
- Separar instrucciones de datos.
- Probar versiones.
- Usar guardrails.
- Medir calidad.
- Evitar incluir secretos.

Riesgos:

- Exposicion de datos.
- Poisoning del contexto.
- Hijacking.
- Jailbreaking.
- Prompt injection.

## 3.3 Entrenamiento y fine-tuning

Elementos clave:

- Pre-training.
- Fine-tuning.
- Continuous pre-training.
- Distillation.
- Instruction tuning.
- Transfer learning.
- RLHF.

Preparacion de datos:

- Curacion.
- Gobernanza.
- Tamano suficiente.
- Etiquetado si aplica.
- Representatividad.
- Calidad.
- Revision humana.

Regla mental: fine-tuning no es la primera respuesta si el problema es informacion actualizada o necesidad de citas. En ese caso, piensa primero en RAG.

## 3.4 Evaluacion de FMs

Enfoques:

- Evaluacion humana.
- Evaluacion human-in-the-loop.
- Benchmarks.
- Amazon Bedrock Model Evaluation.
- Evaluacion de aplicaciones RAG.
- Evaluacion de agentes y flujos.

Metricas:

| Metrica | Uso |
|---|---|
| ROUGE | Resumen |
| BLEU | Traduccion |
| BERTScore | Similitud semantica |
| LLM-as-a-judge | Evaluacion mediante otro modelo |
| Tasa de finalizacion de tarea | Porcentaje de tareas completadas correctamente |
| Satisfaccion de usuario | Percepcion de utilidad y calidad |
| Costo por interaccion | Coste unitario de uso de la aplicacion |

## Evaluar aplicaciones RAG, agentes y workflows

No basta evaluar el texto final. Tambien debes medir:

- Calidad de recuperacion en RAG: relevancia, cobertura, citas y groundedness.
- Calidad del agente: exito de tarea, llamadas correctas a herramientas, permisos, coste y latencia.
- Calidad del workflow: pasos completados, errores, reintentos, tiempos y controles humanos.
- Alineacion con negocio: productividad, engagement, satisfaccion, tasa de finalizacion y costo por interaccion.

## Errores comunes

- Usar fine-tuning para datos que cambian cada semana.
- Subir temperature en casos regulados.
- Olvidar evaluar RAG por calidad de recuperacion.
- Dar herramientas a agentes sin permisos minimos.
- Evaluar solo texto generado y no objetivo de negocio.
- No versionar prompts en aplicaciones que cambian con frecuencia.
- Confundir LLM-as-a-judge con garantia absoluta: es una tecnica de evaluacion, no una verdad final.

## Checklist profesional del dominio

- Puedo elegir entre prompt engineering, RAG, fine-tuning, pre-training y distillation.
- Puedo explicar RAG y sus componentes.
- Puedo reconocer bases vectoriales dentro del alcance.
- Puedo ajustar temperature y longitud de entrada/salida segun riesgo.
- Puedo aplicar tecnicas zero-shot, single-shot, few-shot, plantillas y negativos.
- Puedo explicar riesgos de prompts: injection, poisoning, hijacking y jailbreaking.
- Puedo explicar versionado y gestion de prompts.
- Puedo evaluar FMs, RAG, agentes y workflows con metricas tecnicas y de negocio.

## Ejercicios rapidos

1. Manuales internos cambiantes con citas: RAG.
2. Formato de respuesta incorrecto: prompt engineering.
3. Estilo especifico con muchos ejemplos: fine-tuning.
4. Respuestas creativas: temperature mas alta, con controles.
5. Respuestas reguladas: temperature baja, RAG, guardrails y validacion.
