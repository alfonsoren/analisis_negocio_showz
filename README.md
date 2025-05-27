# 📊 Análisis de Negocio: Showz

## 📌 Descripción del Proyecto

Este proyecto se centra en un análisis de negocio para la plataforma **Showz**, con el objetivo de evaluar el rendimiento de las campañas de marketing, el comportamiento del usuario y la rentabilidad.

Se exploran métricas clave como:

- DAU (Usuarios Activos Diarios)
- WAU (Usuarios Activos Semanales)
- MAU (Usuarios Activos Mensuales)
- LTV (Valor de Vida del Cliente)
- CAC (Costo de Adquisición de Clientes)
- ROMI (Retorno de Inversión en Marketing)

El análisis busca identificar las fuentes de marketing más efectivas, entender la dinámica de retención de usuarios y proporcionar **recomendaciones estratégicas** para maximizar ingresos.

---

## ❓ Preguntas Clave de Negocio

- ¿Cómo se comportan los usuarios en términos de visitas y compras a lo largo del tiempo?
- ¿Cuál es el valor de vida del cliente (LTV) y cómo varía entre cohortes?
- ¿Cuál es el costo de adquisición de clientes (CAC) por fuente de marketing?
- ¿Qué fuentes de marketing tienen el mejor retorno de la inversión (ROMI)?
- ¿Existen diferencias significativas en el comportamiento del usuario según el dispositivo o la plataforma?

---

## 📂 Datos Utilizados

- `visits_log_us.csv`: Registro de visitas de usuarios, dispositivo, timestamps y fuente.
- `orders_log_us.csv`: Compras realizadas, ingresos generados y UID.
- `costs_us.csv`: Costos de marketing por fuente y fecha.

---

## 🔍 Metodología del Análisis

### 1. Limpieza y Preprocesamiento

- Carga de datasets y librerías (pandas, numpy, seaborn, matplotlib, datetime).
- Revisión de tipos de datos, valores nulos y duplicados.
- Normalización de nombres de columnas a snake_case.
- Conversión de fechas a formato datetime.
- Eliminación de sesiones con errores (ej. `end_ts < start_ts`).

### 2. Cálculo de Métricas

- **Usuarios activos** (DAU, WAU, MAU)
- **Duración promedio de sesiones**
- **Retención de usuarios** por cohortes
- **LTV** por cohorte y fuente
- **CAC** por fuente
- **ROMI** (ROI del marketing)
- **Análisis por dispositivo** (móvil vs escritorio)

### 3. Visualización

- Tendencias temporales de usuarios activos
- Heatmaps de retención por cohortes
- Comparativas de CAC y LTV por fuente
- ROMI por canal de marketing

---

## ✅ Conclusiones Clave

- **Usuarios Activos:** Crecimiento constante con un promedio de **907 DAU**, **5716 WAU** y **23228 MAU**.
- **Sesiones:** Duración media de ~30 minutos, indicando buen engagement.
- **LTV:** Promedio de **$6.90 USD**, superando los $10 en algunas cohortes.
- **CAC:** Varía significativamente por fuente.
- **ROMI:** 
  - **Fuente 1** es la más rentable (>60% ROMI).
  - **Fuentes 2, 3, 4 y 10** muestran ROMI negativo.

### 🎯 Recomendaciones

- Reforzar la inversión en la fuente 1.
- Reevaluar fuentes con ROMI negativo.
- Implementar estrategias de **retargeting** para usuarios inactivos.
- Optimizar la experiencia por dispositivo y plataforma.

---

## 🛠 Tecnologías Utilizadas

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Datetime



