# France 24 Español — ficha de orientación

| | |
|---|---|
| **Medio** | France 24 Español · `france24-es` · france24.com |
| **Valor vigente** | **sin medir de forma permanente desde el 2026-10-12** (`bias: null`, `reviewedAt: null`) — decisión del responsable editorial: no autoriza la lectura por IA y no habrá lectura humana (`revision-externa/barridos/france24-es.md`; `DECISIONES.md`, «2026-10-12 · Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Firma** | — |
| **Alta** | 2026-10-12 (ficha mínima, abierta con el barrido) |
| **Última revisión** | — |
| **Departamento / ámbito** | Servicio internacional en español de un medio público extranjero. `country: 'FR'`. En el mapa entra por el feed `france24.com/es/rss` |
| **Fuentes de propiedad** | `shared/mediaOwnership.js` (`france24-es`): 3 fuentes; comprobada el 2026-07-29 |
| **Recogida** | `https://www.france24.com/es/rss` · vía `direct` |
| **Protocolo** | `PROTOCOLO_JUICIO_EDITORIAL.md` |

## Estado

> **SIN MEDIR DE FORMA PERMANENTE DESDE EL 2026-10-12** (decisión del
> responsable editorial; `DECISIONES.md`, «2026-10-12 · Veinte medios: barridos
> firmados, sin medir permanente para quien no autoriza la IA, y feeds que se
> mantienen»). Llevaba 0,00 (por defecto, no con evidencia) (firma en bloque del
> 2026-10-10), apoyado solo en una descripción, sin piezas leídas. Su robots.txt
> cierra todo el sitio a 326 agentes por nombre, entre ellos seis de Anthropic.
> DobleFoco ubica a los medios leyendo sus piezas con sistemas automáticos. El
> sitio se actualiza de forma 100 % automática y no habrá lectura humana, así
> que el medio no tiene lugar en el eje. Si autoriza la lectura, se medirá: se
> le pedirá permiso por correo tras el lanzamiento. **El feed se mantiene**
> (`https://www.france24.com/es/rss`), por decisión del responsable editorial,
> como ejercicio de transparencia, y se vigila: sus titulares siguen en el
> agregador con enlace, y siguen contando en la cobertura de cada historia, no
> en el reparto por bandas. Lo que sigue es historia y se conserva: donde dice
> «valor actual», «propuesta» o «pendiente de firma», es el estado anterior al
> 2026-10-12.

**2026-10-12, SIN MEDIR DE FORMA PERMANENTE.** `bias: null` y `reviewedAt:
null`. Su robots.txt cierra todo el sitio a 326 agentes por nombre, entre ellos
seis de Anthropic. DobleFoco es 100 % automático y no habrá lectura humana; si el
medio autoriza la lectura, se medirá (se pedirá permiso por correo tras el
lanzamiento). El feed se mantiene (`https://www.france24.com/es/rss`), por
decisión del responsable editorial, como ejercicio de transparencia, y se
vigila: sus titulares siguen en el agregador con enlace, y siguen contando en la
cobertura de cada historia, no en el reparto por bandas.

**Historia — antes del 2026-10-12:**

Ficha mínima, sin firmar. El valor sigue en 0,00 hasta la decisión del
responsable editorial sobre la propuesta del barrido («sin medir»).

## Evidencia

### Nivel 1 — Quién lo posee y quién lo dirige, hoy

| Dato | Valor | Fuente |
|---|---|---|
| Titular | **Estado francés**, íntegramente desde 2008, a través del holding **France Médias Monde** (que agrupa también a RFI). `ownerType: 'publico'`, `controlGroup: 'france-medias-monde'` | `shared/mediaOwnership.js`, entrada `france24-es` |
| Financiación | Subvención estatal al holding: 263 millones de euros en 2023 | ídem; [State Media Monitor, France Médias Monde](https://statemediamonitor.com/2025/08/france-medias-monde-fmm/) |
| Salvaguardas de independencia | El perfil no recoge ninguna | ídem |
| Quién dirige hoy el servicio en español | **No consta** | — |

### Nivel 2 — Conducta medida

No consta en el repositorio. El corpus solo guarda lo internacional que un
medio colombiano también cubrió (`DECISIONES.md`), y no hay cifras de France 24.

### Nivel 4 — Lo que declara de sí mismo

No se consultó para esta ficha. El sitio veta la lectura por IA (ver nivel 5).

### Nivel 5 — Hechos editoriales de los últimos 12 meses: el barrido

**Barrido:** [`revision-externa/barridos/france24-es.md`](../revision-externa/barridos/france24-es.md),
hecho por Claude Opus 5.5 el 2026-10-12, a petición del responsable editorial.

- **No leído: el robots.txt excluye la lectura por IA.**
  `www.france24.com/robots.txt` (cabecera «France Medias Monde
  [2026-02-26]») veta el sitio entero a `anthropic-ai`, `ClaudeBot`,
  `Claude-Web`, `Claude-User`, `Claude-SearchBot` y `Claude-Code`
  (`Disallow: /`), y remite a un contacto de sindicación. Solo se descargó el
  robots.txt.
- **Cero piezas** sobre Colombia leídas o clasificadas.
- **No hay ninguna lectura previa** de sus piezas en el repositorio.

## Argumento

El **0,00 vigente** sale de la descripción del registro («cadena internacional
pública francesa; cobertura global con encuadre descriptivo»), con fuentes que
tratan de la propiedad. Se apoya solo en los niveles 4 y 5. Por la precisión
del 2026-10-10, un barrido manda sobre un valor así; este no pudo leer nada, y
la rama que corresponde es **«sin medir»**. Es la propuesta del barrido,
pendiente de firma.

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
- Quién dirige hoy el servicio en español y qué parte de la subvención del
  holding le llega.

## Fuentes

- `shared/mediaRegistry.js` y `shared/mediaOwnership.js`, entrada `france24-es`.
- [Barrido editorial de France 24 Español](../revision-externa/barridos/france24-es.md), 2025-10-12 → 2026-10-12.
- [robots.txt de France 24](https://www.france24.com/robots.txt), consultado el 2026-10-12.

## Historial

### Cabecera anterior (filas superadas)

| | |
|---|---|
| **Valor anterior (histórico, antes del 2026-10-12)** | **0,00** · orientación mixta · `reviewedAt: '2026-10-10'`. Sin cambios en esta ficha. Es un 0,00 por defecto, no un 0,00 con evidencia |
| **Firma (histórico)** | ☐ Pendiente. Esta ficha no propone valor nuevo: la propuesta está en el barrido (ver abajo) |
