# Simulador de clics a WhatsApp — Motorex GA4 · DATA DASH

Calculadora de sensibilidad de tráfico para Motorex (Media Lab), enfocada en la pestaña **«DATA DASH»**: sesiones por canal (Direct / Organic Search), clics a WhatsApp y %CR. Escenarios setiembre–diciembre 2026.

**URL publicada (GitHub Pages):** https://jorgezapanar-ai.github.io/motorex-ga4-adquisicion-dashboard/

## Alcance
- 20 meses observados: ene-25 → ago-26 (hoja «DATA DASH» del Excel fuente).
- Canales: Direct y Organic Search. Conversión proxy = clics a WhatsApp (no transacciones).
- Modelo: sesiones objetivo **por canal** (Direct / Organic Search) → %CR por canal (mediana jun–ago 26: Direct 31.8% / Organic 9.2%) → clics WhatsApp. El mix de sesiones se define por canal y se muestra explícito (ya no es un share fijo).
- Presets de eficiencia Continuidad / +25% / +50% / Manual.
- Export Excel de 8 hojas (Parámetros, Resultados, DATA DASH, Plan, Aporte por canal, Canales referencia, Equivalencias, Embudo (SIM)).
- **Aporte por canal (NUEVO):** el panel «Aporte por canal» mide la contribución de Direct y Organic Search en tres niveles — sesiones, clics WhatsApp y %CR — con barras segmentadas, tabla de contribución (valores, shares y totales) y *clics adicionales atribuibles* al canal o canales intervenidos.
- **Etapa comercial simulada (NUEVO):** la calculadora proyecta ahora también *leads efectivos* y *ventas* ampliando el embudo (Sesiones → Clics WA → Leads → Ventas). Los inputs `%Clic→Lead` y `%Lead→Venta` son **supuestos de escenario editables, etiquetados SIM** — la fuente GA4 de Motorex no registra clic→lead ni lead→venta (termina en «Eventos clave»/clics WA; ingresos GA4 = 0), por lo que esos volúmenes son simulados, no observados.
- Capa de equivalencias entre pestañas del Excel (sección propia en el dashboard): Sesiones DATA DASH = Direct+Organic (Canal mensual) y Clics WA = Eventos clave (Canal/Tendencia), verificados 20/20 con Δ=0; pivote Hoja1 «Suma de Eventos clave» 13,931 (2025) y 9,922 (2026); cobertura 23–39% del tráfico total (la DASH solo incluye Direct + Organic Search).

## Trazabilidad
- Fuente: `Motorex_GA4_Auditoria_Consolidada_Ene2025_Ago2026.xlsx` (copia en `data/raw/`, original intacto).
- Capa derivada: `data/derived/motorex_ga4_data_dash_2026.csv` y manifest de extracción.

## Limitaciones
- Sin inversión ni ingresos en la hoja: sensibilidad de tráfico, no ventas, CAC ni ROAS.
- Junio 2026 marcado REVISAR: %CR Direct > 100% (clics > sesiones), excluido de la tasa de referencia.
- Falta sep-2026 en la fuente.

**Requisito:** revisión humana antes de compartir con clientes.
