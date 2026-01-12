# Documentación

Esta carpeta contiene la documentación técnica y científica del proyecto DengueClima. 

## 📚 Contenido

| Archivo | Descripción | Estado |
|---------|-------------|--------|
| `fuentes_datos.md` | Descripción detallada de SIVIGILA, IDEAM y otras fuentes | 📋 Pendiente |
| `metodologia.md` | Enfoque científico, variables seleccionadas y justificación | 📋 Pendiente |
| `arquitectura.md` | Diseño técnico del sistema y flujo de datos | 📋 Pendiente |
| `referencias.md` | Papers y estudios científicos que respaldan el proyecto | 📋 Pendiente |

## 🔬 Fundamentación Científica

El proyecto DengueClima se basa en evidencia científica que demuestra la relación entre variables climáticas y la transmisión del dengue: 

### Variables Climáticas Clave

| Variable | Relación con Dengue | Fuente |
|----------|---------------------|--------|
| **Precipitación** | Crea criaderos de agua estancada para el mosquito Aedes aegypti | OMS, 2023 |
| **Temperatura** | El rango óptimo de reproducción del mosquito es 25-30°C | Estudios epidemiológicos |
| **Humedad relativa** | Afecta la supervivencia del mosquito adulto | Literatura científica |

### Retardo Temporal (Lag)

La relación entre clima y casos de dengue no es inmediata.  El ciclo completo es: 

1. **Semana 0**: Lluvia genera agua estancada
2. **Semanas 1-2**:  Mosquitos ponen huevos, larvas se desarrollan
3. **Semanas 2-3**: Mosquitos adultos emergen y pican
4. **Semanas 3-4**: Período de incubación del virus en humanos
5. **Semanas 4-6**: Aparición de síntomas y reporte al sistema de salud

Por esto, el modelo utiliza variables con retardo de **4 a 8 semanas**. 

## 🎯 Enfoque del Proyecto

### Diferenciadores

1. **Predicción a nivel municipal**: La mayoría de estudios trabajan a nivel departamental o nacional.  DengueClima predice para cada uno de los 42 municipios del Valle del Cauca.

2. **Doble audiencia**: No solo autoridades de salud, sino también ciudadanía con acceso a información de riesgo. 

3. **Datos abiertos**: Uso exclusivo de fuentes públicas, permitiendo replicabilidad y transparencia.

4. **Escalabilidad regional**: Diseñado para adaptarse a cualquier región de Latinoamérica con datos similares.

## 📖 Referencias Clave

1. Instituto Nacional de Salud (INS) - Protocolos de vigilancia del dengue en Colombia
2. Organización Mundial de la Salud (OMS) - Dengue y dengue grave
3. IDEAM - Metodología de medición de variables climáticas en Colombia

---

*Documentación en desarrollo activo*
