# Proyecto 01 — Exploración de un agente de tarjetas

**Caso 100 % ficticio y educativo.** No representa la infraestructura ni las instrucciones de ninguna entidad financiera. No conecta con servicios bancarios y **no ejecuta un agente**: sus documentos describen un diseño para analizarlo con VS Code y Codex.

## Propósito

Aprender a identificar dónde se define el comportamiento de un agente conversacional, cómo se relacionan sus instrucciones con los requisitos y cómo leer su flujo sin conocimientos de programación.

## Mapa del proyecto

| Ruta | Para qué sirve | Qué NO es |
|---|---|---|
| `prompts/agente-tarjetas.md` | Instrucciones operativas propuestas para el agente | Un agente desplegado o ejecutable |
| `requisitos/reglas-negocio.md` | Fuente de referencia para verificar comportamientos | Un prompt para ejecutar sin revisión |
| `flujos/flujo-conversacional.md` | Representación legible del recorrido y las decisiones | Código que realice operaciones reales |

## Regla de lectura

1. Leer los **requisitos** para saber qué debe cumplirse.
2. Leer el **prompt** para ver cómo se pretende cumplir.
3. Leer el **flujo** para comprobar decisiones, salidas y casos límite.
4. Señalar explícitamente cualquier diferencia entre fuentes. No inventar políticas.

## Límites y privacidad

- Se usan nombres de escenarios y datos inventados; no hay números de tarjetas, credenciales ni datos de clientes.
- El asistente informa y orienta; no bloquea tarjetas, no comprueba saldos ni ejecuta operaciones.
- Las situaciones de fraude o pérdida se remiten a un **canal seguro** genérico, nunca a un enlace real.

No se requiere terminal, API, Git, npm ni dependencias.
