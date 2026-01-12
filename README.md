# 🦟 DengueClima

**Sistema de predicción de dengue basado en variables climáticas usando datos abiertos de Latinoamérica**

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![License:  MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status](https://img.shields.io/badge/Status-En%20Desarrollo-orange.svg)]()

---

## 📋 Descripción

DengueClima es un sistema de predicción temprana de brotes de dengue que utiliza la correlación entre variables climáticas (precipitación, temperatura, humedad) y la incidencia de casos de dengue. 

El proyecto busca proporcionar una herramienta de doble impacto: 

1. **Para autoridades de salud pública**: Anticipar brotes epidémicos con semanas de anticipación, optimizando la asignación de recursos y las campañas de prevención. 

2. **Para la ciudadanía**:  Brindar acceso a información clara y oportuna sobre el nivel de riesgo en su municipio, empoderando a las personas para tomar acciones preventivas en sus hogares y comunidades.

## 🎯 Problema que Resuelve

El dengue es una enfermedad endémica en regiones tropicales que afecta a millones de personas anualmente.  Actualmente existen dos problemas críticos:

**Desde las instituciones:**
- Las autoridades sanitarias reaccionan **después** de detectar aumentos en los casos reportados, perdiendo tiempo valioso para la prevención. 

**Desde la ciudadanía:**
- Las personas no tienen acceso a información anticipada sobre el riesgo en su zona.
- La prevención depende de campañas esporádicas, no de información continua y personalizada.

## 💡 Solución

DengueClima propone un enfoque integral:

### Para Autoridades de Salud Pública
- **Anticipar** brotes con 4-8 semanas de anticipación
- **Focalizar** recursos en municipios de alto riesgo
- **Optimizar** campañas de fumigación y eliminación de criaderos
- **Monitorear** la efectividad de las intervenciones

### Para la Ciudadanía
- **Consultar** mapas de riesgo interactivos por municipio
- **Recibir** alertas tempranas cuando el riesgo aumenta en su zona
- **Aprender** acciones preventivas específicas según el nivel de riesgo
- **Participar** activamente en la eliminación de criaderos

## 🌎 Alcance

- **Fase inicial**: Valle del Cauca, Colombia (42 municipios)
- **Escalabilidad**: Cualquier región con datos epidemiológicos y climáticos disponibles

## 📊 Fuentes de Datos

| Fuente | Tipo de Datos | Cobertura |
|--------|---------------|-----------|
| [SIVIGILA](https://www.datos.gov.co) | Casos de dengue por semana epidemiológica | Colombia, 2007-2024 |
| [IDEAM](http://dhime.ideam.gov.co) | Precipitación, temperatura, humedad | Colombia, estaciones meteorológicas |

## 🔬 Metodología

1. **Recolección de datos**:  Integración de fuentes epidemiológicas y climáticas
2. **Preprocesamiento**:  Agregación por semana epidemiológica y municipio
3. **Ingeniería de características**: Variables con retardo temporal (lag), promedios móviles
4. **Modelado**: Algoritmos de Machine Learning (Random Forest, XGBoost)
5. **Validación**: Evaluación con datos históricos no vistos por el modelo
6. **Visualización**: Interfaces accesibles para autoridades y ciudadanía

## 📁 Estructura del Repositorio

```
DengueClima/
├── README.md                # Este archivo
├── LICENSE                  # Licencia MIT
├── . gitignore               # Archivos ignorados
├── docs/                    # Documentación técnica
├── notebooks/               # Jupyter Notebooks con análisis
├── data/                    # Información sobre fuentes de datos
├── src/                     # Código fuente del proyecto
└── images/                  # Visualizaciones y gráficos
```

## 🚀 Resultados Preliminares

### Datos Analizados
- **170,438** casos de dengue en el Valle del Cauca (2007-2022)
- **42** municipios monitoreados
- **16** años de datos históricos

### Hallazgos Iniciales
- Ciclos epidémicos cada 3-4 años (picos en 2010, 2013, 2016, 2020)
- Correlación entre precipitación y casos de dengue con retardo de 4-8 semanas
- El municipio de Cali concentra el 63% de los casos del departamento

## 🛠️ Tecnologías

- **Lenguaje**:  Python 3.8+
- **Análisis de datos**:  Pandas, NumPy
- **Visualización**: Matplotlib, Seaborn
- **Machine Learning**:  Scikit-learn, XGBoost
- **Notebooks**: Jupyter, Google Colab

## 📈 Estado del Proyecto

| Fase | Descripción | Estado |
|------|-------------|--------|
| 1 | Exploración y validación de datos | ✅ Completado |
| 2 | Integración de fuentes de datos | 🔄 En progreso |
| 3 | Construcción del modelo predictivo | 📋 Pendiente |
| 4 | Validación y ajuste | 📋 Pendiente |
| 5 | Despliegue y documentación | 📋 Pendiente |

## 🎯 Audiencias Objetivo

| Audiencia | Necesidad | Solución DengueClima |
|-----------|-----------|----------------------|
| **Secretarías de Salud** | Anticipar brotes para planificar recursos | Predicciones semanales por municipio con nivel de riesgo |
| **Ciudadanía** | Saber cuándo protegerse y actuar | Mapas de riesgo públicos y alertas por zona |
| **Investigadores** | Datos integrados para estudios | Datasets abiertos y metodología documentada |

## 👥 Equipo

- **Kevin Agredo Jara** - Desarrollador Principal

## 📄 Licencia

Este proyecto está bajo la Licencia MIT.  Ver el archivo [LICENSE](LICENSE) para más detalles. 

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor, abre un issue primero para discutir los cambios propuestos.

---

**Proyecto desarrollado para el [Data2AI Challenge LATAM](https://data2ai.com)**
