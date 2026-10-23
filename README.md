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

`properties
sonar.projectKey=finazly
sonar.organization=equipo-8-auditores
sonar.sources=public
sonar.sourceEncoding=UTF-8`

(Sprint 3)

---

## 🛠️ Tecnologías Utilizadas

* **Frontend:** HTML5, CSS3 (Modo Oscuro/Claro nativo), JavaScript Vanilla (ES6+).
* **Librerías de UI & Visualización:** Chart.js, FullCalendar, Flatpickr, jsPDF, SheetJS (XLSX).
* **Backend & API:** Node.js, Express.js.
* **Base de Datos:** PostgreSQL (Supabase / DB Relacional).
* **Auditoría & Análisis Estático (SAST):** SonarQube Cloud / SonarCloud.
* **Control de Versiones:** Git, GitHub.

---

## 📌 Novedades y Optimizaciones (Sprint 3)

En este Sprint 3, el equipo enfocó sus esfuerzos en la optimización del código, el blindaje de seguridad y la mejora de la accesibilidad, logrando una calificación limpia en **SonarQube Cloud**:

1. **Mitigación de Vulnerabilidades SAST (Ciberseguridad):**
   * **`jssecurity:S8476` en `public/script.js`:** Se eliminó el riesgo de *Client-Side Request Forgery* mediante la sanitización estricta y el casteo numérico explícito (`Number()`) de `id_usuario` en las peticiones `fetch()`.
   * **`javascript:S2068` en `public/login.js`:** Se desacopló la asignación directa de propiedades CSS sobre variables de contraseña para erradicar falsos positivos de credenciales expuestas en código.

2. **Mejoras de Accesibilidad (Estándares W3C):**
   * **`Web:S6853` & `Web:InputWithoutLabelCheck` en `index.html` y `transacciones.html`:** Asociación explícita de etiquetas (`label`) mediante atributos `for` e `id` en controles de formularios y selectores de meses en la comparativa.

---

## 💻 Instrucciones de Instalación y Ejecución Local

### Prerrequisitos
* Tienes que tener instalado **Node.js** (versión 18 o superior).
* Contar con una cuenta o instancia configurada de **Supabase / PostgreSQL**.

### Pasos para iniciar la aplicación:

1. **Clonar el repositorio:**
   ```bash
   git clone [https://github.com/Abraham-7/Finanzly.git](https://github.com/Abraham-7/Finanzly.git)
   cd Finanzly
