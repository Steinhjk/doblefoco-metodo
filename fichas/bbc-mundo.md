# BBC Mundo — ficha de orientación

| | |
|---|---|
| **Medio** | BBC Mundo · `bbc-mundo` · bbc.com |
| **Valor vigente** | **sin medir de forma permanente desde el 2026-10-12** (`bias: null`, `reviewedAt: null`) — decisión del responsable editorial: no autoriza la lectura por IA y no habrá lectura humana (`revision-externa/barridos/bbc-mundo.md`; `DECISIONES.md`, «2026-10-12 · Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Firma** | — |
| **Alta** | 2026-10-12 (ficha mínima, abierta con el barrido) |
| **Última revisión** | — |
| **Departamento / ámbito** | Servicio internacional en español. `country: 'GB'`. Se ingiere por su RSS (`feeds.bbci.co.uk/mundo/rss.xml`) |
| **Fuentes de propiedad** | `shared/mediaOwnership.js` (`bbc-mundo`): 3 fuentes; comprobada el 2026-07-29 |
| **Recogida** | `https://feeds.bbci.co.uk/mundo/rss.xml` · vía `direct` |
| **Protocolo** | `PROTOCOLO_JUICIO_EDITORIAL.md` |

## Estado

> **SIN MEDIR DE FORMA PERMANENTE DESDE EL 2026-10-12** (decisión del
> responsable editorial; `DECISIONES.md`, «2026-10-12 · Veinte medios: barridos
> firmados, sin medir permanente para quien no autoriza la IA, y feeds que se
> mantienen»). Llevaba −0,05 (firma en bloque del 2026-10-10), apoyado solo en
> una descripción, sin piezas leídas. Su robots.txt cierra todo el sitio a
> `ClaudeBot`, `Claude-Web` y `anthropic-ai`, y su cabecera dice «No scraping,
> crawling, or systematic extraction of content». DobleFoco ubica a los medios
> leyendo sus piezas con sistemas automáticos. El sitio se actualiza de forma
> 100 % automática y no habrá lectura humana, así que el medio no tiene lugar en
> el eje. Si autoriza la lectura, se medirá: se le pedirá permiso por correo
> tras el lanzamiento. **El feed se mantiene**
> (`https://feeds.bbci.co.uk/mundo/rss.xml`), por decisión del responsable
> editorial, como ejercicio de transparencia, y se vigila: sus titulares siguen
> en el agregador con enlace, y siguen contando en la cobertura de cada
> historia, no en el reparto por bandas. Su robots.txt prohíbe el uso
> automatizado de su contenido sin permiso; DobleFoco toma solo
> lo que publica su feed (titular, extracto, imagen y enlace), con un rastreador identificado, y lo declara aquí. Lo que sigue es
> historia y se conserva: donde dice «valor actual», «propuesta» o «pendiente de
> firma», es el estado anterior al 2026-10-12.

**2026-10-12, SIN MEDIR DE FORMA PERMANENTE.** `bias: null` y `reviewedAt:
null`. Su robots.txt cierra todo el sitio a `ClaudeBot`, `Claude-Web` y
`anthropic-ai`, y su cabecera dice «No scraping, crawling, or systematic
extraction of content». DobleFoco es 100 % automático y no habrá lectura humana;
si el medio autoriza la lectura, se medirá (se pedirá permiso por correo tras el
lanzamiento). El feed se mantiene (`https://feeds.bbci.co.uk/mundo/rss.xml`),
por decisión del responsable editorial, como ejercicio de transparencia, y se
vigila: sus titulares siguen en el agregador con enlace, y siguen contando en la
cobertura de cada historia, no en el reparto por bandas. Su robots.txt prohíbe
el uso automatizado de su contenido sin permiso; DobleFoco toma solo
lo que publica su feed (titular, extracto, imagen y enlace), con un rastreador identificado, y lo declara aquí.

**Historia — antes del 2026-10-12:**

Ficha mínima, sin valor nuevo. El valor sigue en −0,05 hasta que el
responsable editorial decida sobre la propuesta del barrido.

## Evidencia

### Nivel 1 — Quién lo posee y quién lo dirige, hoy

| Dato | Valor | Fuente |
|---|---|---|
| Dueño | **BBC**, corporación pública británica; BBC Mundo es el servicio en español del **BBC World Service**. `controlGroup: 'bbc'` | `shared/mediaOwnership.js`, entrada `bbc-mundo` |
| Financiación | En 2025-26, 137 millones de libras del ministerio de Exteriores del Reino Unido (FCDO) frente a 221 millones de la licencia: cerca de un tercio del presupuesto del World Service | [House of Commons Library](https://commonslibrary.parliament.uk/research-briefings/cdp-2025-0132/) |

Pertinente para leer su cobertura de política exterior; no da dirección en el
eje colombiano.

### Nivel 2 — Conducta medida

No consta en el repositorio un envío con la conducta medida de BBC Mundo.

### Nivel 4 — Lo que declara de sí mismo

La obligación estatutaria de imparcialidad del servicio público. Es la única
base del −0,05 vigente; el registro no explica el signo.

### Nivel 5 — Hechos editoriales de los últimos 12 meses: el barrido

[`revision-externa/barridos/bbc-mundo.md`](../revision-externa/barridos/bbc-mundo.md),
hecho por Claude Opus 5.5 el 2026-10-12, a petición del responsable editorial.

- **No leído: el robots.txt excluye la lectura por IA.** Excluye de todo el
  sitio, por nombre, a `Claude-Web`, `ClaudeBot` y `anthropic-ai`
  (`Disallow: /`). **0 piezas.**
- No hay lectura previa de BBC Mundo en el repositorio; su texto público ya
  dice que el valor no lo sostiene ninguna lectura documentada.

## Argumento

El −0,05 vigente sale del estatuto de imparcialidad (nivel 4), sin piezas, y
sin razón escrita para el signo. Por la precisión del 2026-10-10, un valor así
cede ante el barrido; el barrido no pudo leer nada, y la rama que queda es
**«sin medir»**.

## El mejor caso en contra

- Un barrido que no se pudo hacer no es un barrido que «no llega». Conservar un
  número es defendible; si se conserva, lo honesto es 0,00 (regla 2), porque el
  −0,05 no tiene evidencia escrita.
- Se ingiere: su valor pesa en la mezcla de las historias, y pasar a `null` se
  nota.
- DW Español está en el mismo caso (servicio exterior público, −0,05, razón de
  nivel 4). Lo que se decida aquí debería valer allí.

## Qué cambiaría el número

Una lectura con permiso de sus análisis, explicadores y titulares sin atribuir
sobre Colombia a los dos lados del cambio de gobierno, con atención a los
calificativos de cada candidato y gobierno.

## Propiedad y lo que no consta

### LAGUNAS

- Toda la conducta editorial sobre Colombia: no se ha leído ninguna pieza.

## Historial

### Cabecera anterior (filas superadas)

| | |
|---|---|
| **Valor anterior (histórico, antes del 2026-10-12)** | **−0,05** · Mixta · `reviewedAt: '2026-10-10'` (firma en bloque tras el ciclo 2). Esta ficha no lo cambia |
| **Propuesta del barrido (histórico)** | **«sin medir»** (`bias: null`), pendiente de firma. Alternativas: conservar −0,05, o 0,00 por la regla 2 (ver abajo) |
