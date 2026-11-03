# Proyecto de seguridad web — ciclo DevSecOps

Cadena de integración continua con controles de seguridad bloqueantes:
`commit → SAST (Semgrep) → DAST (OWASP ZAP) → deploy a preproducción`.

## Estructura

| Ruta | Contenido |
|---|---|
| `jenkins/` | Imagen y compose de Jenkins |
| `pipeline/` | Jenkinsfile y configuración de la tarea |
| `compose/` | Overrides de Compose para CI y preproducción |
| `scripts/` | Utilidades de espera y resumen |
| `docs/` | Memoria del proyecto |
| `capturas/` | Evidencias |

## Entorno

- Ubuntu Server · Docker Engine · Docker Compose
- Jenkins LTS en contenedor, con el workspace montado desde el host
- Laboratorio bajo prueba: WebsVulnerables (Apache + PHP 8.2 + MySQL 8.0)

## Estado

En construcción por fases. Ver `docs/memoria.md`.
