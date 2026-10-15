# Barrido editorial: Noticias Caracol

| | |
|---|---|
| **Medio** | Noticias Caracol (`noticias-caracol`), noticiero de televisión abierta de Caracol Televisión S.A. (la misma sociedad que opera Blu Radio; Valorem 93,49 %). Portal: noticiascaracol.com |
| **Valor vigente** | **+0,10**, firmado en bloque el 2026-10-10 (`reviewedAt: '2026-10-10'`). Su razón escrita es una frase sin fuente: «Informativo de televisión abierta líder en audiencia; cobertura amplia con encuadre institucional y foco en seguridad y orden público». La ficha lo dice sin rodeos: «El +0,10 no tiene ninguna evidencia propia detrás». La propiedad (nivel 1) no da una posición política conocida. Es decir: **el valor se apoya solo en los niveles 4 y 5**, y por la precisión del 2026-10-10 el barrido manda |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con la regla del polo fijo y las precisiones del 2026-10-09 y del 2026-10-10 |
| **Ventana** | 2025-10-12 → 2026-10-12 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-12. Es de la misma casa que el autor de la ficha y de los otros barridos: su acuerdo no es aval |
| **Estado** | **FIRMADO el 2026-10-12: «sin medir»** (antes +0,10), como se propuso: 4 piezas con postura en un año. Se descarta la alternativa de 0,00. Aplicado en el registro, la ficha y el texto público el 2026-10-12 (`DECISIONES.md`, «Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Resultado** | **No cumple los mínimos, ni de lejos.** En 336 piezas leídas y 1.797 titulares (por su slug) hay **4 piezas con postura en voz de la casa: 3 D (dos de ellas «retro») y 1 I**, más 1 mixta. La voz del portal es casi toda atribuida. **Rama: no hay piezas suficientes para juzgar → «sin medir»**. Alternativa: 0,00 con evidencia si las dos investigaciones «retro» se leen como fiscalización y no como postura |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas y el
> criterio están aquí para eso. **La clasificación de cada pieza es el juicio
> de un solo lector.**

---

## 1. Método

- **robots.txt** de `www.noticiascaracol.com`, descargado el 2026-10-12 antes de cualquier otra petición. Líneas literales que importan:
  - `User-agent: *` · `Allow: /` · `Disallow: /_track` · `Disallow: /pushnotifications/*` · `Disallow: /instant-articles-ads`
  - `User-agent: ChatGPT-user` · `Disallow: /` y `User-agent: GPTBot` · `Disallow: /`
  - `User-agent: bingbot` · `Disallow: /busqueda`
  - Declara `Sitemap: https://www.noticiascaracol.com/sitemap.xml`, entre otros.

  **No excluye a ClaudeBot, Claude-Web ni anthropic-ai, ni a todos los agentes, de ninguna ruta usada.** Los vetos con nombre son para agentes de otra empresa. No se tocó `/busqueda`.
- **User-Agent honesto** en todas las peticiones: `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. Nunca el de un navegador. **Ritmo:** en serie, una sola descarga a la vez en el dominio, con 1,6 s de pausa como mínimo más la latencia del servidor. Unas 350 peticiones, todas con respuesta 200.
- **Fuentes de URL: solo las del propio medio.** `sitemap.xml` es un índice con un sitemap por mes. Se bajaron los 13 de octubre de 2025 a octubre de 2026: **19.291 URL**. Sin buscadores, sin Internet Archive. No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex.
- **Quién es la voz de la casa aquí.** Noticias Caracol **no publica editoriales ni tiene sección de opinión** en el portal. Las notas van firmadas por periodistas de la redacción digital, por «Noticias Caracol» o por la **Unidad Investigativa**. Su titular y su entradilla son voz de la casa cuando la valoración no va entre comillas ni atribuida. **No cuentan** las notas de EFE y AFP ni las que firman a medias con ellas («Nombre | EFE»): son reimpresiones.
- **Filtro sistemático.** De las 19.291 URL se tomaron todas las de `politica` y las de `colombia`, `economia`, `judicial`, `salud`, `mundo`, `noticias`, `informes-especiales`, `los-informantes` y `septimo-dia` cuyo slug contiene `petro`, `espriella`, `abelardo`, `cepeda`, `gobierno`, `casa-de-narino`, `presidente-electo`, `mandatario` o `presidente-de-la-republica`: **1.797 piezas**. Se leyeron los 1.797 slugs, que reproducen el titular. Se descargaron: las **264** cuyo slug lleva un término valorativo (la misma lista que en los otros barridos de esta tanda), **34** escogidas a mano al leer los slugs (perfiles de candidatos, piezas de la Unidad Investigativa, el mensaje del director, la cobertura del vendedor de panela) y 38 más, las primeras de la lista general, que se bajaron antes de pasar al filtro. **336 piezas** en total: 267 antes del 07-08, 55 después y 14 fuera de la ventana. De cada una se leyó titular, entradilla y fecha (JSON-LD) y los primeros párrafos.
- **Clases**: las del barrido de Noticias RCN (D, I, M, F y «leve»; F no suma; «retro» es crítica en voz propia al Gobierno Petro cuando ya no gobierna). Se añade **X**: leída y no clasificable.
- **Descargas y scripts** en la carpeta temporal de la sesión, fuera del repositorio y en carpetas separadas; no se ejecutó nada desde las descargas. No se guarda ni se publica el texto de ninguna pieza.

---

## 2. Piezas clasificadas

Títulos literales del campo `headline`. Fecha de `datePublished`.

### 2.1 Antes del cambio: 2025-10-12 → 2026-08-06 (gobierna Petro)

| # | Fecha | Título literal | URL | Clase | Por qué |
|---|---|---|---|---|---|
| 1 | 2026-05-29 | Memoria y política: él es Iván Cepeda, el senador que busca llegar a la Casa de Nariño | [enlace](https://www.noticiascaracol.com/politica/elecciones-colombia/memoria-y-politica-el-es-ivan-cepeda-el-senador-que-busca-llegar-a-la-casa-de-narino-rg10) | **I leve** | Perfil firmado «Noticias Caracol». Entradilla en voz propia: «ha sido un férreo defensor de derechos humanos». Los del candidato de derecha (§2.3) son neutros |
| 2 | 2026-04-16 | El mensaje del director de Noticias Caracol al inicio del debate Colombia Decide su Energía | [enlace](https://www.noticiascaracol.com/politica/elecciones-colombia/el-mensaje-del-director-de-noticias-caracol-al-inicio-del-debate-colombia-decide-su-energia-rg10) | M | El director, Juan Roberto Vargas, reprocha la ausencia **de los dos** punteros, Cepeda y De la Espriella, con la misma fórmula: «Asistir no es un favor a este medio, es un deber con la ciudadanía». No suma |

**Fiscalización del Gobierno Petro mientras gobierna (F: se declara, no suma).** Son de la Unidad Investigativa y son de fondo:

| Fecha | Título literal | URL |
|---|---|---|
| 2025-11-23 | Los archivos secretos de alias Calarcá | [enlace](https://www.noticiascaracol.com/informes-especiales/archivos-secretos-de-calarca-la-charla-con-mordisco-y-senalamientos-a-campana-petro-presidente-ex40) |
| 2025-11-24 | ¿Cómo fue la supuesta infiltración de disidentes con general de Ejército y alto funcionario de DNI? | [enlace](https://www.noticiascaracol.com/informes-especiales/como-fue-la-supuesta-infiltracion-de-disidentes-con-general-de-ejercito-y-alto-funcionario-de-dni-ex40) |
| 2025-11-30 | Noticias Caracol responde a las dudas que ha sembrado Petro frente a los archivos de Calarcá | [enlace](https://www.noticiascaracol.com/informes-especiales/noticias-caracol-responde-a-las-dudas-que-ha-sembrado-petro-frente-a-los-archivos-de-calarca-rg10) |
| 2025-12-08 | Nuevas revelaciones de archivos "Calarcá": sus acciones criminales durante diálogos con el Gobierno | [enlace](https://www.noticiascaracol.com/informes-especiales/nuevas-revelaciones-archivos-de-calarca-acciones-criminales-durante-dia-con-gobierno-petro-rg10) |
| 2026-04-05 | Exclusivo: los contactos secretos entre la DNI, emisarios del Gobierno Petro y ‘Papá Pitufo' | [enlace](https://www.noticiascaracol.com/informes-especiales/exclusivo-los-contactos-secretos-entre-la-dni-emisarios-del-gobierno-petro-y-papa-pitufo-rg10) |
| 2026-06-24 | Secretos de negociación con Clan del Golfo: Gobierno prometió sacar oficiales y frenar bombardeos | [enlace](https://www.noticiascaracol.com/informes-especiales/secretos-de-negociacion-con-clan-del-golfo-gobierno-prometio-sacar-oficiales-y-frenar-bombardeos-rg10) |

No se encontró en lo leído ninguna pieza que elogie en voz propia al Gobierno Petro ni ninguna que pida el voto por un candidato.

### 2.2 Después del cambio: 2026-08-07 → 2026-10-12 (gobierna De la Espriella)

| # | Fecha | Título literal | URL | Clase | Por qué |
|---|---|---|---|---|---|
| 3 | 2026-09-06 | Los golpes de De la Espriella en su ofensiva contra grupos armados y sus objetivos de alto valor | [enlace](https://www.noticiascaracol.com/politica/los-golpes-de-de-la-espriella-en-su-ofensiva-contra-grupos-armados-y-sus-objetivos-de-alto-valor-rg10) | D leve | Balance propio que atribuye los «golpes» al presidente; el cuerpo da también el dato de tres menores muertos en una operación |
| 4 | 2026-08-23 | Los secretos del expediente contra un exedecán de Presidencia señalado de acosar a una mayor | [enlace](https://www.noticiascaracol.com/informes-especiales/los-secretos-del-expediente-contra-el-teniente-coronel-sammy-rodriguez-exedecan-de-presidencia-senalado-de-acoso-sexual-rg10) | D retro leve | Unidad Investigativa, sobre un exedecán del Gobierno Petro. Es una investigación propia, del tipo que el barrido de RCN contó como «retro» |
| 5 | 2026-08-30 | Los vínculos secretos de esmeralderos asesinados con algunos altos funcionarios del gobierno Petro | [enlace](https://www.noticiascaracol.com/informes-especiales/los-vinculos-secretos-de-esmeralderos-asesinados-con-algunos-altos-funcionarios-del-gobierno-petro-rg10) | D retro leve | Ídem, sobre funcionarios del Gobierno saliente |

**Fiscalización del Gobierno De la Espriella (F: se declara, no suma):**

| Fecha | Título literal | URL | Por qué |
|---|---|---|---|
| 2026-08-18 | Minvivienda se disculpa tras polémica por viaje a Santa Marta en medio de emergencia por terremoto | [enlace](https://www.noticiascaracol.com/politica/minvivienda-se-disculpa-tras-polemica-por-viaje-a-santa-marta-en-medio-de-emergencia-por-terremoto-rg10) | Leve. «Polémica», en voz propia, sobre un ministro del nuevo Gobierno |
| 2026-08-26 | ¿Por qué borrador de decreto de Mineducación genera polémica y qué habla sobre las iglesias? | [enlace](https://www.noticiascaracol.com/politica/por-que-borrador-de-decreto-de-mineducacion-genera-polemica-y-que-habla-sobre-las-iglesias-rg10) | Leve. El encuadre es del titular; la crítica de fondo es de un experto y de Fecode |

### 2.3 Leídas y no clasificadas (se declaran)

- **Perfiles neutros del candidato y presidente De la Espriella**: «Abelardo de la Espriella, el "outsider" que quiere llegar a la Presidencia de Colombia» (28-05), «La historia de Abelardo de la Espriella, ganador de segunda vuelta y presidente electo de Colombia» (21-06, con material de agencia). El perfil de José Manuel Restrepo (10-03), con una entradilla elogiosa («se caracterizó por el rigor en el manejo de las finanzas públicas»), va firmado a medias con EFE y su cuerpo es de agencia: **no cuenta**. Tampoco «Él es Abelardo de la Espriella, el abogado penalista que llega a la Presidencia» (06-08, EFE).
- **La cobertura del vendedor de panela** invitado a la posesión (06-08 EFE; 07-08 y 09-08, redacción): historia humana amable con el presidente, sin término valorativo en el titular. Se declara como tono; no cuenta.
- **Atribuidas, en los dos sentidos.** Contra el entrante: la Defensora sobre el arma del presidente (24-09) y sobre la exhibición de cuerpos (07-09), las críticas a Minvivienda (17-08). Contra el saliente: «Cuestionan al presidente Petro por reiterados mensajes en redes sobre resultados de elecciones» (02-06, «algunos analistas»), el ministro de Hacienda y su «presupuesto de la mentira» (14-09), y decenas de reacciones de alcaldes, gremios y candidatos.
- **«Álvaro Uribe se 'quemó'»** (08-03): rótulo en voz propia, pero sobre un expresidente que no era candidato presidencial. No cuenta.
- **Lo que no se leyó y pesa**: la emisión de televisión, que es el producto principal y el de más audiencia del país (42 % semanal fuera de internet, según la ficha). Este barrido es del portal.

**Un hallazgo para la ficha, de paso.** La refutación 6 pedía confirmar quién dirige hoy el noticiero. Las piezas del portal de 2026 lo nombran como director en ejercicio: «el director de Noticias Caracol, Juan Roberto Vargas» (16-04-2026 y 16-09-2026). No se cambia la ficha desde aquí.

---

## 3. Números

| | D | I | M | Con postura | F (no suma) |
|---|---|---|---|---|---|
| Antes del 07-08-2026 (10 meses; 267 piezas leídas) | **0** | **1** (leve) | 1 | 1 | 6 contra Petro (Unidad Investigativa), de fondo |
| Desde el 07-08-2026 (2 meses; 55 piezas leídas) | **3** (leves; 2 retro) | **0** | 0 | 3 | 2 contra De la Espriella, leves |
| **Total** | **3** | **1** | 1 | **4** | |

**Proporción principal: 3 a 1.**

| Lectura | D | I | Proporción | ¿≥10 con postura? | ¿≥3 F o postura a cada lado? | Rama |
|---|---|---|---|---|---|---|
| Principal (las retro como D, como en RCN) | 3 | 1 | **3 : 1** | No (4) | Sí (antes 7; después 5) | La postura no queda «por debajo de 3 a 1», así que no es la del 0,00; tampoco va «en un solo sentido». Con 4 piezas, **no hay suficientes para juzgar → «sin medir»** |
| Sin las retro (las dos investigaciones como F del saliente) | 1 | 1 | 1 : 1 | No (2) | Sí (antes 7; después 3: 1 D y 2 F) | **0,00 con evidencia** |
| Sin ninguna «leve» | 0 | 0 | — | No | — | «sin medir» |

**El trato a quien gobierna (polo fijo).** A Petro, la casa lo fiscalizó con su Unidad Investigativa: seis piezas de fondo en diez meses (0,6 al mes). A De la Espriella, con dos titulares leves en dos meses (1 al mes). **Por número, el ritmo es parecido; por profundidad, no**: lo que el Gobierno Petro recibió fueron investigaciones propias con documentos; lo que recibe el entrante, de momento, es la palabra «polémica» en dos titulares. Después del cambio, la Unidad Investigativa siguió investigando **al Gobierno saliente** (n.º 4 y 5) y no se encontró una pieza suya sobre el entrante. Es un dato a vigilar, no una postura: F no cuenta.

---

## 4. Contrapesos (lo que contradice la dirección, y cuánto pesa)

| Contrapeso | Piezas | Peso |
|---|---|---|
| **El director trata igual a los dos punteros** cuando no asisten a su debate | n.º 2 | **Medio.** Es la única pieza en la voz literal del director, y es simétrica |
| **Perfil favorable del candidato de izquierda** frente a perfiles neutros del de derecha | n.º 1 | **Bajo.** Una entradilla |
| **Sin endoso.** Ninguna pieza de la casa pide el voto | — | **Alto para la magnitud** |
| **Densidad casi nula.** 4 piezas con postura entre 336 leídas (1 %) y 1.797 titulares | §1 | **Alto: es la razón del «sin medir»** |
| **La Unidad Investigativa siguió con el Gobierno saliente** y no se encontró que investigue al entrante | n.º 4, 5; §3 | **Empuja hacia D**, pero es fiscalización y el lado posterior es de dos meses |

---

## 5. Veredicto por condición

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | **Sí, en titulares y entradillas** | No hay editoriales ni opinión en el portal; la emisión no se leyó |
| 2. A los dos lados del cambio, en 12 meses | **Apenas** | 1 pieza con postura antes y 3 después |
| 3a. ≥10 piezas con postura | **No** | 4 |
| 3b. ≥3 a cada lado del cambio | **No** | Antes, ninguna en la dirección D |
| 3c. Proporción ≥3:1 | Exactamente 3:1, sobre 4 piezas | No significa nada con esa base |
| 4. Contrapesos escritos | **Sí** | §4 |
| 5. Reproducible | **Sí** | §2 y §1 |

**No cumple las cinco condiciones.**

---

## 6. Rama de la precisión del 2026-10-10 y valor que resultaría

**El valor vigente se apoya solo en los niveles 4 y 5** (cabecera), así que el barrido manda aunque no llegue.

**Rama: «no llega y no hay piezas suficientes a cada lado para juzgar» → «sin medir»** (`bias: null`).

**Valor propuesto: «sin medir»** (antes +0,10). La ficha ya decía que el +0,10 «no tiene ninguna evidencia propia detrás»; el barrido no se la da en ningún sentido: el portal del noticiero más visto del país apenas toma postura en voz propia.

**Lectura alternativa, declarada: 0,00 con evidencia**, si el responsable editorial lee las dos investigaciones de agosto sobre funcionarios del Gobierno Petro como fiscalización (lo que son por método: documentos propios sobre personas que tuvieron poder) y no como postura «retro». Entonces la postura queda en 1 a 1, hay al menos 3 piezas de fiscalización o postura a cada lado (7 antes; 3 después) y se cumple la rama de la misma conducta. **Quien firme esa lectura debería aplicarla también a las piezas «retro» de otros barridos** (Noticias RCN contó la suya, n.º 24, como D).

**Por qué no se queda en +0,10:** no hay una sola pieza que lo sostenga; la frase que lo justificaba describe temario.

**La pregunta de la misma sociedad.** La ficha consideraba indefendible que dos productos de Caracol Televisión S.A. estuvieran a 0,15 sin conducta medida. Con este barrido y el de Blu Radio (`revision-externa/barridos/blu-radio.md`, que propone 0,00 con evidencia y, como alternativa, «sin medir»), **la diferencia desaparece en cualquiera de las combinaciones**: los dos medios quedarían en 0,00 o fuera de la escala, nunca en dos puntos distintos de ella. El tercer medio del holding, El Espectador, está en 0,00.

**Vecinos:** Noticias RCN (+0,15), el otro noticiero privado, tiene 22 a 4 en su portal y cumple los mínimos; este portal no se le parece. W Radio (0,00), El Tiempo (+0,05) y Pulzo (0,00), los otros medios de gran alcance sin barrido que los mueva, están en el centro.

**Qué lo refutaría:**
- hacia cualquier lado: una lectura de la emisión, que es donde el medio tiene su audiencia;
- hacia la derecha: que la Unidad Investigativa siga sin ocuparse del Gobierno De la Espriella mientras el portal adopta en sus titulares los balances del Ejecutivo, hasta sumar piezas con postura;
- hacia el centro con evidencia: que aparezcan investigaciones propias sobre el Gobierno entrante comparables a las de Calarcá o Papá Pitufo.

---

## 7. Cobertura, huecos y avisos

- **Lo que no se leyó.** La emisión (§2.3). De los 1.797 titulares se leyó el slug; el titular literal, la entradilla y el cuerpo, solo de las 336 piezas descargadas. Una nota con postura en la entradilla y un slug neutro se escapa.
- **El lado posterior es corto**: dos meses y 55 piezas leídas.
- **Robots y red.** El robots.txt no excluyó nada de lo usado. Todas las respuestas fueron 200 y no se reintentó nada.
- **Una sola lectura**, de la misma casa que el autor de la ficha.
- **Datos personales.** No se copia ningún número de documento, teléfono ni dirección. Las personas nombradas son cargos públicos, candidatos o periodistas en su función. El vendedor de panela no se nombra.
