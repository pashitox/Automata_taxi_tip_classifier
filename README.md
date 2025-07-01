# 🚕 Predicción de Propinas Generosas en Taxis de Nueva York

**Modelo predictivo para anticipar si un pasajero dejará una propina ≥20%, usando datos de la Comisión de Taxis y Limusinas (TLC NYC).**


![image](https://github.com/user-attachments/assets/9c20f2d5-3b05-4188-a2a7-bae1770fb8c5)




## 📌 Objetivo del Proyecto

Implementar modelos de Machine Learning capaces de predecir con alta precisión la propensión de un pasajero a dejar una propina generosa *antes* del inicio del viaje, mejorando así estrategias de servicio y bonificación.

## 🗃️ Datos Utilizados

- Dataset TLC NYC
- +22,000 registros históricos de viajes
- Variables: tarifa total, distancia, tipo de pago, peajes, fecha y hora
- Variable objetivo: `generoso` → 1 si la propina fue ≥20%

## 🤖 Modelos Construidos

| Modelo             | Precisión | Recall (Generoso) | AUC   |
|--------------------|-----------|-------------------|-------|
| Random Forest      | 78%       | 86%               | 0.83  |
| XGBoost            | 81%       | 100%              | 0.84  |
| ✅ Mejor modelo     | XGBoost con recall perfecto y alto poder discriminativo |

📌 *Eliminando la variable `video_view_count` (si existiera), el modelo mantiene AUC 1.00 → sin sobreajuste evidente*

## 🔍 Principales Hallazgos

- **Tipo de pago:** predictor más determinante
- **Tarifas altas y viajes largos:** correlación con propinas generosas
- **XGBoost:** excelente en detectar todos los casos positivos, aunque con más falsos positivos

## 🧩 Estructura del Repositorio

📁 data/           → Datos anonimizados de viajes
📁 notebooks/      → Entrenamiento y evaluación de modelos 
📁 docs/           → Informe final (PDF) 
📄 README.md       → Este documento



## 🚀 Próximos pasos

- Integrar el modelo en la app móvil de TLC NYC
- Agregar variables externas (clima, tráfico)
- Automatizar recomendaciones al conductor

## 👤 Autor

Desarrollado por **Juan**, analista de datos orientado a proyectos reales con impacto en la experiencia del cliente.

## 📄 Licencia

Este proyecto está bajo la licencia [MIT](LICENSE).

