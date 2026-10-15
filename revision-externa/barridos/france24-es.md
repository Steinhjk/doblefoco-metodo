# Barrido editorial: France 24 Español

| | |
|---|---|
| **Medio** | France 24 Español (`france24-es`), servicio en español de la cadena internacional pública francesa (France Médias Monde), france24.com/es. Sin ficha técnica hasta este barrido |
| **Valor vigente** | **0,00**, orientación mixta (`reviewedAt: '2026-10-10'`). Su razón en el registro: «Cadena internacional pública francesa; cobertura global con encuadre descriptivo». Es una descripción, sin piezas detrás, y sus `biasSources` tratan de la propiedad: se apoya solo en los niveles 4 y 5. Es un 0,00 por defecto, no un 0,00 con evidencia |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con la regla del polo fijo y la precisión del 2026-10-10 |
| **Ventana** | 2025-10-12 → 2026-10-12 (regla del presente). Solo piezas sobre Colombia |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-12. Es de la misma casa que quien escribió otras fichas y barridos del catálogo: su acuerdo con ellos no es aval |
| **Estado** | **FIRMADO el 2026-10-12: «sin medir» de forma permanente** (`bias: null`); se descarta la alternativa de conservar el valor hasta una lectura humana. **Decisión del responsable editorial (difiere de esa alternativa):** el sitio se actualiza de forma 100 % automática y no habrá lectura humana; mientras el robots.txt excluya la lectura por IA, el medio no tiene lugar en el eje. Si autoriza la lectura, se medirá. Aplicado en el registro, la ficha y el texto público el 2026-10-12 (`DECISIONES.md`, «Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Resultado** | **No leído: el robots.txt excluye la lectura por IA.** Cero piezas descargadas, cero clasificadas. Rama de la precisión del 2026-10-10: **sin datos → «sin medir»** (`bias: null`) |

> Este barrido no tiene piezas. Lo que documenta es por qué no las tiene y
> qué se sigue de eso para un valor que hoy se apoya en una descripción.

---

## 1. Método

- **robots.txt** de `www.france24.com`, descargado el 2026-10-12 con el User-Agent de abajo (HTTP 200, 12.929 bytes, SHA-256 `e9c6fffa8dd78b8d26225f1a6631e52b301b9b90bd415c91ace82c640b47dd2f`). Es la **única** petición que se hizo al medio. Lleva la cabecera `# France Medias Monde [2026-02-26] - francemediasmonde.com`. Para `User-agent: *` no veta nada (`Disallow:` vacío), y bajo `### AI Bots blocking` veta el sitio entero a 326 agentes por nombre, entre ellos seis de Anthropic. Las líneas literales:

  ```
  User-agent: anthropic-ai
  Disallow: /

  User-agent: Claude-Code
  Disallow: /

  User-agent: Claude-SearchBot
  Disallow: /

  User-agent: Claude-User
  Disallow: /

  User-agent: Claude-Web
  Disallow: /

  User-agent: ClaudeBot
  Disallow: /
  ```

  El bloque lleva además la línea `### >> Contact us at syndication[@]francemm.com for partnership opportunities`: el veto es deliberado y remite a un acuerdo de sindicación. `Disallow: /` cubre todo lo que el barrido necesitaba: los sitemaps que anuncia (`/sitemaps/es/index.xml`, `/sitemaps/es/news.xml`), las secciones y las piezas. **Por la regla de red del encargo, no se descargó nada más.**
- **User-Agent honesto:** `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. Nunca se usó el de un navegador. Que nuestro agente no se llame literalmente ClaudeBot no cambia nada: el veto es a la lectura por IA de Anthropic, y eso es lo que haría este barrido.
- **No se usó el feed de ingesta** (`/es/rss`): mismo dominio, mismo veto, y solo trae las últimas piezas. Tampoco el corpus que ya ingiere el mapa: la ingesta no es lectura de postura (`DECISIONES.md`: el robots.txt bloquea la revisión, no la ingesta).
- **Ningún buscador, ningún archivo de terceros, ningún agregador.**
- **Lectura previa en el repositorio:** se buscó `france24-es` y «France 24» en fichas, barridos, respuestas y decisiones. **No hay ninguna lectura de piezas de France 24 sobre Colombia.** Solo constan el registro, el perfil de propiedad, el texto público (que ya dice que el número «no sostiene ninguna lectura documentada») y la decisión que deja en el corpus solo lo internacional que un medio colombiano también cubrió.

## 2. Cobertura y huecos

| | Piezas en la ventana | Con postura (D, I, M) | Fiscalización (F) | X |
|---|---:|---:|---:|---:|
| Antes del 07-08-2026 | no leído | — | — | — |
| Desde el 07-08-2026 | no leído | — | — | — |

**Hueco total.** No se sabe cuántas piezas sobre Colombia publicó France 24 en español en la ventana, ni si tiene voz de la casa sobre Colombia (no consta que publique editoriales; la voz propia estaría en titulares, entradillas y análisis de su redacción). No se leyó nada de la emisión de televisión.

## 3. Piezas clasificadas

Ninguna.

| # | Fecha | Título literal | URL | Clase |
|---|---|---|---|---|
| — | — | — | — | — |

## 4. Números antes / después

| | D | I | M | Con postura | F (no cuenta) |
|---|---:|---:|---:|---:|---:|
| Antes del 07-08-2026 | — | — | — | 0 | — |
| Desde el 07-08-2026 | — | — | — | 0 | — |

## 5. Veredicto por condición

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | No evaluable | Sin lectura |
| 2. A los dos lados del cambio | No evaluable | Sin lectura |
| 3. ≥10 piezas, ≥3 por lado, ≥3:1 | No | 0 piezas |
| 4. Contrapesos escritos | No evaluable | Sin lectura |
| 5. Reproducible | Sí, en lo negativo | El robots.txt literal y su huella están arriba |

**Rama de la precisión del 2026-10-10.** El 0,00 vigente se apoya solo en los niveles 4 y 5, así que el barrido manda. No llega a los mínimos y **no hay piezas a ningún lado para juzgar** → **«sin medir»** (`bias: null`). No es la rama «0,00 con evidencia»: para ella harían falta al menos 3 piezas de fiscalización o postura a cada lado del cambio.

## 6. Valor propuesto y alternativa

**Propuesta: «sin medir»** (`bias: null`). Es lo que la precisión dispone para un valor de niveles 4 y 5 sin barrido posible, y lo que dice el encargo para un medio que veta la lectura por IA.

Frente a los vecinos del mapa internacional (registro al 2026-10-12): EFE 0,00, Reuters 0,00, BBC Mundo −0,05, DW −0,05, Euronews +0,05. El 0,00 de France 24 coincide con el de las agencias, pero por descripción, no por evidencia. Que el número ya sea 0,00 no lo salva: la precisión distingue el 0,00 por defecto del 0,00 con evidencia, y este es el primero.

**Alternativa: conservar el 0,00 hasta una lectura humana.** El veto del robots.txt es a los agentes de IA, no a una persona: un lector humano del equipo puede hacer el barrido con este mismo método. Costo: el mapa seguiría mostrando un 0,00 que el lector toma por «medido y equilibrado» cuando solo es «no medido». Si se elige, el texto público ya lo declara.

**Qué lo movería:** un barrido humano que llegue a los mínimos (valor con tope ±0,30), que muestre la misma conducta con los dos gobiernos (0,00 con evidencia) o que encuentre dirección sin mínimos («sin medir» con tensión).

**No se toca el registro, la propiedad ni los textos públicos.** Si se firma «sin medir», los cambios serían `bias: null` y una `biasRationale` que cite este barrido en `shared/mediaRegistry.js`, el texto de `shared/resumenesPublicos/france24-es.js` y la ficha `fichas/france24-es.md`.
