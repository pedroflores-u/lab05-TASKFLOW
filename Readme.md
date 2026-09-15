# TaskFlow

[![Last Commit](https://img.shields.io/github/last-commit/pedroflores-u/lab05-FLUJO-DE-TAREAS)](https://github.com/pedroflores-u/lab05-FLUJO-DE-TAREAS)
[![License](https://img.shields.io/github/license/pedroflores-u/lab05-FLUJO-DE-TAREAS)](https://github.com/pedroflores-u/lab05-FLUJO-DE-TAREAS/blob/main/LICENSE)

Sistema moderno y colaborativo para la administración y gestión eficiente de tareas en equipo.

---

## Tabla de contenidos
- [Descripción](#descripción)
- [Funcionalidades](#funcionalidades)
- [Tecnologías utilizadas](#tecnologías-utilizadas)
- [Requisitos](#requisitos)
- [Instalación](#instalación)
- [Arquitectura y Diagramas](#arquitectura-y-diagramas)
- [Estructura del proyecto](#estructura-del-proyecto)
- [Capturas de Pantalla](#capturas-de-pantalla)
- [Contribuidores](#contribuidores)
- [Licencia](#licencia)

---

## Descripción
**TaskFlow** es una aplicación diseñada para optimizar el flujo de trabajo diario de equipos de desarrollo u oficinas. Permite organizar pendientes, asignar responsables en tiempo real y hacer un seguimiento transparente del progreso de cada proyecto.

---

## Funcionalidades
- [x] Registrar tareas
- [x] Editar tareas
- [ ] Eliminar tareas
- [ ] Asignar tareas a usuarios
- [ ] Filtrar tareas por estado y prioridad

---

## Tecnologías utilizadas

| Categoría | Tecnología | Versión |
| :--- | :--- | :--- |
| **Frontend** | HTML5, CSS3, JavaScript | ES6+ |
| **Backend** | Node.js / Express | v18.x |
| **Base de Datos** | MySQL | v8.0 |
| **Control de Versiones** | Git & GitHub | Latest |

---

## Requisitos
* Navegador web moderno (Google Chrome, Firefox, Edge o Brave).
* Node.js instalado en el sistema.
* Servidor local de MySQL activo.

---

## Instalación
1. Clonar el repositorio:
   ```bash
   git clone [https://github.com/pedroflores-u/lab05-FLUJO-DE-TAREAS.git](https://github.com/pedroflores-u/lab05-FLUJO-DE-TAREAS.git)

## Arquitectura y Diagramas

El sistema sigue una arquitectura modular orientada a servicios, separando la interfaz de usuario de la lógica de negocio y la persistencia de datos.

### Diagrama de Arquitectura (Mermaid)
```mermaid
graph LR
    Usuario --> Frontend
    Frontend --> API
    API --> Autenticación
    API --> DAO
    API --> Registro[Registro de actividad]
    DAO --> MySQL[(MySQL)]

    
   