# Barrido editorial: La Vanguardia

| | |
|---|---|
| **Medio** | La Vanguardia (`la-vanguardia-es`), diario de Barcelona del Grupo Godó, lavanguardia.com. **No es Vanguardia, de Bucaramanga** (`vanguardia`), que también está en el mapa con otros dueños. Sin ficha técnica hasta este barrido |
| **Valor vigente** | **+0,10**, orientación mixta (`reviewedAt: '2026-10-10'`). Su razón en el registro: «Diario barcelonés de tradición liberal-conservadora moderada». Es una descripción de su trayectoria, sin piezas detrás, y sus `biasSources` tratan de la propiedad: se apoya solo en los niveles 4 y 5 |
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

- **robots.txt** de `www.lavanguardia.com`, descargado el 2026-10-12 con el User-Agent de abajo (HTTP 200, 12.819 bytes, SHA-256 `8de87b013e3fd3a4cadb0a2c370e23cfa58fc59bc14ee3fb4202a987dc601f01`). Es la **única** petición que se hizo al medio. Para `User-agent: *` veta rutas concretas (`/temas/`, `/buscador/`, `/_hemeroteca/*`, `/premium/`, los sitemaps de agencias y el índice `/sitemap-index.xml`, entre otras), y después veta por nombre a 34 agentes, entre ellos el rastreador de Anthropic. Las líneas literales:

  ```
  User-agent: ClaudeBot
  Disallow: /
  Allow: /comprar/
  Allow: /*brl
  ```

  `Disallow: /` cubre todo lo que el barrido necesitaba: las secciones, los sitemaps y las piezas. Las dos excepciones (`/comprar/` y las rutas que contienen `brl`) no son piezas periodísticas sobre Colombia y no se usaron. No hay líneas para `anthropic-ai` ni `Claude-Web`, pero el veto a ClaudeBot basta: el encargo excluye el medio si veta a cualquiera de los tres. **Por la regla de red del encargo, no se descargó nada más.**
- **User-Agent honesto:** `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. Nunca se usó el de un navegador. Que nuestro agente no se llame literalmente ClaudeBot no cambia nada: el veto es a la lectura por IA de Anthropic, y eso es lo que haría este barrido.
- **No se usó el feed de ingesta** (`/rss/home.xml`): mismo dominio, mismo veto, y solo trae las últimas piezas. Tampoco el corpus que ya ingiere el mapa: la ingesta no es lectura de postura (`DECISIONES.md`: el robots.txt bloquea la revisión, no la ingesta).
- **Ningún buscador, ningún archivo de terceros, ningún agregador.** Muro de pago: no aplica, porque no se pidió ninguna pieza.
- **Lectura previa en el repositorio:** se buscó `la-vanguardia-es` y «La Vanguardia» en fichas, barridos, respuestas y decisiones. **No hay ninguna lectura de piezas de La Vanguardia sobre Colombia.** Lo único que consta, además del registro, la propiedad y el texto público, es que en el corpus aparece como el segundo medio que más historias comparte con El País de España (37, en `fichas/el-pais-es.md`). Eso es coincidencia de cobertura, no postura, y la propia ficha dice que esa métrica no sirve para situar un medio.

## 2. Cobertura y huecos

| | Piezas en la ventana | Con postura (D, I, M) | Fiscalización (F) | X |
|---|---:|---:|---:|---:|
| Antes del 07-08-2026 | no leído | — | — | — |
| Desde el 07-08-2026 | no leído | — | — | — |

**Hueco total.** No se sabe cuántas piezas sobre Colombia publicó La Vanguardia en la ventana. A diferencia de DW y France 24, es un diario que publica editoriales sin firma (no se comprobó en el sitio, porque no se leyó), así que un barrido humano tendría voz de la casa en sentido estricto; es probable, pero no está comprobado, que pocos traten de Colombia y que no lleguen a 3 por lado.

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

**Rama de la precisión del 2026-10-10.** El +0,10 vigente se apoya solo en los niveles 4 y 5 (una descripción de su tradición, con fuentes de propiedad), así que el barrido manda. No llega a los mínimos y **no hay piezas a ningún lado para juzgar** → **«sin medir»** (`bias: null`).

## 6. Valor propuesto y alternativa

**Propuesta: «sin medir»** (`bias: null`). Es lo que la precisión dispone para un valor de niveles 4 y 5 sin barrido posible, y lo que dice el encargo para un medio que veta la lectura por IA.

Frente a los vecinos del mapa internacional (registro al 2026-10-12): Euronews +0,05, Financial Times +0,15, Infobae +0,15, EFE 0,00. El +0,10 sale de la línea de La Vanguardia **en la política española y catalana**; la regla mide la postura sobre el Gobierno colombiano y sus candidaturas, y nada asegura que sean la misma. Es la razón de fondo por la que el número no sobrevive sin lectura.

**Alternativa: conservar el +0,10 hasta una lectura humana.** El veto del robots.txt es a los agentes de IA, no a una persona: un lector humano del equipo puede hacer el barrido de editoriales y piezas sobre Colombia con este mismo método, leyendo solo lo que el sitio sirve abierto. Costo: el mapa seguiría mostrando un número sin piezas detrás. Si se elige, el texto público ya lo declara.

**Qué lo movería:** un barrido humano que llegue a los mínimos (valor con tope ±0,30), que muestre la misma conducta con los dos gobiernos (0,00 con evidencia) o que encuentre dirección sin mínimos («sin medir» con tensión).

**No se toca el registro, la propiedad ni los textos públicos.** Si se firma «sin medir», los cambios serían `bias: null` y una `biasRationale` que cite este barrido en `shared/mediaRegistry.js`, el texto de `shared/resumenesPublicos/la-vanguardia-es.js` y la ficha `fichas/la-vanguardia-es.md`.
