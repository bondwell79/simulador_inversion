# 📈 Simulador de Inversión, Dividendos y Análisis Monte Carlo

Un simulador financiero e iterativo desarrollado en una única página web (**Single File Web Application**: HTML5 + CSS3 + JavaScript), diseñado para proyectar la evolución del capital, los rendimientos por dividendos acumulados y realizar análisis estadísticos de riesgo mediante el método de Monte Carlo.

https://bondwell79.github.io/simulador_inversion/

---

## 🚀 Características Principales

* **Cálculo Financiero Preciso**:
  * Determinación automática de acciones compradas: $$\text{Acciones} = \frac{\text{Capital Inicial}}{\text{Precio de Compra}}$$
  * Seguimiento mensual de cotización, capital en acciones, dividendos netos cobrados y rendimiento acumulado.
  * Formulación transparente del **Valor Total Final**:
    $$\text{Valor Total Final} = \text{Capital en Acciones} + \text{Ganancia Acumulada por Dividendos}$$
* **Simulación Individual Iterativa**:
  * Ejecución por bloques de meses ajustables.
  * Botón para avanzar paso a paso (**`+1 Mes`**).
  * Formatos y reglas visuales de resalte (alerta de capital por debajo de la base inicial, ganancia neta en verde, etc.).
* **Análisis Estadístico de Riesgo (Monte Carlo)**:
  * Ejecución masiva de repeticiones de la inversión ($N$ iteraciones parametrizables de $50$ a $5.000$).
  * Cálculo de la **Probabilidad de Pérdida Total** ($\text{Valor Total} < \text{Capital Inicial}$).
  * Cálculo de la **Pérdida por Cotización** ($\text{Capital Acciones} < \text{Capital Inicial}$, aislando el efecto amortiguador de los dividendos).
  * Estadísticas de retorno medio esperado, peor escenario y mejor escenario.
* **Visualización Gráfica Interactiva (Chart.js)**:
  * **Evolución del Capital**: Comparativa temporal de capital en títulos vs. valor total.
  * **Evolución de Dividendos**: Desglose mensual y curva acumulativa.
  * **Abanico de Trayectorias Monte Carlo**: Visualización gráfica del haz de posibilidades en paralelo, destacando en rojo las trayectorias con pérdidas.
  * **Histograma de Frecuencias**: Distribución de probabilidad de los resultados finales organizados por rangos de capital.
* **Sin Dependencias Complejas de Backend**: Corre directamente en cualquier navegador web moderno sin necesidad de servidores ni compilación.

---

## 🛠️ Tecnologías Utilizadas

* **HTML5 / CSS3**: Diseño fluido (*Responsive Layout*) basado en CSS Grid y Flexbox.
* **JavaScript (Vanilla ES6+)**: Lógica matemática, manipulación del DOM y motor Monte Carlo en el cliente.
* **Chart.js (v4.x)**: Renderizado de gráficos interactivos de líneas y histogramas vía CDN.

---
