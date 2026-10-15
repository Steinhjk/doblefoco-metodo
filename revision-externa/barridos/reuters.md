# Barrido editorial: Reuters

| | |
|---|---|
| **Medio** | Reuters (`reuters`), agencia internacional de noticias de Thomson Reuters. `feed: null`: está en el catálogo para resolverse cuando se la cita y no se ingiere. Sin ficha técnica hasta este barrido (se abre `fichas/reuters.md`, mínima) |
| **Valor vigente** | **0,00**, firmado en bloque el 2026-10-10 (`reviewedAt: '2026-10-10'`). Su razón en el registro: «Agencia internacional con estándares de neutralidad codificados (Trust Principles)». Es la norma que la agencia se da, sin piezas detrás: se apoya solo en el nivel 4 |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus precisiones, incluida la del 2026-10-10 |
| **Ventana** | 2025-10-12 → 2026-10-12 (regla del presente). Solo piezas sobre Colombia |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-12. Es de la misma casa que el autor del valor vigente: su acuerdo no es aval |
| **Estado** | **FIRMADO el 2026-10-12: «sin medir» de forma permanente** (`bias: null`); se descarta la alternativa de conservar 0,00. **Decisión del responsable editorial:** el sitio se actualiza de forma 100 % automática y no habrá lectura humana; mientras el robots.txt excluya la lectura por IA, el medio no tiene lugar en el eje. Si autoriza la lectura, se medirá. Aplicado en el registro, la ficha y el texto público el 2026-10-12 (`DECISIONES.md`, «Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Resultado** | **No leído: el robots.txt excluye la lectura por IA** —y la de cualquier agente que no esté en su lista—. **0 piezas.** Rama de la precisión del 2026-10-10: **sin datos → «sin medir»**. Propuesta: **«sin medir» (`bias: null`)**; alternativa: conservar 0,00 como valor por defecto declarado |

> No hay piezas que recontar. Lo reproducible aquí es la comprobación del
> robots.txt: cualquiera puede descargarlo y llegar a la misma línea.

---

## 1. Método

- **robots.txt** de `www.reuters.com`, descargado el 2026-10-12 con el
  User-Agent de abajo (HTTP 200, `text/plain`). Fue **la única petición** al
  dominio.
- **Las líneas que deciden**, literales:

  ```
  # Block all other bots
  User-agent: *
  Allow: /plus/
  Disallow: /
  ```

  Nuestro agente no figura en la lista nominal de unos 80 agentes con permiso
  parcial, así que le aplica el bloque `User-agent: *`: todo el sitio vedado
  salvo `/plus/`. Ni ClaudeBot, ni Claude-Web, ni anthropic-ai están en esa
  lista: les aplica el mismo bloque. Además, **incluso para los agentes con
  permiso, el robots veta las ediciones en otros idiomas**, que son las que
  traerían la cobertura en español:

  ```
  Disallow: /es/
  Disallow: /latam/
  ```

  Y lo encabeza este aviso, también literal:

  ```
  # NOTICE: Collection of content, data and/or information from reuters.com through
  # automated means is prohibited unless you have prior written consent from Reuters
  ```

- **Decisión:** no se descargó nada más. No se leyeron sitemaps, secciones ni
  piezas.
- **User-Agent honesto:** `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`.
  Cliente `curl -sS --ssl-no-revoke`. Nunca el de un navegador.
- **Sin rodeos.** No se buscó la misma cobertura por buscadores, Internet
  Archive, Google News ni las reediciones de Reuters en otros medios. Una nota
  de Reuters reeditada por un medio colombiano es voz de ese medio, no de la
  agencia, y no entraría en el barrido de Reuters.
- **Lectura previa en el repositorio:** **no hay.** Ninguna resolución, envío ni
  barrido anterior lee piezas de Reuters sobre Colombia (búsqueda en
  `revision-externa/`, `fichas/` y `DECISIONES.md`). El registro ya anotaba que
  el sitio responde 401 (DataDome) a clientes que no son navegador
  (`shared/mediaRegistry.js`, comentario sobre los cuatro medios en inglés).

---

## 2. Cobertura y huecos

| | Piezas en la ventana | Con postura (D, I, M) | Fiscalización (F) | X |
|---|---:|---:|---:|---:|
| Antes del 07-08-2026 | — | 0 | 0 | — |
| Desde el 07-08-2026 | — | 0 | 0 | — |
| **Total** | **no leído** | **0** | **0** | — |

**Hueco total:** no se leyó ninguna pieza. No hay universo, ni filtro, ni
lectura.

**Lo que habría que esperar de una lectura, para quien la haga con permiso.**
Una agencia apenas tiene voz propia: no publica editoriales, y sus titulares y
entradillas suelen atribuir. La voz de la casa sería solo lo que el titular y
la entradilla dicen sin atribuir (calificativos, encuadres). Lo probable es un
corpus casi todo X, con algo de fiscalización a cada lado; es decir, o bien
«0,00 con evidencia» si la conducta es la misma con los dos gobiernos, o bien
«sin datos». Es una expectativa, no una medición, y no se usa para nada.

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
  de los Trust Principles (lo que la casa declara de sí misma, nivel 4). El
  nivel 1 —Woodbridge, la familia Thomson, la Founders Share Company— documenta
  salvaguardas de independencia, no una posición política: no da dirección. Por
  eso le alcanza la precisión: si hay barrido, el barrido manda.
- **Las cinco condiciones:** no se cumple ninguna, porque no hay piezas.
- **Rama:** «si no llega y no hay piezas suficientes a cada lado para juzgar →
  «sin medir» (`bias: null`)». Es el caso extremo de esa rama: cero piezas.

---

## 6. Valor propuesto y alternativa

**Propuesta: «sin medir» (`bias: null`).** Es lo que manda la instrucción del
barrido cuando el robots.txt impide leer y no hay lectura previa en el
repositorio, y lo que da la última rama de la precisión. El lector vería que
el 0,00 de Reuters no lo sostiene ninguna pieza leída.

**Alternativa: conservar el 0,00 vigente, declarado como valor por defecto y
no como evidencia.** Argumento: un barrido que no se pudo hacer no es un
barrido que «no llega»; la precisión del 2026-10-10 habla de barridos con
piezas. Reuters además no se ingiere (`feed: null`), así que su valor solo se
ve cuando se la cita como fuente; un `null` ahí no corrige ningún sesgo del
mapa. Si se escoge esta vía, la ficha debe decir que el 0,00 es la regla 2 (la
duda va a la mixta), no una medición.

**Frente a los vecinos del mapa.** Los internacionales del catálogo están en
una franja estrecha alrededor del centro y casi todos sin barrido: DW −0,05,
France 24 0,00, Euronews +0,05, BBC Mundo −0,05, EFE 0,00. Los que se movieron
lo hicieron con piezas: El País (España) −0,25 por cinco editoriales sobre
Colombia. CNN en Español −0,15 se apoya en una descripción. Nada en lo leído
justifica separar a Reuters de su vecina más cercana, EFE, que también es
agencia y tampoco se pudo leer: **las dos deberían tratarse igual**.

**Qué haría falta para medir:** permiso escrito de Reuters (el aviso del
robots remite a `reutersagency.com/contact-us/enquire/`), o una lectura humana
sin automatizar, declarada como tal.

---

## 7. Fuentes

- [robots.txt de Reuters](https://www.reuters.com/robots.txt), consultado el 2026-10-12.
- `shared/mediaRegistry.js` y `shared/mediaOwnership.js`, entrada `reuters`.
- `PROTOCOLO_JUICIO_EDITORIAL.md`, «Evidencia editorial histórica» y precisión del 2026-10-10.
