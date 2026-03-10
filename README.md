# Proyecto Integrador: Unificación de Datos y Chatbot Empresarial

## 📖 Contexto Empresarial
Una empresa líder busca un Ingeniero en Sistemas capaz de unificar sus silos de datos y construir un chatbot profesional para responder preguntas críticas de negocio en tiempo real. Este proyecto da solución a esa necesidad mediante la integración de bases de datos dispersas y la implementación de inteligencia artificial accesible para los usuarios de negocio.

## 🎯 Perfil del Proyecto
**Rol:** Data & Systems Engineer (Proyecto Integrador)

## 🚀 Competencias a Desarrollar
Durante el ciclo de vida de este desarrollo, se pondrán en práctica y se evaluarán las siguientes competencias:
* Análisis de Requerimientos y Estructuras de Datos.
* Diseño de Procesos ETL (Extracción, Transformación y Carga).
* Arquitectura de Software e Integración de Sistemas.

## 🛠️ Stack Tecnológico Propuesto
* **Backend:** Python
* **Base de Datos:** PostgreSQL.
* **Frontend:** HTML, JavaScript y Tailwind CSS.
* **Control de Versiones:** Git y GitHub.

## 📂 Arquitectura de Ramas y Estructura del Repositorio
### 🌿 Arquitectura de Ramas (GitFlow)

Para mantener el orden y facilitar el trabajo colaborativo sin conflictos, utilizaremos el modelo **GitFlow**, basado en ramas `main`, `develop`, `feature/*`, `release/*` y `hotfix/*`.

* 🌿 **`main`**: Rama principal (protegida). Contiene la versión estable de producción. Solo se integra código aquí mediante Pull Requests aprobados.
* 🌿 **`develop`**: Rama de integración. Aquí se consolidan los cambios antes de preparar una entrega hacia `main`.
* 🌿 **`feature/<nombre>`**: Rama por funcionalidad o tarea. Nace desde `develop` y se integra nuevamente a `develop` mediante Pull Request.
* 🌿 **`release/<version>`**: Rama de preparación de entrega. Nace desde `develop` para estabilizar cambios (ajustes finales, documentación, versionado) y luego se integra a `main`. Posteriormente se sincroniza también con `develop`.
* 🌿 **`hotfix/<nombre>`**: Rama para correcciones urgentes. Nace desde `main` y se integra a `main`. Posteriormente se sincroniza también con `develop`.

### 🧱 Estructura del Repositorio

Propuesta de estructura clara y escalable para un proyecto en Python, separando responsabilidades (configuración, base de datos, ETL, API y lógica de negocio):

```text
.
├── README.md
├── pyproject.toml
├── .gitignore
├── .env.example
├── docs/
│   ├── adr/
│   └── diagrams/
├── data/
│   ├── raw/
│   └── processed/
├── scripts/
├── tests/
└── src/
    └── chatbot_business/
        ├── __init__.py
        ├── config/
        ├── db/
        ├── etl/
        ├── services/
        ├── api/
        ├── llm/
        ├── utils/
        └── cli.py
```

> Nota: El nombre `chatbot_business/` es un ejemplo; se recomienda ajustarlo al nombre real del proyecto (sin espacios y en snake_case).

## 🔄 Flujo de Trabajo Colaborativo
El repositorio cuenta con reglas de protección en la rama `main`. Para contribuir al proyecto, los colaboradores deben seguir este flujo exacto:

1. Clonar el repositorio: `git clone <url-del-repositorio>`
2. Actualizar y posicionarse en la rama base de trabajo: `git checkout develop`
3. Crear una rama de trabajo desde `develop` (ejemplo): `git checkout -b feature/<nombre>`
4. Guardar y subir los cambios a la rama en la nube:
   ```bash
   git add .
   git commit -m "feat: descripción clara del cambio"
   git push origin <nombre-de-la-rama>
5. Ir a GitHub y crear un Pull Request hacia la rama `develop` (para ramas `feature/*`).
6. Esperar la revisión y aprobación del administrador del repositorio para la integración final.

> Nota: Las ramas `release/*` y `hotfix/*` se integran a `main` y luego se sincronizan también con `develop`.