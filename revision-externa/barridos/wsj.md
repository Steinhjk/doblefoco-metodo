# Barrido editorial: The Wall Street Journal

| | |
|---|---|
| **Medio** | The Wall Street Journal (`wsj`), diario económico estadounidense de Dow Jones & Company, filial de News Corp. `feed: null`: está en el catálogo para resolverse cuando se le cita y no se ingiere. Sin ficha técnica hasta este barrido |
| **Valor vigente** | **+0,30**, firmado en bloque el 2026-10-10 (`reviewedAt: '2026-10-10'`). Su razón en el registro: «Diario económico estadounidense; página editorial explícitamente conservadora, sección informativa más neutra». Es una descripción, sin piezas detrás, y sobre el eje de Estados Unidos, no sobre Colombia. Las dos `biasSources` tratan de la propiedad. Se apoya solo en los niveles 4 y 5 |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus precisiones, incluida la del 2026-10-10 |
| **Ventana** | 2025-10-12 → 2026-10-12 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Alcance pedido** | Solo piezas sobre Colombia en voz de la casa: editoriales del Editorial Board («Review & Outlook») y piezas del medio sin atribuir. Solo lo que el sitio sirve abierto |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-12 |
| **Estado** | **FIRMADO el 2026-10-12: «sin medir» de forma permanente** (`bias: null`). **Decisión del responsable editorial:** el sitio se actualiza de forma 100 % automática y no habrá lectura humana; mientras el robots.txt excluya la lectura por IA, el medio no tiene lugar en el eje. Si autoriza la lectura, se medirá. Aplicado en el registro, la ficha y el texto público el 2026-10-12 (`DECISIONES.md`, «Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Resultado** | **No leído: el robots.txt excluye la lectura por IA.** Ninguna pieza descargada ni clasificada. Rama de la precisión del 2026-10-10: **sin datos → «sin medir»**. No hay lectura previa del medio en el repositorio |

---

## 1. Método

- **Única petición al dominio:** `https://www.wsj.com/robots.txt`, el 2026-10-12, antes de cualquier otra cosa. HTTP 200, 4.298 bytes.
- **User-Agent honesto:** `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. Nunca se usó el de un navegador. Cliente: `curl -sS --ssl-no-revoke`.
- **Lo que dice el robots.txt, literal.** El primer bloque cierra el sitio a todos los agentes:

  ```
  User-agent: *
  Disallow: /
  ```

  Después abre el sitio (`Allow: /`, con exclusiones de rutas) a una lista cerrada de agentes con nombre: buscadores (googlebot, bingbot, duckduckbot, Applebot…), bots publicitarios y de redes sociales, herramientas de SEO y tres agentes de OpenAI (`ChatGPT-User`, `GPTBot`, `OAI-SearchBot`). **No nombra a ClaudeBot, Claude-Web ni anthropic-ai, ni a nuestro DobleFocoBot**: todos caen en `User-agent: *` → `Disallow: /`. La cabecera del archivo añade: «Collection of content and other data on https://www.wsj.com/ through automated means is prohibited unless you have express written permission from Dow Jones & Company, Inc.» [La recogida de contenido y otros datos de https://www.wsj.com/ por medios automatizados está prohibida sin permiso expreso por escrito de Dow Jones & Company, Inc.]
- **Consecuencia:** como manda el método del barrido, **no se descargó nada más del medio**: ni sitemaps (el robots.txt anuncia doce, entre ellos `/sitemap.xml` y `/wsjsitemaps/wsj_google_news.xml`), ni la sección de opinión, ni piezas, ni el feed `feeds.a.dj.com` que el registro anota como congelado desde enero de 2025 (otro host de Dow Jones; no se pidió ni su robots.txt).
- **Ningún buscador, ningún archivo de terceros** (Internet Archive incluido), ningún agregador. No se intentó ninguna vía alternativa al muro ni al robots.

## 2. Cobertura y huecos

| | Piezas en la ventana | Con postura | F | X |
|---|---:|---:|---:|---:|
| Antes del 07-08-2026 | no leídas | — | — | — |
| Desde el 07-08-2026 | no leídas | — | — | — |

**Hueco total.** No se sabe cuántos editoriales sobre Colombia publicó el Editorial Board en la ventana ni qué dicen. Por el muro de pago, aun con el robots.txt abierto, solo se habrían podido leer titulares, entradillas y lo que el sitio sirva sin suscripción.

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

**Rama de la precisión del 2026-10-10: «no llega y no hay piezas suficientes a cada lado para juzgar» → «sin medir» (`bias: null`).** El +0,30 vigente se apoya en una descripción (nivel 4/5) y además describe el eje político de Estados Unidos, no la posición del diario frente a los gobiernos colombianos, que es lo que mide el mapa.

## 6. Contrapesos y tensión declarada

- **La descripción del registro tiene fundamento público** —la página editorial del Journal es conservadora por declaración propia—, pero eso es el eje estadounidense. Sobre Colombia, sin leer, no se puede afirmar que trate de forma distinta al Gobierno Petro y al Gobierno De la Espriella. **Tensión que se declara:** es razonable esperar que su página editorial fuera más crítica con Petro que con De la Espriella; es una expectativa, no una medición, y el protocolo no permite convertirla en número.
- **Vecinos en el mapa:** ningún medio internacional del catálogo tiene barrido. Los de agencia y servicio público están en 0,00 a −0,05 (EFE, France 24, BBC Mundo, DW); Infobae en +0,15. Un +0,30 sin lectura sitúa al WSJ al nivel de NTN24 (+0,30), que tiene 78 piezas contadas detrás.

## 7. Valor propuesto y alternativa

- **Propuesta: «sin medir» (`bias: null`)**, con la tensión hacia la derecha declarada en la ficha como expectativa no medida. Es lo que manda la precisión del 2026-10-10 para un valor de nivel 4/5 cuando no hay piezas, y es lo que el método del barrido prevé cuando el robots.txt excluye la lectura y no hay lectura previa en el repositorio.
- **Alternativa: conservar el +0,30** firmado el 2026-10-10, con el texto público tal como está, que ya dice que el número «no tiene detrás una lectura documentada de sus piezas». Argumento: un barrido que no pudo hacerse no es un barrido que no llega, y la regla «un barrido que no llega no deshace nada» podría leerse como que aquí no hay barrido que mande. Contra: deja un número sin evidencia por encima de medios que la tienen, que es justo lo que la precisión del 2026-10-10 quiso evitar.
- **Qué lo desbloquearía:** permiso escrito de Dow Jones (el robots.txt da `[correo omitido]`) o una lectura humana con suscripción, hecha y documentada por una persona, de los editoriales sobre Colombia de la ventana.

**No se toca el registro, la propiedad ni los textos públicos.** Si se firma «sin medir», cambiarían `bias`, `reviewedAt` y `biasRationale` en `shared/mediaRegistry.js`, el texto de `shared/resumenesPublicos/wsj.js` y la ficha `fichas/wsj.md`.
