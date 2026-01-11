# Datos

Esta carpeta contiene información sobre las fuentes de datos y muestras representativas. 

## ⚠️ Nota Importante

Los datasets completos **no se almacenan en este repositorio** debido a su tamaño. 
Aquí encontrarás: 
- Documentación de las fuentes
- Muestras pequeñas para pruebas
- Scripts de descarga

## Fuentes de Datos

### 1. Datos Epidemiológicos - SIVIGILA

| Atributo | Valor |
|----------|-------|
| **Fuente** | Sistema de Vigilancia en Salud Pública - Instituto Nacional de Salud (INS) |
| **URL** | https://www.datos.gov. co |
| **Período** | 2007 - 2024 |
| **Cobertura** | Nacional (Colombia) |
| **Granularidad** | Semanal, por municipio |
| **Variables clave** | Año, semana epidemiológica, departamento, municipio, número de casos |
| **Formato** | CSV |
| **Acceso** | Público, sin autenticación |

### 2. Datos Climáticos - IDEAM

| Atributo | Valor |
|----------|-------|
| **Fuente** | Instituto de Hidrología, Meteorología y Estudios Ambientales |
| **URL** | http://dhime.ideam.gov.co |
| **Período** | Variable por estación (desde 1920 en algunas) |
| **Cobertura** | Nacional (Colombia) |
| **Granularidad** | Diaria, por estación meteorológica |
| **Variables clave** | Precipitación, temperatura, humedad relativa |
| **Formato** | CSV |
| **Acceso** | Público, sin autenticación |

## Cómo Obtener los Datos Completos

Consulta los notebooks en la carpeta `notebooks/` para instrucciones detalladas de descarga y procesamiento. 
