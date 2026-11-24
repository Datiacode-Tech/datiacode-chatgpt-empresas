# Flujo conversacional — Tarjetas

Este diagrama es una **representación conceptual**, no un proceso ejecutable. Debe interpretarse junto a `../requisitos/reglas-negocio.md`.

```mermaid
flowchart TD
    A["Mensaje del usuario"] --> B{"¿Incidencia sensible?"}
    B -->|Sí| C["Orientar al canal seguro"]
    C --> Z["Fin"]
    B -->|No| D{"¿Solicita atención humana?"}
    D -->|Sí| E["Orientar a atención humana"]
    E --> Z
    D -->|No| F{"¿Consulta informativa identificada?"}
    F -->|Sí| G["Responder con información verificada"]
    G --> Z
    F -->|No| H{"¿Aclaraciones realizadas < 2?"}
    H -->|Sí| I["Pedir una aclaración sin datos sensibles"]
    I --> B
    H -->|No| E
```

## Significado de las rutas

- **Canal seguro:** orientación al uso de canales oficiales verificados; nunca implica bloqueo ni acceso a datos reales.
- **Atención humana:** salida para solicitudes expresas o dos aclaraciones sin resolución.
- **Informativa:** respuesta general cuando existe información suficiente y verificada.
- **Aclaración:** pregunta para determinar la intención. Su contador se mantiene durante la misma consulta.

## Revisión recomendada

Al analizar el flujo, contrastar cada bifurcación con `REQ-FRA-03`, `REQ-HUM-05`, `REQ-ENR-02` y `REQ-SEC-07`. El objetivo docente es encontrar relaciones entre requisitos, prompt y diagrama.
