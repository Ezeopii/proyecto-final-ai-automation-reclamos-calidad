# Pruebas controladas

Esta carpeta contiene workflows utilizados exclusivamente para validar comportamientos técnicos del sistema.

## PF-TEST-Error-Handler

El workflow `PF-TEST-Error-Handler.json` fue utilizado para comprobar el manejo centralizado de errores.

Secuencia de prueba:

`Webhook de prueba → Stop And Error → PF-07 Manejo de Errores → alerta por Slack`

El error se genera de manera intencional y controlada. Su objetivo es verificar que, ante una falla técnica, el sistema:

- interrumpa la ejecución afectada;
- identifique workflow, ejecución y último nodo;
- capture el mensaje de error;
- derive una alerta automática al canal humano correspondiente.

Este workflow no forma parte de la arquitectura productiva del sistema y se incluye únicamente como evidencia reproducible de robustez.
