# Barrido editorial: The New York Times

| | |
|---|---|
| **Medio** | The New York Times (`nyt`), diario estadounidense de The New York Times Company, controlada por la familia Ochs-Sulzberger. `feed: null`: está en el catálogo para resolverse cuando se le cita y no se ingiere. Sin ficha técnica hasta este barrido |
| **Valor vigente** | **−0,25**, firmado en bloque el 2026-10-10 (`reviewedAt: '2026-10-10'`). Su razón en el registro: «Diario estadounidense de referencia con línea editorial liberal». Es una descripción, sin piezas detrás, y sobre el eje de Estados Unidos, no sobre Colombia. Las dos `biasSources` tratan de la propiedad. Se apoya solo en los niveles 4 y 5 |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus precisiones, incluida la del 2026-10-10 |
| **Ventana** | 2025-10-12 → 2026-10-12 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Alcance pedido** | Solo piezas sobre Colombia en voz de la casa: editoriales del Editorial Board y piezas del medio sin atribuir. Solo lo que el sitio sirve abierto |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-12 |
| **Estado** | **FIRMADO el 2026-10-12: «sin medir» de forma permanente** (`bias: null`). **Decisión del responsable editorial:** el sitio se actualiza de forma 100 % automática y no habrá lectura humana; mientras el robots.txt excluya la lectura por IA, el medio no tiene lugar en el eje. Si autoriza la lectura, se medirá. Aplicado en el registro, la ficha y el texto público el 2026-10-12 (`DECISIONES.md`, «Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Resultado** | **No leído: el robots.txt excluye la lectura por IA.** Ninguna pieza descargada ni clasificada. Rama de la precisión del 2026-10-10: **sin datos → «sin medir»**. No hay lectura previa del medio en el repositorio |

---

## 1. Método

- **Única petición al dominio:** `https://www.nytimes.com/robots.txt`, el 2026-10-12, antes de cualquier otra cosa. HTTP 200, 8.547 bytes.
- **User-Agent honesto:** `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. Nunca se usó el de un navegador. Cliente: `curl -sS --ssl-no-revoke`.
- **Lo que dice el robots.txt, literal.** Bajo «# Disallow Rules», cierra el sitio entero a los agentes de Anthropic, cada uno en su bloque:

  ```
  User-agent: anthropic-ai
  Disallow: /

  User-agent: ClaudeBot
  Disallow: /

  User-agent: Claude-SearchBot
  Disallow: /

  User-agent: Claude-User
  Disallow: /

  User-agent: Claude-Web
  Disallow: /
  ```

  Lo mismo hace con GPTBot, ChatGPT-User, OAI-SearchBot, PerplexityBot, CCBot, Google-Extended y otros. Para `User-agent: *` solo veta rutas técnicas (`/search`, `/svc`, `/ads/`…). La cabecera prohíbe expresamente el uso para IA: «Prohibited uses include but are not limited to: […] (2) the development of any software, machine learning, artificial intelligence (AI), and/or large language models (LLMs)» [Los usos prohibidos incluyen, entre otros: (2) el desarrollo de cualquier software, aprendizaje automático, inteligencia artificial (IA) o grandes modelos de lenguaje (LLM)].
- **Consecuencia:** el método del barrido manda no descargar un medio cuyo robots.txt excluya a ClaudeBot, Claude-Web o anthropic-ai. Aunque nuestro User-Agent no es ninguno de esos, quien lee es un modelo de Anthropic, y la exclusión es del sitio entero. **No se descargó nada más del medio:** ni los sitemaps que anuncia (`/sitemaps/new/news.xml.gz`, `/sitemaps/new/sitemap.xml.gz`, `/sitemaps/new/espanol.xml.gz`…), ni la sección `/section/opinion/editorials`, ni piezas, ni el feed `rss.nytimes.com/services/xml/rss/nyt/Americas.xml` que el registro anota como vivo (otro host de la casa; no se pidió ni su robots.txt).
- **Ningún buscador, ningún archivo de terceros** (Internet Archive incluido), ningún agregador. No se intentó ninguna vía alternativa al muro ni al robots.

## 2. Cobertura y huecos

| | Piezas en la ventana | Con postura | F | X |
|---|---:|---:|---:|---:|
| Antes del 07-08-2026 | no leídas | — | — | — |
| Desde el 07-08-2026 | no leídas | — | — | — |

**Hueco total.** No se sabe cuántos editoriales del Editorial Board trataron de Colombia en la ventana ni qué dicen. Por el muro de pago, aun con el robots.txt abierto, solo se habrían podido leer titulares, entradillas y lo que el sitio sirva sin suscripción. Su edición en español cerró en 2019, así que no hay voz de la casa en español que leer.

## 3. Piezas clasificadas

Ninguna. No hay tabla que recontar.

## 4. Números antes/después

| | D | D leve | I | M | Con postura | F (no cuenta) |
|---|---:|---:|---:|---:|---:|---:|
| Antes del 07-08-2026 | 0 | 0 | 0 | 0 | 0 | 0 |
| Desde el 07-08-2026 | 0 | 0 | 0 | 0 | 0 | 0 |

Ceros por falta de lectura, no por ausencia de postura.

## 5. Veredicto por condición y rama de la precisión

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | No evaluable | Nada leído |
| 2. A los dos lados del cambio | No evaluable | Nada leído |
| 3. ≥10 piezas, ≥3 por lado, ≥3:1 | No | 0 piezas |
| 4. Contrapesos escritos | No evaluable | — |
| 5. Reproducible | Sí, en lo negativo | El robots.txt literal está arriba y cualquiera puede volver a pedirlo |

**Rama de la precisión del 2026-10-10: «no llega y no hay piezas suficientes a cada lado para juzgar» → «sin medir» (`bias: null`).** El −0,25 vigente se apoya en una descripción (nivel 4/5) del eje estadounidense, no en su trato a los gobiernos colombianos.

## 6. Contrapesos y tensión declarada

- **La descripción del registro tiene fundamento público en Estados Unidos** (página editorial liberal, respaldos a candidatos demócratas en ese país), pero un respaldo en una elección estadounidense no es un endoso en Colombia: el protocolo define el endoso por el candidato con nombre de la elección que se mide. **Tensión que se declara:** cabría esperar un trato más severo con un gobierno de mano dura y alineado con la Administración Trump que con el de Petro, pero es una expectativa sacada del eje estadounidense, no de piezas sobre Colombia. Sin leer, no hay dirección que declarar con fundamento; se deja como expectativa no medida.
- **Vecinos en el mapa:** ningún medio internacional del catálogo tiene barrido. CNN en Español está en −0,15; BBC Mundo y DW en −0,05. Un −0,25 sin lectura deja al NYT más lejos del centro que todos los internacionales con lectura o fuentes de conducta.

## 7. Valor propuesto y alternativa

- **Propuesta: «sin medir» (`bias: null`).** Es lo que manda la precisión del 2026-10-10 para un valor de nivel 4/5 cuando no hay piezas, y lo que el método del barrido prevé cuando el robots.txt excluye la lectura y no hay lectura previa en el repositorio.
- **Alternativa: conservar el −0,25** firmado el 2026-10-10, con el texto público tal como está, que ya dice que el número «no tiene detrás una lectura documentada de sus piezas». Argumento: un barrido que no pudo hacerse no es un barrido que no llega. Contra: deja un número sin evidencia más lejos del centro que medios que sí la tienen, que es lo que la precisión del 2026-10-10 quiso evitar.
- **Qué lo desbloquearía:** licencia de The New York Times Company (`nytlicensing.com/contact/`, según su robots.txt) o una lectura humana con suscripción, hecha y documentada por una persona, de los editoriales sobre Colombia de la ventana.

**No se toca el registro, la propiedad ni los textos públicos.** Si se firma «sin medir», cambiarían `bias`, `reviewedAt` y `biasRationale` en `shared/mediaRegistry.js`, el texto de `shared/resumenesPublicos/nyt.js` y la ficha `fichas/nyt.md`.
