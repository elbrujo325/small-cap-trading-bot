# 📈 Trading Bot: Backtesting de Estrategias para Small Caps

**Autor:** Henry Paolo Alfaro Sotil  
**Perfil:** Estudiante de Física (UNMSM) | Analista de Datos Cuantitativos  
**Contacto:** [henry.alfaro1@unmsm.edu.pe](mailto:henry.alfaro1@unmsm.edu.pe)

---

## 📝 Descripción del Proyecto
Este repositorio contiene un sistema de **análisis cuantitativo y backtesting** desarrollado en Python para evaluar estrategias sistemáticas en acciones de baja capitalización (*Small Caps*) del mercado estadounidense. 

El proyecto aplica principios de modelado matemático y física computacional para simular operaciones de mercado, gestionando el riesgo mediante indicadores de volatilidad técnica.

## 🛠️ Tecnologías Utilizadas
* **Lenguaje:** Python
* **Librerías de Datos:** Pandas, NumPy
* **Visualización:** Matplotlib (GridSpec para dashboards analíticos)
* **Finanzas:** yfinance (Extracción de datos de mercado en tiempo real)

## 📊 Lógica de la Estrategia
El bot opera bajo una metodología **Long-Only** con los siguientes parámetros técnicos:

| Parámetro | Configuración |
|-----------|---------------|
| **Universo** | Acciones entre $1.00 y $20.00 USD |
| **Gestión de Riesgo** | 1% del capital por operación |
| **Stop Loss (SL)** | 1.9 × ATR (Volatilidad dinámica) |
| **Take Profit (TP)** | 3.2 × ATR |
| **Ratio R:R** | 1:1.68 |

### Condiciones de Entrada
1. **Filtro de Tendencia:** Precio de apertura superior a la Media Móvil Simple (SMA 10).
2. **Momentum:** Desaceleración del Rate of Change (ROC) para identificar puntos de giro.
3. **Estructura:** Confirmación mediante ruptura de niveles de precios previos.

## 📈 Resultados y KPIs
El notebook genera un reporte estadístico detallado que incluye:
* **Profit Factor:** Relación entre ganancias y pérdidas brutas.
* **Win Rate:** Porcentaje de operaciones exitosas.
* **Max Drawdown:** Máxima pérdida consecutiva desde el pico de capital.
* **Sharpe Ratio:** Retorno ajustado al riesgo.

## 🚀 Cómo Ejecutarlo
1. Clona este repositorio.
2. Asegúrate de tener instalado Python y las dependencias:
   ```bash
   pip install pandas numpy matplotlib yfinance
