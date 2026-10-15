# The Wall Street Journal — ficha de orientación

| | |
|---|---|
| **Medio** | The Wall Street Journal · `wsj` · wsj.com |
| **Valor vigente** | **sin medir de forma permanente desde el 2026-10-12** (`bias: null`, `reviewedAt: null`) — decisión del responsable editorial: no autoriza la lectura por IA y no habrá lectura humana (`revision-externa/barridos/wsj.md`; `DECISIONES.md`, «2026-10-12 · Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Firma** | — |
| **Alta** | 2026-10-12 (ficha mínima, abierta con el barrido) |
| **Última revisión** | — |
| **Departamento / ámbito** | Diario económico estadounidense, en inglés. `country: 'US'`. `feed: null`: está en el catálogo para resolverse cuando se le cita y no se ingiere |
| **Fuentes de propiedad** | `shared/mediaOwnership.js` (`wsj`): 2 fuentes; comprobada el 2026-07-29 |
| **Recogida** | sin feed (`feed: null`) |
| **Protocolo** | `PROTOCOLO_JUICIO_EDITORIAL.md` |

## Estado

> **SIN MEDIR DE FORMA PERMANENTE DESDE EL 2026-10-12** (decisión del
> responsable editorial; `DECISIONES.md`, «2026-10-12 · Veinte medios: barridos
> firmados, sin medir permanente para quien no autoriza la IA, y feeds que se
> mantienen»). Llevaba +0,30 (firma en bloque del 2026-10-10), apoyado solo en
> una descripción, sin piezas leídas. Su robots.txt cierra todo el sitio a
> `User-agent: *` y solo lo abre a una lista cerrada de agentes en la que no
> están los de Anthropic ni el nuestro; su cabecera prohíbe la recolección por
> medios automatizados sin permiso escrito. DobleFoco ubica a los medios leyendo
> sus piezas con sistemas automáticos. DobleFoco se actualiza de forma 100 %
> automática y no habrá lectura humana, así que el medio no tiene lugar en el
> eje. Si autoriza la lectura, se medirá: se le pedirá permiso por correo tras
> el lanzamiento. No se ingiere: tiene `feed: null` desde antes de esta
> decisión, que no cambia ningún feed. Sigue en el catálogo para resolverse
> cuando se le cita. Su robots.txt prohíbe el uso automatizado de su contenido
> sin permiso; DobleFoco no recoge sus titulares (no tiene feed) y lo declara
> aquí. Lo que sigue es historia y se conserva: donde dice «valor actual»,
> «propuesta» o «pendiente de firma», es el estado anterior al 2026-10-12.

**2026-10-12, SIN MEDIR DE FORMA PERMANENTE.** `bias: null` y `reviewedAt:
null`. Su robots.txt cierra todo el sitio a `User-agent: *` y solo lo abre a una
lista cerrada de agentes en la que no están los de Anthropic ni el nuestro; su
cabecera prohíbe la recolección por medios automatizados sin permiso escrito. El
sitio es 100 % automático y no habrá lectura humana; si el medio autoriza la
lectura, se medirá (se pedirá permiso por correo tras el lanzamiento). No se
ingiere: tiene `feed: null` desde antes de esta decisión, que no cambia ningún
feed. Sigue en el catálogo para resolverse cuando se le cita. Su robots.txt
prohíbe el uso automatizado de su contenido sin permiso; DobleFoco no recoge sus
titulares (no tiene feed) y lo declara aquí.

**Historia — antes del 2026-10-12:**

Ficha mínima, abierta con el barrido. **El valor sigue en +0,30** hasta la decisión del responsable editorial sobre la propuesta de «sin medir».

## Evidencia

### Nivel 1 — Quién lo posee y quién lo dirige, hoy

| Dato | Valor | Fuente |
|---|---|---|
| Editor | **Dow Jones & Company**, filial de **News Corp**, que lo compró en 2007. `controlGroup: 'news-corp'` | `shared/mediaOwnership.js`, entrada `wsj`; [Al Jazeera, 2007](https://www.aljazeera.com/news/2007/7/23/dow-jones-board-okays-news-corp-bid) |
| Control | Familia Murdoch, mediante doble clase de acciones y un fideicomiso familiar. Desde septiembre de 2025, Lachlan Murdoch | [CNBC, 2025-09-08](https://www.cnbc.com/2025/09/08/lachlan-murdoch-cements-control-of-fox-wsj-media-empire-in-new-family-deal.html) |
| Quién lo dirige hoy | No consta | — |

### Nivel 2 — Conducta medida

No hay: `feed: null`, el medio no se ingiere.

### Nivel 4 — Lo que declara de sí mismo

No se consultó para esta ficha. La descripción del registro («página editorial explícitamente conservadora, sección informativa más neutra») es del eje estadounidense.

### Nivel 5 — Hechos editoriales de los últimos 12 meses: el barrido

[`revision-externa/barridos/wsj.md`](../revision-externa/barridos/wsj.md), hecho por Claude Opus 5.5 el 2026-10-12, a petición del responsable editorial.

- **No leído: el robots.txt excluye la lectura por IA.** El de `www.wsj.com` empieza con `User-agent: *` / `Disallow: /` y solo abre el sitio a una lista de agentes con nombre en la que no están ClaudeBot, Claude-Web ni anthropic-ai. No se descargó nada más que ese archivo.
- **Cero piezas clasificadas.** No hay lectura previa del medio en el repositorio.

## Argumento

El +0,30 vigente es una descripción de su página editorial en Estados Unidos, no de su trato a los gobiernos colombianos. Por la precisión del 2026-10-10, un valor que solo se apoya en los niveles 4 y 5 cede ante el barrido, y un barrido sin piezas lleva a **«sin medir»**.

## El mejor caso en contra

- Un barrido que no pudo hacerse no es un barrido que no llega; puede sostenerse que no hay barrido que mande y que el +0,30 firmado se queda.
- La página editorial del Journal es conservadora por declaración propia; la tensión hacia la derecha es razonable como expectativa, aunque no está medida sobre Colombia.

## Qué cambiaría el número

1. Una lectura de sus editoriales sobre Colombia de la ventana, con permiso de Dow Jones o hecha por una persona con suscripción, que cumpla las cinco condiciones o muestre la misma conducta con los dos gobiernos.

## Propiedad y lo que no consta

### LAGUNAS

- Toda la conducta editorial sobre Colombia.
- Quién lo dirige hoy y cómo se financia.

## Fuentes

- `shared/mediaRegistry.js` y `shared/mediaOwnership.js`, entrada `wsj`.
- [robots.txt de wsj.com](https://www.wsj.com/robots.txt), consultado el 2026-10-12.
- [Barrido editorial del WSJ](../revision-externa/barridos/wsj.md), 2025-10-12 → 2026-10-12.

## Historial

### Cabecera anterior (filas superadas)

| | |
|---|---|
| **Valor anterior (histórico, antes del 2026-10-12)** | **+0,30** · Derecha moderada · `reviewedAt: '2026-10-10'` (firma en bloque del catálogo, `DECISIONES.md`). Se apoya en una descripción, no en piezas leídas |
| **Propuesta (histórico)** | **«Sin medir»** (`bias: null`), por el barrido del 2026-10-12, que no pudo leer el medio. **Pendiente de firma.** Esta ficha no pone valor nuevo |
