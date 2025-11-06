# Análisis de Datos de AluraStore Latam

## 📋 Descripción del Proyecto

Este proyecto realiza un **análisis exploratorio comprehensivo** de datos de ventas de la red de tiendas **AluraStore** en América Latina. El análisis integra datos de **4 sucursales** diferentes, consolidando información sobre productos, vendedores, transacciones y ubicaciones geográficas para identificar patrones de compra, comportamiento de clientes y oportunidades de negocio.

## 🎯 Objetivo

Extraer insights valiosos del comportamiento de compra de los clientes en diferentes ubicaciones geográficas de América Latina, analizando:
- Distribución de ventas por categoría de producto
- Desempeño de vendedores
- Patrones de pago y financiamiento
- Satisfacción de clientes (calificaciones)
- Análisis geográfico de compras

## 📊 Fuentes de Datos

El proyecto utiliza **4 conjuntos de datos en formato CSV** alojados en un repositorio de GitHub de Alura:

- `tienda_1.csv` - Datos de la Tienda 1
- `tienda_2.csv` - Datos de la Tienda 2
- `tienda_3.csv` - Datos de la Tienda 3
- `tienda_4.csv` - Datos de la Tienda 4

Las URLs se cargan directamente desde el repositorio oficial de desafíos de Data Science.

## 🗂️ Estructura de los Datos

Cada conjunto de datos contiene las siguientes **12 columnas**:

| Columna | Tipo | Descripción |
|---------|------|-------------|
| **Producto** | String | Nombre del artículo vendido |
| **Categoría del Producto** | String | Clasificación del producto (Electrónicos, Muebles, Juguetes, etc.) |
| **Precio** | Float | Valor del producto en moneda local |
| **Costo de envío** | Float | Costo de envío del pedido |
| **Fecha de Compra** | String | Fecha en formato DD/MM/YYYY |
| **Vendedor** | String | Nombre del vendedor responsable |
| **Lugar de Compra** | String | Ciudad donde se realizó la compra |
| **Calificación** | Integer | Puntuación dada por el cliente (1-5) |
| **Método de pago** | String | Forma de pago utilizada (Tarjeta de crédito, Nequi, etc.) |
| **Cantidad de cuotas** | Integer | Número de cuotas si fue a plazos |
| **lat** | Float | Latitud de la ubicación geográfica |
| **lon** | Float | Longitud de la ubicación geográfica |

## 🚀 Requisitos y Dependencias

### Requisitos del Sistema
- **Python 3.7 o superior**
- **Jupyter Notebook** o **Google Colab**
- Conexión a Internet (para descargar los datos desde GitHub)

### Librerías de Python Necesarias

```
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
```

### Instalación de Dependencias

Para instalar todas las dependencias necesarias, ejecuta:

```bash
pip install pandas numpy matplotlib seaborn
```

O si utilizas Google Colab (ya incluye estas librerías):

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

## 📝 Cómo Ejecutar el Proyecto

### Opción 1: En Google Colab (Recomendado)

1. Abre el archivo `AluraStoreLatam-6.ipynb` en Google Colab
2. Ejecuta las celdas en orden secuencial
3. Los datos se cargarán automáticamente desde GitHub

### Opción 2: En Jupyter Notebook Local

1. Clona o descarga este repositorio
2. Abre una terminal en la carpeta del proyecto
3. Inicia Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Abre el archivo `AluraStoreLatam-6.ipynb`
5. Ejecuta las celdas en orden

### Paso a Paso de Ejecución

1. **Importación de Datos**: La primera celda carga los 4 archivos CSV desde GitHub
   ```python
   import pandas as pd
   
   url = "https://raw.githubusercontent.com/alura-es-cursos/..."
   tienda = pd.read_csv(url)
   ```

2. **Exploración Inicial**: Se realiza un análisis exploratorio de cada tienda
   ```python
   tienda.head()
   tienda.info()
   tienda.describe()
   ```

3. **Limpieza y Transformación**: Se procesan y preparan los datos
4. **Análisis y Visualización**: Se generan gráficos e insights
5. **Consolidación**: Se unifican los datos de todas las tiendas

## 📈 Secciones del Análisis

### 1. Exploración Inicial de los Datos
- Visualización de primeras filas de cada tienda
- Información sobre tipos de datos
- Estadísticas descriptivas
- Detección de valores nulos

### 2. Análisis por Tienda
- Información detallada de cada sucursal
- Comparativa entre tiendas
- Productos más vendidos
- Rendimiento de vendedores

### 3. Análisis de Categorías
- Distribución de ventas por categoría
- Precio promedio por categoría
- Categorías más populares
- Análisis de margen (Precio - Costo de envío)

### 4. Análisis de Vendedores
- Desempeño individual de vendedores
- Volumen de ventas
- Calificación promedio
- Consistencia en entregas

### 5. Análisis de Métodos de Pago
- Métodos más utilizados
- Preferencias por tienda
- Análisis de cuotas
- Relación entre método de pago y satisfacción

### 6. Análisis Geográfico
- Mapa de compras por ciudad
- Distribución regional
- Costos de envío por ubicación
- Zonas de mayor demanda

### 7. Análisis de Satisfacción del Cliente
- Distribución de calificaciones
- Relación entre precio y satisfacción
- Influencia del vendedor en la calificación
- Productos mejor valorados

## 🔍 Insights Esperados

Al completar este análisis, obtendrás conclusiones sobre:

✅ **Categorías de éxito**: Cuáles son los productos más rentables  
✅ **Vendedores estrella**: Quiénes generan mayor satisfacción  
✅ **Preferencias geográficas**: Diferencias regionales en comportamiento de compra  
✅ **Tendencias de pago**: Evolución en métodos de financiamiento  
✅ **Oportunidades**: Áreas de mejora y crecimiento  

## 🛠️ Tecnologías Utilizadas

- **Python 3** - Lenguaje de programación
- **Pandas** - Manipulación y análisis de datos
- **NumPy** - Computación numérica
- **Matplotlib** - Visualización de gráficos estáticos
- **Seaborn** - Visualización estadística avanzada
- **Jupyter Notebook** - Entorno interactivo de desarrollo

## 📂 Estructura de Archivos

```
AluraStore-Analysis/
├── AluraStoreLatam-6.ipynb        # Notebook principal
├── README.md                      # Este archivo
└── data/
    ├── tienda_1.csv              # Datos de tienda 1 (descargado)
    ├── tienda_2.csv              # Datos de tienda 2 (descargado)
    ├── tienda_3.csv              # Datos de tienda 3 (descargado)
    └── tienda_4.csv              # Datos de tienda 4 (descargado)
```

## 🐛 Troubleshooting - Problemas Comunes

### Problema: Error al descargar datos desde GitHub
**Solución**: Verifica tu conexión a Internet y que las URLs no hayan cambiado

### Problema: Módulos no encontrados (ImportError)
**Solución**: Instala las dependencias faltantes:
```bash
pip install pandas numpy matplotlib seaborn --upgrade
```

### Problema: El notebook se ejecuta lentamente
**Solución**: Reduce el tamaño de las visualizaciones o ejecuta en Google Colab que tiene más recursos

### Problema: Datos vacíos o inconsistentes
**Solución**: Verifica que todas las 4 tiendas se hayan cargado correctamente

## 📚 Conceptos de Python y Data Science Aplicados

Este proyecto enseña y utiliza:

- **Manipulación de datos**: Carga, limpieza y transformación con Pandas
- **Análisis exploratorio**: EDA (Exploratory Data Analysis)
- **Estadística descriptiva**: Media, mediana, desviación estándar
- **Visualización de datos**: Gráficos exploratorios
- **Consolidación de datos**: Unión de múltiples fuentes
- **Análisis geográfico**: Trabajo con coordenadas lat/lon
- **Interpretación de datos**: Extracción de insights

## 🎓 Contexto Educativo

Este proyecto forma parte del **Challenge de Data Science de Alura en Latinoamérica**, diseñado para:

- Desarrollar habilidades de análisis de datos
- Practicar con datos reales de comercio electrónico
- Aprender metodologías de Data Science
- Mejorar la capacidad de comunicar insights

## 🔗 Enlaces Útiles

- [Repositorio oficial de Alura](https://github.com/alura-es-cursos/challenge1-data-science-latam)
- [Documentación de Pandas](https://pandas.pydata.org/docs/)
- [Documentación de Matplotlib](https://matplotlib.org/stable/contents.html)
- [Documentación de Seaborn](https://seaborn.pydata.org/)

## 📝 Notas Importantes

- El análisis utiliza datos de ejemplo educativo
- No es necesario descargar archivos CSV manualmente
- El proyecto es completamente reproducible ejecutando el notebook
- Los resultados pueden variar según actualizaciones de los datos

## 🤝 Contribuciones y Mejoras

Este proyecto puede expandirse con:
- Análisis predictivo
- Modelos de machine learning
- Dashboards interactivos
- APIs para consultas dinámicas
- Análisis de series temporales

## 📄 Licencia

Este proyecto es educativo y forma parte del programa de formación de Alura.

---

**Creado con ❤️ para estudiantes de Data Science**

*Última actualización: Noviembre 2025*
