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

* 🌿 **`main`**: Rama principal (Protegida). Solo el administrador puede integrar código aquí mediante Pull Requests aprobados. Contiene la versión estable de producción.
* 🌿 **`backend`**: Desarrollo de la API, orquestación del chatbot y procesos ETL
* 🌿 **`database`**: Scripts SQL, esquemas, configuración de PostgreSQL y migraciones.
* 🌿 **`frontend`**: Desarrollo de la interfaz de usuario con Tailwind, HTML y JS.
* 🌿 **`documentation`**: Manuales, diagramas de arquitectura, diccionario de datos y requerimientos.
* 🌿 **`test`**: Entorno seguro para realizar pruebas de integración entre los diferentes módulos antes de pasar a `main`.

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