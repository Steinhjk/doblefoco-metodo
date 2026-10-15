# DW Español — ficha de orientación

| | |
|---|---|
| **Medio** | DW Español · `dw-es` · dw.com |
| **Valor vigente** | **sin medir de forma permanente desde el 2026-10-12** (`bias: null`, `reviewedAt: null`) — decisión del responsable editorial: no autoriza la lectura por IA y no habrá lectura humana (`revision-externa/barridos/dw-es.md`; `DECISIONES.md`, «2026-10-12 · Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Firma** | — |
| **Alta** | 2026-10-12 (ficha mínima, abierta con el barrido) |
| **Última revisión** | — |
| **Departamento / ámbito** | Servicio internacional en español de un medio público extranjero. `country: 'DE'`. En el mapa entra por el feed `rss.dw.com/rdf/rss-sp-all` |
| **Fuentes de propiedad** | `shared/mediaOwnership.js` (`dw-es`): 3 fuentes; comprobada el 2026-07-29 |
| **Recogida** | `https://rss.dw.com/rdf/rss-sp-all` · vía `direct` |
| **Protocolo** | `PROTOCOLO_JUICIO_EDITORIAL.md` |

## Estado

> **SIN MEDIR DE FORMA PERMANENTE DESDE EL 2026-10-12** (decisión del
> responsable editorial; `DECISIONES.md`, «2026-10-12 · Veinte medios: barridos
> firmados, sin medir permanente para quien no autoriza la IA, y feeds que se
> mantienen»). Llevaba −0,05 (firma en bloque del 2026-10-10), apoyado solo en
> una descripción, sin piezas leídas. Su robots.txt cierra todo el sitio a 53
> agentes por nombre, entre ellos los tres de Anthropic. DobleFoco ubica a los
> medios leyendo sus piezas con sistemas automáticos. El sitio se actualiza de
> forma 100 % automática y no habrá lectura humana, así que el medio no tiene
> lugar en el eje. Si autoriza la lectura, se medirá: se le pedirá permiso por
> correo tras el lanzamiento. **El feed se mantiene**
> (`https://rss.dw.com/rdf/rss-sp-all`), por decisión del responsable editorial,
> como ejercicio de transparencia, y se vigila: sus titulares siguen en el
> agregador con enlace, y siguen contando en la cobertura de cada historia, no
> en el reparto por bandas. Lo que sigue es historia y se conserva: donde dice
> «valor actual», «propuesta» o «pendiente de firma», es el estado anterior al
> 2026-10-12.

**2026-10-12, SIN MEDIR DE FORMA PERMANENTE.** `bias: null` y `reviewedAt:
null`. Su robots.txt cierra todo el sitio a 53 agentes por nombre, entre ellos
los tres de Anthropic. DobleFoco es 100 % automático y no habrá lectura humana;
si el medio autoriza la lectura, se medirá (se pedirá permiso por correo tras el
lanzamiento). El feed se mantiene (`https://rss.dw.com/rdf/rss-sp-all`), por
decisión del responsable editorial, como ejercicio de transparencia, y se
vigila: sus titulares siguen en el agregador con enlace, y siguen contando en la
cobertura de cada historia, no en el reparto por bandas.

**Historia — antes del 2026-10-12:**

Ficha mínima, sin firmar. El valor sigue en −0,05 hasta la decisión del
responsable editorial sobre la propuesta del barrido («sin medir»).

## Evidencia

### Nivel 1 — Quién lo posee y quién lo dirige, hoy

| Dato | Valor | Fuente |
|---|---|---|
| Titular | **Deutsche Welle**, servicio exterior de radiodifusión de Alemania. `ownerType: 'publico'`, `controlGroup: 'deutsche-welle'` | `shared/mediaOwnership.js`, entrada `dw-es` |
| Financiación | Presupuesto federal (impuestos), no el canon de las cadenas públicas alemanas | ídem; [Wikipedia, Deutsche Welle](https://en.wikipedia.org/wiki/Deutsche_Welle) |
| Salvaguardas de independencia | El perfil no recoge ninguna | ídem |
| Quién dirige hoy el servicio en español | **No consta** | — |

### Nivel 2 — Conducta medida

No consta en el repositorio. El corpus solo guarda lo internacional que un
medio colombiano también cubrió (`DECISIONES.md`), y no hay cifras de DW.

### Nivel 4 — Lo que declara de sí mismo

No se consultó para esta ficha. El sitio veta la lectura por IA (ver nivel 5).

### Nivel 5 — Hechos editoriales de los últimos 12 meses: el barrido

**Barrido:** [`revision-externa/barridos/dw-es.md`](../revision-externa/barridos/dw-es.md),
hecho por Claude Opus 5.5 el 2026-10-12, a petición del responsable editorial.

- **No leído: el robots.txt excluye la lectura por IA.** `www.dw.com/robots.txt`
  veta el sitio entero a `anthropic-ai`, `ClaudeBot` y `Claude-Web`
  (`Disallow: /`). Solo se descargó el robots.txt.
- **Cero piezas** sobre Colombia leídas o clasificadas.
- **No hay ninguna lectura previa** de sus piezas en el repositorio.

## Argumento

El **−0,05 vigente** sale de la descripción del registro («radiodifusora
pública internacional alemana; encuadre institucional europeo»), con fuentes
que tratan de la propiedad. Se apoya solo en los niveles 4 y 5. Por la
precisión del 2026-10-10, un barrido manda sobre un valor así; este no pudo
leer nada, y la rama que corresponde es **«sin medir»**. Es la propuesta del
barrido, pendiente de firma.

## El mejor caso en contra

- **Que el veto sea a la IA no significa que el medio tenga dirección.** Pasar
  a «sin medir» quita del mapa un número que quizá era correcto. La
  alternativa del barrido era conservarlo hasta una lectura humana, y quedó
  descartada: no habrá lectura humana.
- **Un medio público extranjero puede tener posición sobre Colombia** por la
  política exterior de su Estado. No está medido en ningún sentido.

## Qué cambiaría el número

1. Un barrido humano de 12 meses de piezas sobre Colombia, con la regla de la
   «Evidencia editorial histórica».
2. Que el medio levante el veto a la lectura por IA.

## Propiedad y lo que no consta

### LAGUNAS

- Toda la lectura de piezas (nivel 5).
- Conducta medida (nivel 2).
- Quién dirige hoy el servicio en español y cuánto recibe del presupuesto
  federal.

## Fuentes

- `shared/mediaRegistry.js` y `shared/mediaOwnership.js`, entrada `dw-es`.
- [Barrido editorial de DW Español](../revision-externa/barridos/dw-es.md), 2025-10-12 → 2026-10-12.
- [robots.txt de DW](https://www.dw.com/robots.txt), consultado el 2026-10-12.

## Historial

### Cabecera anterior (filas superadas)

| | |
|---|---|
| **Valor anterior (histórico, antes del 2026-10-12)** | **−0,05** · orientación mixta · `reviewedAt: '2026-10-10'`. Sin cambios en esta ficha |
| **Firma (histórico)** | ☐ Pendiente. Esta ficha no propone valor nuevo: la propuesta está en el barrido (ver abajo) |
