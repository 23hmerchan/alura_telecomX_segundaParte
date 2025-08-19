# alura_telecomX_segundaParte
# 📑 Predicción de Cancelación de Clientes (Churn) – TelecomX LATAM

Este proyecto tiene como objetivo **predecir la cancelación de clientes (churn)** en la empresa **TelecomX LATAM**, utilizando análisis exploratorio de datos (EDA) y modelos de Machine Learning.

---

## 📊 Resumen Ejecutivo

- Se aplicaron modelos predictivos para identificar clientes con mayor probabilidad de cancelar.  
- El modelo **Random Forest** obtuvo el mejor desempeño con **ROC AUC ≈ 0.84**.  
- Se identificaron factores clave que influyen en la cancelación:  
  - Tipo de contrato (mes a mes vs anual).  
  - Método de pago (cheque electrónico más riesgoso).  
  - Tiempo de permanencia (clientes <12 meses cancelan más).  
  - Facturación mensual elevada.  
  - Servicio de internet por fibra óptica presenta mayor churn que DSL.

---

## 🤖 Modelos Evaluados

| Modelo               | ROC AUC | Recall (Churn=Sí) | Comentario |
|----------------------|---------|--------------------|------------|
| **Random Forest**    | 0.84    | 72%               | Mejor balance entre precisión y recall |
| Regresión Logística  | 0.78    | 65%               | Muy útil para interpretar coeficientes |
| SVM (lineal)         | 0.80    | 68%               | Buen rendimiento, menos interpretable |
| KNN                  | 0.76    | 60%               | Sensible a la escala y al ruido |

---

## 🔑 Variables más Relevantes

1. **Contract: Month-to-Month** → mayor riesgo de cancelación.  
2. **Payment Method: Electronic Check** → asociado a churn.  
3. **Tenure (Antigüedad del cliente)** → menor tiempo = mayor riesgo.  
4. **Monthly Charges** → facturas más altas = mayor churn.  
5. **Internet Service: Fiber Optic** → clientes de fibra cancelan más que DSL.  

---

## 🚀 Recomendaciones de Negocio

- Implementar campañas de retención para clientes **con contrato mes a mes** y **pago electrónico**.  
- Incentivar la migración hacia **contratos de 1 o 2 años** con beneficios de lealtad.  
- Dar seguimiento a **clientes nuevos** en sus primeros 12 meses.  
- Revisar y optimizar planes con **facturación mensual alta**.  
- Proactivamente contactar clientes en riesgo antes de la cancelación.  


