# Dominio de contenido 2: Aspectos basicos de la IA generativa

Fuente oficial: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/ai-practitioner-01-domain2.html  
Peso en el examen: 24% del contenido puntuado.

[Volver al indice](ai-practitioner-01.md)

## Que evalua este dominio

Este dominio comprueba que entiendas los conceptos fundamentales de GenAI, sus ventajas y limitaciones para resolver problemas de negocio, y los servicios de AWS usados para construir aplicaciones generativas.

## Tareas del dominio

1. Explicar conceptos basicos de GenAI.
2. Comprender capacidades y limitaciones de GenAI para problemas empresariales.
3. Describir infraestructura y tecnologias AWS para crear aplicaciones GenAI.

## 2.1 Conceptos basicos de GenAI

| Concepto | Definicion para examen |
|---|---|
| Token | Unidad de texto que procesa el modelo |
| Chunking | Division de documentos en fragmentos |
| Embedding | Representacion numerica del significado |
| Vector | Lista numerica usada para similitud |
| Prompt engineering | Diseno de instrucciones, contexto y ejemplos |
| LLM | Modelo grande de lenguaje |
| FM | Modelo fundacional preentrenado para multiples tareas |
| Modelo multimodal | Modelo que trabaja con varias modalidades, como texto e imagen |
| Modelo de difusion | Modelo comun en generacion de imagenes |

## Casos de uso GenAI

- Generacion de texto.
- Resumen.
- Traduccion.
- Generacion de codigo.
- Asistentes conversacionales.
- Servicio al cliente.
- Generacion de imagen, audio o video.
- Busqueda semantica.
- Recomendaciones.
- Agentes que ejecutan tareas.

## Ciclo de vida de un modelo fundacional

1. Seleccion de datos.
2. Seleccion de modelo.
3. Pre-training o uso de modelo preentrenado.
4. Fine-tuning si hace falta.
5. Evaluacion.
6. Despliegue.
7. Feedback y mejora continua.

## Precio basado en tokens

En muchos casos, el costo y el rendimiento dependen de:

- Tokens de entrada.
- Tokens de salida.
- Tamano del modelo.
- Latencia requerida.
- Region.
- Capacidad provisionada.
- Personalizacion del modelo.

Regla mental: mas contexto y mas salida suelen implicar mas costo y mas latencia.

## Ingenieria de contexto, o context engineering

Context engineering es la gestion del contexto completo que recibe el modelo:

- Instrucciones.
- Documentos recuperados.
- Memoria.
- Herramientas disponibles.
- Politicas y restricciones.
- Datos del usuario.
- Historial relevante.

No es solo escribir prompts; es disenar todo lo que rodea la llamada al modelo.

## IA agentica, o agentic AI

Debes reconocer:

- Patrones multiagente.
- Model Context Protocol (MCP) para conectar agentes con sistemas externos.
- Comunicacion entre agentes.
- Gestion de memoria.
- Uso de herramientas.
- Orquestacion de flujos de trabajo.

## 2.2 Capacidades y limitaciones

Ventajas:

- Adaptabilidad.
- Respuestas conversacionales.
- Generacion de contenido.
- Rapidez para prototipos.
- Buen rendimiento en tareas de lenguaje.
- Puede cruzar dominios si el modelo es adecuado.

Limitaciones:

- Alucinaciones.
- Falta de interpretabilidad.
- Inexactitud.
- No determinismo.
- Costo por uso.
- Riesgo de datos sensibles.
- Sesgo en datos o salidas.
- Prompt injection.

## Seleccion de modelos GenAI

Evalua:

- Tipo de modelo.
- Modalidad: texto, imagen, audio, multimodal.
- Rendimiento esperado.
- Restricciones de latencia.
- Costo.
- Compliance.
- Complejidad.
- Region.
- Longitud maxima de entrada/salida.
- Necesidad de herramientas o agentes.

## Metricas de negocio

- ROI.
- Eficiencia.
- Tasa de conversion.
- Ingreso promedio por usuario.
- Precision o exactitud segun tarea.
- Valor de vida del cliente.
- Satisfaccion del usuario.

## 2.3 AWS para GenAI

| Servicio | Uso |
|---|---|
| Amazon Bedrock | Crear aplicaciones GenAI con FMs |
| Amazon SageMaker AI | Entrenar, desplegar y operar modelos |
| SageMaker JumpStart | Modelos y soluciones preconstruidas |
| Amazon Quick | Dentro del alcance oficial en analitica |
| Kiro | Desarrollo asistido |
| Strands Agents | Construccion de agentes |
| Amazon Bedrock AgentCore | Ejecucion y seguridad de agentes |
| Amazon Q | Asistentes generativos |

## Beneficios de AWS para GenAI

- Menor barrera de entrada.
- Servicios administrados.
- Seguridad y cumplimiento.
- Rapidez para salir al mercado.
- Integracion con datos y servicios AWS.
- Opciones de costo y rendimiento.
- Gobierno y monitoreo.

## Errores comunes

- Pensar que GenAI siempre es correcta.
- Olvidar que los tokens impactan costo.
- Confundir RAG con fine-tuning.
- Usar agentes sin permisos minimos.
- Medir solo calidad tecnica y no valor de negocio.
- Elegir un modelo sin revisar latencia, coste, compliance y modalidad.

## Checklist profesional del dominio

- Puedo definir token, chunking, embedding, vector, LLM, FM y modelo multimodal.
- Puedo explicar ciclo de vida de un FM.
- Puedo explicar precio basado en tokens.
- Puedo explicar ingenieria de contexto.
- Puedo describir agentes: memoria, herramientas, MCP y orquestacion.
- Puedo listar ventajas y riesgos de GenAI.
- Puedo relacionar servicios AWS GenAI con casos de uso.

## Ejercicios rapidos

1. Si una respuesta suena bien pero es falsa, es una alucinacion.
2. Si el modelo debe trabajar con texto e imagen, necesitas un modelo multimodal.
3. Si el contexto largo se repite mucho, revisa costo, latencia y cache de prompt.
4. Si un agente llama un CRM, debes controlar permisos, herramientas y logs.
5. Si un asistente debe ser medido por conversion, eso es metrica de negocio.
