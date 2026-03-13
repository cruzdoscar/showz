# Proyecto Showz
## 🎯Objetivo General

Optimizar el gasto de marketing de **Showz** (vta. de entradas) mediante un análisis de **Unit Economics** y **Cohortes**. Debo decidir en qué plataformas invertir y cuánto, basándome en datos de comportamiento, ventas y costos de 2017-2018.

## 📊 Datos Disponibles

1. **`visits`**: Logs de sesiones (`Uid`, `Device`, `Start/End Ts`, `Source Id`). *Métrica clave: Engagement y Retención.*
2. **`orders`**: Transacciones (`Uid`, `Buy Ts`, `Revenue`). *Métrica clave: LTV y Conversión.*
3. **`costs`**: Inversión publicitaria (`source_id`, `dt`, `costs`). *Métrica clave: CAC y ROMI.*

## 🛠 Metodología de Análisis

- **Preparación:** Limpieza, conversión de tipos `datetime` y unión de tablas por `Uid` y `Source Id`.
- **Análisis de Producto (Visitas):** Calcular **DAU/WAU/MAU**, duración de sesiones y factor de adherencia (stickiness).
- **Análisis de Ventas:** Determinar el tiempo de conversión (ej. *Conversion 0d*), tamaño de compra y **LTV** por cohorte.
- **Análisis de Marketing:** Calcular **CAC** por fuente y **ROMI** para identificar canales rentables vs. canales deficitarios.

## ⚖️ Criterios de Éxito (Evaluación)

- **Storytelling:** Explicaciones claras en celdas **Markdown** que interpreten los gráficos.
- **Visualización:** Gráficos que segmenten por **Dispositivo** y **Fuente**.
- **Fundamentación:** Recomendaciones de negocio basadas en métricas, no en suposiciones.
- **Orden:** Código comentado, estructurado y sin redundancias.
