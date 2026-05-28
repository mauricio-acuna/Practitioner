# Dominio de contenido 5: Seguridad, cumplimiento y gobernanza para soluciones de IA

Fuente oficial: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/ai-practitioner-01-domain5.html  
Peso en el examen: 14% del contenido puntuado.

[Volver al indice](ai-practitioner-01.md)

## Que evalua este dominio

Este dominio comprueba que entiendas como proteger sistemas de IA, como documentar origen de datos y como aplicar gobernanza, cumplimiento y auditoria a soluciones IA/GenAI.

## Tareas del dominio

1. Explicar metodos para proteger sistemas de IA.
2. Reconocer gobernanza y cumplimiento para sistemas de IA.

## 5.1 Seguridad de sistemas de IA

Servicios y caracteristicas clave:

| Control | AWS / Practica |
|---|---|
| Identidad y permisos | IAM roles, policies y permisos |
| Cifrado | AWS KMS, cifrado en reposo y en transito |
| Datos sensibles | Amazon Macie |
| Conectividad privada | AWS PrivateLink |
| Responsabilidad compartida | AWS protege la nube; cliente protege lo que configura en la nube |
| Agentes | Amazon Bedrock AgentCore Identity y politicas en AgentCore |
| Contenido GenAI | Amazon Bedrock Guardrails |

## Citacion de fuentes y origen de datos

Debes reconocer:

- Source citation: mostrar o conservar fuentes usadas por la respuesta.
- Data lineage: trazabilidad del origen y transformaciones de datos.
- Data cataloging: catalogar datos para descubrirlos, gobernarlos y auditar su uso.
- SageMaker Model Cards: documentar datos, proposito, riesgos y evaluacion del modelo.

## Ingenieria de datos segura

Buenas practicas:

- Evaluar calidad de datos.
- Controlar acceso a datos.
- Implementar tecnologias que mejoren privacidad.
- Mantener integridad de datos.
- Evitar datos sensibles innecesarios.
- Revisar origen y licencia.

## Riesgos de seguridad y privacidad en IA

- Seguridad de aplicacion.
- Deteccion de amenazas.
- Gestion de vulnerabilidades.
- Proteccion de infraestructura.
- Prompt injection.
- Cifrado en reposo y en transito.
- Prevencion de fuga de datos.
- Filtrado y validacion de salida.
- Logs y auditoria de interacciones IA.
- Toxicidad.

## Grounding y deteccion de alucinaciones

Tecnicas:

- RAG grounding.
- Validacion de salida.
- Confidence scoring.
- Citacion de fuentes.
- Revision humana para respuestas criticas.
- Comparacion contra fuentes autorizadas.

## 5.2 Gobernanza y cumplimiento

Servicios:

| Servicio | Uso |
|---|---|
| AWS Config | Evaluar configuraciones contra reglas |
| Amazon Inspector | Vulnerabilidades |
| AWS Audit Manager | Evidencias de auditoria |
| AWS Artifact | Reportes y acuerdos de cumplimiento |
| AWS CloudTrail | Auditoria de llamadas API |
| AWS Trusted Advisor | Recomendaciones de buenas practicas |

## Estrategias de gobernanza de datos

- Ciclo de vida de datos.
- Logging.
- Residencia de datos.
- Monitoreo.
- Observabilidad.
- Retencion.
- Control de acceso.
- Trazabilidad.

## Protocolos de gobernanza

Incluyen:

- Politicas internas.
- Cadencia de revision.
- Estrategias de revision.
- Marcos de gobernanza.
- Matriz de alcance de seguridad para IA generativa.
- Estandares de transparencia.
- Entrenamiento del equipo.

## Diferencias que suelen aparecer como distractores

| Necesidad | Servicio correcto |
|---|---|
| Quien llamo a una API | AWS CloudTrail |
| Logs, metricas y alarmas | Amazon CloudWatch |
| Configuracion contra reglas | AWS Config |
| Vulnerabilidades | Amazon Inspector |
| Evidencias de auditoria | AWS Audit Manager |
| Reportes y acuerdos de cumplimiento | AWS Artifact |
| Datos sensibles en S3 | Amazon Macie |
| Llaves de cifrado | AWS KMS |
| Secretos | AWS Secrets Manager |

## Errores comunes

- Dar acceso administrador a agentes.
- Guardar secretos en prompts.
- No registrar interacciones relevantes.
- Confundir CloudTrail con CloudWatch.
- Ignorar residencia o retencion de datos.
- Confiar en GenAI sin validacion de salida.

## Checklist profesional del dominio

- Puedo aplicar minimo privilegio con IAM.
- Puedo explicar cifrado en reposo y en transito.
- Puedo elegir Macie, PrivateLink, KMS, Secrets Manager y Guardrails por caso.
- Puedo explicar data lineage, catalogacion y Model Cards.
- Puedo reconocer prompt injection, data leakage, toxicidad y validacion de salida.
- Puedo usar RAG grounding, confidence scoring y citacion de fuentes contra alucinaciones.
- Puedo mapear Config, Inspector, Audit Manager, Artifact, CloudTrail y Trusted Advisor.

## Ejercicios rapidos

1. Quien llamo a una API y cuando: CloudTrail.
2. Datos sensibles en S3: Macie.
3. Llaves de cifrado: KMS.
4. Evidencia de auditoria: Audit Manager.
5. Reportes/acuerdos de cumplimiento: Artifact.
6. Configuraciones contra reglas: AWS Config.
7. Conectividad privada: PrivateLink.
