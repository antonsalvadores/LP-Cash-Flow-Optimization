# Optimización Financiera con Programación Lineal (Python & Gurobi)

Este proyecto aplica técnicas de optimización mediante Programación Lineal (LP) para resolver problemas complejos de planificación financiera y gestión de carteras, desarrollados durante el Máster en Banca y Finanzas Cuantitativas.

## Objetivos del Proyecto

El repositorio incluye modelos para:

1.  [cite_start]**Planificación Financiera (Gestión de Tesorería):** Maximizar la riqueza de una empresa al final de un horizonte de 2 años (8 trimestres) [cite: 37-38]. [cite_start]El modelo optimiza las decisiones de endeudamiento (préstamos a 2 años, 6 meses y trimestrales) e inversión de excedentes para cubrir las necesidades de flujo de caja de cada trimestre [cite: 42-43, 45, 47, 49].
2.  [cite_start]**Gestión de Cartera de Bonos (Gestor):** Maximizar el rendimiento de un portafolio de bonos, sujeto a restricciones de calificación crediticia (riesgo) y vencimiento promedio de la cartera [cite: 219, 224-227].
3.  [cite_start]**Inmunización de Pasivos (Fondo de Pensiones):** Minimizar el coste de una cartera de bonos dedicada a financiar las obligaciones de un fondo de pensiones para los próximos 9 años [cite: 258-260].

## Metodología y Herramientas

* [cite_start]**Lenguaje:** Python [cite: 24, 338]
* [cite_start]**Solver de Optimización:** `gurobipy` (Gurobi) [cite: 21, 25, 338]
* [cite_start]**Análisis de Datos:** `pandas` [cite: 25, 338]

## Análisis Clave Realizados

[cite_start]Aparte de la optimización, se realiza un **Análisis de Sensibilidad** (post-optimalidad)[cite: 30, 103]:

* [cite_start]**Precios Sombra (Shadow Prices):** Se interpretan para entender cómo cambiaría la riqueza final (función objetivo) si se relajan las restricciones (ej. si la necesidad de capital en un trimestre disminuye) [cite: 108-109, 112].
* [cite_start]**Costes Reducidos (Reduced Costs):** Se analizan para determinar cuánto tendría que cambiar el precio de un bono (que no está en la cartera óptima) para que sea atractivo incluirlo[cite: 315, 328].
