# Instrucciones de trabajo para Codex — Proyecto 02

Este archivo establece reglas para **Codex trabajando sobre el proyecto de VS Code**. No es el prompt que hablará con los usuarios finales del agente de préstamos.

## Alcance y fuentes

- Proyecto ficticio y documental. No hay ninguna integración bancaria real.
- `requisitos/requisitos-prestamos.md` es la fuente funcional de referencia.
- `prompts/prestamos-v1.md` es la línea de base defectuosa y **no debe modificarse**.
- `prompts/prestamos-v2.md` es la ubicación autorizada para propuestas cuando el usuario solicite explícitamente cambios.
- `evaluaciones/escenarios-prueba.md` contiene escenarios de comprobación de diseño.

## Comportamiento esperado de Codex

1. Empezar por un análisis **solo lectura**, salvo que el usuario pida expresamente editar.
2. Citar rutas, fragmentos y `REQ-PRE-*` para explicar cada inconsistencia; no inventar requisitos.
3. Antes de editar, resumir los archivos afectados y la propuesta de modificación.
4. No modificar `v1`, `requisitos` ni `evaluaciones` sin autorización explícita.
5. Al crear `v2`, conservar secciones claras: objetivo, alcance, reglas, rutas, límites, tono y manejo de errores.
6. Al finalizar, presentar un resumen de cambios, riesgos pendientes y posibles comprobaciones.
7. No crear carpetas, scripts, dependencias o archivos extra si no se solicitan.
8. No ejecutar comandos, instalar paquetes, acceder a la red, hacer commits, push ni despliegues.
9. No solicitar ni incorporar datos reales de clientes, credenciales o información confidencial.

## Criterio de calidad

La propuesta debe ser coherente con los requisitos, minimizar riesgos, ser legible para perfiles no técnicos y reconocer límites de capacidad. Ante requisitos ambiguos, señalarlos antes de inventar una regla.
