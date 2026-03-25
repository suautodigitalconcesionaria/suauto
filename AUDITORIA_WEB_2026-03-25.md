# Auditoría web integral — suauto

Fecha: 2026-03-25

## Diagnóstico general

El sitio transmite una identidad visual sólida y diferenciada, con una propuesta estética premium y buena riqueza de contenido comercial (stock, logística nacional, importación, FAQs y contacto). Sin embargo, desde una perspectiva de conversión, accesibilidad y performance, existen puntos críticos que están afectando potencialmente la capacidad de captar leads y cerrar acciones clave.

## Hallazgos resumidos

- **Arquitectura y UX:** contenido abundante pero falta de jerarquía orientada a conversión en el primer scroll.
- **UI:** alto nivel visual, pero con potenciales fricciones de legibilidad/contraste y exceso de animaciones.
- **Performance:** CSS y JS inline masivos en una sola página, recursos pesados y posibles costos de renderizado en móviles.
- **SEO técnico:** faltan metadatos clave (description, OG/Twitter, canonical) y estructura semántica mejorable (sin `<main>` visible).
- **Conversión:** CTA principal poco persistente y escasez de señales de confianza verificables (reseñas, testimonios, garantías concretas, etc.).

## Recomendaciones priorizadas

### Alto impacto

1. Reestructurar hero y primer viewport con foco en conversión (valor + prueba + CTA principal + CTA secundario).
2. Mejorar SEO técnico base (meta description, Open Graph, canonical, títulos por página, datos estructurados).
3. Reducir peso inicial: extraer CSS/JS a archivos, diferir scripts no críticos, optimizar imágenes/video hero.
4. Fortalecer accesibilidad (navegación por teclado, estados de foco visibles, contraste mínimo WCAG, semántica landmarks).

### Impacto medio

1. Simplificar navegación y microcopys para orientar más rápido a “Comprar”, “Financiar”, “Vender tu auto”.
2. Incorporar pruebas de confianza: testimonios reales, calificación promedio, casos de entrega con datos concretos.
3. Mejorar buscador con feedback más claro, filtros persistentes y resultados inmediatos.

### Impacto bajo

1. Ajustes finos de consistencia tipográfica/espaciado entre bloques.
2. Estandarización de componentes reutilizables (botones, cards, formularios).
3. Optimización de animaciones para respetar `prefers-reduced-motion`.

## Quick wins (1–2 semanas)

- Agregar metadatos SEO esenciales y social cards.
- Incluir `<main>` y mejorar landmarks semánticos.
- Añadir `loading="lazy"` a imágenes no críticas que aún no lo tengan.
- Revisar contraste de textos secundarios y estados `:focus-visible`.
- Poner un CTA fijo en mobile (WhatsApp / asesor comercial).

## Cambios estratégicos (4–12 semanas)

- Diseño de funnel completo por intención: “comprar usado”, “comprar 0km”, “financiación”, “consignación”.
- Sistema de diseño (tokens + componentes + reglas responsive + accesibilidad).
- Estrategia de contenidos SEO local y transaccional (landing por ciudad/provincia y por tipo de vehículo).
- Medición avanzada: eventos de clic en CTA, scroll depth, abandono en formularios, atribución por canal.

## ¿Con qué seguiría ahora? (plan de ejecución)

### Fase 1 — Próximos 7 días (impacto inmediato)

1. **Cerrar brechas de confianza en home**
   - Incorporar bloque de reseñas verificables (Google/Meta) y casos reales de entrega.
   - Mostrar indicadores duros: tiempo promedio de entrega, % aprobación financiación, NPS o calificación.

2. **Optimizar conversión del primer pantallazo**
   - Hero con 2 CTAs visibles: `Ver stock` + `Hablar con asesor`.
   - Mensaje de valor directo orientado a problema/resultado (no solo branding).

3. **Medición mínima obligatoria**
   - Instrumentar eventos de click en CTAs principales.
   - Medir profundidad de scroll y envío/click a WhatsApp.

### Fase 2 — Próximas 2 a 4 semanas (estabilización)

1. **Performance técnica**
   - Separar CSS/JS inline en archivos cacheables.
   - Definir presupuesto de performance (LCP, CLS, INP) y alertas.

2. **SEO transaccional**
   - Crear páginas orientadas a intención: usados, financiación, consignación.
   - Contenido local por ciudad/provincia con schema apropiado.

3. **Accesibilidad operacional**
   - Auditoría WCAG AA de contraste/foco/navegación por teclado.
   - Checklist de accesibilidad en cada release.

### Fase 3 — Próximos 1 a 3 meses (escalamiento)

1. **Sistema de diseño**
   - Tokens, componentes base y reglas responsive consistentes.
   - Reducción de deuda visual y mayor velocidad de iteración.

2. **Funnel completo y CRO**
   - Definir embudos por intención (comprar, financiar, vender).
   - A/B testing continuo de titulares, CTAs y orden de bloques.

3. **Roadmap de datos**
   - Dashboard semanal con conversiones por canal, tasa de contacto y costo por lead.
   - Decisiones priorizadas por impacto en ingresos.
