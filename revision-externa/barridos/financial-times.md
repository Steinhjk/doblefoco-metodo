# Barrido editorial: Financial Times

| | |
|---|---|
| **Medio** | Financial Times (`financial-times`), diario económico británico del grupo japonés Nikkei Inc. desde 2015. `feed: null`: está en el catálogo para resolverse cuando se le cita y no se ingiere. Sin ficha técnica hasta este barrido |
| **Valor vigente** | **+0,15**, firmado en bloque el 2026-10-10 (`reviewedAt: '2026-10-10'`). Su razón en el registro: «Diario económico británico; encuadre desde mercados y liberalismo económico». Es una descripción, sin piezas detrás. Las dos `biasSources` tratan de la compra por Nikkei. Se apoya solo en los niveles 4 y 5 |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus precisiones, incluida la del 2026-10-10 |
| **Ventana** | 2025-10-12 → 2026-10-12 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Alcance pedido** | Solo piezas sobre Colombia en voz de la casa: los editoriales sin firma («The FT View», del Editorial Board) y piezas del medio sin atribuir. Solo lo que el sitio sirve abierto |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-12 |
| **Estado** | **FIRMADO el 2026-10-12: «sin medir» de forma permanente** (`bias: null`). **Decisión del responsable editorial:** el sitio se actualiza de forma 100 % automática y no habrá lectura humana; mientras el robots.txt excluya la lectura por IA, el medio no tiene lugar en el eje. Si autoriza la lectura, se medirá. Aplicado en el registro, la ficha y el texto público el 2026-10-12 (`DECISIONES.md`, «Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Resultado** | **No leído: el robots.txt excluye la lectura por IA.** Ninguna pieza descargada ni clasificada. Rama de la precisión del 2026-10-10: **sin datos → «sin medir»**. No hay lectura previa del medio en el repositorio |

---

## 1. Método

- **Única petición al dominio:** `https://www.ft.com/robots.txt`, el 2026-10-12, antes de cualquier otra cosa. HTTP 200, 1.556 bytes.
- **User-Agent honesto:** `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. Nunca se usó el de un navegador. Cliente: `curl -sS --ssl-no-revoke`.
- **Lo que dice el robots.txt, literal.** Para `User-agent: *` solo veta rutas de cuenta y búsqueda (`/login`, `/myft`, `/search`…) con `Crawl-Delay: 1`, pero cierra el sitio entero a los agentes de Anthropic:

  ```
  User-agent: anthropic-ai
  Disallow: /

  User-agent: Claude-Web
  Disallow: /

  User-agent: ClaudeBot
  Disallow: /
  ```

  Y la cabecera: «We expressly prohibit any use of our content or data for any machine learning or artificial intelligence purposes, including the training or development of AI technologies or machine learning language models.» [Prohibimos expresamente cualquier uso de nuestro contenido o datos con fines de aprendizaje automático o inteligencia artificial, incluido el entrenamiento o desarrollo de tecnologías de IA o de modelos de lenguaje.]
- **Consecuencia:** el método del barrido manda no descargar un medio cuyo robots.txt excluya a ClaudeBot, Claude-Web o anthropic-ai. Aunque nuestro User-Agent no es ninguno de esos y cae en `User-agent: *`, quien lee es un modelo de Anthropic. **No se descargó nada más del medio:** ni `/sitemaps/index.xml`, ni la sección de editoriales, ni piezas, ni los feeds `ft.com/rss/home` y `ft.com/world?format=rss` que el registro anota como vivos.
- **Ningún buscador, ningún archivo de terceros** (Internet Archive incluido), ningún agregador. No se intentó ninguna vía alternativa al muro ni al robots.

## 2. Cobertura y huecos

| | Piezas en la ventana | Con postura | F | X |
|---|---:|---:|---:|---:|
| Antes del 07-08-2026 | no leídas | — | — | — |
| Desde el 07-08-2026 | no leídas | — | — | — |

**Hueco total.** No se sabe cuántos editoriales del FT trataron de Colombia en la ventana ni qué dicen. Por el muro de pago, aun con el robots.txt abierto, solo se habrían podido leer titulares, entradillas y lo que el sitio sirva sin suscripción.

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

**Rama de la precisión del 2026-10-10: «no llega y no hay piezas suficientes a cada lado para juzgar» → «sin medir» (`bias: null`).**

## 6. Contrapesos y tensión declarada

- **El +0,15 ya está en la banda mixta** y su texto público lo presenta como «orientación mixta» que no sostiene «ninguna lectura documentada de sus piezas sobre Colombia». Pasar a «sin medir» cambia poco lo que el lector ve, pero cambia lo que afirma: hoy el número dice una posición, y no hay piezas que la respalden.
- **Tensión:** ninguna que pueda declararse con fundamento. «Liberalismo económico» describe un encuadre de mercado, no un trato distinto a uno u otro gobierno colombiano.
- **Vecinos en el mapa:** Infobae (+0,15), La Vanguardia (+0,10), EFE y France 24 (0,00). Ninguno de los internacionales tiene barrido.

## 7. Valor propuesto y alternativa

- **Propuesta: «sin medir» (`bias: null`).** Es lo que manda la precisión del 2026-10-10 para un valor de nivel 4/5 cuando no hay piezas, y lo que el método del barrido prevé cuando el robots.txt excluye la lectura y no hay lectura previa en el repositorio.
- **Alternativa: conservar el +0,15** firmado el 2026-10-10. Es el caso más defendible de los tres internacionales en inglés, porque ya está en la banda mixta y su texto público dice que no hay lectura. Argumento: un barrido que no pudo hacerse no es un barrido que no llega. Contra: el +0,15 no es 0,00, y un número distinto de cero afirma una dirección que nadie ha leído.
- **Qué lo desbloquearía:** licencia del FT (`[correo omitido]`, según su robots.txt) o una lectura humana con suscripción, hecha y documentada por una persona, de los editoriales sobre Colombia de la ventana.

**No se toca el registro, la propiedad ni los textos públicos.** Si se firma «sin medir», cambiarían `bias`, `reviewedAt` y `biasRationale` en `shared/mediaRegistry.js`, el texto de `shared/resumenesPublicos/financial-times.js` y la ficha `fichas/financial-times.md`.
