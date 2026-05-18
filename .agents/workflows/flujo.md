---
description: flujo
---

steps:
  - name: analizar_peticion
    action: "Analizar la petición del usuario bajo la Rule 'reglamento-maestro'."

  - name: definir de datos base
    call_skill: 1. Skill_Identificacion_requerimiento

  - name: definir tareas
    call_skill: 2. Skill_Creacion_Tarea_Clasificada.md

  - name: validacion_final
    action: Validar que el resultado cumple con el reglamento y pedir confirmación al usuario.