Competitor offers, silent price creep, and an app nobody opens - 5,000 subscription customers and a real answer to who cancels.

The churn dataset everyone learns on was built for landlines and DSL. This one is built for the subscription era: streaming, fintech, fitness, gaming and cloud plans. 31 columns covering age, service segment, signup channel, tenure, contract type, plan tier, number of services, monthly and total charges, payment method, auto-pay, payment failures, support tickets, average resolution hours, app logins, session length, days since last login, email open rate, satisfaction, NPS, competitor offers received, last year's price increase, discounts offered, referrals made, and a binary churn label. 5,000 rows, zero missing values. The label is genuinely learnable - a plain gradient boosting model reaches roughly 0.75 ROC-AUC - so feature engineering pays off and nothing is handed to you.

Ideas to get you started:

Build a churn classifier and see what ROC-AUC you can beat.
Does a discount actually save a customer who got a competitor offer?
Find the engagement cliff: at what login frequency does churn take off?
Compare month-to-month against annual and two-year contracts.
Does auto-pay retain people, or is that just a proxy for something else?
Estimate the churn cost of last year's price increase.
Tackle the class imbalance: SMOTE vs. class weights vs. threshold tuning.
Note on data: This is a synthetic dataset generated with NumPy (see gen.py) for classification and visualization practice. Providers appear only as generic service-segment categories - no real customer, person, or company record is included, and none of the figures describe any real service's actual churn. Use freely under CC0. If you find it useful, an upvote is hugely appreciated

_ ___ _  _ _ _ _ _ __  _ _ _ _ _ _ _ _ _ _ _  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 

Ofertas de la competencia, un aumento silencioso de precios y una aplicación que nadie abre: 5.000 clientes de suscripción y una respuesta real a quién cancela el servicio.

El conjunto de datos de churn con el que todo el mundo aprende fue diseñado para líneas fijas y conexiones DSL. Este está construido para la era de las suscripciones: streaming, tecnología financiera (fintech), gimnasios, videojuegos y planes en la nube.

Contiene 31 columnas que cubren: edad, segmento de servicio, canal de registro, antigüedad (tenure), tipo de contrato, nivel de plan (plan tier), número de servicios, cargos mensuales y totales, método de pago, pago automático, fallos de pago, tickets de soporte, tiempo promedio de resolución, inicios de sesión en la app, duración de la sesión, días desde el último inicio de sesión, tasa de apertura de correos electrónicos, satisfacción, NPS, ofertas recibidas de la competencia, aumento de precio del último año, descuentos ofrecidos, recomendaciones realizadas (referrals) y una etiqueta binaria de cancelación (churn).

Estructura: 5.000 filas, cero valores faltantes.

Modelado: La variable objetivo es realmente predecible (un modelo básico de gradient boosting alcanza aproximadamente un ROC-AUC de 0,75), por lo que la ingeniería de características da frutos y nada viene servido en bandeja.

Ideas para empezar
Construye un clasificador de churn y descubre qué valor de ROC-AUC puedes superar.

¿Un descuento realmente salva a un cliente que recibió una oferta de la competencia?

Encuentra el "acantilado del compromiso" (engagement cliff): ¿a qué frecuencia de inicio de sesión se dispara el abandono?

Compara los contratos mes a mes frente a los anuales y de dos años.

¿El pago automático retiene a las personas, o es solo una variable indicadora (proxy) de algo más?

Estima el costo de churn provocado por el aumento de precio del año pasado.

Aborda el desequilibrio de clases: SMOTE vs. pesos de clase (class weights) vs. ajuste de umbrales (threshold tuning).

📌 Nota sobre los datos: Este es un conjunto de datos sintético generado con NumPy (ver gen.py) para la práctica de clasificación y visualización. Los proveedores aparecen únicamente como categorías genéricas de segmentos de servicio; no se incluye ningún registro real de clientes, personas o empresas, y ninguna de las cifras describe el churn real de ningún servicio. Úsalo libremente bajo la licencia CC0. Si te resulta útil, ¡un voto positivo en Kaggle (upvote) se agradece enormemente!