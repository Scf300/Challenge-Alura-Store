# 📊 AluraStore Latam - Análisis Comparativo de Tiendas

## 📋 Descripción del Proyecto

Este proyecto presenta un **análisis exhaustivo de datos** de cuatro tiendas pertenecientes a AluraStore Latam, con el objetivo de proporcionar una recomendación estratégica sobre cuál tienda es más conveniente vender. El análisis considera múltiples factores operacionales, financieros y de satisfacción del cliente.

## 🎯 Objetivo Principal

Determinar cuál de las cuatro tiendas del Sr. Juan presenta el menor potencial estratégico y es recomendable vender, considerando:
- Ingresos totales generados
- Desempeño por categorías de productos
- Satisfacción del cliente (calificaciones promedio)
- Análisis de eficiencia de ventas por categoría
- Costos operativos de envío

## 📁 Estructura del Proyecto

```
├── AluraStoreLatam-8.ipynb       # Notebook principal con análisis completo
├── README.md                      # Este archivo
└── datos/                         # Fuente de datos (URLs de GitHub)
    ├── tienda_1.csv
    ├── tienda_2.csv
    ├── tienda_3.csv
    └── tienda_4.csv
```

## 🔍 Análisis Realizado

### 1. **Análisis de Ingresos Totales**
- **Tienda 1**: $1,150,880,400 (Mayor facturación)
- **Tienda 2**: $1,116,343,500
- **Tienda 3**: $1,098,019,600
- **Tienda 4**: $1,038,375,700 (Menor facturación - 10.8% menos que Tienda 1)

### 2. **Desempeño por Categorías de Productos**
Las cuatro tiendas operan con un patrón de categorías consistente:
- **Top 3 categorías** (por facturación): Electrónicos, Electrodomésticos, Muebles
- **Bottom 3 categorías** (por facturación): Libros, Artículos para el hogar, Deportes y diversión

### 3. **Calificaciones Promedio de Clientes**
- **Tienda 3**: 4.048 (Mejor satisfacción)
- **Tienda 2**: 4.037
- **Tienda 4**: 3.996
- **Tienda 1**: 3.977 (Menor satisfacción)

### 4. **Análisis de Eficiencia de Ventas**
Se identificaron patrones estratégicos diferenciados:
- **Tienda 1**: Estrategia de precios premium (12.4% más alto en Instrumentos Musicales)
- **Tienda 4**: Estrategia de competencia por precio (vende más unidades a precios más bajos)
- **Tienda 3**: Balance óptimo (vende más a precios competitivos)
- **Tienda 2**: Precios premium en Electrónicos

### 5. **Costo Promedio de Envío**
- **Tienda 4**: $23,459.46 (Más bajo)
- **Tienda 3**: $24,805.68
- **Tienda 2**: $25,216.24
- **Tienda 1**: $26,018.61 (Más alto)

**Nota**: Los costos de envío son cubiertos por los clientes y no representan un costo directo para la tienda.

## 💡 Hallazgos Clave

### Patrón Anómalo de Tienda 4
La Tienda 4 sigue una estrategia de **competencia por volumen con márgenes bajos**:
- ✓ Vende más unidades en varias categorías
- ✗ Genera menores ingresos totales porque sus precios promedio son más bajos
- ✗ No percibe ventaja competitiva en satisfacción del cliente
- ✗ Menor margen de utilidad potencial

### Estrategias Exitosas
- **Tienda 1**: Precios premium generan mayores ingresos a pesar de menor volumen
- **Tienda 3**: Balance perfecto entre cantidad y precio = Mayor satisfacción del cliente

## 🎯 Recomendación Final

### **Se recomienda vender la Tienda 4**

#### Justificación:

1. **Menores ingresos totales**: $112 millones menos que Tienda 1 (10.8% de diferencia)

2. **Estrategia inefectiva**: Compite por precio pero no obtiene ventaja en satisfacción del cliente (calificación: 3.996)

3. **Márgenes más ajustados**: Vende más unidades a precios más bajos, limitando ganancias por transacción

4. **Menor potencial de crecimiento**: Las limitaciones estructurales (ubicación, mercado) no se compensan únicamente con eficiencia logística

5. **Optimización del portafolio**: Permite concentrar recursos en las tres tiendas más rentables y eficientes

#### Por qué NO vender las otras:

- **Tienda 1**: Máximo desempeño financiero con estrategia de precios premium exitosa
- **Tienda 2**: Balance sólido entre ingresos y satisfacción del cliente
- **Tienda 3**: Mejor modelo operativo en términos de satisfacción y balance eficiencia-volumen

## 📊 Visualizaciones Principales

El notebook incluye múltiples visualizaciones:
1. **Gráfico de Cantidad vs Facturación**: Comparación normalizada (escala 0-100) que evidencia diferencias de precios
2. **Tabla Comparativa de Calificaciones**: Desempeño por categoría en cada tienda
3. **Análisis de Facturación por Categoría**: Identificación de categorías clave
4. **Métodos de Pago**: Preferencias de clientes por tienda

## 🛠️ Tecnologías Utilizadas

- **Python 3**: Lenguaje principal
- **Pandas**: Análisis y manipulación de datos
- **NumPy**: Operaciones numéricas
- **Matplotlib**: Visualización de datos
- **Google Colab**: Entorno de desarrollo

## 📈 Métodos de Análisis

- **Análisis Descriptivo**: Cálculo de métricas y estadísticas
- **Análisis Comparativo**: Benchmarking entre tiendas
- **Normalización de Datos**: Escala 0-100 para comparación de variables con rangos diferentes
- **Visualización Avanzada**: Gráficos de barras agrupadas y superpuestas

## 📌 Datos Base

- **Período**: 2020-2023
- **Registros por tienda**: ~2,359 transacciones
- **Categorías**: 8 categorías de productos
- **Ciudades**: Múltiples ciudades en Colombia (Bogotá, Medellín, Cali, etc.)

## 🎓 Contexto Educativo

Este proyecto fue desarrollado como parte de un desafío de análisis de datos, implementando técnicas de:
- Carga y exploración de datos
- Limpieza y validación de datos
- Análisis exploratorio (EDA)
- Storytelling con datos
- Toma de decisiones basada en datos

## 📞 Instrucciones de Uso

1. **Abrir el notebook** en Google Colab
2. **Ejecutar celdas secuencialmente** para reproducir el análisis
3. **Visualizar gráficos** para comprender patrones
4. **Revisar conclusiones** en la sección final

## 🔧 Personalización

Para adaptarse a otros análisis:
- Modificar URLs de datos en la sección de importación
- Ajustar los rangos de normalización según necesidad
- Agregar nuevas categorías o tiendas
- Extender el período de análisis

## 📝 Notas Importantes

- Los costos de envío son **pagados por clientes**, no por tiendas
- Análisis **normalizado a escala 0-100** para comparabilidad
- Recomendación basada en **análisis cuantitativo integral**
- Considera factores financieros, operacionales y de satisfacción

## ✅ Conclusión

El análisis integral de AluraStore Latam proporciona evidencia clara de que **Tienda 4 es la candidata ideal para vender**, permitiendo al Sr. Juan optimizar su portafolio concentrándose en operaciones más rentables y eficientes con modelos comerciales más exitosos.

---

**Autor**: Estudiante de Data Science  
**Fecha**: Noviembre 2025  
**Desafío**: Challenge Alura Store - Data Science Latam