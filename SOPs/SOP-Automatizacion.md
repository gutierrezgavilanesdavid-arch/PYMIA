# SOP — Servicio de Automatización para PYMEs
**Empresa:** PYMIA ANTIGRAV  
**Versión:** 1.0  
**Fecha:** Mayo 2026  
**Responsable:** Consultor de Automatización

---

## 1. Propósito

Estandarizar el proceso de consultoría de automatización para PYMEs colombianas, desde el diagnóstico inicial hasta la entrega e implementación de soluciones, garantizando resultados medibles y reproducibles en cada proyecto.

---

## 2. Alcance

Aplica a todos los proyectos de automatización de procesos para clientes PYME en Colombia. Cubre automatización de procesos administrativos, operativos y comerciales usando herramientas de bajo/sin código (Make, Zapier, n8n, Google Apps Script, etc.).

---

## 3. Definiciones

| Término | Definición |
|--------|-----------|
| **Proceso candidato** | Tarea repetitiva, basada en reglas y con volumen suficiente para justificar automatización |
| **ROI de automatización** | Horas ahorradas × costo/hora del empleado vs. costo de implementación |
| **Flujo de trabajo** | Secuencia de pasos automatizados que reemplazan una tarea manual |
| **Integración** | Conexión entre dos o más herramientas/plataformas de software |

---

## 4. Responsabilidades

| Rol | Responsabilidad |
|-----|----------------|
| Consultor PYMIA | Diagnóstico, diseño de solución, implementación y entrega |
| Cliente (dueño o gerente) | Proveer acceso a herramientas, validar procesos, aprobar soluciones |
| Equipo del cliente | Participar en levantamiento de información y pruebas de usuario |

---

## 5. Proceso Paso a Paso

### FASE 1 — Diagnóstico (Semana 1)

**Objetivo:** Identificar los 3 procesos con mayor potencial de automatización.

**Paso 1.1 — Reunión de descubrimiento (90 min)**
- Agenda la reunión usando la Plantilla de Onboarding de Automatización
- Preguntas clave a hacer:
  - ¿Qué tareas repites todos los días o todas las semanas?
  - ¿Dónde está la mayor pérdida de tiempo en tu operación?
  - ¿Qué errores humanos ocurren con más frecuencia?
  - ¿Qué herramientas digitales usan actualmente? (CRM, ERP, Excel, correo, WhatsApp, etc.)
- Documenta las respuestas en el formulario de diagnóstico

**Paso 1.2 — Mapeo de procesos actuales**
- Para cada proceso identificado, documenta:
  - Quién lo ejecuta (cargo)
  - Frecuencia (diario/semanal/mensual)
  - Tiempo promedio de ejecución
  - Herramientas involucradas
  - Puntos de error frecuentes
- Usa la matriz de priorización (Impacto vs. Esfuerzo)

**Paso 1.3 — Entregable: Informe de Diagnóstico**
- Top 3 procesos candidatos con justificación
- Estimado de horas/mes ahorradas por cada uno
- Herramientas recomendadas para cada automatización
- Presupuesto estimado de implementación

**Criterio de éxito Fase 1:** Cliente aprueba el informe de diagnóstico y selecciona al menos 1 proceso para automatizar.

---

### FASE 2 — Diseño de Solución (Semana 1-2)

**Objetivo:** Diseñar el flujo de trabajo automatizado antes de tocar ninguna herramienta.

**Paso 2.1 — Diagrama de flujo**
- Dibuja el proceso actual (AS-IS) paso a paso
- Dibuja el proceso automatizado (TO-BE)
- Identifica: disparadores (triggers), condiciones, acciones, excepciones

**Paso 2.2 — Selección de herramientas**

| Necesidad | Herramienta recomendada |
|-----------|------------------------|
| Automatización entre apps (sin código) | Make (Integromat) o Zapier |
| Automatización avanzada / on-premise | n8n |
| Automatización dentro de Google Workspace | Google Apps Script |
| Formularios + flujos de aprobación | Jotform + Make |
| WhatsApp Business automatizado | Twilio / Meta API + Make |
| Reportes automáticos | Google Looker Studio + Sheets |

**Paso 2.3 — Presentación al cliente**
- Presenta el diagrama TO-BE y explica cada paso
- Obtén aprobación escrita (email o mensaje documentado)
- Confirma accesos necesarios a las herramientas

**Criterio de éxito Fase 2:** Cliente aprueba el diseño y provee todos los accesos en menos de 3 días hábiles.

---

### FASE 3 — Implementación (Semana 2-3)

**Objetivo:** Construir y probar la automatización en ambiente de pruebas antes de activar en producción.

**Paso 3.1 — Configuración en ambiente de pruebas**
- Crea una copia/ambiente separado para pruebas
- Configura el flujo paso a paso siguiendo el diagrama aprobado
- Documenta cada configuración relevante (credenciales, IDs, campos mapeados)

**Paso 3.2 — Pruebas internas (QA)**
- Ejecuta mínimo 3 pruebas end-to-end con datos reales del cliente
- Verifica que cada condición y excepción funcione correctamente
- Documenta los resultados en la bitácora de pruebas

**Paso 3.3 — Prueba de usuario (UAT)**
- El cliente ejecuta el proceso 2-3 veces con tu acompañamiento
- Recoge feedback y ajusta si es necesario
- Documenta los ajustes realizados

**Paso 3.4 — Activación en producción**
- Activa el flujo en el ambiente de producción
- Monitorea durante las primeras 48 horas
- Confirma que los datos/resultados son correctos

**Criterio de éxito Fase 3:** La automatización corre sin intervención manual durante 48 horas continuas sin errores.

---

### FASE 4 — Entrega y Cierre (Semana 3-4)

**Objetivo:** Transferir el conocimiento al cliente y cerrar el proyecto formalmente.

**Paso 4.1 — Documentación de la solución**
- Escribe el manual de usuario (máx. 2 páginas por flujo)
  - Cómo funciona el flujo
  - Qué hacer si algo falla
  - Cómo hacer cambios básicos
- Comparte credenciales y accesos de forma segura (no por WhatsApp)

**Paso 4.2 — Sesión de capacitación (60 min)**
- Muestra al cliente cómo monitorear el flujo
- Explica cómo interpretar errores y notificaciones
- Responde preguntas y deja grabación si el cliente lo requiere

**Paso 4.3 — Entrega formal**
- Envía el Acta de Entrega para firma del cliente
- Incluye: resumen del proyecto, métricas de ahorro estimado, accesos entregados, garantía de soporte

**Paso 4.4 — Seguimiento post-entrega (30 días)**
- Check-in a los 7 días: ¿Todo funciona bien?
- Check-in a los 30 días: ¿Cuántas horas/semana están ahorrando?
- Documenta el resultado para el caso de estudio del cliente

**Criterio de éxito Fase 4:** Cliente firma el Acta de Entrega y confirma satisfacción.

---

## 6. Métricas de Éxito del Servicio

| Métrica | Meta |
|---------|------|
| Tiempo de diagnóstico a entrega | ≤ 4 semanas |
| Horas ahorradas al cliente (mínimo) | 8 horas/mes por automatización |
| Tasa de errores post-implementación | < 2% de ejecuciones |
| NPS del cliente | ≥ 8/10 |
| Tasa de upsell / segundo proyecto | ≥ 40% de clientes |

---

## 7. Escalamiento y Excepciones

- **Si el cliente no provee accesos en 5 días hábiles:** Escala al responsable de la empresa; si persiste, aplaza el proyecto formalmente con acta de pausa.
- **Si la herramienta seleccionada no soporta el proceso:** Evalúa alternativa y notifica al cliente con nueva propuesta antes de implementar.
- **Si el cliente cambia el alcance durante la implementación:** Usa el proceso de Gestión de Cambios (solicitud escrita, cotización adicional, aprobación antes de ejecutar).

---

## 8. Herramientas del Consultor

- **Gestión de proyectos:** Notion / Trello
- **Comunicación:** WhatsApp Business + Email
- **Documentación:** Google Docs / Notion
- **Automatización:** Make, n8n, Zapier, Google Apps Script
- **Diagramas:** Miro / Lucidchart / draw.io

---

## 9. Historial de Versiones

| Versión | Fecha | Cambio |
|---------|-------|--------|
| 1.0 | Mayo 2026 | Versión inicial |
