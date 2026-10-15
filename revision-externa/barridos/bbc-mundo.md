# Barrido editorial: BBC Mundo

| | |
|---|---|
| **Medio** | BBC Mundo (`bbc-mundo`), servicio en español del BBC World Service. Entra al agregador por su RSS (`feeds.bbci.co.uk/mundo/rss.xml`). Sin ficha técnica hasta este barrido (se abre `fichas/bbc-mundo.md`, mínima) |
| **Valor vigente** | **−0,05**, firmado en bloque el 2026-10-10 (`reviewedAt: '2026-10-10'`). Su razón en el registro: «Servicio público con obligación estatutaria de imparcialidad y estándares de verificación altos». Son las reglas del servicio, sin piezas detrás: se apoya solo en el nivel 4. El texto público ya lo dice: «un valor que no sostiene ninguna lectura documentada de sus piezas sobre Colombia» |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus precisiones, incluida la del 2026-10-10 |
| **Ventana** | 2025-10-12 → 2026-10-12 (regla del presente). Solo piezas sobre Colombia |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-12. Es de la misma casa que el autor del valor vigente: su acuerdo no es aval |
| **Estado** | **FIRMADO el 2026-10-12: «sin medir» de forma permanente** (`bias: null`); se descartan las alternativas (conservar −0,05 o llevarlo a 0,00). **Decisión del responsable editorial:** el sitio se actualiza de forma 100 % automática y no habrá lectura humana; mientras el robots.txt excluya la lectura por IA, el medio no tiene lugar en el eje. Si autoriza la lectura, se medirá. Aplicado en el registro, la ficha y el texto público el 2026-10-12 (`DECISIONES.md`, «Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Resultado** | **No leído: el robots.txt excluye la lectura por IA**, por nombre, a ClaudeBot, Claude-Web y anthropic-ai. **0 piezas.** Rama de la precisión del 2026-10-10: **sin datos → «sin medir»**. Propuesta: **«sin medir» (`bias: null`)**; alternativa: conservar −0,05, o llevarlo a 0,00 por la regla 2 |

> No hay piezas que recontar. Lo reproducible aquí es la comprobación del
> robots.txt: cualquiera puede descargarlo y llegar a las mismas líneas.

---

## 1. Método

- **robots.txt** de `www.bbc.com`, descargado el 2026-10-12 con el User-Agent
  de abajo (HTTP 200, `text/plain`). Fue **la única petición** al dominio.
- **Las líneas que deciden**, literales:

  ```
  User-agent: Claude-Web
  Disallow: /

  User-agent: ClaudeBot
  Disallow: /

  User-agent: anthropic-ai
  Disallow: /
  ```

  El bloque `User-agent: *` sí permite `/mundo/` (solo veta búsquedas y unas
  pocas rutas) y anuncia los sitemaps de BBC Mundo
  (`/mundo/sitemap.xml`, `/sitemaps/https-index-com-mundo-archive.xml`,
  `/sitemaps/https-index-com-mundo-news.xml`). **No se usaron:** quien lee es
  un agente de Anthropic, y el robots lo excluye por nombre de todo el sitio.
  Cambiar de nombre de agente para caer en el bloque general sería eludir la
  exclusión. La cabecera del archivo lo dice además en prosa, literal:

  ```
  # - No scraping, crawling, or systematic extraction of content
  # - No retrieval-augmented generation (RAG), AI-powered search, agentic AI or grounding using BBC content
  ```

- **Decisión:** no se descargó nada más. Ni sitemaps, ni secciones, ni piezas,
  ni el RSS de `feeds.bbci.co.uk` para este barrido.
- **User-Agent honesto:** `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`.
  Cliente `curl -sS --ssl-no-revoke`. Nunca el de un navegador.
- **Sin rodeos.** Ni buscadores, ni Internet Archive, ni Google News, ni
  reediciones de la BBC en otros medios.
- **Lectura previa en el repositorio:** **no hay.** Ninguna resolución, envío ni
  barrido anterior lee piezas de BBC Mundo sobre Colombia. El texto público
  (`shared/resumenesPublicos/bbc-mundo.js`) ya declara esa ausencia.

**Nota sobre la ingesta, fuera de este barrido.** Que el robots excluya a
Claude bloquea la **revisión**, no la ingesta del feed, que corre con su propio
agente y por otro dominio (`feeds.bbci.co.uk`). Es el mismo criterio que se
escribió para Diario del Sur (`DECISIONES.md`). La prosa de la cabecera
(«No retrieval-augmented generation… agentic AI», «No using BBC content to
create summaries») sí merece que el responsable editorial la mire a la luz de
cómo el agregador muestra las piezas; no es asunto de este barrido y no se
toca.

---

## 2. Cobertura y huecos

| | Piezas en la ventana | Con postura (D, I, M) | Fiscalización (F) | X |
|---|---:|---:|---:|---:|
| Antes del 07-08-2026 | — | 0 | 0 | — |
| Desde el 07-08-2026 | — | 0 | 0 | — |
| **Total** | **no leído** | **0** | **0** | — |

**Hueco total:** no se leyó ninguna pieza.

**Lo que habría que buscar en una lectura con permiso.** BBC Mundo, a
diferencia de una agencia, sí tiene voz propia: análisis firmados por la casa,
explicadores y titulares interpretativos. Ahí es donde se podrían ver
calificativos asimétricos (cómo nombra a cada candidato y a cada gobierno),
que es lo que movió a El País (España). Sin lectura no se sabe.

---

## 3. Piezas clasificadas

Ninguna. No se descargó ninguna pieza.

---

## 4. Números antes y después del cambio

| | D | I | M | F | Con postura que cuenta |
|---|---:|---:|---:|---:|---:|
| Antes del 07-08-2026 | 0 | 0 | 0 | 0 | 0 |
| Desde el 07-08-2026 | 0 | 0 | 0 | 0 | 0 |

Sin lectura, los ceros no son conducta medida: son ausencia de datos.

---

## 5. Rama de la precisión del 2026-10-10

- **¿El valor vigente se apoya solo en los niveles 4 y 5?** Sí. El −0,05 sale
  de la obligación estatutaria de imparcialidad (nivel 4). El nivel 1 —servicio
  público británico; un tercio del presupuesto del World Service viene del
  ministerio de Exteriores del Reino Unido— es pertinente para la política
  exterior, pero no da dirección en el eje colombiano. Además, el −0,05 no
  tiene escrita la razón del signo: nada en el registro explica por qué
  −0,05 y no 0,00.
- **Las cinco condiciones:** no se cumple ninguna, porque no hay piezas.
- **Rama:** «si no llega y no hay piezas suficientes a cada lado para juzgar →
  «sin medir» (`bias: null`)», en su caso extremo: cero piezas.

---

## 6. Valor propuesto y alternativa

**Propuesta: «sin medir» (`bias: null`).** Es lo que manda la instrucción
cuando el robots.txt excluye la lectura por IA y no hay lectura previa, y lo
que da la última rama de la precisión. Encaja con lo que ya dice su texto
público.

**Alternativas:**
1. **Conservar −0,05**, declarado como valor por defecto. Argumento: un barrido
   que no se pudo hacer no es un barrido que «no llega».
2. **Llevarlo a 0,00 por la regla 2** (ante la duda, la mixta), si se prefiere
   conservar un número. El −0,05 es un matiz sin evidencia escrita; si el
   número se mantiene sin lectura, lo honesto es el centro.

BBC Mundo se ingiere: su valor pesa en la mezcla de las historias en que
aparece, así que la elección entre número y `null` sí se nota en la portada.

**Frente a los vecinos del mapa.** DW −0,05, France 24 0,00, Euronews +0,05,
EFE 0,00 y Reuters 0,00: franja central, sin barrido leído. El País (España),
−0,25, es el único movido por piezas. DW es su vecino natural —servicio
exterior público europeo, mismo −0,05, misma razón de nivel 4—: **lo que se
decida para BBC Mundo debería decidirse también para DW**, aunque DW no está
en este grupo.

**Qué haría falta para medir:** permiso de la BBC, o una lectura humana sin
automatizar, declarada como tal.

---

## 7. Fuentes

- [robots.txt de la BBC](https://www.bbc.com/robots.txt), consultado el 2026-10-12.
- `shared/mediaRegistry.js`, `shared/mediaOwnership.js` y `shared/resumenesPublicos/bbc-mundo.js`, entrada `bbc-mundo`.
- `PROTOCOLO_JUICIO_EDITORIAL.md`, «Evidencia editorial histórica» y precisión del 2026-10-10.
- `DECISIONES.md`, criterio sobre Diario del Sur («Su robots.txt excluye a Claude. Eso bloquea la revisión, no la ingesta»).
