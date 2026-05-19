---
tipo: Tarea
subtipo: "Operativo / Técnico"
prioridad: "Alta"
responsable: "Desarrollador Backend / Oficial de Riesgo"
fecha_creacion: "2026-05-18"
tags: [tarea, chatbot, limites, montos, historia_usuario]
---

# 🛠️ Tarea: Actualización y Parametrización de Nuevos Límites de Montos para Chatbot

## 📋 Resumen del Requerimiento
- **Clasificación:** Tarea
- **Tipo de Requerimiento:** Operativo / Técnico
- **Prioridad Sugerida:** Alta
- **Solicitante / Origen:** Minuta de Reunión: [[Puntos a tratar reunion]]
- **Responsable:** Desarrollador Backend / Oficial de Riesgo

---

## 👤 Historia de Usuario (Básica)
- **COMO:** Oficial de Control de Riesgos
- **QUIERO:** Que se configuren y validen nuevos montos máximos y mínimos para transacciones en el canal de chatbot
- **PARA:** Controlar la exposición al riesgo transaccional y prevenir fraudes o errores de digitación por parte de los clientes.

---

## 🎯 Criterios de Aceptación
Para dar esta tarea como finalizada con éxito, se deben cumplir los siguientes puntos:
- [ ] **Criterio 1:** El chatbot debe bloquear e informar al usuario si intenta realizar una transacción que supere el monto máximo por transacción o diario establecido.
- [ ] **Criterio 2:** La validación de montos debe realizarse a nivel de backend y no solo en la interfaz del chatbot para garantizar la seguridad de API.
- [ ] **Criterio 3:** Las alertas de seguridad del sistema deben dispararse si un usuario intenta evadir el límite mediante múltiples transacciones consecutivas en un período menor a 5 minutos.

---

## 🛠️ Plan de Ejecución y Desglose Técnico
Pasos detallados para la realización de la tarea:
1. **Paso 1:** Definir y validar la matriz de límites autorizados por tipo de cliente y nivel de autenticación del chatbot.
2. **Paso 2:** Modificar el código de validación transaccional en las APIs del backend de chatbot para reflejar los nuevos límites aprobados.
3. **Paso 3:** Ejecutar pruebas automatizadas simulando peticiones que excedan los montos permitidos para validar la restricción.

---

## 🔗 Referencias y Contexto
- **Solicitud de Origen:** [[Requerimiento_Limites_Montos_Chatbot]] extraído de [[Puntos a tratar reunion]]
- **Impacto:** Seguridad Transaccional, Control de Fraudes y Clientes del Chatbot.
