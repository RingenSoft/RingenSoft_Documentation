# 🚢 RingenSoft Operations Center v6.0
> **Plataforma de Inteligencia Operativa y Optimización Logística para la Industria Pesquera.**

[![FastAPI](https://img.shields.io/badge/Backend-FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![Angular](https://img.shields.io/badge/Frontend-Angular%2017-DD0031?style=for-the-badge&logo=angular&logoColor=white)](https://angular.io/)
[![Scikit-Learn](https://img.shields.io/badge/AI-Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Google OR-Tools](https://img.shields.io/badge/Optimization-OR--Tools-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://developers.google.com/optimization)

## 🎯 Visión General
RingenSoft es un ecosistema híbrido diseñado para modernizar la gestión de flotas pesqueras en el litoral peruano. Mediante la integración de **telemetría satelital en tiempo real**, modelos de **Machine Learning** y algoritmos de **Investigación de Operaciones**, la plataforma transforma datos complejos en rutas de navegación optimizadas, minimizando costos de combustible y maximizando la captura de biomasa.

---

## 🚀 Componentes de Alto Impacto

### 🧠 Capa de Inteligencia Artificial (Data Science)
* **K-Means Clustering:** Implementación de un modelo de agrupamiento dinámico para identificar "Clusters Alfa" de biomasa, calculando centroides geográficos basados en densidad y tonelaje detectado.
* **Análisis Bioestadístico:** Aplicación de curvas Gaussianas de probabilidad sobre datos de Temperatura Superficial del Mar (SST) para predecir la presencia de especies pelágicas.
* **Telemetría Satelital:** Consumo asíncrono de la API de Open-Meteo para monitoreo oceanográfico en vivo sin latencia para el usuario.

### 🛣️ Motor de Optimización Logística
* **Google OR-Tools VRP:** Resolución del *Capacitated Vehicle Routing Problem* (CVRP) para asignar las rutas de recolección más eficientes a cada embarcación.
* **Algoritmo 2-Opt:** Refinamiento heurístico de rutas para eliminar cruces ineficientes y reducir el recorrido total en un **12-18%**.
* **Restricciones de Negocio:** Lógica programada para respetar la zona de exclusión artesanal (5 millas náuticas) y radios de autonomía operativa.

### 🛠️ Ecosistema DevSecOps y UI
* **Seguridad:** Autenticación robusta basada en **JWT (JSON Web Tokens)** con encriptación de contraseñas.
* **Rendimiento:** Implementación de caché en memoria para peticiones externas y optimización de consultas SQL (ORM) para cargas instantáneas.
* **Dashboard Gerencial:** Centro de control intuitivo con **Chart.js** y exportación de auditorías técnicas a PDF mediante **jsPDF**.



---

## 🛠️ Stack Tecnológico

| Capa | Tecnologías |
| :--- | :--- |
| **Backend** | Python, FastAPI, SQLAlchemy, MySQL/SQLite |
| **Data Science** | Scikit-Learn (ML), NumPy, Pandas |
| **Optimización** | Google OR-Tools (Constraint Programming) |
| **Frontend** | Angular 17+, Tailwind CSS, Chart.js |
| **Documentación** | OpenAPI (Swagger), Markdown |

---

## 🛰️ Próximo Hito: Engine de Visión Computacional (Alpha)
Estamos trabajando en la integración de un modelo de **Computer Vision** basado en redes neuronales (CNN) para el procesamiento de imágenes satelitales multiespectrales.

* **Procesamiento:** Filtrado de reflectancia para detección de biomasa superficial.
* **IA:** Entrenamiento de modelos para la clasificación de especies según morfología de cardúmenes.
* **Objetivo:** Eliminar la dependencia de reportes externos y generar alertas de pesca autónomas.

## 📦 Despliegue Rápido

### 1️⃣ Clonar y Backend
```bash
# Clonar repositorio
git clone [https://github.com/tu-usuario/ringensoft-project.git](https://github.com/tu-usuario/ringensoft-project.git)
cd ringensoft-project/backend

# Crear entorno virtual e instalar dependencias
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate
pip install -r requirements.txt

# Iniciar servidor
uvicorn main:app --reload


