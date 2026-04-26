# Proyecto Integrador: Gestión de Logística Segura 

##  Descripción del Proyecto
Este proyecto consiste en el diseño técnico y la planificación de una plataforma logística para el transporte de mercancías críticas. El sistema garantiza la seguridad y la integridad de la carga mediante la monitorización en tiempo real de rutas, conductores, vehículos y sensores de temperatura.

Actuamos como una consultora tecnológica proporcionando la arquitectura, el plan de pruebas y la estrategia de optimización requerida.

---

## Equipo y Roles
* **[Javier Delgado]** - **Arquitecto de Software & DevOps**: Responsable de la estructura UML, elección tecnológica y gestión de Git.
* **[Sara Moreno]** - **Analista de QA & Optimización**: Responsable del plan de pruebas y detección de fallos de diseño.
* **[Lourdes Molina]** - **Analista de Sistemas & Documentalista**: Responsable de requisitos, casos de uso y manuales técnicos.

---

##  Metodología de Trabajo
Hemos seleccionado la metodología **Scrum (Ágil)** para este proyecto. 
* **Justificación**: Dada la naturaleza crítica del transporte y la necesidad de integrar sensores en tiempo real, Scrum nos permite realizar revisiones incrementales y adaptar el diseño ante cualquier fallo detectado en las fases de prueba o análisis de riesgos.
* **Gestión de Tareas**: Utilizamos un tablero de tareas para la organización del flujo de trabajo.

---

## Flujo de Trabajo (GitFlow)
Para garantizar la integridad del diseño, utilizamos el siguiente esquema de ramas:

* **`main`**: Contiene exclusivamente la documentación y el diseño final listo para la entrega.
* **`develop`**: Rama de integración donde se consolidan las fases del proyecto antes de pasar a la versión final.
* **`feature/`**: Ramas de trabajo individuales para cada funcionalidad o fase:
    * `feature/disenio-uml`: Modelado de diagramas.
    * `feature/plan-pruebas`: Diseño de tests de calidad.
    * `feature/documentacion`: Elaboración de manuales y Javadoc.

---

##  Tecnologías y Entorno
* **IDE**: Visual Studio Code.
* **Extensiones Imprescindibles**:
    1.  **Extension Pack for Java**: Soporte de lenguaje y estructura.
    2.  **PlantUML**: Creación de diagramas de Casos de Uso, Clases y Secuencia.

---

##  Estructura del Repositorio
* `/docs`: Diagramas UML y Manuales Técnicos.
* `/src`: Estructura de clases y lógica del sistema.
* `/tests`: Plan de pruebas de caja negra y unitarias.
