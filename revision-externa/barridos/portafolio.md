# Barrido editorial: Portafolio

| | |
|---|---|
| **Medio** | Portafolio (`portafolio`), diario de economía y negocios de Casa Editorial El Tiempo, portafolio.co. No tenía ficha técnica: la crea este mismo encargo, mínima, en `fichas/portafolio.md` |
| **Valor vigente** | **+0,10**, orientación mixta, `reviewedAt: '2026-10-10'` (firma en bloque). Su razón en el registro es una frase: «Diario económico; encuadre desde indicadores y perspectiva empresarial». Sus tres fuentes (Wikipedia, una nota del archivo de El Tiempo y el Media Ownership Monitor) tratan de su historia y su propiedad. No hay lectura de piezas detrás: se apoya solo en los niveles 4 y 5. El texto público ya lo dice (`shared/resumenesPublicos/portafolio.js`) |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con la regla del polo fijo y la precisión del 2026-10-10 |
| **Ventana** | 2025-10-12 → 2026-10-12 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-12. Es de la misma casa que quien escribió otras fichas y barridos del catálogo: su acuerdo con ellos no es aval |
| **Estado** | **FIRMADO el 2026-10-12: «sin medir» de forma permanente** (`bias: null`). **Decisión del responsable editorial:** el sitio se actualiza de forma 100 % automática y no habrá lectura humana; mientras el robots.txt excluya la lectura por IA, el medio no tiene lugar en el eje. Si autoriza la lectura, se medirá. Aplicado en el registro, la ficha y el texto público el 2026-10-12 (`DECISIONES.md`, «Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Resultado** | **No leído: el robots.txt excluye la lectura por IA.** El de `www.portafolio.co` cierra todo el sitio a `ClaudeBot`, `Claude-Web` y `anthropic-ai` (`Disallow: /`), y su cabecera prohíbe la minería de textos y el uso del contenido para inteligencia artificial sin permiso escrito de Casa Editorial El Tiempo. No se descargó ninguna pieza, ni sección, ni sitemap. **Propuesta: «sin medir»** (`bias: null`), por la cuarta rama de la precisión del 2026-10-10: no hay piezas leídas para juzgar, y en el repositorio no consta ninguna lectura previa |

---

## 1. Método

- **Una sola petición al dominio:** `https://www.portafolio.co/robots.txt`, el 2026-10-12, HTTP 200, antes de cualquier otra. Ninguna más. No se pidieron los sitemaps que el propio robots.txt anuncia, ni el feed, ni una sola pieza.
- **User-Agent honesto:** `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. Nunca el de un navegador.
- **Lo que excluye, literal.** El fichero tiene un bloque titulado `# IA` con, entre otros:

  ```
  User-agent: ClaudeBot
  Disallow: /

  User-agent: Claude-Web
  Disallow: /

  User-agent: anthropic-ai
  Disallow: /
  ```

  Y su cabecera dice, literal: «El uso de cualquier dispositivo, herramienta o proceso diseñado para extraer datos o raspar el contenido, utilizando medios automatizados, está prohibido sin el permiso previo por escrito de Casa Editorial El Tiempo», y entre los usos prohibidos: «(1) actividades de minería de textos y datos; (2) el desarrollo de cualquier software, aprendizaje automático, inteligencia artificial (IA) y/o grandes modelos de lenguaje (LLM)».

  El bloque `User-agent: *` solo veta rutas concretas (`/buscar`, `/ingreso`, `/terminos-y-condiciones`, la zona de usuario, `/get-ads/` y tres de `/indicators/`). Que nuestro User-Agent no se llame `ClaudeBot` no cambia nada: **quien leería y clasificaría es un modelo de Anthropic**, que es justo lo que esas líneas excluyen, y la cabecera excluye el uso además del agente. La regla del encargo es no descargar, y no se descargó.
- **No se buscó otra puerta.** Ni buscadores, ni Internet Archive, ni agregadores, ni copias en otros medios, ni el archivo de eltiempo.com (prohibido para este encargo, y de la misma casa). Tampoco se usaron las piezas de Portafolio que el motor del catálogo ingiere por su feed (ver §4): no son una lectura documentada, y usarlas para clasificar sería leer por IA lo que el medio no permite.
- **Búsqueda en el repositorio** de una lectura previa de piezas: ninguna. No hay ficha técnica, ni respuesta de revisión sobre Portafolio, ni una sola URL de `portafolio.co` en los `.md` del repositorio. Las menciones (fichas de Valora Analitik, La República y El Tiempo; `DECISIONES.md`) lo citan como vecino de banda, no como medio leído.

## 2. Cobertura y huecos

| Universo | En la ventana | Leídas | Cuentan |
|---|---:|---:|---|
| Editoriales de Portafolio | sin contar | 0 | — |
| Titulares y entradillas sobre la política económica del Gobierno nacional | sin contar | 0 | — |

Todo es hueco. No se sabe cuántas piezas hay, ni si el diario publica editorial propio en la ventana.

## 3. Piezas

Ninguna. No hay tabla que recontar.

## 4. Números y rama de la precisión

| | D | I | M | F | X |
|---|---:|---:|---:|---:|---:|
| Antes del 07-08-2026 | — | — | — | — | — |
| Desde el 07-08-2026 | — | — | — | — | — |

**Antes:** +0,10, firmado el 2026-10-10, apoyado solo en los niveles 4 y 5 (descripción del género y propiedad). **Después (propuesto):** «sin medir».

**Rama: la cuarta** («no llega y no hay piezas suficientes a cada lado para juzgar → sin medir»). La salvedad de la precisión se aplica porque el +0,10 no sale de ninguna lectura: «si el número salió de la misión declarada, de la comparación con otros medios o de una frase sin fuente, el barrido manda». Aquí el barrido no pudo hacerse, y lo que manda es que no hay evidencia.

**Coherencia con el catálogo.** Es el mismo trato que recibió KienyKe el 2026-10-11 (un +0,30 sin lectura de piezas pasó a «sin medir» antes de su barrido) y el que dejó en «sin medir» a Razón Pública, Vorágine y Cuestión Pública cuando su barrido no permitía juzgar.

## 5. Alternativa

**Conservar +0,10.** Es defendible si el responsable editorial lee la primera precisión del 2026-10-09 («un barrido que no llega a los mínimos no deshace nada») como aplicable también a un barrido que no se pudo hacer. Argumentos: el +0,10 está dentro de la banda mixta; `DECISIONES.md` lo sostuvo como lectura estructural de un diario del capital («su orientación no se sitúa en el eje izquierda-derecha»); y Valora Analitik, su vecino de género, está en el mismo +0,10. En contra: la salvedad de la precisión del 2026-10-10 dice que un número apoyado solo en los niveles 4 y 5 no sobrevive al barrido, y mantenerlo dejaría a Portafolio con un valor más firme que el de los medios que sí fueron leídos y no llegaron. **Esta propuesta prefiere «sin medir».**

## 6. Lo que habría que hacer para medirlo

- **Lectura humana.** Que una persona lea los editoriales de Portafolio de la ventana y los titulares sobre la política económica de los dos gobiernos (presupuesto, reforma tributaria, emergencia económica, impuesto al patrimonio, regla fiscal, pensiones), y los clasifique con las mismas clases. La exclusión es a la lectura por IA; nada impide la lectura de una persona.
- **Permiso escrito de Casa Editorial El Tiempo**, que es lo que su robots.txt pide para cualquier uso automatizado. Si se obtuviera, el barrido se hace con el mismo método que el de Valora Analitik.

## 7. Lo que el responsable editorial debe ver

- **El feed del catálogo.** El registro ingiere `https://www.portafolio.co/rss/economia.xml` (`feed.via: 'direct'`). Nuestro motor no es un modelo de lenguaje ni se llama `ClaudeBot`, y el robots.txt no veta `/rss/` al agente `*`. Pero la cabecera prohíbe «actividades de minería de textos y datos» y el «uso de cualquier dispositivo, herramienta o proceso» automatizado sin permiso escrito, y eso es una decisión de política del proyecto, no de este barrido. **Este barrido no toca el registro**: lo deja señalado.
- **El hermano de casa.** El Tiempo (+0,05, firmado el 2026-10-10) es del mismo editor, y su dominio está prohibido para este encargo. Si se decidiera «sin medir» para Portafolio por falta de lectura, la misma pregunta vale para El Tiempo, que tampoco tiene barrido. Es otra decisión; aquí solo se declara.
