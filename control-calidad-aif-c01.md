# Control de calidad del material AIF-C01

Fecha de revision: 2026-05-27  
Objetivo: verificar que los archivos creados tengan calidad profesional, cobertura suficiente y alineacion con la guia oficial de AWS Certified AI Practitioner AIF-C01.

## Fuentes oficiales verificadas

- Guia principal: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/ai-practitioner-01.html
- Dominio 1: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/ai-practitioner-01-domain1.html
- Dominio 2: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/ai-practitioner-01-domain2.html
- Dominio 3: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/ai-practitioner-01-domain3.html
- Dominio 4: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/ai-practitioner-01-domain4.html
- Dominio 5: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/ai-practitioner-01-domain5.html
- Servicios dentro del alcance: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/aif-01-in-scope-services.html
- Servicios fuera del alcance: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/aif-01-out-of-scope-services.html
- Revisiones: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/aif-01-revisions.html

## Archivos revisados

- `ai-practitioner-01.md`
- `ai-practitioner-01-domain1.md`
- `ai-practitioner-01-domain2.md`
- `ai-practitioner-01-domain3.md`
- `ai-practitioner-01-domain4.md`
- `ai-practitioner-01-domain5.md`
- `aif-01-in-scope-services.md`
- `aif-01-out-of-scope-services.md`
- `aif-01-revisions.md`
- `programa-entrenamiento-aif-c01.md`
- `ejercicios-explicados-por-dominio-aif-c01.md`
- `simulador-2-aif-c01.md`
- `tarjetas-memoria-aif-c01.md`

## Comprobaciones realizadas

| Criterio | Estado | Evidencia |
|---|---|---|
| Enlaces locales `.md` | OK | No hay enlaces locales Markdown faltantes |
| Archivos de `Topics` | OK | Los 8 archivos externos existen |
| Anclas internas de `ai-practitioner-01.md` | OK | `intro`, `target`, `exam-content`, `domains`, `survey` existen |
| Pesos de dominios | OK | 20%, 24%, 28%, 14%, 14% reflejados |
| Servicios dentro del alcance | OK | Lista oficial reflejada, incluido `Amazon Quick` como aparece en AWS |
| Servicios fuera del alcance | OK | Lista oficial actual reflejada |
| Revision 1.1 | Mejorado | Se agregaron Agentic AI, MCP, AgentCore, Kiro, Strands Agents, Amazon Q, Prompt Management, LLM-as-a-judge y metricas de negocio |
| Idioma | OK | Redaccion en castellano, manteniendo terminos tecnicos oficiales |
| Practica | OK | Hay simuladores, ejercicios explicados y tarjetas |

## Mejoras aplicadas en esta revision

- Se reforzo Dominio 1 con redes neuronales, metricas de negocio y checklist profesional.
- Se reforzo Dominio 2 con ingenieria de contexto, IA agentica y checklist profesional.
- Se reforzo Dominio 3 con versionado/gestion de prompts, Amazon Bedrock Prompt Management, LLM-as-a-judge, metricas de negocio y evaluacion de RAG/agentes/workflows.
- Se reforzo Dominio 4 con senales de respuesta correcta y checklist profesional.
- Se reforzo Dominio 5 con tabla de distractores de seguridad/gobernanza y checklist profesional.
- Se actualizaron tarjetas de memoria con Prompt Management, versionado de prompts y LLM-as-a-judge.
- Se actualizaron reglas mentales del banco de ejercicios.

## Riesgos residuales

- AWS puede actualizar la guia despues de esta fecha. Antes de rendir, conviene revisar de nuevo la pagina oficial de revisiones.
- `Amazon Quick` aparece literalmente en la lista oficial de servicios dentro del alcance. No se reemplazo por `Amazon QuickSight` para no desviarse de la fuente oficial.
- Las preguntas de practica son originales y no oficiales. Sirven para entrenar razonamiento, no para predecir preguntas exactas del examen.

## Veredicto

El material ya no queda como una creacion rapida minima. Tiene estructura de estudio, cobertura por dominio, practica, respuestas explicadas, tarjetas, listas de servicios, pagina de revisiones y control de calidad. Aun asi, debe mantenerse vivo: si AWS publica una nueva revision, este archivo debe actualizarse primero.
