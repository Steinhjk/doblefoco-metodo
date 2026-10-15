# Barrido editorial: Agencia EFE

| | |
|---|---|
| **Medio** | Agencia EFE (`efe`), agencia estatal española (capital de la SEPI). Entra al agregador por Google News (`via: 'gnews'`). Sin ficha técnica hasta este barrido (se abre `fichas/efe.md`, mínima) |
| **Valor vigente** | **0,00**, firmado en bloque el 2026-10-10 (`reviewedAt: '2026-10-10'`). Su razón en el registro: «Agencia de noticias; produce despachos factuales destinados a ser reutilizados por medios de todo el espectro». Es una descripción del oficio, sin piezas detrás: se apoya solo en el nivel 4 |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus precisiones, incluida la del 2026-10-10 |
| **Ventana** | 2025-10-12 → 2026-10-12 (regla del presente). Solo piezas sobre Colombia |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-12. Es de la misma casa que el autor del valor vigente: su acuerdo no es aval |
| **Estado** | **FIRMADO el 2026-10-12: «sin medir» de forma permanente** (`bias: null`); se descarta la alternativa de conservar 0,00. **Decisión del responsable editorial:** el sitio se actualiza de forma 100 % automática y no habrá lectura humana; mientras su sitio no ofrezca un robots.txt legible que autorice la lectura por IA, el medio no tiene lugar en el eje. Aplicado en el registro, la ficha y el texto público el 2026-10-12 (`DECISIONES.md`, «Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Resultado** | **No leído: no se pudo leer el robots.txt**, que está detrás de una verificación anti-bots, así que no consta que permita la lectura. **0 piezas.** Rama de la precisión del 2026-10-10: **sin datos → «sin medir»**. Propuesta: **«sin medir» (`bias: null`)**; alternativa: conservar 0,00 como valor por defecto declarado |

> No hay piezas que recontar. Lo reproducible aquí es la respuesta del
> servidor al pedir el robots.txt.

---

## 1. Método

- **La instrucción del barrido:** usar solo `efe.com`, y solo si su robots.txt
  lo permite. EFE ya entra por Google News en el agregador; esa vía no se usa
  para el barrido (y además el robots de Google News veta `/rss` a todos los
  agentes; ver `DECISIONES.md`, «`robots.txt`: dos excepciones escritas y una
  búsqueda»).
- **robots.txt** de `efe.com`, pedido el 2026-10-12 con el User-Agent de abajo.
  Fue **la única petición** al dominio. Respuesta: **HTTP 403, `text/html`**,
  y en lugar del robots una página de desafío. Sus primeras líneas, literales:

  ```
  <!DOCTYPE html><title>Checking your browser...</title><noscript><p>Javascript required</p></noscript>
  ```

  seguidas de un script de prueba de trabajo (`/__challenge/probes.js`).
- **No hay línea de robots que citar, porque no hay robots legible.** Lo que
  hay es más fuerte: el dominio entero, incluido el robots.txt, exige ejecutar
  JavaScript para pasar. No se intentó saltar la verificación —ni ejecutando el
  script, ni con el User-Agent de un navegador—. Sin un robots que lo permita,
  la instrucción manda no descargar.
- **Es la misma barrera que ya documentó el registro el 2026-10-10**
  (`shared/mediaRegistry.js`, entrada `efe`): `/robots.txt` y
  `/news-sitemap.xml` daban 403 «Checking your browser…». La API REST de
  WordPress (`/wp-json/wp/v2/posts`) que se anotó como alternativa vive detrás
  del mismo muro y no se pidió.
- **User-Agent honesto:** `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`.
  Cliente `curl -sS --ssl-no-revoke`. Nunca el de un navegador.
- **Sin rodeos.** Ni Google News, ni buscadores, ni Internet Archive, ni las
  reediciones de EFE en medios colombianos. Un despacho de EFE reeditado por
  otro medio es voz de ese medio para su barrido, no de la agencia.
- **Lectura previa en el repositorio:** **no hay.** Ninguna resolución, envío
  ni barrido anterior lee piezas de EFE sobre Colombia. Lo que hay de EFE en la
  revisión externa es su uso como filtro de agencia al medir a otros medios
  (`revision-externa/ciclo-1-conclusiones.md`), no una lectura de su voz.
  Tampoco se usaron los titulares de EFE guardados en la base por la ingesta de
  Google News: la instrucción excluye esa vía, y la base no guarda 12 meses.

---

## 2. Cobertura y huecos

| | Piezas en la ventana | Con postura (D, I, M) | Fiscalización (F) | X |
|---|---:|---:|---:|---:|
| Antes del 07-08-2026 | — | 0 | 0 | — |
| Desde el 07-08-2026 | — | 0 | 0 | — |
| **Total** | **no leído** | **0** | **0** | — |

**Hueco total:** no se leyó ninguna pieza.

**Lo que habría que esperar de una lectura.** EFE no tiene editoriales; su voz
propia son los titulares y entradillas sin atribuir. Lo probable es un corpus
casi todo X, con algo de fiscalización a cada lado; o «0,00 con evidencia» si
la conducta es la misma con los dos gobiernos, o «sin datos». Es una
expectativa, no una medición, y no se usa para nada.

---

## 3. Piezas clasificadas

Ninguna. No se descargó ninguna pieza.

---

## 4. Números antes y después del cambio

| | D | I | M | F | Con postura que cuenta |
|---|---:|---:|---:|---:|---:|
| Antes del 07-08-2026 | 0 | 0 | 0 | 0 | 0 |
| Desde el 07-08-2026 | 0 | 0 | 0 | 0 | 0 |

Sin lectura, los ceros no son conducta medida: son ausencia de datos.

---

## 5. Rama de la precisión del 2026-10-10

- **¿El valor vigente se apoya solo en los niveles 4 y 5?** Sí. El 0,00 sale
  de lo que es una agencia, no de piezas. El nivel 1 —capital íntegro de la
  SEPI, holding del Ministerio de Hacienda español— documenta un dueño público,
  pero el dueño es el Estado español y no un actor de la política colombiana:
  no da dirección en el eje colombiano.
- **Las cinco condiciones:** no se cumple ninguna, porque no hay piezas.
- **Rama:** «si no llega y no hay piezas suficientes a cada lado para juzgar →
  «sin medir» (`bias: null`)», en su caso extremo: cero piezas.

**Lo que no aplica:** la excepción de «Medios del Gobierno nacional» es para
medios que dependen del Gobierno nacional **colombiano**. EFE depende del
Gobierno de España; no le alcanza.

---

## 6. Valor propuesto y alternativa

**Propuesta: «sin medir» (`bias: null`).** Es lo que manda la instrucción
cuando el robots.txt no permite leer y no hay lectura previa, y lo que da la
última rama de la precisión. El texto público ya debería decir que el 0,00 no
lo sostiene ninguna pieza leída.

**Alternativa: conservar el 0,00, declarado como valor por defecto (regla 2)
y no como evidencia.** Argumento: un barrido que no se pudo hacer no es un
barrido que «no llega», y la precisión habla de barridos con piezas. EFE sí se
ingiere (por Google News): su valor pesa en la mezcla de las historias en que
aparece. Ahí la diferencia entre 0,00 y `null` sí se ve, y conviene que el
responsable editorial decida sabiendo eso.

**Frente a los vecinos del mapa.** DW −0,05, France 24 0,00, Euronews +0,05,
BBC Mundo −0,05 y Reuters 0,00 están todos en la franja central y sin barrido
leído; El País (España), −0,25, es el único internacional movido por piezas.
**EFE y Reuters son el mismo caso** —agencias, sin lectura posible por robots—
y deberían tratarse igual, sea cual sea la vía elegida.

**Qué haría falta para medir:** que EFE deje pasar a nuestro agente o publique
un robots legible que lo permita. El registro ya anota que el camino es
escribirles, como a RAYA.

---

## 7. Fuentes

- `https://efe.com/robots.txt`, pedido el 2026-10-12: HTTP 403 con página de desafío.
- `shared/mediaRegistry.js` (entrada `efe`, comentario del 2026-10-10) y `shared/mediaOwnership.js`, entrada `efe`.
- `PROTOCOLO_JUICIO_EDITORIAL.md`, «Evidencia editorial histórica» y precisión del 2026-10-10.
