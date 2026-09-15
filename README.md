# Simulador de adquisición web — Motorex GA4

Simulador de sensibilidad de tráfico para Motorex (Media Lab), periodo enero-2025 a ago-2026, con variables editables, presets (+25% / +50%), plan set–dic 2026, distribución por canal y export Excel.

**URL publicada (GitHub Pages):** (tras el push)

## Fuente y trazabilidad
- Fuente: auditoría consolidada GA4 Motorex ene-2025 → ago-2026 (archivo en `data/raw/` del workspace).
- Capas derivadas en `data/derived/` (con manifest de extracción).

## Limitaciones
- Indicadores de entrada: sesiones, eventos clave/sesión (proxy conversión), tasa de interacción.
- Sin datos de inversión ni ingresos: el simulador modela sensibilidad de tráfico, no ventas, CAC ni ROAS.
- Feb–mar 2026 marcados REVISAR por anomalía; falta sep-2026 en la fuente.

**Requisito:** revisión humana antes de compartir con clientes.