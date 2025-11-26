# Configuración Jenkins para Integración Continua

Este repositorio contiene un ejemplo básico de configuración para **Jenkins**, orientado a la automatización de tareas de integración continua (CI) en proyectos Python.

---

## ⚙️ Contenido del repositorio

```
Jenkins/
│── Jenkinsfile        # Pipeline declarativo para Jenkins
│── ejemplo.py         # Script de ejemplo para pruebas o despliegue
```

---

## 🧩 ¿Qué hace el Jenkinsfile?

El archivo `Jenkinsfile` define un pipeline de CI que puede incluir:

- Instalación de dependencias
- Ejecución de pruebas
- Validación de código
- Despliegue automatizado

Este archivo está diseñado para ser usado en un entorno Jenkins con agentes configurados para ejecutar scripts Python.

---

## 🚀 Uso

1. Clona el repositorio en tu servidor Jenkins:

```bash
git clone https://github.com/Devsebastian44/Jenkins.git
```

2. Crea un nuevo proyecto tipo *Pipeline* en Jenkins.

3. En la configuración del proyecto, selecciona “Pipeline script from SCM” y apunta al repositorio.

4. Jenkins ejecutará automáticamente el pipeline definido en `Jenkinsfile`.

---

## 📜 Licencia

Este proyecto está bajo la licencia **GPL-3.0**.  
Puedes usarlo libremente con fines educativos y de investigación.
