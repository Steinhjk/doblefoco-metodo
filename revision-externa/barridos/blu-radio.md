# Barrido editorial: Blu Radio

| | |
|---|---|
| **Medio** | Blu Radio (`blu-radio`), cadena radial informativa de Caracol Televisión S.A. (la misma sociedad que produce Noticias Caracol; Valorem 93,5 %). Portal: bluradio.com |
| **Valor vigente** | **+0,25**, firmado en bloque el 2026-10-10 (`reviewedAt: '2026-10-10'`). Su razón escrita es una frase de temario, no de línea: «Radio informativa con énfasis en seguridad y orden público». La propiedad (nivel 1) no da una posición política conocida. El nivel 5 de la ficha tiene tres hechos: la intervención del MinTrabajo (no dice nada del eje), las encuestas Invamer conjuntas con Noticias Caracol (tampoco) y la frase al aire del director de Mañanas Blu del 13-08-2026, que critica la respuesta **del Gobierno De la Espriella** al terremoto (es fiscalización del Gobierno entrante, no evidencia de derecha). Es decir: **el valor se apoya solo en los niveles 4 y 5**, y por la precisión del 2026-10-10 el barrido manda |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con la regla del polo fijo y las precisiones del 2026-10-09 y del 2026-10-10 |
| **Ventana** | 2025-10-12 → 2026-10-12 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-12. Es de la misma casa que el autor de la ficha y de los otros barridos: su acuerdo no es aval |
| **Estado** | **FIRMADO el 2026-10-12: 0,00 con evidencia** (antes +0,25), como se propuso; se descarta la alternativa «sin medir». Aplicado en el registro, la ficha y el texto público el 2026-10-12 (`DECISIONES.md`, «Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Resultado** | **No cumple los mínimos.** 15 piezas con postura en la voz de la casa: **10 D y 5 I (2 a 1)**, más 1 F del Gobierno entrante. Antes del cambio, 7 D y 5 I; después, 3 D (dos de ellas «retro») y 0 I. Hay al menos 3 piezas de fiscalización o postura a cada lado y la postura queda por debajo de 3 a 1: **rama «misma conducta» → 0,00 con evidencia**, por poco y con piezas leves. Alternativa: «sin medir» |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas y el
> criterio están aquí para eso. **La clasificación de cada pieza es el juicio
> de un solo lector.**

---

## 1. Método

- **robots.txt** de `www.bluradio.com`, descargado el 2026-10-12 antes de cualquier otra petición. Líneas literales que importan:
  - `User-agent: *` · `Disallow: /_track` · `Disallow: /pushnotifications/*` · `Disallow: /instant-articles-ads`
  - `User-agent: ChatGPT-user` · `Disallow: /` y `User-agent: GPTBot` · `Disallow: /`
  - `User-agent: bingbot` · `Disallow: /busqueda`
  - Declara `Sitemap: https://www.bluradio.com/sitemap.xml`, entre otros.

  **No excluye a ClaudeBot, Claude-Web ni anthropic-ai, ni a todos los agentes, de ninguna ruta usada.** Los vetos con nombre son para agentes de otra empresa, que no son el nuestro. No se tocó `/busqueda`.
- **User-Agent honesto** en todas las peticiones: `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. Nunca el de un navegador. **Ritmo:** en serie, una sola descarga a la vez en el dominio, con 1,6 s de pausa como mínimo más la latencia del servidor (entre 3 y 5 s por pieza). Unas 850 peticiones, todas con respuesta 200.
- **Fuentes de URL: solo las del propio medio.** `sitemap.xml` es un índice con un sitemap por mes (`sitemap-AAAAMM.xml`). Se bajaron los 13 de octubre de 2025 a octubre de 2026: **48.604 URL**. Sin buscadores, sin Internet Archive. No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex.
- **Quién es la voz de la casa aquí.** Blu Radio **no publica editoriales sin firma**. Su sección `/opinion/` (156 piezas en los sitemaps, 149 dentro de la ventana) mezcla cuatro cosas, que se leyeron todas:
  - **111 análisis de Ricardo Ospina, «director del servicio informativo de Blu Radio»** (así lo firma el JSON-LD). Es el director de la sala de noticias escribiendo en el espacio de opinión del medio: **cuentan como voz de la casa**, igual que la «Carta del director» de La FM. Hay una pieza más suya en `/nacion/` (15-12-2025). **La serie se interrumpe el 26-08-2026**: después del cambio de gobierno solo hay 5.
  - 2 piezas de Camila Zuluaga, conductora de Mañanas Blu 10:30 («Editorial» sobre acoso en Caracol, 24-03; «Reflexión pública» sobre su entrevista a la directora de Planeación, 02-02). Voz de la casa; ninguna toma partido en el eje.
  - 32 reflexiones de Alberto Linero (autoayuda y espiritualidad) y 2 más en la misma línea firmadas «Redacción BLU Radio»: no tratan del Gobierno ni de las candidaturas.
  - 1 reimpresión de un editorial de El Espectador (30-01-2026). **No cuenta** (condición 1).
- **Titulares y entradillas de la redacción.** Las notas van firmadas por periodistas de planta o por «Redacción BLU Radio». Su titular y su entradilla son voz de la casa cuando la valoración no va entre comillas ni atribuida a una fuente. **No cuentan** las notas de EFE y AFP (reimpresiones) ni las firmadas «Redacción comercial» (contenido pagado; hay dos del Gobierno Petro sobre reparación de víctimas, del 20-02 y el 25-02, que se declaran y no cuentan).
- **Filtro sistemático por términos.** De las 48.604 URL se tomaron las de las secciones `politica`, `nacion`, `economia`, `judicial`, `salud`, `sociedad`, `regiones`, `mundo`, `venezuela`, `noticias` y `el-radar` cuyo slug contiene `petro`, `espriella`, `abelardo`, `cepeda`, `gobierno`, `casa-de-narino`, `presidente-electo`, `mandatario` o `presidente-de-la-republica`: **3.818 piezas** (más las 76 de `/opinion/` que también pasan el filtro y ya se leían completas). El slug de Blu reproduce el titular. Un segundo filtro, sobre esos slugs, tomó los que llevan un término valorativo (polémica, escándalo, golpe, histórico, éxito, fracaso, crisis, crítica, derrota, victoria, herencia, balance, tigre, mano dura, etc.): **678 piezas**, que se descargaron todas (593 antes del 07-08, 63 después y 22 fuera de la ventana). De cada una se leyó titular, entradilla y fecha (`headline`, `description` y `datePublished` del JSON-LD) y los primeros párrafos.
- **Qué se clasificó.** Solo postura **en voz propia** sobre el Gobierno nacional, las candidaturas presidenciales o el presidente (electo o en ejercicio). Las clases son las del barrido de Noticias RCN:
  - **D**: encuadre desfavorable a la candidatura de izquierda o favorable a De la Espriella como candidato o presidente electo; desde el 07-08, elogio o disculpa al Gobierno De la Espriella, o crítica en voz propia al Gobierno Petro ya fuera del poder (**retro**).
  - **I**: lo simétrico, incluido el elogio al Gobierno Petro mientras gobierna.
  - **M**: reparte a los dos lados. No suma.
  - **F**: solo fiscaliza a quien gobierna. No suma (precisión del 2026-10-09), pero se declara y se usa para comparar el trato.
  - **X**: leída y no clasificable (atribuida, de servicio, contenido pagado o reimpresión). Se declara si es relevante.
  - **«leve»**: la postura está en una palabra o en una pregunta del titular, o la entradilla la matiza.
- **Descargas y scripts** en la carpeta temporal de la sesión, fuera del repositorio y en carpetas separadas; no se ejecutó nada desde las descargas. No se guarda ni se publica el texto de ninguna pieza: aquí van titulares literales y fragmentos breves.

---

## 2. Piezas clasificadas

Títulos literales del campo `headline`. Fecha de `datePublished`.

### 2.1 Antes del cambio: 2025-10-12 → 2026-08-06 (gobierna Petro)

| # | Fecha | Título literal | URL | Clase | Por qué |
|---|---|---|---|---|---|
| 1 | 2026-03-16 | Polémica en Antioquia por programa de Iván Cepeda que llamó al departamento cuna de parapolítica | [enlace](https://www.bluradio.com/nacion/elecciones/polemica-en-antioquia-por-programa-de-ivan-cepeda-que-llamo-al-departamento-cuna-de-parapolitica-rg10) | D | Nota de la redacción. En voz propia: «en toda una tormenta polémica se convirtió el ataque contra el departamento de Antioquia, que ha hecho el candidato Iván Cepeda»; «Cepeda reafirmó su ofensiva contra el uribismo» |
| 2 | 2026-05-04 | Presidente Petro no se retirará de política el 7 de agosto; busca sacar adelante una Constituyente | [enlace](https://www.bluradio.com/opinion/presidente-petro-no-se-retirara-de-politica-el-7-de-agosto-busca-sacar-adelante-una-constituyente-pr30) | D leve | Ospina. Sobre todo fiscaliza al presidente, pero añade que «su candidato, Iván Cepeda, no ha tenido la suficiente claridad» |
| 3 | 2026-05-05 | Polémica en Florencia, Caquetá, por valla publicitaria de Iván Cepeda con imagen de Gustavo Petro | [enlace](https://www.bluradio.com/nacion/elecciones/polemica-en-florencia-caqueta-por-valla-publicitaria-de-ivan-cepeda-con-imagen-de-gustavo-petro-rg10) | D leve | «Polémica» en el titular sobre el candidato de izquierda; el cuerpo es descriptivo |
| 4 | 2026-06-01 | Petro y Uribe, entre los perdedores de la primera vuelta tras victoria de Abelardo De La Espriella | [enlace](https://www.bluradio.com/opinion/petro-y-uribe-entre-los-perdedores-de-la-primera-vuelta-tras-victoria-de-abelardo-de-la-espriella-pr30) | D leve | Ospina. Entre los ganadores, el candidato «que logró hacer una campaña interesante, emotiva y que conectó con el electorado» |
| 5 | 2026-06-04 | ¿Hasta cuándo esperarán Petro y Cepeda para reconocer los resultados de la primera vuelta? | [enlace](https://www.bluradio.com/opinion/hasta-cuando-esperaran-petro-y-cepeda-para-reconocer-los-resultados-de-la-primera-vuelta-pr30) | D | Ospina. La presión al candidato de izquierda es del titular. Al presidente lo fiscaliza (eso no suma); al candidato, lo encuadra |
| 6 | 2026-06-10 | Otra orden judicial incumplible termina impulsando candidatura de Abelardo De La Espriella | [enlace](https://www.bluradio.com/opinion/otra-orden-judicial-incumplible-termina-impulsando-candidatura-de-abelardo-de-la-espriella-pr30) | D leve | Ospina. Califica de «incumplible» la medida contra la propaganda del candidato de derecha |
| 7 | 2026-07-09 | A un mes de su posesión, De La Espriella sigue enviando mensajes de que su gobierno será disruptivo | [enlace](https://www.bluradio.com/opinion/a-un-mes-de-su-posesion-de-la-espriella-sigue-enviando-mensajes-de-que-su-gobierno-sera-disruptivo-pr30) | D leve | Ospina, sobre el presidente electo: «Si se cumple, sin duda se trataría de un cambio en la forma en la que se ha hecho política en el país» |
| 8 | 2025-11-11 | Por fortuna, por ahora, prevalece la diplomacia en nueva crisis entre Colombia y Estados Unidos | [enlace](https://www.bluradio.com/opinion/por-fortuna-por-ahora-prevalece-la-diplomacia-en-nueva-crisis-entre-colombia-y-estados-unidos-pr30) | **I leve** | Ospina. Valora como acierto («por fortuna») la decisión del Gobierno Petro de no escalar |
| 9 | 2025-11-19 | Operaciones militares contra disidencias de 'Iván Mordisco' deben continuar | [enlace](https://www.bluradio.com/opinion/operaciones-militares-contra-disidencias-de-ivan-mordisco-deben-continuar-pr30) | **I leve** | Ospina. Respalda los bombardeos ordenados por el Gobierno Petro frente a las investigaciones que los cuestionan |
| 10 | 2026-02-04 | Triunfó la sensatez en el encuentro entre los presidentes Petro y Trump | [enlace](https://www.bluradio.com/opinion/triunfo-la-sensatez-en-el-encuentro-entre-los-presidentes-petro-y-trump-pr30) | **I** | Ospina. Elogio en el titular a un resultado del Gobierno Petro |
| 11 | 2026-02-05 | Se comenzaron a sentir los efectos del encuentro Petro-Trump en la lucha contra grupos criminales | [enlace](https://www.bluradio.com/opinion/se-comenzaron-a-sentir-los-efectos-del-encuentro-petro-trump-en-la-lucha-contra-grupos-criminales-pr30) | **I leve** | Ospina: «No habían pasado 24 horas […] y ya se habían producido los primeros resultados» |
| 12 | 2026-05-13 | De La Espriella se disculpa con periodista por polémico "chiste": declaraciones causaron indignación | [enlace](https://www.bluradio.com/nacion/de-la-espriella-se-disculpa-con-periodista-por-polemico-chiste-declaraciones-causan-indignacion-so35) | **I leve** | «Polémico» e «indignación», en voz propia, sobre el candidato de derecha |

**Fiscalización del Gobierno Petro mientras gobierna (F: se declara, no suma).** De los 106 análisis de Ospina anteriores al cambio, la mayoría trata del Gobierno Petro y buena parte lo fiscaliza con la valoración en el titular. La lista no es exhaustiva, porque F no cuenta:

| Fecha | Título literal | URL |
|---|---|---|
| 2025-11-18 | Las incoherencias del Gobierno nacional frente a los bombardeos y la compra de aviones de combate | [enlace](https://www.bluradio.com/opinion/las-incoherencias-del-gobierno-nacional-frente-a-los-bombardeos-y-la-compra-de-aviones-de-combate-pr30) |
| 2025-11-25 | Petro nombra gestor de paz a disidente responsable del asesinato de 13 policías en Amalfi | [enlace](https://www.bluradio.com/nacion/paz/dias-antes-de-escandalo-de-infiltraciones-en-calarca-gobierno-nombro-gestores-de-paz-a-4-disidentes-rg10) |
| 2025-12-04 | Cifras oficiales contradicen al presidente Petro sobre seguridad y homicidios | [enlace](https://www.bluradio.com/nacion/cifras-oficiales-contradicen-al-presidente-petro-sobre-seguridad-y-homicidios-rg10) |
| 2025-12-12 | Con diálogos con bandas criminales, Gobierno Petro intenta salvar la paz total del fracaso total | [enlace](https://www.bluradio.com/opinion/con-dialogos-con-bandas-criminales-el-gobierno-petro-intenta-salvar-a-paz-total-del-fracaso-total-pr30) |
| 2025-12-15 | Arremetida terrorista del ELN sigue golpeando la agónica paz total del presidente Gustavo Petro | [enlace](https://www.bluradio.com/nacion/arremetida-terrorista-del-eln-sigue-golpeando-la-agonica-paz-total-del-presidente-gustavo-petro-pr30) |
| 2025-12-19 | Faltan explicaciones de Petro sobre escándalo de la UNGRD tras captura de dos de sus alfiles | [enlace](https://www.bluradio.com/opinion/faltan-explicaciones-de-petro-sobre-escandalo-de-la-ungrd-tras-captura-de-dos-de-sus-alfiles-pr30) |
| 2026-01-22 | Gobierno juega intentando dilatar el hundimiento de emergencia económica en la Corte Constitucional | [enlace](https://www.bluradio.com/opinion/gobierno-juega-intentando-dilatar-el-hundimiento-de-emergencia-economica-en-la-corte-constitucional-pr30) |
| 2026-01-28 | Desaparecieron la prudencia y la mesura en el discurso de Petro a una semana del encuentro con Trump | [enlace](https://www.bluradio.com/opinion/desaparecieron-la-prudencia-y-la-mesura-en-el-discurso-de-petro-a-una-semana-del-encuentro-con-trump-pr30) |
| 2026-02-11 | Continuidad de Ricardo Roa como presidente de Ecopetrol perjudica a la principal empresa del país | [enlace](https://www.bluradio.com/opinion/continuidad-de-ricardo-roa-como-presidente-de-ecopetrol-perjudica-a-la-principal-empresa-del-pais-pr30) |
| 2026-02-18 | Cierre del Parque Tayrona por amenazas de grupos criminales, nueva muestra de fracaso de Paz Total | [enlace](https://www.bluradio.com/opinion/cierre-del-parque-tayrona-por-amenazas-de-grupos-criminales-nueva-muestra-de-fracaso-de-paz-total-pr30) |
| 2026-02-20 | Es peligroso para democracia que presidente Petro hable sin sustento de posible fraude en elecciones | [enlace](https://www.bluradio.com/opinion/es-peligroso-para-democracia-que-presidente-petro-hable-sin-sustento-de-posible-fraude-en-elecciones-pr30) |
| 2026-02-24 | No es primera vez que Petro habla de fraude electoral; hoy, como presidente, debe dar tranquilidad | [enlace](https://www.bluradio.com/opinion/no-es-primera-vez-que-petro-habla-de-fraude-electoral-hoy-como-presidente-debe-dar-tranquilidad-pr30) |
| 2026-03-12 | Néstor Morales responde a mensaje del presidente Petro sobre escándalo de corrupción | [enlace](https://www.bluradio.com/nacion/nestor-morales-responde-a-mensaje-del-presidente-petro-sobre-escandalo-de-corrupcion-so35) |
| 2026-04-07 | Las preguntas que no ha respondido Petro sobre la infiltración de 'Papá Pitufo' en su Gobierno | [enlace](https://www.bluradio.com/opinion/las-preguntas-que-no-ha-respondido-petro-sobre-la-infiltracion-de-papa-pitufo-en-su-gobierno-pr30) |
| 2026-04-14 | Frente a amenazas de Petro por bloqueo de vías, hay que recodarle que “el presidente no es un rey” | [enlace](https://www.bluradio.com/opinion/frente-a-amenazas-de-petro-por-bloqueo-de-vias-hay-que-recodarle-que-el-presidente-no-es-un-rey-pr30) |
| 2026-04-22 | El informe de Amnistía Internacional confirma fracaso de la Paz Total del presidente Gustavo Petro | [enlace](https://www.bluradio.com/opinion/el-informe-de-amnistia-internacional-confirma-fracaso-de-la-paz-total-del-presidente-gustavo-petro-pr30) |
| 2026-05-27 | Noticias falsas, estrategia de última hora de varios líderes políticos a 4 días de las elecciones | [enlace](https://www.bluradio.com/opinion/noticias-falsas-estrategia-de-ultima-hora-de-varios-lideres-politicos-a-4-dias-de-las-elecciones-pr30) |
| 2026-06-03 | ¿Por qué el presidente Petro no tiene razón en denuncias sobre supuesto fraude en elecciones? | [enlace](https://www.bluradio.com/opinion/por-que-el-presidente-petro-no-tiene-razon-en-denuncias-sobre-supuesto-fraude-en-elecciones-pr30) |
| 2026-07-02 | Varios hechos recientes confirman que la política de paz total del Gobierno de Gustavo Petro fracasó | [enlace](https://www.bluradio.com/opinion/varios-hechos-recientes-confirman-que-la-politica-de-paz-total-del-gobierno-de-gustavo-petro-fracaso-pr30) |
| 2026-08-03 | El Gobierno de Gustavo Petro está terminando en medio de graves escándalos de corrupción | [enlace](https://www.bluradio.com/opinion/el-gobierno-de-gustavo-petro-esta-terminando-en-medio-de-graves-escandalos-de-corrupcion-pr30) |

No se encontró en los 106 análisis de Ospina ni en los 593 titulares filtrados anteriores al cambio **ningún endoso**: ninguna pieza pide el voto ni declara apoyo a un candidato.

### 2.2 Después del cambio: 2026-08-07 → 2026-10-12 (gobierna De la Espriella)

| # | Fecha | Título literal | URL | Clase | Por qué |
|---|---|---|---|---|---|
| 13 | 2026-08-13 | ¿Ricardo Roa delatará las posibles irregularidades en financiación de la campaña de Gustavo Petro? | [enlace](https://www.bluradio.com/opinion/ricardo-roa-delatara-las-posibles-irregularidades-en-financiacion-de-la-campana-de-gustavo-petro-pr30) | D retro leve | Ospina. Sigue el proceso por la campaña del expresidente; la pregunta es del titular |
| 14 | 2026-09-14 | Crisis fiscal y presupuesto de $634 billones desatan polémica por herencia del gobierno Petro | [enlace](https://www.bluradio.com/economia/crisis-fiscal-y-presupuesto-de-634-billones-desatan-polemica-por-herencia-del-gobierno-petro-pr30) | D retro leve | El encuadre de la «herencia» es del titular; el cuerpo lo atribuye a la oposición y a sectores económicos |
| 15 | 2026-10-07 | Gobierno resuelve tratamientos represados de más de 70.000 personas mediante plan de choque en salud | [enlace](https://www.bluradio.com/salud/gobierno-resuelve-tratamientos-represados-de-mas-de-70-000-personas-mediante-plan-de-choque-en-salud-rg10) | D leve | El titular hace suyo el balance del Ministerio («resuelve»); la entradilla lo atribuye |

**Fiscalización del Gobierno De la Espriella (F: se declara, no suma):**

| Fecha | Título literal | URL | Por qué |
|---|---|---|---|
| 2026-09-05 | ¿Tendrá límites la política de mano dura del Gobierno con criminales? Indepaz analiza | [enlace](https://www.bluradio.com/nacion/tendra-limites-la-politica-de-mano-dura-del-gobierno-con-criminales-indepaz-analiza-pr30) | Leve. La pregunta es del titular; el análisis, de la FIP en El Radar |

Los 5 análisis de Ospina posteriores al cambio, salvo el n.º 13, son descriptivos: «Solidaridad de colombianos con víctimas del terremoto es buena noticia» (18-08), «Los grandes retos que tendrá que asumir la nueva cúpula militar» (20-08), «Así será la estrategia de "mano dura" del gobierno de De La Espriella» (25-08, con la expresión entre comillas) y «¿Por qué el presidente Abelardo De La Espriella despachará desde la Casa de Nariño?» (26-08). No elogian ni fiscalizan.

### 2.3 Leídas y no clasificadas (se declaran)

- **Atribuidas, en los dos sentidos.** Contra el entrante: «Así como criticamos a De La Espriella, también lo hacemos con Cepeda» (19-05; el «criticamos» es de Edna Bonilla, en cita), las críticas de Pizarro (11-09) y del alcalde de Sincelejo (04-10). A su favor: los saludos de Trump, Rubio, Milei y otros gobiernos; los gremios que «celebran». Contra el saliente: alcaldes, gobernadores, gremios, expresidentes y candidatos, decenas de veces.
- **Probable contenido comercial o promocional**, que no cuenta: «¿Dónde estuvo el éxito de la campaña de Abelardo De La Espriella? Cobertura superó el 60 %» (02-07-2026; son las cifras de la agencia que hizo la publicidad) y «"Las otras rayas del tigre", el libro sobre Abelardo De La Espriella» (06-10-2026; presentación del libro con la voz de su autor). Las dos «Redacción comercial» del Gobierno Petro (20-02 y 25-02) tampoco cuentan.
- **Análisis de Ospina sin postura**, en los dos sentidos: «Acusaciones entre Abelardo y Paloma fortalecen a Iván Cepeda» (27-04), «¿Cuáles son las polémicas que afrontan Iván Cepeda, Paloma Valencia y Juan Daniel Oviedo?» (16-03, M: reparte), «¿Hasta dónde puede llegar el presidente De La Espriella con su propuesta de acabar la JEP?» (15-07, descriptivo), la serie sobre el choque entre De la Espriella y el uribismo por la presidencia del Senado (16, 17, 21, 22 y 27 de julio).
- **Datos electorales con adjetivo factual**, que no cuentan: «sacó la mayor votación de la historia en Antioquia y Medellín» (21-06) y «reafirma a los santanderes como fortín de la derecha» (01-06).
- **Lo que no se leyó y pesa**: la emisión. Mañanas Blu, su franja insignia, y El Radar son programas hablados; sus páginas de programa completo (`/mananas-blu/`, `/mananas-blu-10-30/`) son audio. La frase del director de Mañanas Blu del 13-08-2026 contra la respuesta del Gobierno al terremoto, que la ficha registra en su nivel 5, es de esa emisión y no está en el corpus escrito.

---

## 3. Números

| | D | I | M | Con postura | F (no suma) |
|---|---|---|---|---|---|
| Antes del 07-08-2026 (10 meses; 106 análisis de Ospina y 593 notas filtradas) | **7** (2 plenas, 5 leves) | **5** (1 plena, 4 leves) | 1 | 12 | Al menos 20 contra Petro, con la valoración en el titular (§2.1); en total, varias decenas |
| Desde el 07-08-2026 (2 meses; 5 análisis de Ospina y 63 notas filtradas) | **3** (leves; 2 retro) | **0** | 0 | 3 | 1 contra De la Espriella (leve) |
| **Total** | **10** | **5** | 1 | **15** | |

**Proporción principal: 10 a 5, es decir, 2 a 1.**

| Lectura | D | I | Proporción | ¿≥10 con postura? | ¿≥3 por lado en la dirección D (elogios, disculpas, rótulos)? | ¿≥3 F o postura a cada lado? |
|---|---|---|---|---|---|---|
| Principal | 10 | 5 | **2 : 1** | Sí (15) | **No**: después del cambio hay 3 D, pero dos son «retro» (crítica al gobierno saliente, no elogio ni disculpa) | **Sí**: antes, decenas; después, 3 D + 1 F = 4 |
| Sin las retro | 8 | 5 | 1,6 : 1 | Sí (13) | No | **No**: después, 1 D + 1 F = 2 |
| Sin ninguna «leve» | 2 | 1 | 2 : 1 | No (3) | No | No |

**El trato a quien gobierna (polo fijo).** El director del servicio informativo fiscalizó al Gobierno Petro en buena parte de sus 106 análisis de diez meses, con titulares como «fracaso total», «agónica paz total» o «el presidente no es un rey». Al Gobierno De la Espriella, en los cinco análisis que alcanzó a escribir antes de que la serie se interrumpiera el 26-08, no lo fiscalizó ni lo elogió. En las notas filtradas de los dos meses posteriores aparece una sola fiscalización leve. **La asimetría en la fiscalización existe, pero el lado posterior tiene tres semanas de columna**, y la regla no cuenta F.

Lo que sí cuenta, la postura, **va repartida**: antes del cambio la casa encuadró a Cepeda y elogió al candidato De la Espriella (7 veces), pero también elogió al Gobierno Petro cuando acertó con Washington y respaldó sus bombardeos (4 veces), y rotuló al candidato de derecha (1). No es la pauta de Noticias RCN (22 a 4).

---

## 4. Contrapesos (lo que contradice la dirección, y cuánto pesa)

| Contrapeso | Piezas | Peso |
|---|---|---|
| **Elogios al Gobierno Petro en voz del director** («Triunfó la sensatez», «Por fortuna […] prevalece la diplomacia», respaldo a sus bombardeos) | n.º 8-11 | **Alto.** Son de la voz más fuerte de la casa y van contra la dirección D que sugieren los titulares de campaña |
| **El director de Mañanas Blu critica al Gobierno entrante** (13-08-2026, terremoto; disculpa al día siguiente) | Nivel 5 de la ficha; audio | **Medio.** Es la franja insignia, pero está fuera del corpus escrito y no suma |
| **Sin endoso.** En 12 meses no hay pieza de la casa que pida el voto o declare apoyo | — | **Alto para la magnitud** |
| **Densidad baja.** 15 piezas con postura entre 678 notas filtradas y 149 piezas de opinión | §1 | **Alto para la magnitud** |
| **El lado posterior es corto y casi mudo**: la columna de Ospina se interrumpe el 26-08 | §2.2 | **Contra la propia conclusión**: por eso la alternativa es «sin medir» |
| **La fiscalización del saliente supera con mucho a la del entrante** | §2.1, §2.2 | **No es contrapeso; empuja hacia D**, pero F no cuenta y el lado posterior es de tres semanas |

---

## 5. Veredicto por condición

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | **Sí, en parte** | Análisis firmados por el director del servicio informativo, dos piezas de la conductora de una franja, titulares y entradillas de la redacción. No hay editoriales sin firma. La emisión no se leyó |
| 2. A los dos lados del cambio, en 12 meses | **Sí, con poco después** | 12 piezas con postura antes y 3 después |
| 3a. ≥10 piezas con postura | **Sí** | 15 |
| 3b. ≥3 a cada lado del cambio, en la misma dirección | **No** | Después del cambio, 3 D, de las cuales 2 son retro: solo 1 elogio |
| 3c. Proporción ≥3:1 | **No** | 2:1 |
| 4. Contrapesos escritos | **Sí** | §4 |
| 5. Reproducible | **Sí** | §2, con fecha, título literal, URL y clase; §1, con el filtro exacto |

**No cumple las cinco condiciones** (fallan 3b y 3c).

---

## 6. Rama de la precisión del 2026-10-10 y valor que resultaría

**El valor vigente se apoya solo en los niveles 4 y 5** (cabecera), así que el barrido manda aunque no llegue.

**Rama: «no llega, pero documenta la misma conducta con los dos gobiernos» → 0,00 con evidencia.** Hay al menos 3 piezas de fiscalización o postura a cada lado del cambio (decenas antes; 4 después: 3 D y 1 F) y la postura queda en 2 a 1, por debajo de 3 a 1.

**Valor propuesto: 0,00 con evidencia** (antes +0,25).

**Por qué no se queda en +0,25:**
- el +0,25 no tenía evidencia de línea («énfasis en seguridad» es temario) y el único hecho de su nivel 5 con contenido político es una crítica del director de la franja insignia **al Gobierno De la Espriella**;
- la voz de la casa reparte la postura (10 a 5) y elogia al Gobierno Petro cuando acierta;
- La FM (+0,25) y Noticias RCN (+0,15) llegaron a su número con barridos que cumplen; este no se acerca a sus proporciones.

**Por qué no un valor positivo pequeño (+0,05 o +0,10):** la rama que no cumple no admite un número de juicio entre 0 y el tope; o es 0,00 con evidencia o es «sin medir».

**Lectura alternativa, declarada: «sin medir»** (`bias: null`), si el responsable editorial pesa más que el lado posterior es corto y depende de dos piezas «retro»: sin ellas solo quedan 2 piezas después del cambio y la rama del 0,00 no se cumple. La dirección no es clara (1,6 a 1 sin retro), así que no habría tensión que declarar. Ninguna de las dos lecturas sostiene el +0,25.

**Vecinos:**
- **El Espectador (0,00)**, del mismo holding: misma posición;
- **Noticias Caracol**, de la **misma sociedad**: su barrido (`revision-externa/barridos/noticias-caracol.md`) propone «sin medir» y, como alternativa, 0,00. Con cualquiera de las lecturas **desaparece la diferencia de 0,15 entre dos productos de una sola sociedad** que la ficha llamaba indefendible (refutación 2);
- **W Radio (0,00)** y **Caracol Radio** (su barrido propone 0,00), las otras radios habladas de cobertura nacional.

**Qué lo refutaría:**
- hacia la derecha: que la serie de análisis del director o una pieza equivalente vuelva y elogie o disculpe al Gobierno De la Espriella mientras deja de fiscalizarlo, hasta pasar los mínimos;
- hacia la izquierda: lo simétrico;
- en cualquier sentido: una lectura de la emisión (Mañanas Blu), ponderada por audiencia, que es lo que la refutación 5 de la ficha pedía.

---

## 7. Cobertura, huecos y avisos

- **Lo que no se leyó.** La emisión, que es el producto principal (§2.3). Las notas cuyo slug no lleva ninguno de los términos del §1, y las que los llevan pero sin un término valorativo en el slug: de 3.818 se descargaron 678. Una nota con postura en la entradilla y un slug neutro se escapa.
- **El lado posterior es corto**: dos meses y 63 notas filtradas, frente a diez meses y 593. Además, la columna del director termina el 26-08-2026 y en la ventana no hay otra pieza suya.
- **F no es exhaustiva.** La lista de fiscalización a Petro es de titulares con la valoración en voz propia, no un recuento cerrado.
- **Cuerpos leídos en parte**: los primeros párrafos. La clase se apoya en titular y entradilla, que es lo que la regla cuenta; en los análisis de Ospina, en el texto del análisis.
- **Robots y red.** El robots.txt no excluyó nada de lo usado. Todas las respuestas fueron 200 y no se reintentó nada.
- **Una sola lectura**, de la misma casa que el autor de la ficha. Las piezas límite van marcadas «leve» y el §3 da el recuento con y sin ellas.
- **Datos personales.** No se copia ningún número de documento, teléfono ni dirección. Las personas nombradas son cargos públicos, candidatos o periodistas en su función.
