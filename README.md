Planificación Patrimonial Estratégica & Family Office (Modelo HNWI)

Panel de control interactivo y modelo analítico diseñado para la estructuración patrimonial de un cliente HNWI (High Net Worth Individual) tras un evento de liquidez de 2.500.000 €.

🔗 Ver el Cuadro de Mando Interactivo: https://aguarinosm.github.io/family-office-model/

Resumen del Business Case

El proyecto simula el mandato de un Family Office o mesa de Banca Privada para preservar el capital de un empresario (62 años, residente fiscal en la Comunidad Valenciana) y generar una renta vitalicia pasiva de 90.000 € netos anuales actualizados por inflación.

Arquitectura Analítica y Financiera

Asset Allocation & Liquidez (Mitigación SoRR):

Implementación de una cartera 40/60 (Renta Variable / Renta Fija) utilizando clases institucionales de Vanguard.

Aislamiento de un Liquidity Buffer (270.000 € en duración ultra-corta) para cubrir 3 años de reembolsos y neutralizar el Riesgo de Secuencia de Retornos (Sequence of Returns Risk).

Motor Estocástico (Simulación Monte Carlo):

El dashboard no utiliza proyecciones deterministas lineales. Integra un motor estocástico programado en JavaScript (Transformada de Box-Muller) que ejecuta 1.000 iteraciones aleatorias de mercado.

Extrae los percentiles estadísticos P10, P50 y P90 a 20 años vista.

Optimización Fiscal y Regulatoria:

Aplicación de la regla FIFO (First In, First Out) para el cálculo del IRPF sobre plusvalías afloradas en los reembolsos anuales.

Impacto del Impuesto sobre el Patrimonio (escala autonómica de la Comunidad Valenciana).

Stack Tecnológico

Front-End: HTML5, CSS3 (Tailwind CSS).

Lógica Financiera y Motor Estocástico: JavaScript (ES6+).

Visualización de Datos: Chart.js (renderizado dinámico de proyecciones probabilísticas).

Autor

Abel Guarinos Marín
Analista Financiero | Máster FEBF | Candidato EFA
