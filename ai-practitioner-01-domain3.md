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
| Resolver con ejemplos dentro del prompt | In-context learning / few-shot prompting |
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

## Senales para elegir respuesta en examen

- Si la informacion cambia con frecuencia, requiere fuentes o viene de documentos privados: piensa en RAG.
- Si el problema es formato, tono, estructura o cumplimiento de instrucciones: piensa en prompt engineering.
- Si el modelo necesita aprender un estilo, patron de respuesta o dominio con ejemplos persistentes: piensa en fine-tuning.
- Si la empresa quiere adaptar conocimiento amplio del modelo con muchos datos de dominio: piensa en continuous pre-training.
- Si la prioridad es bajar costo o latencia manteniendo comportamiento similar: piensa en distillation.
- Si el caso implica varios pasos, herramientas, memoria o ejecucion de acciones: piensa en agentes.
- Si el caso es de alto riesgo, regulado o sensible: combina controles, guardrails, evaluacion humana, logs y permisos minimos.

## Tabla de decision rapida

| Pista del enunciado | Respuesta probable | Motivo |
|---|---|---|
| "Necesitamos respuestas con citas sobre politicas internas" | RAG / Bedrock Knowledge Bases | Grounding con datos propios |
| "La respuesta debe estar siempre en JSON" | Prompt template y validacion | Control de formato |
| "El modelo ignora instrucciones ocasionalmente" | Mejor prompt, ejemplos, guardrails y pruebas | El problema es comportamiento de inferencia |
| "Los documentos cambian cada semana" | RAG | Evita reentrenar por cada cambio |
| "Se desea un modelo mas pequeno y barato" | Distillation | Reduce costo/latencia |
| "Debe usar APIs corporativas para completar tareas" | Agente con permisos minimos | Necesita herramientas y accion |
| "Necesitamos comparar dos modelos para resumen" | ROUGE, evaluacion humana, Bedrock Model Evaluation | Metricas y revision adecuadas |
| "La calidad depende de que recupere documentos correctos" | Evaluacion RAG | Hay que medir recuperacion y respuesta |

## Coste y complejidad de personalizacion

De menor a mayor esfuerzo aproximado:

1. Prompt engineering: rapido, barato, ideal para formato e instrucciones.
2. In-context learning: incluye ejemplos en el prompt, util sin cambiar el modelo.
3. RAG: agrega datos externos y actualizados; requiere recuperacion, embeddings y base vectorial.
4. Fine-tuning: ajusta el modelo con ejemplos; mas costoso que prompts/RAG.
5. Continuous pre-training: adapta conocimiento amplio del modelo con grandes datos de dominio.
6. Pre-training: entrenamiento desde cero; normalmente el mas caro y complejo.

## Evaluacion por tipo de aplicacion

| Aplicacion | Que medir |
|---|---|
| Chatbot de soporte | Exactitud, satisfaccion, tasa de resolucion, escalamiento humano |
| Resumen de documentos | ROUGE, evaluacion humana, cobertura, fidelidad |
| Traduccion | BLEU, fluidez, terminologia, revision humana |
| Busqueda/RAG | Relevancia de documentos, groundedness, citas, precision de respuesta |
| Agente | Tarea completada, herramientas correctas, errores, permisos, latencia y costo |
| Workflow GenAI | Pasos completados, fallos, reintentos, aprobaciones humanas, valor de negocio |

## Mini casos resueltos

### Caso 1

Una empresa quiere que un asistente responda preguntas sobre contratos internos y muestre la fuente exacta usada.

Respuesta: RAG con Amazon Bedrock Knowledge Bases, una base vectorial compatible y citacion de fuentes. Fine-tuning no es la mejor primera opcion porque el objetivo principal es usar datos privados recuperables y verificables.

### Caso 2

Un equipo ya tiene buenas respuestas, pero quiere que salgan siempre con la misma estructura y campos.

Respuesta: prompt template, ejemplos few-shot y validacion del formato. Si el formato es critico, no dependas solo del prompt; valida la salida en la aplicacion.

### Caso 3

Un asistente debe revisar tickets, consultar un sistema externo y crear una tarea si falta informacion.

Respuesta: agente con herramientas autorizadas, permisos minimos, logs y aprobacion humana si la accion tiene impacto. La clave no es solo generar texto, sino ejecutar pasos.

### Caso 4

Un modelo grande funciona bien, pero es caro para miles de interacciones diarias simples.

Respuesta: evaluar un modelo mas pequeno o usar distillation. Tambien conviene revisar longitud de entrada/salida, cache de prompt y eleccion de modelo.

### Caso 5

Un modelo responde con informacion plausible pero no verificable en un caso regulado.

Respuesta: bajar variabilidad, usar RAG con fuentes autorizadas, aplicar guardrails, validar salida y agregar revision humana cuando el riesgo lo justifique.

## Preguntas tipo examen

1. Una organizacion necesita respuestas sobre documentacion interna que cambia con frecuencia. Que enfoque minimiza mantenimiento y mejora grounding?
   - Respuesta: RAG.

2. Que metrica se asocia mas con evaluacion de resumen?
   - Respuesta: ROUGE.

3. Que tecnica permite adaptar un modelo a una tarea con ejemplos en el prompt, sin modificar pesos?
   - Respuesta: in-context learning / few-shot prompting.

4. Que control es clave cuando un agente puede llamar herramientas externas?
   - Respuesta: permisos minimos, validacion de herramientas, logs y aprobacion humana para acciones sensibles.

5. Que tecnica suele ser mas adecuada si quieres reducir coste y latencia de un modelo grande manteniendo comportamiento parecido?
   - Respuesta: distillation.

6. Que debes evaluar en una aplicacion RAG ademas de la respuesta final?
   - Respuesta: calidad de recuperacion, relevancia, citas, cobertura y groundedness.

## Diferencias que suelen confundirse

| Conceptos | Diferencia clave |
|---|---|
| RAG vs fine-tuning | RAG recupera informacion externa; fine-tuning ajusta comportamiento del modelo |
| Prompt engineering vs in-context learning | Prompt engineering disena instrucciones; in-context learning aprende del ejemplo dentro del prompt |
| Fine-tuning vs continuous pre-training | Fine-tuning adapta tarea/estilo; continuous pre-training amplia conocimiento con datos de dominio |
| Modelo vs aplicacion | El modelo genera; la aplicacion agrega contexto, herramientas, validacion, UI, logs y controles |
| Evaluacion de modelo vs evaluacion de negocio | La primera mide calidad tecnica; la segunda mide valor real, productividad, satisfaccion y coste |
| Guardrails vs prompt | Guardrails son controles de seguridad; el prompt no debe ser el unico mecanismo de control |
| Agente vs chatbot simple | El agente planifica, usa herramientas y puede ejecutar acciones |

## Mapa mental por objetivo oficial

### Objetivo 3.1

Debes saber disenar aplicaciones con FMs:

- Elegir modelo por costo, modalidad, latencia, idioma, tamano, complejidad, region y compliance.
- Ajustar parametros de inferencia segun creatividad, consistencia, costo y latencia.
- Usar RAG cuando hacen falta datos externos, privados, actuales o verificables.
- Reconocer bases vectoriales compatibles para embeddings.
- Comparar personalizacion por costo y complejidad.
- Identificar cuando conviene usar agentes.

### Objetivo 3.2

Debes elegir tecnicas de prompt:

- Zero-shot para tareas simples sin ejemplos.
- One-shot o few-shot cuando quieres mostrar patron de respuesta.
- Prompt templates para reutilizacion y consistencia.
- Negative prompts para indicar que evitar.
- Guardrails y validacion para reducir riesgo.
- Versionado de prompts para comparar, auditar y revertir.

### Objetivo 3.3

Debes entender entrenamiento y ajuste:

- Pre-training crea o aprende capacidades generales.
- Continuous pre-training adapta conocimiento amplio con mas datos.
- Fine-tuning ajusta el modelo para una tarea, estilo o dominio especifico.
- Instruction tuning mejora seguimiento de instrucciones.
- RLHF usa feedback humano para alinear respuestas.
- Distillation transfiere comportamiento a un modelo mas pequeno.

### Objetivo 3.4

Debes evaluar rendimiento:

- Usa benchmarks y datasets de prueba cuando sean relevantes.
- Usa evaluacion humana para calidad, utilidad, tono y riesgos.
- Usa metricas como ROUGE, BLEU, BERTScore o LLM-as-a-judge segun tarea.
- Evalua la aplicacion completa, no solo el modelo.
- Conecta metricas tecnicas con productividad, satisfaccion, engagement y costo por interaccion.

## Mas preguntas de practica

1. Un asistente debe responder en varios idiomas y con baja latencia. Que criterios debes revisar al elegir el FM?
   - Respuesta: soporte multilingue, latencia, region, costo, tamano del modelo y longitud de entrada/salida.

2. Una empresa quiere probar rapidamente si un modelo puede clasificar correos sin entrenarlo. Que tecnica usa primero?
   - Respuesta: zero-shot o few-shot prompting.

3. Una aplicacion repite el mismo contexto largo en muchas llamadas. Que factor puede ayudar a reducir costo o latencia?
   - Respuesta: prompt caching, ademas de optimizar longitud de contexto.

4. Que tecnica mejora la respuesta con documentos recuperados desde una base vectorial?
   - Respuesta: RAG.

5. Que riesgo ocurre cuando contenido malicioso dentro de un documento recuperado intenta cambiar instrucciones del sistema?
   - Respuesta: prompt injection o poisoning del contexto.

6. Que enfoque usar si la prioridad es que el modelo siga mejor instrucciones en un formato concreto despues de entrenarlo con ejemplos?
   - Respuesta: instruction tuning o fine-tuning, segun el caso.

7. Que opcion es mejor para tareas reguladas: temperature alta o baja?
   - Respuesta: temperature baja, con grounding, guardrails y validacion.

8. Que debes revisar si una opcion del examen propone que "el prompt garantiza seguridad"?
   - Respuesta: es sospechosa; los controles reales deben estar fuera del prompt.

9. Que mide la tasa de finalizacion de tarea?
   - Respuesta: si la aplicacion completa correctamente el objetivo del usuario.

10. Que enfoque ayuda a comparar respuestas de modelos usando otro modelo como evaluador?
   - Respuesta: LLM-as-a-judge, idealmente con calibracion y revision humana.
