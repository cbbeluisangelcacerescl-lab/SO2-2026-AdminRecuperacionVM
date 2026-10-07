# Plataforma de Monitoreo y Observabilidad de Infraestructura TI

## Descripción general

El proyecto consiste en diseñar e implementar una plataforma centralizada de monitoreo y observabilidad de infraestructura TI. La plataforma permite recolectar, almacenar, visualizar y analizar métricas de servidores, dispositivos de red y servicios, facilitando la detección temprana de incidentes mediante reglas de alerta configurables.

## Problema que resuelve

La supervisión manual de una infraestructura tecnológica puede dificultar la identificación temprana de problemas.

Las principales dificultades son:

* Falta de información centralizada.
* Dificultad para consultar información histórica.
* Detección tardía de fallas.
* Dependencia de verificaciones manuales.
* Falta de alertas automáticas.
* Dificultad para identificar tendencias en el uso de recursos.
* Necesidad de utilizar diferentes herramientas para supervisar distintos tipos de infraestructura.

La plataforma busca centralizar el monitoreo, recolectar métricas, almacenarlas, visualizarlas y generar alertas ante determinadas condiciones.

## Propósito

El propósito del proyecto es facilitar la administración de infraestructura TI mediante una plataforma centralizada que permita supervisar servidores, dispositivos de red y servicios.

La solución busca mejorar la detección de incidentes y proporcionar información útil para el análisis y la toma de decisiones técnicas.

## Usuarios objetivo

La plataforma está dirigida principalmente a:

* Administradores de sistemas.
* Administradores de redes.
* Personal de infraestructura TI.
* Técnicos de soporte.
* Responsables de servicios tecnológicos.

Los usuarios de los servicios tecnológicos también pueden beneficiarse indirectamente gracias a una detección más rápida de incidentes.

## Tecnologías utilizadas

| Tecnología        | Función                                  |
| ----------------- | ---------------------------------------- |
| Docker            | Ejecución de componentes                 |
| Docker Compose    | Administración del entorno               |
| FastAPI           | API y lógica de gestión                  |
| PostgreSQL        | Base de datos                            |
| Alembic           | Migraciones de base de datos             |
| Prometheus        | Recolección y almacenamiento de métricas |
| Node Exporter     | Métricas de Linux                        |
| Windows Exporter  | Métricas de Windows                      |
| SNMP Exporter     | Métricas de dispositivos de red          |
| Blackbox Exporter | Verificación de servicios                |
| Grafana           | Visualización mediante dashboards        |
| Alertmanager      | Gestión de alertas                       |
| Python            | Desarrollo del backend                   |
| React/TypeScript  | Interfaz de gestión                      |

## Arquitectura

El flujo principal de monitoreo es:

**Dispositivos y servicios → Exporters/Monitoreo → Prometheus → Dashboards y Alertas**

La gestión de la plataforma funciona mediante:

**Usuario → Plataforma web → FastAPI → PostgreSQL**

Prometheus administra las métricas de series temporales y PostgreSQL almacena la información estructural y administrativa.

## Alcance inicial del proyecto (MVP)

El MVP contempla una infraestructura funcional de monitoreo capaz de integrar diferentes componentes tecnológicos.

Actualmente se cuenta con:

* Docker Compose.
* PostgreSQL.
* FastAPI.
* Prometheus.
* Node Exporter.
* Blackbox Exporter.
* SNMP Exporter.
* Instrumentación de FastAPI.
* Recolección de métricas aproximadamente cada 15 segundos.
* Retención aproximada de 90 días.
* 13 reglas de alerta configuradas.

## Estado actual

| Fase    | Actividad                              | Estado               |
| ------- | -------------------------------------- | -------------------- |
| Fase 0  | Investigación, problema y arquitectura | ✅ Completada         |
| Fase 1  | Infraestructura y Docker Compose       | ✅ Completada         |
| Fase 2  | PostgreSQL y Alembic                   | ✅ Completada         |
| Fase 3  | FastAPI y API REST                     | ✅ Completada         |
| Fase 4  | Prometheus y exporters                 | ✅ Completada         |
| Fase 5  | Evaluación de agente propio            | ⏳ Pendiente/opcional |
| Fase 6  | Alertmanager y notificaciones          | ⏳ Pendiente          |
| Fase 7  | Grafana y dashboards                   | ⏳ Pendiente          |
| Fase 8  | Integración y seguridad                | ⏳ Pendiente          |
| Fase 9  | Pruebas finales                        | ⏳ Pendiente          |
| Fase 10 | Documentación y presentación           | ⏳ Pendiente          |

## Integrantes y roles

| N.º | Integrante                  | Rol                                 |
| --- | --------------------------- | ----------------------------------- |
| 1   | Adam Fabricio Sánchez López | Líder de Repositorio                |
| 2   | Brandon González Salazar    | Líder de Documentación Técnica      |
| 3   | Luis Angel Caceres          | Líder de Integración IA y Auditoría |
| 4   | Rudi Choque Bautista        | Líder de Gestión de Tareas          |

## Beneficios esperados

* Centralización de información.
* Supervisión continua.
* Consulta de métricas históricas.
* Detección temprana de problemas.
* Identificación de dispositivos no disponibles.
* Identificación de problemas de recursos.
* Visualización del comportamiento de la infraestructura.
* Generación de alertas.
* Apoyo a la toma de decisiones técnicas.

## Repositorio

**GitHub:**
https://github.com/CBBELUISANGELCACERESCL-lab/SO2-2026-AdminRecuperacionVM

## Información académica

**Materia:** Sistemas Operativos P2 (SO2-2026)
**Carrera:** Ingeniería de Sistemas
**Docente:** Diego Patrick Cárdenas Sejas
# SO2-2026-AdminRecuperacionVM
