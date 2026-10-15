# Barrido editorial: El Informador (Santa Marta)

| | |
|---|---|
| **Medio** | El Informador, Santa Marta, Magdalena (`el-informador`). **En el catálogo desde el 2026-10-10** (`fichas/el-informador.md`); era candidatura |
| **Valor vigente** | **+0,45**, sin firmar, decidido por el responsable editorial el 2026-10-10 con este barrido (antes: ninguno, candidatura) |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus dos precisiones |
| **Ventana** | 2025-10-10 → 2026-10-10 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Resolución de origen** | `revision-externa/respuestas/opus-5-5-el-informador.md` (revisor: 24 piezas con postura, todas a la derecha) |
| **Quién lo hizo** | Claude Opus 5.5 (`claude-opus-5-5`), verificador del ciclo 2, tanda 7, a petición del responsable editorial, el 2026-10-10. Es de la misma casa que el autor de la ficha y que el revisor: su acuerdo no es aval |
| **Estado** | **Aplicado el 2026-10-10** (decisión del responsable editorial: alta en +0,45, sin firmar hasta tener los socios) |
| **Resultado** | **Cumple las cinco condiciones, con mucho margen.** 100 piezas con postura en voz de la casa en la misma dirección (67 antes del cambio y 33 después; 86 sin las leves), frente a 5 contrapesos (1 pleno y 4 parciales). Proporción 20 a 1. Hay además **endoso explícito con nombre** (21-06-2026) y llamadas previas a votar (08-03 y 11-05-2026) |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas, el
> fragmento y el método están aquí para eso. **La clasificación de cada pieza
> es juicio de un solo lector**, de la misma casa que el autor de la ficha y
> que el revisor.

---

## 1. Método

- **robots.txt** de `www.elinformador.com.co` (descargado el 2026-10-10): el de Joomla por defecto. `User-agent: *` con `Disallow` solo para `/administrator/`, `/bin/`, `/cache/`, `/cli/`, `/components/`, `/includes/`, `/installation/`, `/language/`, `/layouts/`, `/libraries/`, `/logs/`, `/modules/`, `/plugins/` y `/tmp/`. No nombra a ClaudeBot, Claude-Web ni anthropic-ai. Las rutas usadas (`/index.php/...` e `index.php?option=com_content...`) no están vetadas.
- **Descarga:** `curl -sL --ssl-no-revoke` con User-Agent de navegador (Chrome 126), con pausa entre peticiones.
- **Universo, sin muestreo:**
  1. El **archivo mensual de la categoría Editorial** (id 37), con el patrón que dio el revisor:
     `https://www.elinformador.com.co/index.php?option=com_content&view=archive&year=AAAA&month=M&catid%5B%5D=37&limit=0`,
     de 2025-10 a 2026-09. Devuelve **347 piezas** (del 2025-10-01 al 2026-09-27), los mismos 347 identificadores que el revisor. El de 2026-10 devuelve 0.
  2. El **feed de la sección** para octubre: `https://www.elinformador.com.co/index.php/opinion/37-editorial?format=feed&type=rss`, 13 ítems del 28-09 al 09-10-2026.
  3. **Las 360 páginas, una por una, con el texto completo** (no solo título e intro, que en la mayoría del archivo es «...»).
- **Ventana.** Se quitan las 7 piezas del 1 al 9 de octubre de 2025, fuera de los 12 meses: quedan **353**, 290 antes del 07-08-2026 y 63 desde ese día. **El medio publicó 10 editoriales dos veces** (con otra URL o al día siguiente); cada uno cuenta una sola vez: 344773 = 344818; 345853 = 345913; 346931 = 346972; 347694 = 348027; 351010 = 354326; 352007 = 352008; 354629 = 354632; 356533 = 356657; 358301 = 358307; 359411 = 359450. **343 piezas únicas.**
- **Voz de la casa (condición 1).** Ninguna de las 360 páginas lleva autor: no hay `itemprop="author"` ni firma en el cuerpo. Hablan como la casa: «Oportunamente comentamos…» (09-06-2026), «siempre lo hemos afirmado» (27-07-2026), «Hoy en este espacio editorial le tocó el turno a la senadora Valencia» (12-12-2025). Una pieza internacional cierra con «EFE» (344500, 08-12-2025, sin postura en el eje): hay texto de agencia en las piezas internacionales, que **no se cuentan**. Ninguna de las 360 páginas contiene «publirreportaje», «contenido patrocinado» ni «publicidad pagada».
- **Filtro.** Sobre el texto completo de las 353, términos nacionales: Petro, Espriella/Abelardo, Cepeda, Paloma, comunis-, marxis-, izquierd-, derech-, petris-, Pacto Histórico, guerriller-, terrorist-, tiran-, dictad-, populis-, Uribe, Centro Democrático, Fajardo, «gobierno nacional», «presidente electo», Tigre, «patria milagro», socialis-, estalin-. Las piezas con 2 o más coincidencias se leyeron por fragmentos alrededor de cada término; las de después del 07-08, las 63, se leyeron todas desde el principio, tuvieran o no términos.
- **Clases.**
  - **D, dirección derecha** (cuenta): rótulo ideológico o descalificador en voz propia contra Petro, su gobierno, Cepeda o «los comunistas» («tirano», «guerrillero comunista», «terrorista dictatorial», «mitomanía leninista»); elogio o petición de voto para candidatos de la derecha; celebración del presidente electo o del Gobierno De la Espriella; crítica al gobierno saliente cuando ya no manda.
  - **D (leve)** (cuenta, pero se marca): la postura existe pero es lateral o tibia.
  - **F, solo fiscaliza a quien manda** (no cuenta, se declara): crítica a la gestión del Gobierno Petro mientras gobierna, sin rótulo ideológico ni toma de partido electoral. **Precisión del responsable editorial del 2026-10-09: no suma para el mínimo por lado.**
  - **C, contrapeso:** crítica o reparo al Gobierno De la Espriella; reconocimiento a Petro, a su gobierno o a la izquierda.
  - **Fuera:** internacionales (aunque tengan encuadre: Maduro, Kast, Trump, Honduras), locales sin destinatario nacional, deportes, servicio, efemérides, y las nacionales de postura mixta o descriptiva (M).
- **Límite declarado.** Una pieza con F y un rótulo suelto se ha llevado a D solo si el rótulo es de la casa y no una cita. Las piezas límite van como «leve». Ver §5.

---

## 2. Tabla de piezas que cuentan (voz de la casa, sección Editorial)

Todas las URL son `https://www.elinformador.com.co/index.php/opinion/37-editorial/<id>-<slug>`. El fragmento se comprobó por programa contra el texto completo de cada página (2026-10-10).

### 2.1 Antes del cambio: 2025-10-10 → 2026-08-06 (gobierna Petro)

| # | Fecha | Id | Título | Clase | Fragmento literal (breve) |
|---|---|---|---|---|---|
| 1 | 2025-10-14 | [341596](https://www.elinformador.com.co/index.php/opinion/37-editorial/341596-petro-desubicado-y-castigado) | Petro desubicado y castigado | D | «como buen terrorista» |
| 2 | 2025-10-16 | [341757](https://www.elinformador.com.co/index.php/opinion/37-editorial/341757-muy-tarde) | Muy tarde | D | «solo restan 10 meses para que “cese la horrible noche”» |
| 3 | 2025-10-20 | [341947](https://www.elinformador.com.co/index.php/opinion/37-editorial/341947-defensor-de-la-criminalidad-y-las-guerrillas) | Defensor de la criminalidad y las guerrillas | D | «Petro siempre ha estado comportándose como un guerrillero comunista» |
| 4 | 2025-10-27 | [342374](https://www.elinformador.com.co/index.php/opinion/37-editorial/342374-dictador-narcoterrorista-y-criminal) | Dictador narcoterrorista y criminal | D | «como un terrorista dictatorial» |
| 5 | 2025-11-04 | [342810](https://www.elinformador.com.co/index.php/opinion/37-editorial/342810-se-esta-definiendo-el-futuro-de-colombia) | Se está definiendo el futuro de Colombia | D | «ideológicamente extremistas» |
| 6 | 2025-11-11 | [343149](https://www.elinformador.com.co/index.php/opinion/37-editorial/343149-transparencia-total-en-el-2026) | Transparencia total en el 2026 | D | «había un registrador petrista, Alexander Vega; el colaboró en el fraude» |
| 7 | 2025-11-18 | [343490](https://www.elinformador.com.co/index.php/opinion/37-editorial/343490-ataque-sanguinario-y-cruel) | Ataque sanguinario y cruel | D | «los comunistas por su adoctrinamiento leninista falsean la historia» |
| 8 | 2025-11-24 | [343807](https://www.elinformador.com.co/index.php/opinion/37-editorial/343807-libertad-democratica-o-tirania-estalinista) | Libertad democrática o tiranía estalinista | D | «los comunistas con Iván Cepeda, ya están trabajando por su candidatura» |
| 9 | 2025-12-01 | [344161](https://www.elinformador.com.co/index.php/opinion/37-editorial/344161-el-mejor-cierre-del-2025) | El mejor cierre del 2025 | D | «al candidato tan marxista como él, cual es Iván Cepeda» |
| 10 | 2025-12-12 | [344660](https://www.elinformador.com.co/index.php/opinion/37-editorial/344660-la-tercera-es-la-vencida-2) | La tercera es la vencida | D | «Hoy en este espacio editorial le tocó el turno a la senadora Valencia» |
| 11 | 2025-12-14 | [344773](https://www.elinformador.com.co/index.php/opinion/37-editorial/344773-comunismo-en-colombia) | Comunismo en Colombia | D | «Gustavo Petro lo único que ha querido y quiere es implantarnos el sistema comunista» |
| 12 | 2025-12-22 | [345133](https://www.elinformador.com.co/index.php/opinion/37-editorial/345133-austeridad-fe-y-patriotismo) | Austeridad, fe y patriotismo | D | «el erario se lo han robado Petro, sus amigos y sus colaboradores» |
| 13 | 2025-12-29 | [345437](https://www.elinformador.com.co/index.php/opinion/37-editorial/345437-2026-elecciones-legislativas-y-presidenciales) | 2026, elecciones legislativas y presidenciales | D | «rechazamos por ende la opresión leninista derivada del régimen petrista» |
| 14 | 2026-01-05 | [345744](https://www.elinformador.com.co/index.php/opinion/37-editorial/345744-asamblea-constituyente) | Asamblea Constituyente | D | «esos abusos del tirano» |
| 15 | 2026-01-22 | [346401](https://www.elinformador.com.co/index.php/opinion/37-editorial/346401-las-cuentas-de-la-campana-presidencial) | Las cuentas de la campaña presidencial | D (leve) | «el candidato de izquierda y heredero de Gustavo Petro» |
| 16 | 2026-01-26 | [346625](https://www.elinformador.com.co/index.php/opinion/37-editorial/346625-liderazgo-en-la-jefatura-de-estado) | Liderazgo en la jefatura de Estado | D | «Petro representa en grado superlativo el negativo liderazgo» |
| 17 | 2026-02-09 | [347347](https://www.elinformador.com.co/index.php/opinion/37-editorial/347347-reflexiones-frente-a-las-proximas-elecciones) | Reflexiones frente a las próximas elecciones | D | «estamos ad-portas de perder nuestra democracia» |
| 18 | 2026-02-18 | [347787](https://www.elinformador.com.co/index.php/opinion/37-editorial/347787-populismo-contra-la-democracia) | Populismo contra la democracia | D | «muy parecidos a Petro» |
| 19 | 2026-02-23 | [348071](https://www.elinformador.com.co/index.php/opinion/37-editorial/348071-caracteristicas-relevantes-de-los-lideres) | Características relevantes de los líderes | D | «nunca en nuestra historia habíamos tenido un presidente tan corrupto como Petro» |
| 20 | 2026-03-02 | [348422](https://www.elinformador.com.co/index.php/opinion/37-editorial/348422-petro-decidido-a-perpetuarse) | Petro decidido a perpetuarse | D | «lo que se le antoje al tirano» |
| 21 | 2026-03-06 | [348632](https://www.elinformador.com.co/index.php/opinion/37-editorial/348632-eleccion-de-legisladores-y-presidencial) | Elección de legisladores y presidencial | D | «Los antecedentes de Cepeda son delincuenciales» |
| 22 | 2026-03-08 | [348748](https://www.elinformador.com.co/index.php/opinion/37-editorial/348748-a-votar-por-la-libertad-y-la-democracia) | A votar por la libertad y la democracia | D | «Partidos como Centro Democrático, Cambio Radical, Salvación Nacional» |
| 23 | 2026-03-10 | [348815](https://www.elinformador.com.co/index.php/opinion/37-editorial/348815-paloma-valencia) | Paloma Valencia | D | «ser la primera mujer en la presidencia de la República, Dios mediante» |
| 24 | 2026-03-16 | [349165](https://www.elinformador.com.co/index.php/opinion/37-editorial/349165-futuro-presidencial-en-colombia) | Futuro presidencial en Colombia | D | «los demócratas estamos obligados a votar en pro de nuestra libertad» |
| 25 | 2026-03-24 | [349542](https://www.elinformador.com.co/index.php/opinion/37-editorial/349542-que-pasara-en-las-elecciones-presidenciales) | Que pasará en las elecciones presidenciales | D | «estamos convencidos de que Abelardo es quién despierta más fervor» |
| 26 | 2026-03-28 | [349726](https://www.elinformador.com.co/index.php/opinion/37-editorial/349726-faltan-los-instigadores) | Faltan los instigadores | D | «amigo personal del candidato a la presidencia, Iván Cepeda» |
| 27 | 2026-03-30 | [349805](https://www.elinformador.com.co/index.php/opinion/37-editorial/349805-prueba-de-fuego-a-la-sensatez) | Prueba de fuego a la sensatez | D | «tan inepto, tan corrupto e ideologizado» |
| 28 | 2026-04-06 | [350073](https://www.elinformador.com.co/index.php/opinion/37-editorial/350073-el-peor-balance-de-un-gobierno) | El peor balance de un gobierno | D | «podemos considerar su administración como la más nefasta» |
| 29 | 2026-04-13 | [350449](https://www.elinformador.com.co/index.php/opinion/37-editorial/350449-ruina-economica-fruto-del-populismo-marxista) | Ruina económica fruto del populismo marxista | D | «lo acontecido en nuestro territorio con el petrismo» |
| 30 | 2026-04-18 | [350738](https://www.elinformador.com.co/index.php/opinion/37-editorial/350738-revolucion-politica) | Revolución política | D | «pensó en Colombia, en cómo sacarla de esta terrible situación» |
| 31 | 2026-04-27 | [351238](https://www.elinformador.com.co/index.php/opinion/37-editorial/351238-pastorcitos-mentirosos-y-narrativas-distorsionadas) | Pastorcitos mentirosos y narrativas distorsionadas | D | «Nicaragua, Venezuela y ahora Colombia» |
| 32 | 2026-05-04 | [351585](https://www.elinformador.com.co/index.php/opinion/37-editorial/351585-petro-obsesionado-por-el-poder) | Petro obsesionado por el poder | D | «la campaña del comunista Iván Cepeda» |
| 33 | 2026-05-06 | [351723](https://www.elinformador.com.co/index.php/opinion/37-editorial/351723-muestra-de-buena-voluntad) | Muestra de buena voluntad | D | «podamos salir de este gobierno de izquierda» |
| 34 | 2026-05-07 | [351784](https://www.elinformador.com.co/index.php/opinion/37-editorial/351784-el-debate-en-redes) | El debate en redes | D | «heredero del desastre del actual gobierno» |
| 35 | 2026-05-11 | [352007](https://www.elinformador.com.co/index.php/opinion/37-editorial/352007-primera-vuelta-presidencial) | Primera vuelta presidencial | D | «deberán depositar su voto por Abelardo» |
| 36 | 2026-05-15 | [352230](https://www.elinformador.com.co/index.php/opinion/37-editorial/352230-una-amenaza-latente-2) | Una amenaza latente | D (leve) | «Pero Noboa no es Petro, gracias a Dios» |
| 37 | 2026-05-18 | [352371](https://www.elinformador.com.co/index.php/opinion/37-editorial/352371-no-hay-garantias) | No hay garantías | D | «quién les asegurara otros cuatro años más de impunidad y violencia» |
| 38 | 2026-05-19 | [352420](https://www.elinformador.com.co/index.php/opinion/37-editorial/352420-modus-operandi-comunista-y-populista) | Modus operandi comunista y populista | D | «en manos de los violentos bandidos de las guerrillas comunistas» |
| 39 | 2026-05-21 | [352544](https://www.elinformador.com.co/index.php/opinion/37-editorial/352544-flagrante-intromision) | Flagrante intromisión | D | «sigue metiendo sus narices rojas comunistas» |
| 40 | 2026-05-28 | [352911](https://www.elinformador.com.co/index.php/opinion/37-editorial/352911-presion-fiscal-y-el-legado-economico) | Presión fiscal y el legado económico | D (leve) | «no solo estará en juego la sucesión de Petro, sino también la libertad y la democracia» |
| 41 | 2026-05-30 | [353045](https://www.elinformador.com.co/index.php/opinion/37-editorial/353045-petro-y-el-fraude-en-las-elecciones-presidenciales) | Petro y el fraude en las elecciones presidenciales | D | «la mitomanía leninista» |
| 42 | 2026-06-02 | [353234](https://www.elinformador.com.co/index.php/opinion/37-editorial/353234-ganadores-y-perdedores) | Ganadores y perdedores | D | «heredero del desastre del gobierno de Gustavo Petro» |
| 43 | 2026-06-03 | [353294](https://www.elinformador.com.co/index.php/opinion/37-editorial/353294-estan-desesperados) | Están desesperados | D | «miedo, pánico y desespero» |
| 44 | 2026-06-04 | [353354](https://www.elinformador.com.co/index.php/opinion/37-editorial/353354-plena-identidad) | Plena identidad | D | «un frente común contra el comunismo. Y así es» |
| 45 | 2026-06-09 | [353563](https://www.elinformador.com.co/index.php/opinion/37-editorial/353563-dictadura-estalinista-o-libertad-democratica) | Dictadura estalinista o libertad democrática | D | «Oportunamente comentamos que la votación de Abelardo sorprendería» |
| 46 | 2026-06-11 | [353682](https://www.elinformador.com.co/index.php/opinion/37-editorial/353682-restringir-la-libertad) | Restringir la libertad | D | «el heredero de este nefasto gobierno» |
| 47 | 2026-06-18 | [354023](https://www.elinformador.com.co/index.php/opinion/37-editorial/354023-se-necesita-una-revolucion-economica-y-social) | Se necesita una revolución económica y social | D | «que sin duda ayudaran a solucionar la terr» |
| 48 | 2026-06-19 | [354083](https://www.elinformador.com.co/index.php/opinion/37-editorial/354083-una-vida-exitosa) | Una vida exitosa | D (leve) | «hizo fortuna como abogado, emprendedor y exitoso hombre de negocios» |
| 49 | 2026-06-20 | [354149](https://www.elinformador.com.co/index.php/opinion/37-editorial/354149-mano-derecha-y-cerebro-economico) | Mano derecha y cerebro económico | D (leve) | «principal escudero del candidato Abelardo De La Espriella» |
| 50 | 2026-06-21 | [354190](https://www.elinformador.com.co/index.php/opinion/37-editorial/354190-abelardo-de-la-espriella-o-ivan-cepeda) | Abelardo De La Espriella o Iván Cepeda | D | «con Abelardo habrá institucionalidad, democracia y libertad; con Cepeda habrá instituciones propias, tiranía y abolición hasta de la libertad de prensa» |
| 51 | 2026-06-22 | [354254](https://www.elinformador.com.co/index.php/opinion/37-editorial/354254-triunfo-la-esperanza) | Triunfó la esperanza | D | «triunfó la democracia, el sentido común y la decencia» |
| 52 | 2026-06-24 | [354386](https://www.elinformador.com.co/index.php/opinion/37-editorial/354386-elecciones-transparentes-y-con-garantias) | Elecciones transparentes y con garantías | D | «las pataletas de ahogado» |
| 53 | 2026-06-26 | [354522](https://www.elinformador.com.co/index.php/opinion/37-editorial/354522-renovar-compromisos) | Renovar compromisos | D (leve) | «gracias a los cambios positivos con el nuevo gobierno» |
| 54 | 2026-06-30 | [354685](https://www.elinformador.com.co/index.php/opinion/37-editorial/354685-triunfo-de-la-democracia) | Triunfo de la democracia | D | «Estamos convencidos de que Abelardo brillará en el panorama hispanoamericano» |
| 55 | 2026-07-02 | [354791](https://www.elinformador.com.co/index.php/opinion/37-editorial/354791-desobediencia-civil) | Desobediencia civil | D | «La era del Tigre, dejará sin duda alguna una huella de transparencia» |
| 56 | 2026-07-03 | [354886](https://www.elinformador.com.co/index.php/opinion/37-editorial/354886-el-mayor-reto-es-recuperar-la-inversion) | El mayor reto es recuperar la inversión | D (leve) | «durante el gobierno nefastos de Gustavo Petro» |
| 57 | 2026-07-06 | [355015](https://www.elinformador.com.co/index.php/opinion/37-editorial/355015-colombia-patria-milagro) | Colombia, patria milagro | D | «Nadie puede dudar de que con nuestro presidente Abelardo De La Espriella, todo va a cambiar» |
| 58 | 2026-07-08 | [355144](https://www.elinformador.com.co/index.php/opinion/37-editorial/355144-debe-ser-juzgado) | Debe ser juzgado | D | «desmantelar un gobierno corrupto y descompuesto» |
| 59 | 2026-07-14 | [355457](https://www.elinformador.com.co/index.php/opinion/37-editorial/355457-presidente-entrante-versus-presidente-saliente) | Presidente entrante versus presidente saliente | D | «para fortuna de todos los colombianos, están feneciendo estos oscuros días» |
| 60 | 2026-07-16 | [355599](https://www.elinformador.com.co/index.php/opinion/37-editorial/355599-jovenes-a-postularse) | Jóvenes a postularse | D | «Con estos pasos agigantados de De La Espriella» |
| 61 | 2026-07-17 | [355643](https://www.elinformador.com.co/index.php/opinion/37-editorial/355643-exitosa-gira) | Exitosa gira | D | «Todo el país sigue con orgullo, complacencia y tranquilidad» |
| 62 | 2026-07-20 | [355780](https://www.elinformador.com.co/index.php/opinion/37-editorial/355780-etapa-de-mas-ayuda) | Etapa de más ayuda | D | «los alzados en armas y sus amigos en el gobierno nacional» |
| 63 | 2026-07-21 | [355807](https://www.elinformador.com.co/index.php/opinion/37-editorial/355807-abelardo-hombre-de-empresa-eficaz) | Abelardo, hombre de empresa eficaz | D | «abogado comunista defensor de derechos humanos» |
| 64 | 2026-07-27 | [356119](https://www.elinformador.com.co/index.php/opinion/37-editorial/356119-requiem-de-petro-el-20-de-julio-2026) | Réquiem de Petro el 20 de julio 2026 | D | «Petro es un personaje siniestro, siempre lo hemos afirmado» |
| 65 | 2026-07-29 | [356230](https://www.elinformador.com.co/index.php/opinion/37-editorial/356230-la-ciudad-milagro) | La Ciudad Milagro | D (leve) | «Un presidente que ha reiterado, con hechos y palab» |
| 66 | 2026-08-03 | [356483](https://www.elinformador.com.co/index.php/opinion/37-editorial/356483-centralizacion-politica-y-descentralizacion-administrativa) | Centralización política y descentralización administrativa | D (leve) | «nuestro presidente electo, Abelardo De La Espriella» |
| 67 | 2026-08-04 | [356533](https://www.elinformador.com.co/index.php/opinion/37-editorial/356533-un-legado-de-corrupcion) | Un legado de corrupción | D | «Colombia sea nuevamente, un país viable» |
| 68 | 2025-12-31 | [345540](https://www.elinformador.com.co/index.php/opinion/37-editorial/345540-el-renacer-samario) | El renacer samario | **C parcial** | «reconocer que no cayó en la dinámica de pelear con el Presi» |
| 69 | 2026-03-14 | [349067](https://www.elinformador.com.co/index.php/opinion/37-editorial/349067-una-gran-oportunidad-comercial) | Una gran oportunidad comercial | **C parcial** | «la recuperación comenzó con la llegada de Petro al poder en 2022» |

### 2.2 Después del cambio: 2026-08-07 → 2026-10-10 (gobierna De la Espriella)

| # | Fecha | Id | Título | Clase | Fragmento literal (breve) |
|---|---|---|---|---|---|
| 70 | 2026-08-07 | [356885](https://www.elinformador.com.co/index.php/opinion/37-editorial/356885-la-posesion-del-nuevo-presidente) | La posesión del nuevo presidente | D | «también ha brillado por su coherencia, por su oratoria» |
| 71 | 2026-08-08 | [356753](https://www.elinformador.com.co/index.php/opinion/37-editorial/356753-ceso-la-horrible-noche) | ¡Cesó la horrible noche! | D | «Petro Urrego terminó su mandato bajo la sombra de la corrupción» |
| 72 | 2026-08-10 | [356833](https://www.elinformador.com.co/index.php/opinion/37-editorial/356833-cuatro-anos-de-discursos-sin-guion) | Cuatro años de discursos sin guión | D | «concluyó, gracias a Dios, el pasado 7 de agosto» |
| 73 | 2026-08-12 | [356952](https://www.elinformador.com.co/index.php/opinion/37-editorial/356952-comenzar-por-la-seguridad-nacional-2) | Comenzar por la seguridad nacional | D | «los buenos vientos llenos de esperanza y de verdadero cambio» |
| 74 | 2026-08-14 | [357089](https://www.elinformador.com.co/index.php/opinion/37-editorial/357089-primer-balance-positivo) | Primer balance positivo | D | «presenta sus resultados positivos contra el terrorismo» |
| 75 | 2026-08-15 | [357188](https://www.elinformador.com.co/index.php/opinion/37-editorial/357188-carencias-historicas) | Carencias históricas | D (leve) | «Gracias a Dios, el gobierno nacional y regional» |
| 76 | 2026-08-18 | [357270](https://www.elinformador.com.co/index.php/opinion/37-editorial/357270-apoyo-a-los-damnificados-del-terremoto) | Apoyo a los damnificados del terremoto | D | «Felizmente está manejando la crisis un mandatario organiz» |
| 77 | 2026-08-20 | [357381](https://www.elinformador.com.co/index.php/opinion/37-editorial/357381-el-libro-de-la-verdad) | El Libro de la Verdad | D | «durante los cuatro desastrosos años de gobierno de Gustavo Petro Urrego» |
| 78 | 2026-08-21 | [357444](https://www.elinformador.com.co/index.php/opinion/37-editorial/357444-colombia-se-levanta) | Colombia se levanta | D | «El presidente De La Espriella, no ha descansado» |
| 79 | 2026-08-22 | [357492](https://www.elinformador.com.co/index.php/opinion/37-editorial/357492-medida-necesaria) | Medida necesaria | D | «a un presidente que se asegurará que los recursos de la Nación» |
| 80 | 2026-08-26 | [357683](https://www.elinformador.com.co/index.php/opinion/37-editorial/357683-cinco-ejes-esenciales) | Cinco ejes esenciales | D | «heredada del desastroso gobierno de Gustavo Petro» |
| 81 | 2026-08-27 | [357732](https://www.elinformador.com.co/index.php/opinion/37-editorial/357732-abriendo-caminos) | Abriendo caminos | D | «la nefasta herencia del cuatrienio desastroso de Gustavo Petro» |
| 82 | 2026-08-28 | [357784](https://www.elinformador.com.co/index.php/opinion/37-editorial/357784-subieron-las-cifras) | Subieron las cifras | D | «Otras de la cifras que dejó en rojo el pasado gobierno de Gustavo Petro Urrego» |
| 83 | 2026-08-29 | [357848](https://www.elinformador.com.co/index.php/opinion/37-editorial/357848-cooperacion-andina) | Cooperación andina | D (leve) | «El gobierno nacional la tiene clara» |
| 84 | 2026-08-31 | [357935](https://www.elinformador.com.co/index.php/opinion/37-editorial/357935-los-regimenes-comunistas-destruyen-la-institucionalidad) | Los regímenes comunistas destruyen la institucionalidad | D | «súbditos y esclavos de sus gobernantes sátrapas» |
| 85 | 2026-09-02 | [358039](https://www.elinformador.com.co/index.php/opinion/37-editorial/358039-se-acabo-no-va-mas) | Se acabó, no va más | D | «tristemente célebres por ser ex presidentes» |
| 86 | 2026-09-04 | [358183](https://www.elinformador.com.co/index.php/opinion/37-editorial/358183-volveran-a-las-carceles) | Volverán a las cárceles | D | «Se les acabó la ‘guachafita’» |
| 87 | 2026-09-05 | [358243](https://www.elinformador.com.co/index.php/opinion/37-editorial/358243-nain-sintio-la-mano-del-estado) | Naín sintió la mano del Estado | D (leve) | «Es un resultado que debe reconocerse» |
| 88 | 2026-09-06 | [358301](https://www.elinformador.com.co/index.php/opinion/37-editorial/358301-fue-la-mejor-eleccion) | Fue la mejor elección | D | «el simpatizante de la guerrilla y amigo personal de Petro» |
| 89 | 2026-09-08 | [358383](https://www.elinformador.com.co/index.php/opinion/37-editorial/358383-de-la-espriella-un-mes-de-mano-firme) | De La Espriella: un mes de mano firme | D | «El balance de este primer mes merece, por lo menos, un reconocimiento» |
| 90 | 2026-09-12 | [358605](https://www.elinformador.com.co/index.php/opinion/37-editorial/358605-la-politica-no-puede-estar-por-encima-de-la-verdad) | La política no puede estar por encima de la verdad | D (leve) | «las declaraciones y publicaciones del entonces presidente Gustavo Petro en defensa de Guerrero» |
| 91 | 2026-09-14 | [358718](https://www.elinformador.com.co/index.php/opinion/37-editorial/358718-expresidente-ecuatoriano-fugitivo-y-expresidente-colombiano-en-la-lista-clinton) | Expresidente ecuatoriano fugitivo y expresidente colombiano en la lista Clinton | D | «Atacan a Abelardo señalándolo como un ciudadano americano» |
| 92 | 2026-09-16 | [358832](https://www.elinformador.com.co/index.php/opinion/37-editorial/358832-paz-total-o-derroche-total) | ¿Paz Total o derroche total? | D | «representa, en ese sentido, un cambio profundo» |
| 93 | 2026-09-17 | [358902](https://www.elinformador.com.co/index.php/opinion/37-editorial/358902-comienzan-a-caer) | Comienzan a caer | D | «las fichas de la corrupción del desastroso gobierno de Gustavo Petro» |
| 94 | 2026-09-21 | [359111](https://www.elinformador.com.co/index.php/opinion/37-editorial/359111-un-conductor-un-jefe-un-comandante) | Un conductor, un jefe, un comandante | D | «Abelardo hace contraste con Petro una vergüenza como gobernante» |
| 95 | 2026-09-22 | [359176](https://www.elinformador.com.co/index.php/opinion/37-editorial/359176-firme-y-coherente) | Firme y coherente | D | «como un hombre firme en sus convicciones» |
| 96 | 2026-09-24 | [359281](https://www.elinformador.com.co/index.php/opinion/37-editorial/359281-rendirse-antes-de-terminar-en-una-tumba) | Rendirse antes de terminar en una tumba | D | «hay un presidente que está haciendo presencia» |
| 97 | 2026-09-30 | [359575](https://www.elinformador.com.co/index.php/opinion/37-editorial/359575-con-resultados) | Con resultados | D | «se encuentran a buen recaudo en el infierno» |
| 98 | 2026-10-01 | [359653](https://www.elinformador.com.co/index.php/opinion/37-editorial/359653-una-puerta-que-se-abre) | Una puerta que se abre | D | «dejado por el líder intergaláctico, Gustavo Petro» |
| 99 | 2026-10-02 | [359693](https://www.elinformador.com.co/index.php/opinion/37-editorial/359693-en-defensa-de-los-ciudadanos) | En defensa de los ciudadanos | D (leve) | «propuso modificar el protocolo» |
| 100 | 2026-10-03 | [359795](https://www.elinformador.com.co/index.php/opinion/37-editorial/359795-importantes-acercamientos) | Importantes acercamientos | D | «gobierno del líder intergaláctico Gustavo Petro» |
| 101 | 2026-10-05 | [359858](https://www.elinformador.com.co/index.php/opinion/37-editorial/359858-desconocimiento-del-comunismo) | Desconocimiento del comunismo | D | «el más marxista entre los marxistas, es el señor Iván Cepeda» |
| 102 | 2026-10-06 | [359918](https://www.elinformador.com.co/index.php/opinion/37-editorial/359918-alianza-firme) | Alianza firme | D | «un presidente que no le teme a nada» |
| 103 | 2026-09-09 | [358422](https://www.elinformador.com.co/index.php/opinion/37-editorial/358422-esta-preparada-colombia-para-volver-al-porte-legal-de-armas) | ¿Está preparada Colombia para volver al porte legal de armas? | **C** | «puede convertir un conflicto que antes terminaba en insultos o golpes en una tragedia irreversible» |
| 104 | 2026-09-11 | [358555](https://www.elinformador.com.co/index.php/opinion/37-editorial/358555-ahora-hay-que-reconstruir) | Ahora hay que reconstruir | **C parcial** | «la rapidez no puede confundirse con ausencia de controles» |
| 105 | 2026-09-29 | [359516](https://www.elinformador.com.co/index.php/opinion/37-editorial/359516-santa-marta-no-puede-seguir-esperando-por-el-agua) | Santa Marta no puede seguir esperando por el agua | **C parcial** | «Es una decisión que puede ser discutida desde el punto de vista técnico, financiero o ambiental» |

### 2.3 Lo que no cuenta, y se declara

**Solo fiscalizan al Gobierno Petro mientras gobierna (F, 62 piezas; no suman para el mínimo por lado):** 2025-10-17 341802; 2025-10-18 341854; 2025-10-25 342270; 2025-10-28 342424; 2025-10-29 342477; 2025-11-14 343323; 2025-11-26 343899; 2025-11-27 343951; 2025-12-04 344298; 2025-12-13 344727; 2025-12-17 344880; 2025-12-18 344949; 2025-12-23 345164; 2026-01-03 345648; 2026-01-06 345807; 2026-01-07 345853; 2026-01-09 345987; 2026-01-10 346044; 2026-01-16 346320; 2026-01-21 346368; 2026-01-24 346560; 2026-01-28 346710; 2026-01-29 346762; 2026-01-30 346813; 2026-02-03 347008; 2026-02-05 347139; 2026-02-06 347187; 2026-02-07 347252; 2026-02-12 347479; 2026-02-13 347540; 2026-02-19 347863; 2026-02-20 347939; 2026-02-21 347965; 2026-02-25 348194; 2026-02-27 348271; 2026-02-28 348331; 2026-03-18 349287; 2026-03-19 349337; 2026-03-22 349483; 2026-03-23 349525; 2026-03-27 349678; 2026-04-08 350154; 2026-04-09 350220; 2026-04-15 350558; 2026-04-24 351056; 2026-04-25 351134; 2026-04-29 351338; 2026-05-02 351515; 2026-05-05 351654; 2026-05-08 351867; 2026-05-14 352180; 2026-05-16 352286; 2026-05-17 352346; 2026-05-22 352596; 2026-05-23 352649; 2026-05-25 352747; 2026-05-27 352854; 2026-05-29 352982; 2026-07-11 355370; 2026-07-15 355520; 2026-07-24 356012; 2026-07-30 356252.

**Nacionales con postura mixta o descriptiva (M, 11):** 2025-10-15 341680 «El escalafón de la dignidad presidencial»; 2025-11-23 343780 «Todos a votar para derrotar la falta de garantías»; 2026-01-14 346197 «Definiendo el futuro político»; 2026-03-11 348863 «Prendieron motores»; 2026-03-12 348929 «Buen comportamiento»; 2026-04-22 350938 «La 'paz total' fue un rotundo fracaso»; 2026-05-12 352069 «Uno de los políticos más poderosos de Colombia»; 2026-07-04 354940 «Se debe conocer la verdad»; 2026-07-10 355257 «Desafíos y retos»; 2026-07-18 355725 «Proteger a la población civil»; 2026-08-05 356606 «Abelardo De La Espriella, el fenómeno que sacude la política». Entre ellas, la guía de voto de las atípicas del Magdalena (23-11-2025) critica a la vez a la izquierda departamental y a quienes «son nada más que serviles al gobierno de turno sea de izquierda o de derecha».

**Internacionales con encuadre (fuera):** Machado y el Nobel (11-10-2025), Honduras (07-12-2025), «Nuevo polo ultraderechista en Suramérica» (21-12-2025), Kast (26-12-2025 y 30-08-2026), «Junta de Paz, nueva Onu» (01-02-2026, con su duplicado), «Escudo de las Américas» (09-10-2026). Casi todas a favor de la derecha regional o de Trump, pero no son gobierno ni candidatura colombianos. **Ojo:** la reforma de Kast del 30-08 es la que el revisor llamaba contrapeso (c), y aquí queda fuera, igual que en el barrido de El Diario (Pereira).

---

## 3. Recuento

| | D | D (leve) | Suman | C | C parcial | Contrapesos |
|---|---|---|---|---|---|---|
| Antes del 07-08-2026 | **58** | 9 | **67** | 0 | 2 | 2 |
| Desde el 07-08-2026 | **28** | 5 | **33** | 1 | 2 | 3 |
| **Total** | **86** | 14 | **100** | 1 | 4 | **5** |

- **Proporción:** 100 a 5, **20 a 1**. Sin las leves y contando los 4 parciales como plenos: 86 a 5, más de 17 a 1.
- **A cada lado del cambio** (solo elogios, disculpas y rótulos; ninguna F): 67 antes y 33 después; sin las leves, 58 y 28.
- **Solo con lo que no puede leerse como fiscalización de Petro en el poder** (elogios y peticiones de voto a la derecha antes del cambio, y todo lo de después): siguen siendo decenas a cada lado. Antes, por ejemplo, 344660, 348748, 348815, 349165, 349542, 350738, 351723, 352007, 353563, 354023, 354190, 354254, 354685, 355015, 355599, 355643: 16 sin contar rótulos.

**La lectura del polo fijo:**

| Trato al gobierno **en ejercicio** | Favorables | Críticos |
|---|---|---|
| Petro, mientras gobierna | **0** | 62 F + rótulos en decenas de D |
| De la Espriella, ya en el poder | **33** (28 + 5 leves) | **3** (1 pleno, 2 parciales) |

- Con Petro, la casa no solo fiscaliza: rotula. «Guerrillero comunista» (20-10-2025), «terrorista dictatorial» (27-10-2025), «tirano» (05-01 y 02-03-2026), «mitomanía leninista» (30-05-2026).
- Con De la Espriella, celebra: «los buenos vientos llenos de esperanza y de verdadero cambio» (12-08), «un presidente que no le teme a nada» (06-10), y al anterior lo sigue llamando «líder intergaláctico» (01-10 y 03-10).

**Endoso y peticiones de voto, con nombre:**

| Fecha | Pieza | Qué dice |
|---|---|---|
| 2026-03-08 | 348748 «A votar por la libertad y la democracia» | Día de legislativas. Pide alejarse «de los que representan sectores del comunismo» y enumera «Partidos como Centro Democrático, Cambio Radical, Salvación Nacional, Creemos, Colombia Segura y Próspera, y Oxigeno» |
| 2026-03-10 | 348815 «Paloma Valencia» | «ser la primera mujer en la presidencia de la República, Dios mediante» |
| 2026-05-11 | 352007 «Primera vuelta presidencial» (y su duplicado 352008) | «los palomistas […] deberán depositar su voto por Abelardo pensando en función de Colombia y ante la posibilidad de que Cepeda gane la presidencia» |
| **2026-06-21** | **354190 «Abelardo De La Espriella o Iván Cepeda»**, día de la segunda vuelta | «con Abelardo habrá institucionalidad, democracia y libertad; con Cepeda habrá instituciones propias, tiranía y abolición hasta de la libertad de prensa»; «Tenemos la plena seguridad de que Abelardo se constituirá en el líder hispanoamericano, dadas sus virtudes intelectuales y humanas». **Endoso explícito**, comprobado en el HTML crudo; publicado con fecha `2026-06-21T00:00:00-05:00` y sin autor |

---

## 4. Contrapesos (lo que contradice la dirección, y cuánto pesa)

1. **09-09-2026, [358422](https://www.elinformador.com.co/index.php/opinion/37-editorial/358422-esta-preparada-colombia-para-volver-al-porte-legal-de-armas) «¿Está preparada Colombia para volver al porte legal de armas?»** Cuestiona una medida del nuevo Gobierno: «Poner un arma de fuego en medio de esas situaciones puede convertir un conflicto que antes terminaba en insultos o golpes en una tragedia irreversible». Pero también recoge el otro lado («tampoco sería responsable ignorar el otro lado de la discusión»). **Peso: medio.** Es el único reparo de política al Gobierno entrante, y en tono de pregunta.
2. **11-09-2026, 358555 «Ahora hay que reconstruir».** Exige controles al gasto de la reconstrucción del terremoto: «la rapidez no puede confundirse con ausencia de controles». **Peso: bajo.** Es exigencia de transparencia, no crítica a una decisión tomada.
3. **29-09-2026, 359516 «Santa Marta no puede seguir esperando por el agua».** Sobre el descarte de las desalinizadoras: «Es una decisión que puede ser discutida desde el punto de vista técnico, financiero o ambiental». **Peso: bajo y local.** No critica al presidente; le pide una alternativa para Santa Marta.
4. **31-12-2025, 345540 «El renacer samario».** Reconoce el «afecto especial» de Petro por Santa Marta, pero el elogio es para el alcalde por «no cayó en la dinámica de pelear con el Presidente». **Peso: bajo.** Ver la tensión del §6.
5. **14-03-2026, 349067 «Una gran oportunidad comercial».** Registra que la recuperación del comercio con Venezuela «comenzó con la llegada de Petro al poder en 2022», y en la misma pieza duda de su promesa de gas. **Peso: bajo**, es descriptivo.
6. **Concesiones dentro de piezas hostiles, que no se cuentan aparte:** Petro «avanzó en materia de derechos» (08-08-2026, dentro de «¡Cesó la horrible noche!»).
7. **No hay ninguna pieza favorable a un candidato o gobierno de izquierda** en las 343 únicas. Tampoco ninguna que critique a Paloma Valencia o a De la Espriella como candidatos.
8. **Mucho de lo publicado no es partidista.** De las 343, unas 100 tienen postura nacional en la dirección D y 62 fiscalizan; el resto (unas 170) son internacionales, locales, de servicio o deporte. La casa no habla solo de política, pero cuando habla, habla siempre en la misma dirección.

---

## 5. Comprobaciones y avisos de lectura

- **Las 24 del revisor están todas** en la tabla y en la misma clase. Lo que el revisor no hizo fue leer el cuerpo: contó por título e intro, y la intro es «...» en casi todo el archivo. Por eso se quedó en 24.
- **El revisor excluyó como fiscalización** «El peor balance de un gobierno» (06-04-2026) y «Un legado de corrupción» (04-08-2026). Aquí cuentan: la primera desea «una copiosa votación» a Abelardo y Paloma («ojalá ambos arrojen una copiosa v[otación]»), y la segunda celebra que el 7 de agosto «Colombia sea nuevamente, un país viable». Si se pasan a F, el recuento baja a 98.
- **Piezas límite** («leve»): 14. Aunque se pasaran todas a M, quedarían 86 a 5.
- **343490 (18-11-2025) «Ataque sanguinario y cruel»** trata del Palacio de Justicia (historia), pero el rótulo es de presente: «los comunistas por su adoctrinamiento leninista falsean la historia». Se cuenta; sin ella, 99.
- **El 07-08-2026, en el lado de después:** 356885 «La posesión del nuevo presidente». Si se pasa al lado de antes, el resultado no cambia.
- **Las piezas del 22-06 al 06-08-2026** elogian al presidente electo mientras Petro todavía gobierna. Van en «antes» por fecha. No son fiscalización de nadie.

---

## 6. Tensión que se declara (no mueve el eje)

**La Alcaldía Distrital de Santa Marta es el mayor cliente público de la editora** (SECOP II: 10 contratos, $1.444.000.000 contratados entre 2020 y 2025, todos por contratación directa; el último, CO1.PCCNTR.8611101, de $72.000.000, firmado el 26-11-2025). **Dos editoriales sin firma elogian al alcalde Carlos Pinedo Cuello** sin declarar la relación:
- 31-12-2025, 345540 «El renacer samario»: «Hay que reconocer la labor del Alcalde, Carlos Pinedo Cuello, como gestor de los recursos requeridos…», 35 días después de ese contrato.
- 02-04-2026, 349934 «La ciudad engalanada con los turistas»: «El alcalde de Santa Marta, Carlos Pinedo Cuello, ha dispuesto lo necesario…».

Es el supuesto del protocolo («Si los editoriales elogian a quien contrata, eso se declara como tensión»). Desvelamiento, no acusación. **No entra como hecho** que un editorial sea consecuencia de un contrato.

---

## 7. Veredicto por condición

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | **Sí** | Editoriales sin firma de la sección Editorial (id 37); ninguna página lleva autor. Las piezas de agencia son internacionales y no se cuentan |
| 2. A los dos lados del cambio (07-08-2026), en 12 meses | **Sí** | 290 piezas antes y 63 después. Asimetría de contenido: a Petro en el poder se le rotula; a De la Espriella en el poder se le celebra |
| 3a. ≥10 piezas con postura | **Sí** | 100 (86 sin las leves) |
| 3b. ≥3 a cada lado del cambio, sin fiscalización | **Sí** | 67 antes y 33 después (58 y 28 sin las leves). Ninguna F suma |
| 3c. Proporción ≥3:1 | **Sí** | 100:5 = 20:1. Solo desde el 07-08: 33:3 = 11:1 |
| 4. Contrapesos escritos | **Sí** | §4, con peso asignado a cada uno |
| 5. Reproducible | **Sí** | §1 da las consultas; §2 da id, URL, fecha, clase y fragmento de cada pieza |

**Las cinco condiciones se cumplen.** Y hay **endoso explícito** (§3).

---

## 8. Magnitud: ¿sigue el tope de ±0,30?

**El texto del protocolo:**
- §1, «Cuánto mueve»: «Sin propiedad documentada con posición conocida (nivel 1) **ni endoso explícito**, **la magnitud no pasa de ±0,30**, la banda moderada. El valor exacto es un **juicio declarado**: se razona contra los medios vecinos de la escala y se escribe así. La regla 2 sigue en pie».
- §1, regla del polo fijo: «Un **endoso editorial** no es fiscalización: es tomar partido, y sigue siendo evidencia de primer orden».
- §5, regla 3, excepción: «cuenta como nivel 2 si cumple las cinco condiciones […] y mueve como mucho hasta ±0,30». **Este resumen no repite la salvedad del endoso.**

**Lectura.** El tope está escrito como condicional: rige cuando no hay ni nivel 1 con posición ni endoso. Aquí hay endoso. Así lo han leído los barridos anteriores: «dentro del tope de ±0,30: no hay propiedad documentada con posición nacional (nivel 1) ni endoso explícito» (El Diario de Pereira, §6) y «Si en cambio llega un endoso con nombre en la próxima elección, el tope de ±0,30 dejaría de aplicarse» (ídem, §7). **Con endoso, el protocolo permite superar ±0,30.** El valor sigue siendo juicio declarado contra los vecinos, y la regla 2 sigue en pie. La frase de la regla 3 del §5 debería alinearse con el §1, y esa decisión es del responsable editorial. *(Corregido el 2026-10-10: el §5 recoge ya la salvedad; ver `PROTOCOLO_JUICIO_EDITORIAL.md`, regla 3.)*

---

## 9. PROPUESTA (pendiente de la firma del responsable editorial)

**+0,45, derecha moderada.** Es el primer valor de la ficha: hoy no tiene ninguno.

**Por qué por encima de +0,30 (Archipiélago Press) y de +0,35 (El Colombiano):**
- Archipiélago llegó a +0,30 con 26 piezas y sin endoso. Aquí son 100, y la casa toma partido con nombre cuatro veces en el año (§3).
- El Colombiano (+0,35) celebró después de la segunda vuelta, pero sin endoso previo confirmado. El Informador endosó el día de la votación y pidió el voto por Abelardo tres semanas antes de la primera vuelta.
- Los rótulos («tirano», «terrorista dictatorial», «líder intergaláctico», «el más marxista entre los marxistas») no tienen equivalente en esos medios.

**Por qué por debajo de +0,55 (El Nuevo Siglo, que también endosó):**
- El nivel 1 está incompleto: hay editora, NIT y representante legal (RUES), pero **no constan los socios**.
- La clasificación es de un solo lector de la misma casa.
- Hay 3 reparos al Gobierno entrante, aunque débiles.
- La regla 2, en su espíritu: es el primer valor que se pone con la excepción por encima de ±0,30, y conviene no estrenarlo en el techo de la banda.

**Lecturas alternativas, que se declaran:**
- **+0,30**, si el responsable editorial lee la regla 3 del §5 como tope sin salvedad. La dirección no cambia; solo la magnitud.
- **+0,55**, a la par de El Nuevo Siglo, si se pesa más el endoso y los rótulos que la falta de socios.

**Lo que el barrido no sostiene:** 0,00, ni una banda que no sea la derecha.

**Lo que esta propuesta NO hace:**
- No hace firmable la ficha: falta el certificado de la Cámara de Comercio de Santa Marta, con los accionistas.
- No convierte la tensión con la Alcaldía (§6) en evidencia de orientación.

**Qué la refutaría:**
- que en los próximos meses la casa critique el programa del Gobierno De la Espriella (seguridad, Paz Total, fracking, porte de armas) en más de un editorial sin contrapartida;
- o que el certificado muestre accionistas cuya posición contradiga la dirección. Si, al contrario, muestra capital de una casa política de derecha, el valor se sostiene con nivel 1 y puede subir.
