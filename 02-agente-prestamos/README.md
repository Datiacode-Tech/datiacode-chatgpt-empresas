# Proyecto 02 — Optimización de un agente de préstamos

**Caso educativo ficticio.** La versión `prompts/prestamos-v1.md` contiene **errores deliberados** para que sean detectados. No se debe reutilizar como instrucción de un agente real.

## Objetivo

Aprender a utilizar Codex como asistente de **revisión y propuesta de cambios**, manteniendo separados los requisitos aprobados, el prompt original y la versión mejorada.

## Estructura

| Archivo | Función |
|---|---|
| `AGENTS.md` | Acuerdos de trabajo para Codex dentro de esta carpeta. |
| `requisitos/requisitos-prestamos.md` | Fuente funcional de referencia e identificadores de comprobación. |
| `prompts/prestamos-v1.md` | Prompt defectuoso, conservado como línea de base. |
| `prompts/prestamos-v2.md` | Plantilla para escribir una propuesta revisada sin sobreescribir la v1. |
| `evaluaciones/escenarios-prueba.md` | Casos que permiten discutir si los cambios cubren riesgos y necesidades. |

## Método de trabajo previsto

1. Abrir **esta carpeta** como proyecto en VS Code.
2. Pedir un diagnóstico en modo **solo lectura**, con referencias a archivos y requisitos.
3. Solicitar una propuesta en `prompts/prestamos-v2.md` sin tocar `v1`.
4. Comparar ambos archivos en VS Code y justificar cada cambio.
5. Revisar la propuesta contra `evaluaciones/escenarios-prueba.md`.

## Qué significa «evaluar» en este proyecto

Estos escenarios son **casos de revisión de diseño**. No hay infraestructura, aplicación ni motor de pruebas conectado: Codex puede analizar la coherencia y simular respuestas propuestas, pero eso **no equivale a ejecutar pruebas reales del agente ni a comprobar su producción**.

No se requieren APIs, terminal, dependencias, Git ni conexión a recursos corporativos.
