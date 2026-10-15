# Barrido editorial: CNN en Español

| | |
|---|---|
| **Medio** | CNN en Español (`cnn-es`), cadena internacional de Warner Bros. Discovery, cnnespanol.cnn.com. Ficha técnica: `fichas/cnn-es.md` |
| **Valor vigente** | **−0,15**, firmado en bloque el 2026-10-10 (`reviewedAt: '2026-10-10'`). Su razón en el registro: «Cadena internacional; encuadre editorial estadounidense de centro-izquierda». Es una frase sobre la posición de CNN en el sistema político de Estados Unidos, sin piezas detrás: se apoya solo en los niveles 4 y 5. Las fuentes del registro tratan de la propiedad (la venta a Paramount Skydance, la salida de Cynthia Hudson), no de la línea |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con la regla del polo fijo y la precisión del 2026-10-10 |
| **Ventana** | 2025-10-12 → 2026-10-12 (regla del presente). Para un medio internacional, solo sus piezas sobre Colombia |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-12. Es de la misma casa que quien escribió otras fichas y barridos del catálogo: su acuerdo con ellos no es aval |
| **Estado** | **FIRMADO el 2026-10-12: «sin medir» de forma permanente** (`bias: null`). **Decisión del responsable editorial:** el sitio se actualiza de forma 100 % automática y no habrá lectura humana; mientras el robots.txt excluya la lectura por IA, el medio no tiene lugar en el eje. Si autoriza la lectura, se medirá. Aplicado en el registro, la ficha y el texto público el 2026-10-12 (`DECISIONES.md`, «Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Resultado** | **No leído: el robots.txt excluye la lectura por IA.** El sitio veta `Disallow: /` a `ClaudeBot`, `Claude-Web` y `anthropic-ai`, entre otros 50 agentes. No se descargó ninguna pieza. No hay en el repositorio ninguna lectura previa de piezas de CNN en Español sobre Colombia. **Propuesta: «sin medir»** (`bias: null`) |

---

## 1. Método

- **robots.txt** de `cnnespanol.cnn.com`, descargado el 2026-10-12 con el User-Agent de abajo (HTTP 200). Es lo único que se pidió al dominio. El bloque que importa, literal:

  ```
  User-agent: AI2Bot
  User-agent: Ai2Bot-Dolma
  User-agent: Amazonbot
  User-agent: anthropic-ai
  …
  User-agent: ClaudeBot
  User-agent: Claude-Web
  …
  User-agent: YouBot
  Disallow: /
  ```

  (La lista completa nombra 56 agentes, entre ellos GPTBot, CCBot, Google-Extended, PerplexityBot y Meta-ExternalAgent; los puntos suspensivos solo acortan la cita.) Después vienen un bloque `User-agent: *` que veta `/api/`, `/search`, `/ads/` y otras rutas técnicas, y uno de Yoast con `User-agent: *` / `Disallow:` vacío.
- **Por qué no se leyó.** Este barrido lo hace un modelo de Anthropic. El sitio excluye por nombre a los tres agentes de Anthropic de todas sus rutas, y la regla del encargo es no descargar en ese caso. Nuestro User-Agent (`DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`) no está en la lista, pero usarlo para que un modelo de Anthropic lea lo que el sitio veta a los agentes de Anthropic sería saltarse la voluntad declarada del medio. No se hizo.
- **No se usó ninguna otra vía:** ni buscadores, ni Internet Archive, ni agregadores, ni copias de sus piezas en otros sitios.

## 2. Cobertura y huecos

| | Piezas en la ventana | Con postura | Fiscalización | X |
|---|---:|---:|---:|---:|
| Antes del 07-08-2026 | no leídas | — | — | — |
| Desde el 07-08-2026 | no leídas | — | — | — |

- **No hay universo.** No se sabe cuántas piezas sobre Colombia publicó CNN en Español en la ventana.
- **Lo que hay en el repositorio no es lectura de piezas.** La revisión de Kimi K3 (`revision-externa/respuestas/kimi-k3-cnn-es.md`, 2026-08-18) dice que «un barrido» de su cobertura colombiana «no produjo piezas destacadas citables». No lista ninguna pieza, ninguna URL ni ninguna clase. No sirve como evidencia de nivel 5.
- **El motor del producto sí lee su sitemap de noticias** desde el 2026-10-10 (`via: 'sitemap'`, `shared/mediaRegistry.js`), con el User-Agent del proyecto, que el robots.txt no nombra. Eso es la ingesta de titulares, no una lectura editorial, y no la hace un agente de Anthropic. Se declara para que nadie lo confunda con este barrido: **este barrido no usó el corpus ingerido.** Si se quisiera medir la conducta con ese corpus, sería una decisión de la dirección editorial y otro procedimiento.

## 3. Piezas clasificadas

Ninguna.

## 4. Números

| | D | I | M | Con postura | F (no cuenta) |
|---|---:|---:|---:|---:|---:|
| Antes | — | — | — | — | — |
| Después | — | — | — | — | — |

**Antes de este barrido:** −0,15 sin piezas. **Después:** −0,15 sin piezas. El barrido no añade ningún dato de conducta.

## 5. Veredicto por condición

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | No se puede saber | No se leyó |
| 2. A los dos lados del cambio | No se puede saber | No se leyó |
| 3. Mínimos (10 / 3 por lado / 3:1) | No | 0 piezas |
| 4. Contrapesos escritos | — | No hay dirección que contrapesar |
| 5. Reproducible | Sí, en su resultado | Cualquiera puede bajar el robots.txt y ver el veto |

**Rama de la precisión del 2026-10-10:** el −0,15 se apoya solo en los niveles 4 y 5 (una frase sobre el eje estadounidense, que su propia ficha discute), así que el barrido manda aunque no llegue. **No llega y no hay piezas a ningún lado para juzgar → «sin medir»** (`bias: null`).

## 6. Lo que se declara y no cuenta

- La posición de CNN en el eje político de **Estados Unidos**. La ficha ya señala que trasladarla al eje colombiano es una operación que nadie ha justificado (pregunta transversal 4 del ciclo 1).
- La operación de compra por Paramount Skydance (juicio el 02-03-2027, cierre congelado hasta junio de 2027) y la vacante en la dirección. Son nivel 1 y vigilancia; no dicen nada de la línea sobre Colombia.

## 7. Contrapesos y su peso

No aplica: no hay dirección medida.

## 8. Valor propuesto

- **Propuesta: «sin medir»** (`bias: null`). Es la rama del encargo para un medio no leído por robots sin lectura previa en el repositorio, y coincide con la rama «sin datos» de la precisión del 2026-10-10.
- **Frente a los vecinos del mapa:** el −0,15 lo ponía en la franja mixta junto a otros internacionales cuyo número también salió de una frase (NYT −0,25, Euronews +0,05 antes de su barrido). Dejarlo en −0,15 sería mantener un número que este procedimiento no puede comprobar y que su propia ficha considera mal planteado. Quedar sin medir es lo que la regla prevé para ese caso: «un medio puede quedar sin firmar; es mejor que firmarlo sin fundamento».
- **Alternativa:** conservar el −0,15 como valor firmado el 2026-10-10 hasta que haya una lectura permitida. Solo cabe si la dirección editorial entiende que la firma en bloque del 2026-10-10 lo sacó de los niveles 4 y 5. Este barrido no lo cree: la firma no añadió piezas.
- **Qué lo cerraría:** que el medio autorice la lectura (o retire el veto), o que una persona lea sus piezas sobre Colombia de la ventana con el método de los demás barridos.
- **No se toca el registro, la propiedad ni los textos públicos.** Si se firma, los cambios serían: `bias: null` y una `biasRationale` que cite este barrido en `shared/mediaRegistry.js`, el texto de `shared/resumenesPublicos` para `cnn-es` y la ficha `fichas/cnn-es.md`.
