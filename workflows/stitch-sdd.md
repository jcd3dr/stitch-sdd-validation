---
description: Spec-Driven Development Integrado con Stitch MCP (Stitch-SDD)
---

# Workflow: Stitch-SDD

Este workflow optimiza el proceso de desarrollo de interfaces utilizando **Stitch MCP** como núcleo de diseño y referencia técnica.

## 1. Fase de Briefing & Concepto
- Usa `doc-brd` para definir los requerimientos de negocio.
- **Acción Tool-First**: Identifica si la interfaz se beneficia de Stitch (UI compleja/premium). Si es así, menciónalo explícitamente en el `brief.md`.

## 2. Fase de Especificación & Diseño (Stitch)
- Genera la especificación técnica en `spec.md`.
- **Integración Stitch**: 
    1. Crea un proyecto en Stitch usando `mcp_StitchMCP_create_project`.
    2. Genera pantallas iniciales basadas en el `spec.md` para validar visualmente los requerimientos antes de codificar.

## 3. Fase de Extracción de Referencia (Paso 0)
*Este paso es obligatorio para asegurar la fidelidad técnica.*
- Descarga el código HTML/CSS de las pantallas aprobadas en Stitch.
- Extrae los tokens de diseño (colores, fuentes, sombras) y guarda esta "fuente de verdad" en `.stitch/DESIGN.md`.

## 4. Fase de Implementación Funcional
- Inicializa el entorno (React/Vite/Etc.).
- **Mapeo de Código**: Usa el código extraído de Stitch para crear componentes funcionales. No "adivines" los estilos; tradúcelos directamente del HTML de Stitch.

## 5. Fase de Verificación Permanente
- Compara la app funcional contra el screenshot oficial de Stitch en el `walkthrough.md`.
- Asegura que cualquier cambio en el diseño se actualice primero en Stitch para mantener la trazabilidad.
