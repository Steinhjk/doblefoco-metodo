# Agencia EFE — ficha de orientación

| | |
|---|---|
| **Medio** | Agencia EFE · `efe` · efe.com |
| **Valor vigente** | **sin medir de forma permanente desde el 2026-10-12** (`bias: null`, `reviewedAt: null`) — decisión del responsable editorial: no autoriza la lectura por IA y no habrá lectura humana (`revision-externa/barridos/efe.md`; `DECISIONES.md`, «2026-10-12 · Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Firma** | — |
| **Alta** | 2026-10-12 (ficha mínima, abierta con el barrido) |
| **Última revisión** | — |
| **Departamento / ámbito** | Agencia internacional. `country: 'ES'`. Se ingiere por Google News (`via: 'gnews'`), porque `efe.com` tiene los feeds desactivados y el dominio está detrás de una verificación anti-bots |
| **Fuentes de propiedad** | `shared/mediaOwnership.js` (`efe`): 3 fuentes; comprobada el 2026-07-29 |
| **Recogida** | `https://news.google.com/rss/search?q=site%3Aefe.com&hl=es-419&gl=CO&ceid=CO:es-419` · vía `gnews` |
| **Protocolo** | `PROTOCOLO_JUICIO_EDITORIAL.md` |

## Estado

> **SIN MEDIR DE FORMA PERMANENTE DESDE EL 2026-10-12** (decisión del
> responsable editorial; `DECISIONES.md`, «2026-10-12 · Veinte medios: barridos
> firmados, sin medir permanente para quien no autoriza la IA, y feeds que se
> mantienen»). Llevaba 0,00 (firma en bloque del 2026-10-10), apoyado solo en
> una descripción, sin piezas leídas. Su sitio no ofrece un robots.txt legible:
> `efe.com/robots.txt` responde con una verificación anti-bots que exige
> JavaScript, así que no consta que autorice la lectura por IA. DobleFoco ubica
> a los medios leyendo sus piezas con sistemas automáticos. El sitio se
> actualiza de forma 100 % automática y no habrá lectura humana, así que el
> medio no tiene lugar en el eje. Si autoriza la lectura, se medirá: se le
> pedirá permiso por correo tras el lanzamiento. **El feed se mantiene** (Google
> News, `via: "gnews"`), por decisión del responsable editorial, como ejercicio
> de transparencia, y se vigila: sus titulares siguen en el agregador con
> enlace, y siguen contando en la cobertura de cada historia, no en el reparto
> por bandas. Lo que sigue es historia y se conserva: donde dice «valor actual»,
> «propuesta» o «pendiente de firma», es el estado anterior al 2026-10-12.

**2026-10-12, SIN MEDIR DE FORMA PERMANENTE.** `bias: null` y `reviewedAt:
null`. Su sitio no ofrece un robots.txt legible: `efe.com/robots.txt` responde
con una verificación anti-bots que exige JavaScript, así que no consta que
autorice la lectura por IA. DobleFoco es 100 % automático y no habrá lectura
humana; si el medio autoriza la lectura, se medirá (se pedirá permiso por correo
tras el lanzamiento). El feed se mantiene (Google News, `via: "gnews"`), por
decisión del responsable editorial, como ejercicio de transparencia, y se
vigila: sus titulares siguen en el agregador con enlace, y siguen contando en la
cobertura de cada historia, no en el reparto por bandas.

**Historia — antes del 2026-10-12:**

Ficha mínima, sin valor nuevo. El valor sigue en 0,00 hasta que el responsable
editorial decida sobre la propuesta del barrido. Debe decidirse igual que
Reuters, que es el mismo caso.

## Evidencia

### Nivel 1 — Quién lo posee y quién lo dirige, hoy

| Dato | Valor | Fuente |
|---|---|---|
| Dueño | **Sociedad Estatal de Participaciones Industriales (SEPI)**, holding público del Ministerio de Hacienda de España, con el 100 % del capital. `controlGroup: 'sepi'` | `shared/mediaOwnership.js`, entrada `efe`; [SEPI, Agencia EFE](https://www.sepi.es/en/sectores/agencia-efe) |
| Financiación | Venta de contenidos y una subvención anual del Estado español | ídem |

Dueño público, pero del Estado español: no es un actor de la política
colombiana y no da dirección en este eje. La excepción de «Medios del Gobierno
nacional» del protocolo no le alcanza: cubre al Gobierno de Colombia.

### Nivel 2 — Conducta medida

No consta un envío con la conducta medida de EFE.

### Nivel 4 — Lo que declara de sí mismo

No se consultó para esta ficha. El 0,00 vigente se apoya en la descripción del
oficio de agencia («despachos factuales destinados a ser reutilizados por
medios de todo el espectro»).

### Nivel 5 — Hechos editoriales de los últimos 12 meses: el barrido

[`revision-externa/barridos/efe.md`](../revision-externa/barridos/efe.md),
hecho por Claude Opus 5.5 el 2026-10-12, a petición del responsable editorial.

- **No leído:** el robots.txt de `efe.com` responde **HTTP 403** con una página
  «Checking your browser… Javascript required». No hay robots legible que
  permita la lectura, y no se intentó saltar la verificación. Google News no se
  usó para el barrido. **0 piezas.**
- No hay lectura previa de EFE en el repositorio.

## Argumento

El 0,00 vigente sale de lo que es una agencia, sin piezas (nivel 4). Por la
precisión del 2026-10-10, un valor así cede ante el barrido; el barrido no pudo
leer nada, y la rama que queda es **«sin medir»**.

## El mejor caso en contra

- Un barrido que no se pudo hacer no es un barrido que «no llega». Conservar el
  0,00 por la regla 2 es defendible, declarado como valor por defecto.
- EFE sí se ingiere: su valor pesa en la mezcla de las historias en que
  aparece, y pasar a `null` se nota.

## Qué cambiaría el número

Una lectura permitida de sus piezas sobre Colombia a los dos lados del cambio
de gobierno: la misma conducta con ambos daría «0,00 con evidencia»; una
asimetría sostenida en titulares y entradillas sin atribuir lo movería.

## Propiedad y lo que no consta

### LAGUNAS

- Toda la conducta editorial sobre Colombia: no se ha leído ninguna pieza.
- Un acceso permitido a `efe.com` (el registro anota escribirles, como a RAYA).

## Historial

### Cabecera anterior (filas superadas)

| | |
|---|---|
| **Valor anterior (histórico, antes del 2026-10-12)** | **0,00** · Mixta · `reviewedAt: '2026-10-10'` (firma en bloque tras el ciclo 2). Esta ficha no lo cambia |
| **Propuesta del barrido (histórico)** | **«sin medir»** (`bias: null`), pendiente de firma. Alternativa: conservar 0,00 como valor por defecto declarado (ver abajo) |
