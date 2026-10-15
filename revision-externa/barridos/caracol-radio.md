# Barrido editorial: Caracol Radio

| | |
|---|---|
| **Medio** | Caracol Radio (`caracol-radio`), cadena radial de Prisa Media. **Desde el 13-01-2026 integra a W Radio** en una sola cadena (sistema 6AM/W, dirección editorial de Roberto Pombo, servicio informativo de Orlando Villar). Portal: caracol.com.co. **No tiene relación de propiedad con Noticias Caracol** |
| **Valor vigente** | **+0,05**, firmado en bloque el 2026-10-10 (`reviewedAt: '2026-10-10'`). Su razón escrita no dice nada de la línea: «Radio informativa de cobertura nacional con agenda noticiosa amplia». La ficha lo resume así: «no es que esté mal fundado, es que no está fundado en absoluto». La propiedad (nivel 1, Prisa / Amber Capital) no da una posición política conocida en Colombia. Es decir: **el valor se apoya solo en los niveles 4 y 5**, y por la precisión del 2026-10-10 el barrido manda |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con la regla del polo fijo y las precisiones del 2026-10-09 y del 2026-10-10 |
| **Ventana** | 2025-10-12 → 2026-10-12 (regla del presente). Cruza la fusión con W del 13-01-2026: los primeros tres meses son de Caracol Radio sola |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-12. Es de la misma casa que el autor de la ficha y de los otros barridos: su acuerdo no es aval |
| **Estado** | **FIRMADO el 2026-10-12: 0,00 con evidencia** (antes +0,05), como se propuso. Aplicado en el registro, la ficha y el texto público el 2026-10-12 (`DECISIONES.md`, «Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Resultado** | **No cumple los mínimos**, pero documenta **la misma conducta con los dos gobiernos**. 14 piezas con postura en la voz de la casa: **8 D y 6 I (1,3 a 1)**, casi todas leves. Fiscalización en voz propia: 15 piezas contra el Gobierno Petro en diez meses (1,5 al mes) y 4 contra el de De la Espriella en dos (2 al mes). **Rama: 0,00 con evidencia** |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas y el
> criterio están aquí para eso. **La clasificación de cada pieza es el juicio
> de un solo lector.**

---

## 1. Método

- **robots.txt** de `caracol.com.co`, descargado el 2026-10-12 antes de cualquier otra petición. Líneas literales que importan:
  - `User-agent: PetalBot` · `Disallow: /` (el único agente con veto total).
  - `User-Agent: *` con `Disallow` en recursos y rutas técnicas (`/pf/`, `/images/`, `/embed/`, `/audio/`, `/tag//*`, `/m/`, etc.) y en el buscador: `Disallow: /buscar/` · `Disallow: /buscador/` · `Disallow: /search-audios/`.
  - Declara seis `Sitemap`, entre ellos `https://caracol.com.co/arc/outboundfeeds/news-sitemap-index/?outputType=xml` y `https://caracol.com.co/arc/outboundfeeds/news-sitemap/2022-09-27/?outputType=xml` (la forma por día).

  **No excluye a ClaudeBot, Claude-Web ni anthropic-ai, ni a todos los agentes, de ninguna ruta usada** (`/arc/outboundfeeds/news-sitemap/…` y las notas `/AAAA/MM/DD/…`). No se tocaron el buscador ni el audio.
- **User-Agent honesto** en todas las peticiones: `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. Nunca el de un navegador. **Ritmo:** en serie, una sola descarga a la vez en el dominio, con 1,6 s de pausa como mínimo más la latencia del servidor (unos 2,3 s por sitemap diario). Unas 460 peticiones.
- **Fuentes de URL: solo las del propio medio.** El gestor (Arc) sirve un sitemap de noticias por día, con el **título literal** de cada pieza (`news:title`) y su fecha. Se pidieron los 366 días de la ventana: **347 respondieron 200 y 19 devolvieron 504** dos veces, en dos pasadas separadas por horas (15, 20 y 21 de enero; 2 a 6 y 9 a 11 de febrero; 9 y 27 a 31 de julio; 10 y 11 de agosto de 2026). Resultado: **69.904 titulares** en la ventana. Sin buscadores, sin Internet Archive. No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex.
- **Quién es la voz de la casa aquí.** Caracol Radio **no publica editoriales en el portal**. Las notas van firmadas por periodistas o por «Caracol Radio»; su titular y su entradilla son voz de la casa cuando la valoración no va entre comillas ni atribuida. El director editorial tiene un espacio propio en el portal, «Mis Preguntas, con Roberto Pombo»: se leyeron sus 12 entregas sobre política; son entrevistas a invitados con una presentación neutra, y ninguna toma partido (§2.3). Las columnas firmadas por terceros y las notas de agencia **no cuentan**.
- **Filtro sistemático por términos, sobre el título literal.** De los 69.904 titulares se tomaron los que nombran a `Petro`, `Espriella`, `Abelardo`, `Cepeda`, `Gobierno`, `presidente electo`, `Casa de Nariño`, `mandatario` o `paz total`: **5.346**. De esos, los que llevan un término valorativo **fuera de las comillas** (polémica, escándalo, golpe, histórico, éxito, fracaso, crisis, crítica, derrota, victoria, herencia, balance, tigre, mano dura, reversazo, desplante, etc.): **736**, que se leyeron uno por uno. Se descargaron las **54** con postura posible o dudosa, más las entregas políticas de «Mis Preguntas», para leer entradilla y primeros párrafos.
- **Clases**: las del barrido de Noticias RCN (D, I, M, F y «leve»; F no suma; «retro» es crítica en voz propia al Gobierno Petro cuando ya no gobierna).
- **Descargas y scripts** en la carpeta temporal de la sesión, fuera del repositorio y en carpetas separadas; no se ejecutó nada desde las descargas. No se guarda ni se publica el texto de ninguna pieza.

---

## 2. Piezas clasificadas

Títulos literales (`headline` del JSON-LD, que coincide con el `news:title`). Fecha de `datePublished`.

### 2.1 Antes del cambio: 2025-10-12 → 2026-08-06 (gobierna Petro)

| # | Fecha | Título literal | URL | Clase | Por qué |
|---|---|---|---|---|---|
| 1 | 2025-12-10 | Elecciones 2026: La reunión de Iván Cepeda con empresarios que generó cuestionamientos y sinsabores | [enlace](https://caracol.com.co/2025/12/10/elecciones-2026-la-reunion-de-ivan-cepeda-con-empresarios-que-genero-cuestionamientos-y-sinsabores/) | D leve | En voz propia: «estrategias que no caen muy bien en todos los sectores. Un claro ejemplo de esto es Iván Cepeda» |
| 2 | 2026-01-16 | La polémica por los gastos y aportes de la campaña de la consulta de Iván Cepeda | [enlace](https://caracol.com.co/2026/01/16/la-polemica-por-los-gastos-y-aportes-de-la-campana-de-la-consulta-de-ivan-cepeda/) | D leve | «Polémica», en voz propia; el cuerpo da las cifras del reporte al CNE |
| 3 | 2026-03-15 | Polémica política por declaraciones de Iván Cepeda sobre Antioquia agitó la campaña presidencial | [enlace](https://caracol.com.co/2026/03/15/polemica-politica-por-declaraciones-de-ivan-cepeda-sobre-antioquia-agito-la-campana-presidencial/) | D leve | Titular en voz propia; la entradilla atribuye la crítica a «la centro derecha» |
| 4 | 2026-04-13 | Polémica reacción de Cepeda a fiesta en cárcel de Itagüí: Alejandro Ocampo y Hernán Cadavid debaten | [enlace](https://caracol.com.co/2026/04/13/polemica-reaccion-de-cepeda-a-fiesta-en-carcel-de-itagui-alejandro-ocampo-y-hernan-cadavid-debaten/) | D leve | «Polémica reacción», en voz propia; el formato es un debate con un congresista de cada lado |
| 5 | 2026-06-04 | Caída de la Constituyente: ¿Una realidad o solo promesa de campaña de Iván Cepeda? | [enlace](https://caracol.com.co/2026/06/04/caida-de-la-constituyente-una-realidad-o-solo-promesa-de-campana-de-ivan-cepeda/) | D leve | La duda sobre el candidato de izquierda es del titular |
| 6 | 2026-06-25 | Así nació la estrategia del “tigre” para la campaña presidencial de Abelardo de la Espriella | [enlace](https://caracol.com.co/2026/06/25/asi-nacio-la-estrategia-del-tigre-para-la-campana-presidencial-de-abelardo-de-la-espriella/) | D leve | Entradilla: «Carlos Suárez, estratega detrás del éxito de Abelardo de la Espriella». La misma pieza que Noticias RCN tituló con «genio» y «éxito» (su n.º 9) |
| 7 | 2025-12-29 | ¡Histórico! Salario Mínimo 2026 queda en $2.000.000: Así regirá el pago tras decreto de Petro | [enlace](https://caracol.com.co/2025/12/29/cuando-se-oficializa-el-salario-minimo-2026-en-colombia-fecha-y-hora-del-anuncio-de-petro/) | **I leve** | Elogio en el titular; el cuerpo: «el presidente Gustavo Petro sorprendió al país con un anuncio histórico» |
| 8 | 2026-02-16 | Interpretación de Abelardo de la Espriella en el Conservatorio del Tolima generó polémica | [enlace](https://caracol.com.co/2026/02/16/interpretacion-de-abelardo-de-la-espriella-en-el-conservatorio-del-tolima-genero-polemica/) | **I leve** | «Polémica», en voz propia, sobre el candidato de derecha |
| 9 | 2026-03-11 | Gobierno Nacional lanza histórico plan de $2 billones para reactivar el campo tras la ola invernal | [enlace](https://caracol.com.co/2026/03/11/gobierno-nacional-lanza-historico-plan-de-2-billones-para-reactivar-el-campo-tras-la-ola-invernal/) | **I leve** | «Histórico», en voz propia, sobre un programa del Gobierno Petro |
| 10 | 2026-07-08 | Gobierno entrega una Reforma Agraria con inversión récord de $ 8 billones | [enlace](https://caracol.com.co/2026/07/08/gobierno-entrega-una-reforma-agraria-con-inversion-record-de-8-billones/) | **I leve** | El titular hace suyo el balance de la ministra («récord») |
| 11 | 2026-07-18 | Gobierno aprueba presupuesto histórico para el SENA: aumentará $4,46 billones | [enlace](https://caracol.com.co/2026/07/18/gobierno-aprueba-presupuesto-historico-para-el-sena-aumentara-446-billones/) | **I leve** | «Histórico», en voz propia; el dato es del SENA |
| 12 | 2026-08-01 | De la Espriella genera polémica en el Tolima por anuncio sobre eliminación de las APPA | [enlace](https://caracol.com.co/2026/08/01/de-la-espriella-genera-polemica-en-el-tolima-por-anuncio-sobre-eliminacion-de-las-appa/) | **I leve** | «Polémica», en voz propia, sobre el presidente electo; el cuerpo llama también «polémica» a la resolución del Gobierno saliente |

**Mixtas (M, no suman):** «Equipo diplomático secreto del presidente Petro logró acercamiento con gobierno Trump» (09-01-2026; el titular dice «logró» y la entradilla, que el Gobierno «cedió en temas cruciales», [enlace](https://caracol.com.co/2026/01/09/equipo-diplomatico-secreto-del-presidente-petro-logro-acercamiento-con-gobierno-trump/)) y «Cuatro años en ocho indicadores: así deja Gustavo Petro a Colombia frente a la región» (05-08-2026; «mejoró en inflación, desempleo y salario mínimo, pero cayó en inversión extranjera, deuda pública y calificación crediticia», [enlace](https://caracol.com.co/2026/08/05/cuatro-anos-en-ocho-indicadores-asi-deja-gustavo-petro-a-colombia-frente-a-la-region/)).

**Fiscalización del Gobierno Petro mientras gobierna (F: se declara, no suma).** Con la valoración en voz propia; la lista sale del filtro del §1 y no es exhaustiva:

| Fecha | Título literal | URL |
|---|---|---|
| 2025-10-16 | Desplante del Gobierno en Cartagena: ministro de Defensa canceló nuevamente un consejo de seguridad | [enlace](https://caracol.com.co/2025/10/16/desplante-del-gobierno-en-cartagena-ministro-de-defensa-cancelo-nuevamente-un-consejo-de-seguridad/) |
| 2025-11-11 | 7 de 12 funcionarios del gobierno Petro denunciados por acoso o violencia siguen en sus cargos | [enlace](https://caracol.com.co/2025/11/12/funcionarios-del-gob-petro-siete-de-doce-denunciados-por-acoso-o-violencia-siguen-en-sus-cargos/) |
| 2025-11-24 | Escándalo en gobierno Petro: ¿Quién es Wilmar Mejía y por qué lo involucran con las disidencias? | [enlace](https://caracol.com.co/2025/11/24/escandalo-en-gobierno-petro-quien-es-wilmer-mejia-y-por-que-lo-involucran-con-las-disidencias/) |
| 2025-11-25 | Petro mantiene negociaciones con alias “Calarcá”, pese a escándalo con funcionarios y militares | [enlace](https://caracol.com.co/2025/11/25/petro-mantiene-negociaciones-con-alias-calarca-pese-a-escandalo-con-funcionarios-y-militares/) |
| 2025-12-16 | Nuevo golpe al gobierno Petro: Senado hunde la reforma a la salud | [enlace](https://caracol.com.co/2025/12/16/nuevo-golpe-al-gobierno-petro-senado-hunde-la-reforma-a-la-salud/) |
| 2026-01-27 | Jalón de orejas de la Corte Constitucional al gobierno por crisis en el Catatumbo | [enlace](https://caracol.com.co/2026/01/27/jalon-de-orejas-de-la-corte-constitucional-al-gobierno-por-crisis-en-el-catatumbo/) |
| 2026-02-05 | Polémica por preguntas del Gobierno de tarifas de productos: estas son las empresas; responde gremio | [enlace](https://caracol.com.co/2026/02/05/polemica-por-preguntas-del-gobierno-de-tarifas-de-productos-estas-son-las-empresas-responde-gremio/) |
| 2026-02-17 | Polémico nombramiento directivo en la UIAF, poderosa entidad del Gobierno | [enlace](https://caracol.com.co/2026/02/17/polemico-nombramiento-directivo-en-la-uiaf-poderosa-entidad-del-gobierno/) |
| 2026-03-10 | Gobierno baja requisitos para nombrar Superfinanciero, SIC y Sociedades, ¿salvavidas a Rusinque? | [enlace](https://caracol.com.co/2026/03/10/gobierno-baja-requisitos-para-nombrar-superfinanciero-sic-y-sociedades-salvavidas-a-rusinque/) |
| 2026-03-28 | Hija de Petro es nombrada madrina del buque ARC “24 de Julio” y desata polémica | [enlace](https://caracol.com.co/2026/03/28/hija-de-petro-es-nombrada-madrina-del-buque-arc-24-de-julio-y-desata-polemica/) |
| 2026-04-04 | Presidente Petro reaviva choque con el Banco de la República y desata nueva polémica | [enlace](https://caracol.com.co/2026/04/04/presidente-petro-reaviva-choque-con-el-banco-de-la-republica-y-desata-nueva-polemica/) |
| 2026-04-06 | Las seis contradicciones del presidente de Ecopetrol, Ricardo Roa | [enlace](https://caracol.com.co/2026/04/06/las-seis-contradicciones-del-presidente-de-ecopetrol-ricardo-roa/) |
| 2026-04-24 | Tras señalamientos de Angie Rodríguez, Petro pidió reforzar publicidad sobre logros de su Gobierno | [enlace](https://caracol.com.co/2026/04/24/tras-senalamientos-de-angie-rodriguez-petro-pidio-reforzar-publicidad-sobre-logros-de-su-gobierno/) |
| 2026-05-21 | ¿Embajadas son castigo? La lista de funcionarios del gobierno Petro que han llegado tras escándalos | [enlace](https://caracol.com.co/2026/05/21/embajadas-son-castigo-la-lista-de-funcionarios-del-gobierno-petro-que-han-llegado-tras-escandalos/) |
| 2026-06-11 | El fracaso de los aeropuertos del gobierno Petro para la Colombia profunda: ninguno llega al 20% | [enlace](https://caracol.com.co/2026/06/11/el-fracaso-de-los-aeropuertos-del-gobierno-petro-para-la-colombia-profunda-ninguno-llega-al-20/) |

No se encontró en lo leído ninguna pieza de la casa que pida el voto o declare apoyo a un candidato.

### 2.2 Después del cambio: 2026-08-07 → 2026-10-12 (gobierna De la Espriella)

| # | Fecha | Título literal | URL | Clase | Por qué |
|---|---|---|---|---|---|
| 13 | 2026-09-05 | Mi Casa Ya: así golpeó a las familias el fin del programa en el gobierno Petro | [enlace](https://caracol.com.co/2026/09/05/del-sueno-a-la-incertidumbre-asi-golpeo-a-las-familias-el-fin-de-mi-casa-ya-en-el-gobierno-petro/) | D retro | Reportaje propio sobre una decisión del Gobierno saliente («así golpeó») |
| 14 | 2026-09-26 | Gobierno de Colombia en New York logra atraer inversión extranjera: anuncian promoción Milagro Week | [enlace](https://caracol.com.co/2026/09/26/comitiva-colombiana-en-nueva-york-logro-despertar-interes-y-atraer-inversion-extranjera/) | D leve | «Logra», en voz propia, sobre la gira del Gobierno entrante |

**Mixta (M):** «La herencia económica de Petro: lo bueno, lo malo y lo feo que recibe De La Espriella» (07-08-2026; «balance agridulce», con mejores cifras sociales y peor base productiva, [enlace](https://caracol.com.co/2026/08/07/la-herencia-economica-de-petro-lo-bueno-lo-malo-y-lo-feo-que-recibe-de-la-espriella/)).

**Fiscalización del Gobierno De la Espriella (F: se declara, no suma):**

| Fecha | Título literal | URL | Por qué |
|---|---|---|---|
| 2026-08-21 | Nueva derrota de coalición de Gobierno: oposición logró mayorías en Comisión Sexta del Senado | [enlace](https://caracol.com.co/2026/08/21/nueva-derrota-del-gobierno-en-el-congreso-oposicion-logro-mayorias-en-comision-sexta-del-senado/) | Leve. En voz propia: «las mayorías del presidente Abelardo de la Espriella tambalean en el Congreso» |
| 2026-08-27 | Siete ciclos para lograr la ‘Patria Milagro’ de De la Espriella: estos son los puntos polémicos | [enlace](https://caracol.com.co/2026/08/27/siete-ciclos-para-lograr-la-patria-milagro-de-de-la-espriella-estos-son-los-puntos-polemicos/) | Primicia propia: un documento reservado de Planeación, con la prohibición de adopción a parejas del mismo sexo entre las prioridades |
| 2026-08-31 | Gobierno de la Espriella reversó multas contra la polémica empresa Charry Trading de Ibagué | [enlace](https://caracol.com.co/2026/08/31/gobierno-de-la-espriella-reverso-multas-contra-la-polemica-empresa-charry-trading-de-ibague/) | En voz propia: el Ministerio del Trabajo «tomó la polémica decisión de reversar parcialmente las multas» |
| 2026-10-01 | “Es desconcertante”, ex viceministro de Minas sobre reversazo del Gobierno por precio de la gasolina | [enlace](https://caracol.com.co/2026/10/01/es-desconcertante-ex-viceministro-de-minas-sobre-reversazo-del-gobierno-por-precio-de-la-gasolina/) | Leve. «Reversazo» es de la casa; la crítica, del entrevistado |

### 2.3 Leídas y no clasificadas (se declaran)

- **«Mis Preguntas, con Roberto Pombo».** Las 12 entregas políticas de la ventana (por ejemplo, «¿Tiene ganada la izquierda las elecciones?», 07-12-2025; «¿Qué retos de gobernabilidad tendría cada candidato presidencial?», 24-05-2026; «¿Cuál ha sido la relación entre gremios y gobiernos en Colombia?», 11-10-2026) son programas de entrevistas: la página presenta la pregunta y a los invitados, sin postura de la casa. Tampoco toma partido «Gobierno entrante debe poner sus antenas en la gente que perdió: Roberto Pombo en Los Protagonistas» (28-06-2026), una reflexión sobre el periodismo y la polarización.
- **Datos electorales con adjetivo factual**: «obtuvo una victoria contundente en todo el Huila» (01-06; ganó los 37 municipios) y «consigue históricos de votación en Medellín y Antioquia» (21-06; es un récord verificable). No cuentan.
- **Cifras oficiales sin adjetivo**: «Gobierno ha firmado 70 extradiciones en 32 días» (09-09), con la frase del presidente entre comillas. No cuenta (Noticias RCN contó una pieza parecida porque su titular decía «en tan solo»).
- **Atribuidas, en los dos sentidos**, que son la gran mayoría de los 736 titulares leídos: gobernadores, alcaldes, gremios, expresidentes, candidatos y congresistas contra el Gobierno Petro; la Defensora, el Pacto Histórico, el uribismo y analistas contra el de De la Espriella; felicitaciones y respaldos al entrante.
- **Lo que no se leyó y pesa**: la emisión. 6AM W, Hoy por Hoy, La Luciérnaga y Hora 20 son programas hablados; el portal publica notas de ellos («habló en 6AM W…»), y esas notas sí están en el corpus, pero la conversación al aire no.
- **W Radio** sigue teniendo dominio propio (wradio.com.co, robots.txt sin veto para nosotros) y entrada propia en el catálogo (`w-radio`, 0,00). No se barrió aquí: no es el medio de este encargo.

---

## 3. Números

| | D | I | M | Con postura | F (no suma) |
|---|---|---|---|---|---|
| Antes del 07-08-2026 (10 meses; 610 de los 736 titulares filtrados) | **6** (leves) | **6** (leves) | 2 | 12 | 15 contra Petro |
| Desde el 07-08-2026 (2 meses; 126 titulares filtrados) | **2** (1 retro plena, 1 leve) | **0** | 1 | 2 | 4 contra De la Espriella |
| **Total** | **8** | **6** | 3 | **14** | |

**Proporción principal: 8 a 6, es decir, 1,3 a 1.**

| Lectura | D | I | Proporción | ¿≥10 con postura? | ¿≥3 por lado en la dirección D? | ¿≥3 F o postura a cada lado? | Rama |
|---|---|---|---|---|---|---|---|
| Principal | 8 | 6 | **1,3 : 1** | Sí (14) | No (después, 1 elogio y 1 retro) | **Sí** (antes 27; después 6) | **0,00 con evidencia** |
| Sin la retro | 7 | 6 | 1,2 : 1 | Sí (13) | No | Sí (después 5) | 0,00 con evidencia |
| Sin ninguna «leve» | 1 | 0 | — | No | No | Sí, contando F | «sin medir» |

**El trato a quien gobierna (polo fijo).** Con la vara de la voz propia en el titular o la entradilla, la casa fiscalizó al Gobierno Petro **15 veces en 10 meses (1,5 al mes)** y al de De la Espriella **4 veces en 2 meses (2 al mes)**, incluida una primicia con un documento reservado. Elogió en voz propia al Gobierno Petro cuatro veces («histórico», «récord») y al de De la Espriella una («logra»). Encuadró al candidato de izquierda cinco veces con la palabra «polémica» o una duda en el titular, y al de derecha dos veces con la misma palabra. **Es la misma conducta con los dos gobiernos**, que es lo que la rama del 0,00 pide.

---

## 4. Contrapesos (lo que contradice el 0,00, y cuánto pesa)

| Contrapeso | Piezas | Peso |
|---|---|---|
| **Más «polémicas» para Cepeda (5) que para De la Espriella (2) en campaña** | n.º 1-5, 8, 12 | **Bajo-medio.** Empuja hacia D; queda compensado por los elogios al Gobierno Petro |
| **Los elogios al Gobierno Petro adoptan cifras oficiales** («récord», «histórico») | n.º 7, 9-11 | **Bajo.** Pueden ser comunicados de prensa con titular amable más que postura: si se descuentan, la proporción pasa a 8 a 2, pero con piezas leves y sin llegar a los mínimos del lado posterior |
| **Sin endoso** | — | **Alto para la magnitud** |
| **Densidad baja.** 14 piezas con postura entre 736 titulares filtrados y 69.904 en la ventana | §1 | **Alto para la magnitud** |
| **19 días sin sitemap** (504 del servidor) | §1 | **Bajo.** El 5 % de la ventana; no se concentra en un lado del cambio |

---

## 5. Veredicto por condición

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | **Sí, en titulares y entradillas** | No hay editoriales en el portal; el espacio del director editorial son entrevistas; la emisión no se leyó |
| 2. A los dos lados del cambio, en 12 meses | **Sí** | 12 piezas con postura antes y 2 después, más 15 y 4 de fiscalización |
| 3a. ≥10 piezas con postura | **Sí** | 14 |
| 3b. ≥3 a cada lado del cambio, en la misma dirección | **No** | Después del cambio, 1 elogio y 1 retro |
| 3c. Proporción ≥3:1 | **No** | 1,3:1 |
| 4. Contrapesos escritos | **Sí** | §4 |
| 5. Reproducible | **Sí** | §2, con fecha, título literal, URL y clase; §1, con el filtro exacto |

**No cumple las cinco condiciones** (fallan 3b y 3c).

---

## 6. Rama de la precisión del 2026-10-10 y valor que resultaría

**El valor vigente se apoya solo en los niveles 4 y 5** (cabecera), así que el barrido manda aunque no llegue.

**Rama: «no llega, pero documenta la misma conducta con los dos gobiernos» → 0,00 con evidencia.** Hay al menos 3 piezas de fiscalización o postura a cada lado (27 antes; 6 después), la postura está en 1,3 a 1 y la fiscalización en voz propia tiene un ritmo parecido con los dos gobiernos.

**Valor propuesto: 0,00 con evidencia** (antes +0,05). Es la rama más sólida de los tres barridos de esta tanda: se sostiene sin la pieza retro y no depende de una sola sección.

**Por qué no se queda en +0,05:** el +0,05 no tenía detrás ninguna afirmación sobre la línea; con evidencia, la conducta documentada es simétrica, y entre +0,05 y 0,00 la regla 2 manda la más cercana a la mixta.

**Lectura alternativa:** no se ve una defendible distinta de «sin medir», y solo si se descuentan todas las leves, lo que dejaría el barrido sin base en los dos sentidos.

**Vecinos:**
- **W Radio (0,00)**, de la misma casa y hoy de la misma cadena: misma posición. El catálogo sigue con dos entradas para un solo medio (refutación 2 de la ficha, decisión pendiente del responsable editorial); con este barrido, al menos, las dos estarían en el mismo número;
- **El Tiempo (+0,05)** y **Pulzo (0,00)**, los otros medios generalistas de gran alcance sin barrido que los mueva;
- **La FM (+0,25)**, la radio hablada con la que más se la compara: llegó a su número con un editorial diario firmado por su director que cumple los mínimos; Caracol Radio no tiene nada parecido en el portal;
- **Blu Radio**: su barrido propone también 0,00 con evidencia.

**Qué lo refutaría:**
- que la fiscalización en voz propia del Gobierno De la Espriella se apague mientras siguen los elogios («logra») y las piezas retro, hasta pasar los mínimos;
- una lectura de 6AM W ponderada por audiencia, que es lo que la refutación 4 de la ficha pide y lo que un portal no puede sustituir.

---

## 7. Cobertura, huecos y avisos

- **Lo que no se leyó.** La emisión (§2.3). Los titulares que no nombran al Gobierno ni a los candidatos con los términos del §1, y los que los nombran sin un término valorativo fuera de comillas. De los 736 leídos, se abrió la pieza de 54.
- **19 días sin sitemap** (§1), tras dos intentos separados por horas.
- **Fechas.** El filtro del §1 usa la fecha del sitemap (UTC); la clasificación, la `datePublished` de cada pieza (hora de Colombia). Una pieza de la noche del 06-08 puede figurar en el sitemap del 07-08; ninguna de las clasificadas está en ese borde.
- **La ventana cruza la fusión con W** (13-01-2026): las piezas de octubre a enero son de Caracol Radio sola. Dos de las 14 piezas con postura (n.º 1 y 7) y 5 de las 15 fiscalizaciones del Gobierno Petro son anteriores a la fusión; el resultado no cambia de rama si se quitan.
- **Robots y red.** El robots.txt no excluyó nada de lo usado. Todas las notas respondieron 200; los únicos errores fueron los 504 de los sitemaps del §1.
- **Una sola lectura**, de la misma casa que el autor de la ficha. Las piezas límite van marcadas «leve» y el §3 da el recuento con y sin ellas.
- **Datos personales.** No se copia ningún número de documento, teléfono ni dirección. Las personas nombradas son cargos públicos, candidatos o periodistas en su función.
