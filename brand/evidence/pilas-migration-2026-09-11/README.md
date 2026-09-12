# Pilas — evidencia de migración visual del prototipo 2026-09-11

## Fuente normativa
- Assets, favicon, CSS y tokens provienen de Pilas Brand Package v2.0.
- El paquete normativo no fue reinterpretado ni modificado.
- Messaging activo: `Tu dinero conectado`.
- Descriptor activo: `Conectamos tu información financiera para transformarla en decisiones más inteligentes`.

## Regresión funcional
- El JavaScript inline candidato, normalizado únicamente por cambios de identidad/metadata, es exactamente equivalente al baseline (`FUNCTIONAL_JS_EQUIVALENT_AFTER_BRAND_NORMALIZATION=true`).
- No se modificaron rutas, filtros, navegación, scroll restore, moneda, presupuestos ni lógica funcional como parte del rebranding.
- `node --check` del JavaScript extraído: PASS.
- Assets Pilas referenciados existen y sus copias normativas fueron verificadas por hash.

## Evidencia visual
- Home: 1348×926, 390×844, 412×915, 844×390, 320×568, 360×800 y 768×1024.
- Presupuestos: 1348×926, 390×844 y 412×915.
- La disposición horizontal observada en Home móvil fue comparada con la baseline y ya existía; no es regresión de identidad.

## Gate
La evidencia nueva reemplaza la baseline temporal de migración. Los scans finales se ejecutan después de retirarla del HEAD.

## Resultado final del gate
- JavaScript funcional equivalente al baseline tras normalizar exclusivamente identidad/metadata: PASS.
- JavaScript extraído: `node --check` PASS.
- Filenames con identidad/namespace anterior: 0.
- Contenido con identidad/namespace anterior: 0.
- Colores de la paleta anterior: 0.
- Rutas locales de assets rotas: 0.
- Logo, favicon, CSS y tokens críticos: MATCH por SHA-256 contra el ZIP normativo.

## Excepción deliberada de messaging v2.0
Los archivos normativos copiados desde v2.0 permanecen byte-exact. Si contienen los mensajes originales del paquete, estos no son usados como copy activo del prototipo; el override aprobado rige hasta la homologación v2.1.
