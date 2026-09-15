# Simulador de clics a WhatsApp — Motorex GA4 · DATA DASH

Calculadora de sensibilidad de tráfico para Motorex (Media Lab), enfocada en la pestaña **«DATA DASH»**: sesiones por canal (Direct / Organic Search), clics a WhatsApp y %CR. Escenarios setiembre–diciembre 2026.

**URL publicada (GitHub Pages):** https://jorgezapanar-ai.github.io/motorex-ga4-adquisicion-dashboard/

## Alcance
- 20 meses observados: ene-25 → ago-26 (hoja «DATA DASH» del Excel fuente).
- Canales: Direct y Organic Search. Conversión proxy = clics a WhatsApp (no transacciones).
- Modelo: sesiones objetivo → mix de referencia (jun–ago 26: Direct 35.4% / Organic 64.6%) → %CR por canal (mediana: Direct 31.8% / Organic 9.2%) → clics WhatsApp.
- Presets de eficiencia Continuidad / +25% / +50% / Manual.
- Export Excel de 5 hojas (Parámetros, Resultados, DATA DASH, Plan, Canales referencia).

## Trazabilidad
- Fuente: `Motorex_GA4_Auditoria_Consolidada_Ene2025_Ago2026.xlsx` (copia en `data/raw/`, original intacto).
- Capa derivada: `data/derived/motorex_ga4_data_dash_2026.csv` y manifest de extracción.

## Limitaciones
- Sin inversión ni ingresos en la hoja: sensibilidad de tráfico, no ventas, CAC ni ROAS.
- Junio 2026 marcado REVISAR: %CR Direct > 100% (clics > sesiones), excluido de la tasa de referencia.
- Falta sep-2026 en la fuente.

**Requisito:** revisión humana antes de compartir con clientes.
