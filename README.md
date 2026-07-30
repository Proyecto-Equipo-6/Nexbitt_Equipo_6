# Nexbitt — Proyecto ADSO

Sistema de comercio electrónico con backend, frontend web y aplicación móvil.

## Estructura del Proyecto

```
├── docs/               # Documentación del proyecto
│   ├── RF/             Requisitos funcionales
│   ├── RNF/            Requisitos no funcionales
│   ├── Casos_de_Uso/   Diagramas y descripciones
│   ├── BPMN/           Diagramas de procesos
│   ├── DER/            Diagrama entidad-relación
│   ├── Diccionario_BD/ Diccionario de base de datos
│   └── Manuales/       Manuales de usuario/técnico
│
├── backend/            # API REST (Node.js + Express + Prisma)
│
├── frontend/           # Aplicación web (React + Vite)
│
├── mobile/             # Aplicación móvil (Android/Kotlin)
│
├── database/           # Scripts SQL (schema, seed, migraciones)
│
├── docker/             # Archivos Docker (compose, Dockerfiles)
│
├── qa/                 # Aseguramiento de calidad
│   ├── 01_Plan_Maestro_Pruebas/
│   ├── 02_Casos_de_Prueba/
│   ├── 03_Matriz_Trazabilidad/
│   ├── 04_Registro_Bugs/
│   ├── 05_Evidencias/
│   ├── 06_Informes/
│   ├── 07_Metricas/
│   └── 08_Presentaciones/
│
├── .github/            # Workflows y templates de GitHub
│
└── README.md
```

## Stack

| Módulo | Tecnologías |
|--------|------------|
| Backend | Node.js, Express 5, Prisma ORM, MySQL, Socket.IO, JWT, Cloudinary |
| Frontend | React 19, Vite, Bootstrap, React Router, Socket.IO Client |
| Mobile | Kotlin, Android SDK, Jetpack |
| Base de datos | MySQL 8 |
| Docker | Docker Compose |
| QA | Plan de pruebas, casos de prueba, matriz de trazabilidad, bugs |

## Requisitos

- Node.js v18+
- MySQL 8+
- Android Studio + SDK (para mobile)
- Docker (opcional)

## Inicio Rápido

Ver README individual de cada módulo:

- [`backend/README.md`](backend/README.md)
- [`frontend/README.MD`](frontend/README.MD)
- [`mobile/README.md`](mobile/README.md)

## Docker

```bash
docker compose -f docker/docker-compose.yml up -d
```
