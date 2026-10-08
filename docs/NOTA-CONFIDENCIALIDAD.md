# Nota de confidencialidad

Este repositorio contiene una versión sanitizada de los workflows desarrollados para el proyecto final **Asistente para la Gestión de Reclamos de Calidad**.

Con el objetivo de preservar la seguridad de la información y evitar la exposición de datos internos, fueron excluidos o anonimizados:

- credenciales, API keys, tokens y secretos;
- direcciones de correo electrónico y usuarios personales;
- identificadores internos de Slack, Airtable y n8n;
- IDs de credenciales, workflows, webhooks, instancias y versiones;
- documentación operativa real de clientes;
- datos de prueba fijados o mock data;
- referencias identificables a clientes y documentos internos.

Los workflows publicados conservan la lógica funcional necesaria para comprender la arquitectura, incluyendo:

- orquestación Manager–Worker;
- RAG;
- AI-as-a-Judge;
- reintento controlado;
- Human-in-the-Loop (HITL);
- idempotencia;
- trazabilidad;
- manejo centralizado de errores.

## Documentación RAG

La documentación empresarial utilizada durante las pruebas del sistema no se publica en este repositorio por razones de confidencialidad.

En la versión pública, las referencias documentales fueron reemplazadas por nombres genéricos de demostración. Para reproducir el flujo RAG, debe utilizarse documentación propia o de prueba y volver a configurar las credenciales correspondientes.

## Importación

Al importar los workflows en otra instancia de n8n será necesario volver a configurar:

1. credenciales;
2. IDs de subworkflows;
3. conexiones con Airtable;
4. destinatarios de Gmail;
5. usuarios/canales de Slack;
6. workflow de errores PF-07 en los Settings de PF-00 a PF-06.

Esta sanitización se realizó únicamente sobre las copias destinadas al repositorio. Los workflows originales utilizados en la demostración no fueron modificados.
