# KI: Equilibrio Agilidad/Proceso en Stitch MCP

## Contexto
Durante el diseño de una interfaz de inventario, se identificó que la adherencia estricta al flujo Spec-Driven Development (SDD) puede retrasar excesivamente la entrega de resultados visuales de Stitch, frustrando la validación de la herramienta por parte del usuario.

## Aprendizaje Clave
1. **Planificación Integrada (Tool-First Planning)**: La planificación (BRD/Spec) debe diseñarse *contemplando* las capacidades de `mcp_stitch` para que la herramienta actúe como un catalizador del proceso y no como un obstáculo burocrático.
2. **Stitch como Referencia, no como Ley**: `mcp_stitch` es la herramienta preferida para el diseño de UI de alta fidelidad, pero no es obligatoria si una tarea específica no lo requiere. Debe usarse donde aporte valor real.
3. **Sinergia Tool-Spec**: El éxito radica en usar la planificación para guiar a la herramienta, asegurando que el output del MCP cumpla con los requisitos de negocio de forma inmediata.

## Recomendación para el Futuro
- **Seguir el Workflow Formal**: Usar siempre el proceso definido en [/stitch-sdd](file:///c:/dadecore/.agents/workflows/stitch-sdd.md).
- **Generar primero, documentar después**: Si la tarea es "Diseña X con Stitch", realizar la llamada al MCP inmediatamente después de una breve mejora del prompt (`enhance-prompt`).
- **Uso de IDs**: Siempre usar IDs de proyecto reales y documentarlos de inmediato para asegurar trazabilidad.

## Confirmación
Este aprendizaje ha sido integrado en la base de conocimientos para futuras interacciones.
