# Barrido editorial: DW Español

| | |
|---|---|
| **Medio** | DW Español (`dw-es`), servicio en español de Deutsche Welle, la radiodifusora exterior de Alemania, dw.com. Sin ficha técnica hasta este barrido |
| **Valor vigente** | **−0,05**, orientación mixta (`reviewedAt: '2026-10-10'`). Su razón en el registro: «Radiodifusora pública internacional alemana; encuadre institucional europeo». Es una descripción del perfil, sin piezas detrás, y sus `biasSources` tratan de la propiedad: se apoya solo en los niveles 4 y 5 |
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

- **robots.txt** de `www.dw.com`, descargado el 2026-10-12 con el User-Agent de abajo (HTTP 200, 2.874 bytes, SHA-256 `f7daa7ad2ba66d113657a45c8ef5269c60701e204bee0c0560f196b3b985c98c`). Es la **única** petición que se hizo al medio. Abre con `User-agent: *` y una lista de rutas vetadas (`/search/`, `/overlay/`, cuentas de usuario…), y después veta el sitio entero a 53 agentes por nombre, entre ellos los tres de Anthropic. Las líneas literales:

  ```
  User-agent: anthropic-ai
  Disallow: /

  User-agent: ClaudeBot
  Disallow: /

  User-agent: Claude-Web
  Disallow: /
  ```

  `Disallow: /` cubre todo lo que el barrido necesitaba: el sitemap que anuncia (`Sitemap: https://www.dw.com/sitemap.xml`), las secciones y las piezas. **Por la regla de red del encargo, no se descargó nada más.**
- **User-Agent honesto:** `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. Nunca se usó el de un navegador. Que nuestro agente no se llame literalmente ClaudeBot no cambia nada: el veto es a la lectura por IA de Anthropic, y eso es lo que haría este barrido.
- **No se usó el feed de ingesta** (`rss.dw.com/rdf/rss-sp-all`, otro subdominio): el veto es del medio y el feed solo trae las últimas piezas, no 12 meses. Tampoco el corpus que ya ingiere el mapa: la ingesta no es lectura de postura (`DECISIONES.md`: el robots.txt bloquea la revisión, no la ingesta).
- **Ningún buscador, ningún archivo de terceros, ningún agregador.**
- **Lectura previa en el repositorio:** se buscó `dw-es`, «Deutsche Welle» y «DW» en fichas, barridos, respuestas y decisiones. **No hay ninguna lectura de piezas de DW sobre Colombia.** Solo constan el registro, el perfil de propiedad, el texto público (que ya dice que el número «no sostiene ninguna lectura documentada») y la decisión que deja en el corpus solo lo internacional que un medio colombiano también cubrió (`DECISIONES.md`, «Se aplica a todos por igual, incluidos Euronews, DW, France 24…»).

## 2. Cobertura y huecos

| | Piezas en la ventana | Con postura (D, I, M) | Fiscalización (F) | X |
|---|---:|---:|---:|---:|
| Antes del 07-08-2026 | no leído | — | — | — |
| Desde el 07-08-2026 | no leído | — | — | — |

**Hueco total.** No se sabe cuántas piezas sobre Colombia publicó DW Español en la ventana, ni si tiene voz de la casa sobre Colombia (no consta que publique editoriales; lo previsible es que la voz propia esté en titulares, entradillas y análisis de su redacción). No se leyó nada de la emisión de radio ni de televisión.

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

**Rama de la precisión del 2026-10-10.** El −0,05 vigente se apoya solo en los niveles 4 y 5 (una descripción del perfil, con fuentes de propiedad), así que el barrido manda. No llega a los mínimos y **no hay piezas a ningún lado para juzgar** → **«sin medir»** (`bias: null`). No es la rama «0,00 con evidencia»: para ella harían falta al menos 3 piezas a cada lado.

## 6. Valor propuesto y alternativa

**Propuesta: «sin medir»** (`bias: null`). Es lo que la precisión dispone para un valor de niveles 4 y 5 sin barrido posible, y lo que dice el encargo para un medio que veta la lectura por IA.

Frente a los vecinos del mapa internacional (registro al 2026-10-12): BBC Mundo −0,05, EFE 0,00, Reuters 0,00, France 24 0,00, Euronews +0,05. Ninguno de esos números tiene, por lo que consta en el repositorio, una lectura de piezas sobre Colombia detrás; el −0,05 de DW no se distingue de ellos por evidencia, sino por la descripción. Pasar a «sin medir» no dice que DW tenga dirección: dice que nadie la ha medido.

**Alternativa: conservar el −0,05 hasta una lectura humana.** El veto del robots.txt es a los agentes de IA, no a una persona: un lector humano del equipo puede hacer el barrido con este mismo método (sitemap del medio, piezas sobre Colombia, voz de la casa, polo fijo). Costo de la alternativa: el mapa seguiría mostrando un número sin piezas detrás, que es justo lo que la precisión del 2026-10-10 quiso evitar. Si se elige, el texto público ya lo declara.

**Qué lo movería:** un barrido humano que llegue a los mínimos (valor con tope ±0,30), que muestre la misma conducta con los dos gobiernos (0,00 con evidencia) o que encuentre dirección sin mínimos («sin medir» con tensión).

**No se toca el registro, la propiedad ni los textos públicos.** Si se firma «sin medir», los cambios serían `bias: null` y una `biasRationale` que cite este barrido en `shared/mediaRegistry.js`, el texto de `shared/resumenesPublicos/dw-es.js` y la ficha `fichas/dw-es.md`.
