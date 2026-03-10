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
Para mantener el orden y facilitar el trabajo colaborativo sin conflictos, el proyecto está dividido en ramas de trabajo específicas. Cada equipo o colaborador debe trabajar **exclusivamente** en su rama designada:

* 🌿 **`main`**: Rama principal (Protegida). Solo el administrador puede integrar código aquí mediante Pull Requests aprobados. Contiene la versión estable de producción.
* 🌿 **`backend`**: Desarrollo de la API, orquestación del chatbot y procesos ETL
* 🌿 **`database`**: Scripts SQL, esquemas, configuración de PostgreSQL y migraciones.
* 🌿 **`frontend`**: Desarrollo de la interfaz de usuario con Tailwind, HTML y JS.
* 🌿 **`documentation`**: Manuales, diagramas de arquitectura, diccionario de datos y requerimientos.
* 🌿 **`test`**: Entorno seguro para realizar pruebas de integración entre los diferentes módulos antes de pasar a `main`.

## 🔄 Flujo de Trabajo Colaborativo
El repositorio cuenta con reglas de protección en la rama `main`. Para contribuir al proyecto, los colaboradores deben seguir este flujo exacto:

1. Clonar el repositorio: `git clone <url-del-repositorio>`
2. Cambiar a la rama asignada (ejemplo, para trabajar en la interfaz): `git checkout frontend`
3. Trabajar únicamente en los archivos correspondientes a su área para evitar conflictos.
4. Guardar y subir los cambios a la rama en la nube:
   ```bash
   git add .
   git commit -m "feat: descripción clara del cambio"
   git push origin <nombre-de-la-rama>
5. Ir a GitHub y crear un Pull Request hacia la rama main.
6. Esperar la revisión y aprobación del administrador del repositorio para la integración final.