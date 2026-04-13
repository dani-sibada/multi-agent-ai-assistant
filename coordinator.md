# Coordinator - Orquestador de Subagents

## Flujo de Ejecucion

### Paso 1: SQL Specialist (exploracion de datos)
- Analiza requisito
- Escribe query SQL
- Valida en ambiente testing
- Documenta query

### Paso 2: Dashboards Developer (visualizacion)
- Recibe query del SQL Specialist
- Diseña dashboard Metabase
- Implementa filtros globales
- Prepara componentes React

### Paso 3: Odoo Automation (integracion)
- Si es necesario, crea automatizaciones
- Configura flujos de trabajo
- Integra con CRM
- Documenta cambios

### Paso 4: QA Validator (validacion)
- Ejecuta tests
- Valida seguridad
- Verifica integridad de datos
- Genera reporte de validacion

### Paso 5: Deploy (manual - requiere aprobacion humana)
- Merge a rama principal
- Deploy a produccion
- Monitores activos
- Logs auditados

## Ventajas de esta Arquitectura

- Especialización: cada agente es experto en su area
- Seguridad: cada paso tiene validacion
- Paralelismo: tareas independientes se ejecutan simultaneas
- Auditabilidad: todo queda registrado
- Escalabilidad: agregar nuevos subagents es simple
- Costos: tareas simples usan Haiku (mas economico)
