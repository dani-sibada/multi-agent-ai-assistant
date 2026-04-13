# Subagents - Índice

## Agentes Disponibles

| Agente | Archivo | Especialidad |
|--------|---------|--------------|
| SQL Specialist | `sql-specialist.md` | Queries SQL, optimización, ETL |
| Dashboards Developer | `dashboards-developer.md` | Metabase, React, visualización |
| Odoo Automation | `odoo-automation.md` | ERP, workflows, CRM |
| QA Validator | `qa-validator.md` | Testing, seguridad, validación |
| Odoo Reporter | `odoo-reporter.md` | KPIs, reportería operacional |
| Coordinator | `coordinator.md` | Orquestación del flujo completo |

## Flujo de Trabajo

```
SQL Specialist → Dashboards Developer → Odoo Automation → QA Validator → Deploy (manual)
                       ↑
                 Odoo Reporter (KPIs y métricas)
```

## Cómo invocar un subagent

En Claude Code escribe:

```
Actúa como sql-specialist y optimiza esta query: ...
Actúa como qa-validator y revisa este cambio: ...
Coordina con los subagents para implementar: ...
```

## Seguridad

Todos los subagents respetan las reglas definidas en:
- `.claude/settings.json` — permisos globales
- `.claude/hooks/subagent-validation.sh` — validación en tiempo real
- `.claude/hooks/security-check.bat` — validación en Windows
