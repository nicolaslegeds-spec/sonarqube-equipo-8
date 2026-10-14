# sonarqube-equipo-8
Proyecto de especialización en herramientas de testing - SonarQube
## 🚀 Finanzly - Sistema de Gestión Financiera y Control de Inventario

Proyecto desarrollado para la materia de testing e integración continua, enfocado en el control de finanzas personales.

### 👥 Equipo de Trabajo
* **Abraham** (Lead)
* **Lucas**
* **Marta**

---

### 💻 Instrucciones para la Ejecución Local

(Sprint 1)

Para ejecutar el proyecto en tu entorno local de desarrollo, sigue los siguientes pasos:

1. **Abrir la carpeta raíz** en tu entorno de desarrollo (por ejemplo, Visual Studio Code).
2. **Abrir la terminal integrada** en la ruta del proyecto (`Finanzly`).
3. **Instalar las dependencias** ejecutando el siguiente comando en la terminal: **npm install**
4. Luego ejecutar el siguiente comando en la terminal de VSCode **npm start**
5. Luego en la terminal presionar la tecla CTRL + Click Izquierdo sobre la URL generada.
6. Acceso a Finanzly desde tu navegador local

(Sprint 2)

## ⚙️ Archivos de Configuración y Análisis

El proyecto está configurado para ejecutarse localmente y ser analizado mediante **SonarQube Cloud / SonarCloud**. El archivo `sonar-project.properties` en la raíz contiene las reglas e inclusiones del análisis estático:

```properties
sonar.projectKey=finazly
sonar.organization=equipo-8-auditores
sonar.sources=public
sonar.sourceEncoding=UTF-8
