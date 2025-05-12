# Proyecto Final: Dashboard de Monitoreo de Torres Meteorológicas

## 🎯 Objetivo

Desarrollar un **dashboard interactivo** en Python que consuma, procese y visualice información en **tiempo real** proveniente de **torres meteorológicas simuladas**, gestionando la persistencia de datos en **múltiples bases de datos** y permitiendo la **interacción remota** a través de una interfaz y un bot de Telegram.

---

## 🛠️ Requisitos del Proyecto

### 1. Simulador de Torres Meteorológicas
- Implementado por el equipo utilizando **Python**.
- Funciona en **tiempo real** mediante **multihilos (threading)**.
- Genera datos meteorológicos que alimentan el sistema continuamente.
- Generar datos de fallos o problemas tecnicos de la misma torre.
- Datos que contendra la torren en el archivo anexo llamada [torres.md](torres.md)

### 2. Bases de Datos
El sistema debe almacenar y consultar datos desde al menos **tres fuentes**:
- [x] **SQLite**
- [x] **Supabase**
- [ ] **Base de datos adicional servidor propio** (ej: PostgreSQL, MySQL, MongoDB, Redis.)

### 3. Dashboard Web
El dashboard debe permitir:
- [x] **CRUD torres meteorológicas** desde la interfaz.
- [x] Enviar **comandos** a las torres en tiempo real.
- [x] **Crear y gestionar usuarios**.
- [x] **Asignar torres a usuarios específicos**.
- [x] **Subir archivos Excel** con información histórica.
- [x] **Descargar reportes** por torre(s) o por usuario y todas sus torres, formatos excel, pdf y imagen.
- [x] **Visualizar gráficas** con todas las torres.
- [x] **Filtros** en general o por grafica (Ejemplo: Ver solo temperatura).
- [x] **Mapa en tiempo real** con las ubicaciones de torres.
- [x] **Emitir alertas automáticas** si se detectan valores anómalos o fallas en torres, enviadas por medio del bot y en forma de alerta en el dashboard.

### 4. Funcionalidades Adicionales
- [x] **Sistema de login** con manejo de sesiones.
- [x] **Bot de Telegram** para:
  - Consultar el estado de las torres.
  - Recibir alertas o notificaciones en tiempo real.

### 5. Tecnologias base del proyecto
-   Python 
-   [plotly](https://plotly.com/product-tour/)
-   [streamlit](https://streamlit.io)
-   [dash](https://dash.plotly.com)
---

## ✅ Criterios de Evaluación

- ✔️ Funcionamiento correcto en **tiempo real**.
- ✔️ Integración efectiva de las bases de datos.
- ✔️ **Calidad del código**: modularidad, buenas prácticas, estructura.
- ✔️ **Diseño y usabilidad** del dashboard.
- ✔️ Nivel de **automatización e interacción** (bot, alertas, informes).
- ✔️ Documento de plan de trabajo, como y porque de las acciones tomadas, incluira diagramas, graficos.
- ✔️ **Repositorio en github y documentacion tecnica** del proyecto, para su correcta ejecuccion.
- ✔️ **Documentación y presentación** del proyecto.


