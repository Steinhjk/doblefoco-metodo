# Reuters — ficha de orientación

| | |
|---|---|
| **Medio** | Reuters · `reuters` · reuters.com |
| **Valor vigente** | **sin medir de forma permanente desde el 2026-10-12** (`bias: null`, `reviewedAt: null`) — decisión del responsable editorial: no autoriza la lectura por IA y no habrá lectura humana (`revision-externa/barridos/reuters.md`; `DECISIONES.md`, «2026-10-12 · Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Firma** | — |
| **Alta** | 2026-10-12 (ficha mínima, abierta con el barrido) |
| **Última revisión** | — |
| **Departamento / ámbito** | Agencia internacional. `country: 'GB'`. **No se ingiere** (`feed: null`): está en el catálogo para resolverse cuando se la cita como fuente |
| **Fuentes de propiedad** | `shared/mediaOwnership.js` (`reuters`): 2 fuentes; comprobada el 2026-07-29 |
| **Recogida** | sin feed (`feed: null`) |
| **Protocolo** | `PROTOCOLO_JUICIO_EDITORIAL.md` |

## Estado

> **SIN MEDIR DE FORMA PERMANENTE DESDE EL 2026-10-12** (decisión del
> responsable editorial; `DECISIONES.md`, «2026-10-12 · Veinte medios: barridos
> firmados, sin medir permanente para quien no autoriza la IA, y feeds que se
> mantienen»). Llevaba 0,00 (firma en bloque del 2026-10-10), apoyado solo en
> una descripción, sin piezas leídas. Su robots.txt cierra todo el sitio (salvo
> `/plus/`) a cualquier agente que no esté en su lista nominal, y en ella no
> están los de Anthropic ni el nuestro; su aviso prohíbe la recolección por
> medios automatizados sin consentimiento escrito de Reuters. DobleFoco ubica a
> los medios leyendo sus piezas con sistemas automáticos. El sitio se actualiza
> de forma 100 % automática y no habrá lectura humana, así que el medio no tiene
> lugar en el eje. Si autoriza la lectura, se medirá: se le pedirá permiso por
> correo tras el lanzamiento. No se ingiere: tiene `feed: null` desde antes de
> esta decisión, que no cambia ningún feed. Sigue en el catálogo para resolverse
> cuando se le cita. Su robots.txt prohíbe el uso automatizado de su contenido
> sin permiso; DobleFoco no recoge sus titulares (no tiene feed) y lo declara
> aquí. Lo que sigue es historia y se conserva: donde dice «valor actual»,
> «propuesta» o «pendiente de firma», es el estado anterior al 2026-10-12.

**2026-10-12, SIN MEDIR DE FORMA PERMANENTE.** `bias: null` y `reviewedAt:
null`. Su robots.txt cierra todo el sitio (salvo `/plus/`) a cualquier agente
que no esté en su lista nominal, y en ella no están los de Anthropic ni el
nuestro; su aviso prohíbe la recolección por medios automatizados sin
consentimiento escrito de Reuters. DobleFoco es 100 % automático y no habrá
lectura humana; si el medio autoriza la lectura, se medirá (se pedirá permiso
por correo tras el lanzamiento). No se ingiere: tiene `feed: null` desde antes
de esta decisión, que no cambia ningún feed. Sigue en el catálogo para
resolverse cuando se le cita. Su robots.txt prohíbe el uso automatizado de su
contenido sin permiso; DobleFoco no recoge sus titulares (no tiene feed) y lo
declara aquí.

**Historia — antes del 2026-10-12:**

Ficha mínima, sin valor nuevo. El valor sigue en 0,00 hasta que el responsable
editorial decida sobre la propuesta del barrido. Debe decidirse igual que EFE,
que es el mismo caso (agencia, sin lectura posible).

## Evidencia

### Nivel 1 — Quién lo posee y quién lo dirige, hoy

| Dato | Valor | Fuente |
|---|---|---|
| Grupo | **Thomson Reuters**; accionista mayoritario **The Woodbridge Company**, sociedad de inversión de la familia Thomson (Canadá), con cerca del 68 %. `controlGroup: 'woodbridge'` | `shared/mediaOwnership.js`, entrada `reuters` |
| Salvaguarda | **Trust Principles**, respaldados por la Reuters Founders Share Company, con una acción especial con veto ante una toma de control que amenace la independencia | ídem |

El nivel 1 documenta salvaguardas de independencia, no una posición política
en el eje colombiano.

### Nivel 2 — Conducta medida

No consta. No se ingiere, así que no hay corpus propio.

### Nivel 4 — Lo que declara de sí mismo

Los Trust Principles: integridad, independencia y ausencia de sesgo. Es la
única base del 0,00 vigente.

### Nivel 5 — Hechos editoriales de los últimos 12 meses: el barrido

[`revision-externa/barridos/reuters.md`](../revision-externa/barridos/reuters.md),
hecho por Claude Opus 5.5 el 2026-10-12, a petición del responsable editorial.

- **No leído: el robots.txt excluye la lectura por IA.** Su bloque
  `User-agent: *` dice `Disallow: /` (solo permite `/plus/`), y para los
  agentes con permiso veta además `/es/` y `/latam/`. **0 piezas.**
- No hay lectura previa de Reuters en el repositorio.

## Argumento

El 0,00 vigente sale de las normas que la agencia se da (nivel 4), sin piezas.
Por la precisión del 2026-10-10, un valor así cede ante el barrido; el barrido
no pudo leer nada, y la rama que queda es **«sin medir»**.

## El mejor caso en contra

- Un barrido que no se pudo hacer no es un barrido que «no llega». Conservar el
  0,00 por la regla 2 (la duda va a la mixta) es defendible, siempre que se
  declare como valor por defecto y no como medición.
- Como no se ingiere, su valor solo se ve cuando se la cita: la diferencia
  práctica entre 0,00 y `null` es pequeña.

## Qué cambiaría el número

Una lectura con permiso de Reuters de sus piezas sobre Colombia a los dos lados
del cambio de gobierno: la misma conducta con ambos daría «0,00 con
evidencia»; una asimetría sostenida en titulares y entradillas sin atribuir lo
movería.

## Propiedad y lo que no consta

### LAGUNAS

- Toda la conducta editorial sobre Colombia: no se ha leído ninguna pieza.

## Historial

### Cabecera anterior (filas superadas)

| | |
|---|---|
| **Valor anterior (histórico, antes del 2026-10-12)** | **0,00** · Mixta · `reviewedAt: '2026-10-10'` (firma en bloque tras el ciclo 2). Esta ficha no lo cambia |
| **Propuesta del barrido (histórico)** | **«sin medir»** (`bias: null`), pendiente de firma. Alternativa: conservar 0,00 como valor por defecto declarado (ver abajo) |
