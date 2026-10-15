# Barrido editorial: Proclama del Pacífico

| | |
|---|---|
| **Medio** | Proclama del Pacífico, Santander de Quilichao, Cauca (`proclama-del-pacifico`) |
| **Valor vigente** | 0,00, provisional de alta, sin firmar. Es 0,00 «por la regla 3, no por ausencia de evidencia». Dirección declarada en la ficha: izquierda, con encuadre pro-Cepeda de enero a junio de 2026 |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09) |
| **Ventana** | 2025-10-09 → 2026-10-09 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5 (`claude-opus-5-5`), a petición del responsable editorial, el 2026-10-09. Es de la misma casa que el autor de la ficha y que quien escribió la resolución del ciclo 2: su acuerdo no es aval |
| **Estado** | **DECIDIDO el 2026-10-09: se queda en 0,00**, con la inclinación a la izquierda como tensión, por el responsable editorial; firmado en bloque el 2026-10-10 (`DECISIONES.md`, «2026-10-09 · Reexamen de cinco fichas cerradas con la regla nueva»). Lo que más abajo dice «propuesta» o «pendiente» es el estado anterior a la decisión y se conserva como historia |
| **Decisión (2026-10-09)** | el responsable editorial: **se queda en 0,00.** Con la precisión del mismo día (fiscalizar no cuenta para el mínimo por lado), después del 07-08 solo suma 1 pieza, el rótulo del 24-08; el −0,25 que propone este barrido no se aplica. Se reconta hacia diciembre de 2026 (`DECISIONES.md`, «Reexamen de cinco fichas cerradas con la regla nueva»; ver la ficha) |

---

## 1. Método

- **robots.txt** (descargado el 2026-10-09): bloque de Yoast, `User-agent: * / Disallow:` (vacío) y `Sitemap: https://proclamadelpacifico.com/sitemap_index.xml`. No excluye a ningún agente ni ninguna ruta.
- **No se tocaron** eltiempo.com, cambiocolombia.com ni lasillavacia.com. No hubo buscador web.
- **Descarga.** Con `curl -sL --ssl-no-revoke` y el UA de un navegador (Chrome 126 en Windows), el 2026-10-09 (hora de Colombia).
  - `/wp-json/…` devuelve **403** con el desafío de Cloudflare («Just a moment…»).
  - La misma API por `/?rest_route=/wp/v2/…` devuelve **200**. Es la vía que se usó.
  - `/?rest_route=/wp/v2/users` devuelve **403 «Sorry, you have been blocked»**. No se insistió. El nombre del autor de los editoriales sale del `schema` de una pieza: «Alfonso José Luna Geller» (usuario 2 de la API).
- **El archivo entero de 12 meses, sin muestreo.**
  - Consulta: `/?rest_route=/wp/v2/posts&per_page=100&after=2025-10-09T00:00:00&before=2026-10-10T00:00:00&_fields=id,date,link,title,categories,author,content,excerpt`, páginas 1 a 45.
  - Resultado: **4.427 entradas** (cabecera `X-WP-Total: 4427`), del 2025-10-09 05:56 al 2026-10-09 18:32. Son 3.767 antes del 07-08-2026 y 660 desde ese día. Las 45 páginas dieron 200.
  - Las fechas son las de la API (`date`, hora local del sitio).
  - Las categorías se leyeron con `/?rest_route=/wp/v2/categories` (79).
- **Voz de la casa.** Es la sección «Editorial - Alfonso J. Luna Geller» (categoría 1914). Tiene **194 entradas** en la ventana, todas del usuario 2 (el director): 171 antes del 07-08 y 23 después.
  - Hay **2 entradas más rotuladas «Editorial Proclama del Pacífico»** fuera de la sección (24-02-2026 y 07-10-2026).
  - Total: **196 piezas** (172 antes, 24 después).
  - Algunas llevan como firma «Por Alfonso Luna Geller», «Unidad Investigativa Proclama del Pacífico», «Redacción Política», «Periscopio Político» o «Director de Proclama del Pacífico». Todo eso es la casa o su director, y cuenta (condición 1).
- **Excluidas dentro de la sección**, porque la postura es de una fuente atribuida y no de la casa:
  - la entrevista a Jorge Hernán Bastidas, del Pacto Histórico (18-01-2026);
  - la entrevista a Camilo Romero (24-02-2026, rotulada «Editorial»);
  - «CRIC responde a De La Espriella y descarta bloqueos» (08-10-2026), que es la nota de una rueda de prensa.
- **Qué no cuenta, y se declara:**
  - **Columnas de terceros:** 1.019 entradas en «Opinión» y sus 50 subcategorías de columnistas (848 antes, 171 después). No se clasificaron.
  - **Contenido pagado:** 66 «Edictos clasificados». No se clasificaron.
  - **Comunicados y notas informativas:** ver el §5.
- **Filtro de las 196.**
  - Primero se buscaron en el texto completo términos nacionales: Petro, Gobierno Nacional, Cepeda, Espriella/Abelardo, Uribe, Paloma, Pacto Histórico, derecha/izquierda, progresis-, uribis-, Fajardo, Centro Democrático, Francia, ministr-.
  - Las que tenían alguno se leyeron una a una: la entrada, las frases con esos términos y, cuando hacía falta, el final o la pieza entera.
  - Las demás se leyeron por título. Son locales (Popayán, Quilichao, la CEO, hospitales), culturales, de periodismo o internacionales.
- **Qué se clasificó.** Solo las piezas con postura sobre el Gobierno nacional, su candidato, la candidatura rival y el presidente electo o el nuevo Gobierno.
  - **I, dirección izquierda:**
    - celebra o disculpa al Gobierno Petro o a sus funcionarios;
    - favorece la candidatura de Cepeda;
    - critica a candidatos o figuras de la derecha (De la Espriella, Valencia, Uribe);
    - critica o fiscaliza al presidente electo o al Gobierno De la Espriella. Se marca «fiscaliza» para leerla con el polo fijo (§3).
  - **C, contrapeso:**
    - critica o fiscaliza al Gobierno Petro;
    - elogia o reconoce a De la Espriella o a su Gobierno.
  - **M (mixta):** tiene postura, pero reparte a los dos lados. No cuenta en la proporción.
  - **Fuera del recuento:**
    - los editoriales locales, aunque nombren a un ministerio;
    - los electorales de procedimiento o de encuestas sin inclinación: 01-12-2025, 10-01-2026, 23-02-2026, 12-05-2026, 23-05-2026, 31-05-2026 y 14-06-2026;
    - los internacionales sin Gobierno colombiano;
    - los de efemérides;
    - los que dan una postura atribuida a otro: 05-03-2026 (la doble calzada, con elogios de la ministra y del gobernador), 05-07-2026 y 20-07-2026.
  - Los elogios al gobernador del Cauca (12-09 y 07-10-2026) son locales y ya están en la ficha como tensión. No cuentan aquí.
- **Límite declarado.** La clasificación es el juicio de un solo verificador. Las URL y las fechas están en la tabla para que cualquiera la rehaga. Los cuerpos de las 4.231 entradas que no son de la casa no se leyeron uno a uno; ver el §5.

---

## 2. Tabla de piezas que cuentan (voz de la casa)

Todas son de la sección «Editorial - Alfonso J. Luna Geller»; ninguna de las dos rotuladas fuera de la sección tiene postura nacional que cuente. Las citas se buscaron literalmente en el `content.rendered` de la API, sin etiquetas.

| # | Fecha | Lado del 07-08 | Pieza | Clase | Postura |
|---|---|---|---|---|---|
| 1 | 20-10-2025 | antes | [Colombia ante la nueva forma de dominación internacional](https://proclamadelpacifico.com/colombia-ante-la-nueva-forma-de-dominacion-internacional/) | Izquierda | Favorable al gobierno Petro frente a Trump; rótulo «extrema derecha» |
| 2 | 21-10-2025 | antes | [El fallo absolutorio no equivale a inocencia](https://proclamadelpacifico.com/el-fallo-absolutorio-no-equivale-a-inocencia/) | Izquierda | Crítica a Uribe tras su absolución («no equivale a inocencia») |
| 3 | 08-11-2025 | antes | [LA ANTIPETROPOLÍTICA](https://proclamadelpacifico.com/la-antipetropolitica/) | Izquierda | Crítica a los precandidatos de oposición («antipetropolítica») |
| 4 | 15-11-2025 | antes | [De la paz a la indignación total](https://proclamadelpacifico.com/de-la-paz-a-la-indignacion-total/) | Izquierda | Disculpa al gobierno: reprocha a Vicky Dávila «atacar al gobierno nacional» (débil) |
| 5 | 29-11-2025 | antes | [De montonera a ciudadanía](https://proclamadelpacifico.com/de-montonera-a-ciudadania-voto-informado-colombia/) | Mixta | Mixta: critica a la «derecha extrema» y al «progresismo» que cierra filas «sin autocrítica» |
| 6 | 03-12-2025 | antes | [La República Popular del Cauca es una falacia](https://proclamadelpacifico.com/la-republica-popular-del-cauca-es-una-falacia/) | Izquierda | Disculpa a Petro por el Cauca («No fue Petro el que empezó…») |
| 7 | 07-12-2025 | antes | [La vida en Cauca es un riesgo](https://proclamadelpacifico.com/la-vida-en-cauca-es-un-riesgo/) | Contrapeso | Crítica al gobierno: «el Gobierno Nacional perdió el control» del Cauca |
| 8 | 11-12-2025 | antes | [Estados Unidos administra el narcotráfico. Colombia lo combate.](https://proclamadelpacifico.com/estados-unidos-administra-narcotrafico-colombia-lo-combate/) | Izquierda | Favorable a Petro frente a Trump («no encaja en el molde del sometimiento») |
| 9 | 16-12-2025 | antes | [LA PARADOJA DEL CAUCA](https://proclamadelpacifico.com/la-paradoja-del-cauca/) | Izquierda | Crítica a la candidatura de Paloma Valencia («recuperar el poder ejecutivo para el uribismo») |
| 10 | 18-12-2025 | antes | [LA TRAGEDIA DE BUENOS AIRES CONVERTIDA EN TARIMA ELECTORAL](https://proclamadelpacifico.com/tragedia-de-buenos-aires-convertida-en-tarima-electoral/) | Izquierda | Crítica al uso electoral de la tragedia de Buenos Aires contra la Paz Total (débil) |
| 11 | 30-12-2025 | antes | [Salario mínimo y fabricación de miedo preelectoral](https://proclamadelpacifico.com/salario-minimo-fabricacion-miedo-preelectoral/) | Izquierda | Favorable al decreto del salario mínimo; crítica a gremios y oposición |
| 12 | 02-01-2026 | antes | [El miedo como estrategia política](https://proclamadelpacifico.com/el-miedo-como-estrategia-politica/) | Izquierda | Ídem; «extrema derecha» |
| 13 | 03-01-2026 | antes | [La mentalidad de sumisión y anhelo colonial](https://proclamadelpacifico.com/la-mentalidad-de-sumision-y-anhelo-colonial-alfonso-luna-geller/) | Izquierda | Favorable a Petro frente a Trump; crítica a «la extrema derecha colombiana» |
| 14 | 04-01-2026 | antes | [Los muertos que nadie quiso contar](https://proclamadelpacifico.com/los-muertos-que-nadie-quiso-contar-alfonso-luna-geller/) | Izquierda | Crítica a Uribe, Duque, Valencia y Dávila (Venezuela) |
| 15 | 20-01-2026 | antes | [Censura y persecución: el peligroso riesgo que Colombia corre con Abelardo](https://proclamadelpacifico.com/censura-y-persecucion-el-peligroso-riesgo-que-colombia-corre-con-abelardo/) | Izquierda | Crítica al candidato De la Espriella («instrumentaliza el aparato de justicia») |
| 16 | 21-01-2026 | antes | [La tecnocracia del privilegio contra la sabiduría del territorio](https://proclamadelpacifico.com/la-tecnocracia-del-privilegio-contra-la-sabiduria-del-territorio-alfonso-luna-geller/) | Izquierda | Favorable al nombramiento del ministro de la Igualdad |
| 17 | 26-01-2026 | antes | [Unidad de Víctimas: Entre el festín politiquero y la burla a periodistas](https://proclamadelpacifico.com/unidad-de-victimas-entre-el-festin-politiquero-y-la-burla-a-periodistas/) | Contrapeso | Crítica al gobierno: Unidad de Víctimas, «festín politiquero» |
| 18 | 28-01-2026 | antes | [Incertidumbre en Unidad de Víctimas tras voraz festín del clan Barrancabermeja](https://proclamadelpacifico.com/incertidumbre-en-unidad-de-victimas-tras-voraz-festin-del-clan-de-barrancabermeja/) | Contrapeso | Crítica al gobierno: Unidad de Víctimas, «captura institucional» |
| 19 | 04-02-2026 | antes | [¡ZARPAZO A LA DEMOCRACIA!](https://proclamadelpacifico.com/zarpazo-a-la-democracia-cne-elecciones/) | Izquierda | A favor de Cepeda y del Pacto frente al CNE |
| 20 | 05-02-2026 | antes | [El CNE no derrotará a los colombianos](https://proclamadelpacifico.com/el-cne-no-derrotara-a-los-colombianos/) | Izquierda | A favor de Cepeda; crítica al CNE «uribista» |
| 21 | 20-02-2026 | antes | [La elección del Congreso y la trampa del tarjetón](https://proclamadelpacifico.com/la-eleccion-del-congreso-y-la-trampa-del-tarjeton-alfonso-luna-geller/) | Izquierda | A favor de Cepeda («unidad de la izquierda») |
| 22 | 09-03-2026 | antes | [Comparación de votos Paloma Valencia – Iván Cepeda induce a una lectura engañosa de los resultados](https://proclamadelpacifico.com/comparacion-de-votos-paloma-valencia-ivan-cepeda-induce-a-una-lectura-enganosa-de-los-resultados/) | Izquierda | A favor de Cepeda: discute la lectura del triunfo de Valencia |
| 23 | 14-03-2026 | antes | [Definitivamente, la derecha no es alternativa de poder](https://proclamadelpacifico.com/definitivamente-la-derecha-no-es-alternativa-de-poder/) | Izquierda | A favor de Cepeda: programa compartido «para lectura pública» |
| 24 | 14-03-2026 | antes | [El invisible Ministerio de la Igualdad permanece silenciado](https://proclamadelpacifico.com/el-invisible-ministerio-de-la-igualdad-permanece-silenciado/) | Contrapeso | Crítica al gobierno: el Ministerio de la Igualdad, «silenciado» |
| 25 | 15-03-2026 | antes | [El Cauca no es un feudo electoral sino la raíz de la República](https://proclamadelpacifico.com/el-cauca-no-es-un-feudo-electoral-sino-la-raiz-de-la-republica/) | Izquierda | Defensa de la fórmula Cepeda–Quilcué |
| 26 | 15-03-2026 | antes | [Proponer la división del Cauca delata incapacidad para gobernar](https://proclamadelpacifico.com/proponer-la-division-del-cauca-delata-incapacidad-para-gobernar/) | Izquierda | Crítica a la candidata Valencia (división del Cauca) |
| 27 | 25-03-2026 | antes | [Si todos se unen contra Cepeda, ganará la democracia](https://proclamadelpacifico.com/si-todos-se-unen-contra-cepeda-ganara-la-democracia/) | Izquierda | A favor de Cepeda («ganará la democracia») |
| 28 | 30-03-2026 | antes | [De la Espriella no supera exigencias para aspirar a la Presidencia](https://proclamadelpacifico.com/de-la-espriella-no-supera-exigencias-para-aspirar-a-la-presidencia/) | Izquierda | Crítica a De la Espriella («intenciones autoritarias») |
| 29 | 31-03-2026 | antes | [El prontuario que Uribe no puede borrar con esta campaña electoral](https://proclamadelpacifico.com/el-prontuario-que-uribe-no-puede-borrar-con-esta-campana-electoral/) | Izquierda | Crítica a Uribe; defensa de Cepeda |
| 30 | 01-04-2026 | antes | [El Banco de la República eligió partido antes del 31 de mayo](https://proclamadelpacifico.com/el-banco-de-la-republica-eligio-partido-antes-del-31-de-mayo/) | Izquierda | Favorable al gobierno Petro frente al Banco de la República |
| 31 | 10-04-2026 | antes | [Pedagogía del garrote, manipulación tecnológica y deber cívico](https://proclamadelpacifico.com/pedagogia-del-garrote-manipulacion-tecnologica-y-deber-civico/) | Izquierda | Crítica a la «extrema derecha» y a Valencia; a favor de Cepeda |
| 32 | 12-04-2026 | antes | [Felipe López Caballero le pone nombre y rostro al candidato que los grandes medios prefieren ignorar](https://proclamadelpacifico.com/felipe-lopez-caballero-le-pone-nombre-y-rostro-al-candidato-que-los-grandes-medios-prefieren-ignorar/) | Izquierda | A favor de Cepeda |
| 33 | 14-04-2026 | antes | [Noboa y Uribe actúan contra la soberanía en la región](https://proclamadelpacifico.com/noboa-y-uribe-actuan-contra-la-soberania-en-la-region/) | Izquierda | Favorable al gobierno Petro; crítica a Uribe y Noboa |
| 34 | 17-04-2026 | antes | [La injusta justicia colombiana](https://proclamadelpacifico.com/la-injusta-justicia-colombiana/) | Izquierda | Disculpa a los ministros de Petro; crítica a los legisladores «uribistas» |
| 35 | 25-04-2026 | antes | [Oportunidad histórica convertida en oportunidad perdida](https://proclamadelpacifico.com/oportunidad-historica-convertida-en-oportunidad-perdida/) | Contrapeso | Crítica al gobierno: la gestión de Francia Márquez «no estuvo a la altura» |
| 36 | 09-05-2026 | antes | [La Caja de Pandora de la UNGRD](https://proclamadelpacifico.com/la-caja-de-pandora-de-la-ungrd/) | Izquierda | Defensa del exministro Velasco («No se le acusa de haberse apropiado de un solo peso») |
| 37 | 13-05-2026 | antes | [Ahorro pensional atrapado por banqueros con aval del Consejo de Estado](https://proclamadelpacifico.com/ahorro-pensional-atrapado-por-banqueros-con-aval-del-consejo-de-estado/) | Izquierda | Favorable al gobierno Petro (traslado pensional) |
| 38 | 15-05-2026 | antes | [Lo que dicen las encuestas y lo que no dicen](https://proclamadelpacifico.com/lo-que-dicen-las-encuestas-y-lo-que-no-dicen/) | Izquierda | A favor de Cepeda en la lectura de encuestas (débil) |
| 39 | 18-05-2026 | antes | [El argumento se degenera a medida que nos acercamos a las urnas](https://proclamadelpacifico.com/el-argumento-se-degenera-a-medida-que-nos-acercamos-a-las-urnas/) | Izquierda | Crítica a Valencia y a De la Espriella («extrema derecha») |
| 40 | 20-05-2026 | antes | [Parece que el Estado ya se rindió y entregó la soberanía en el Cauca](https://proclamadelpacifico.com/parece-que-el-estado-ya-se-rindio-y-entrego-la-soberania-en-el-cauca/) | Contrapeso | Crítica al gobierno: el reclamo de Petro es «a su propio gobierno» |
| 41 | 21-05-2026 | antes | [El Gobierno Nacional debe declarar la emergencia en el Cauca](https://proclamadelpacifico.com/el-gobierno-nacional-debe-declarar-la-emergencia-en-el-cauca/) | Contrapeso | Crítica al gobierno: «debe declarar la emergencia en el Cauca» |
| 42 | 29-05-2026 | antes | [Miranda no se rinde ante la injuria ni la estigmatización](https://proclamadelpacifico.com/miranda-no-se-rinde-ante-la-injuria-ni-la-estigmatizacion/) | Izquierda | Crítica a «una extrema derecha» que estigmatiza a Miranda |
| 43 | 03-06-2026 | antes | [La soberanía electoral bajo asedio](https://proclamadelpacifico.com/la-soberania-electoral-bajo-asedio/) | Izquierda | Crítica a De la Espriella entre vueltas |
| 44 | 12-06-2026 | antes | [El rito burocrático del fracaso estatal](https://proclamadelpacifico.com/el-rito-burocratico-del-fracaso-estatal/) | Contrapeso | Crítica al gobierno: «atrapado en su propia inercia» |
| 45 | 21-06-2026 | antes | [El ganador debe esperar la proclamación oficial](https://proclamadelpacifico.com/el-ganador-debe-esperar-la-proclamacion-oficial/) | Izquierda | Preferencia declarada: «Quienes acompañamos la opción que aparece en segundo lugar» |
| 46 | 27-06-2026 | antes | [De la pasión ideológica al pragmatismo analítico](https://proclamadelpacifico.com/de-la-pasion-ideologica-al-pragmatismo-analitico/) | Izquierda | Preferencia declarada («quería que ganara Iván Cepeda»), con compromiso de auditar al entrante |
| 47 | 03-07-2026 | antes | [Crónica de una divisa esquizofrénica](https://proclamadelpacifico.com/cronica-de-una-divisa-esquizofrenica/) | Mixta | Mixta: reprocha a opositores y a defensores del gobierno por el dólar |
| 48 | 07-07-2026 | antes | [El Bloque de Defensa para la Seguridad Urbana revela más de lo que pretende resolver](https://proclamadelpacifico.com/el-bloque-de-defensa-para-la-seguridad-urbana-revela-mas-de-lo-que-pretende-resolver/) | Izquierda (fiscaliza) | Fiscaliza al presidente electo (decreto de seguridad): «más preguntas que aplausos» |
| 49 | 22-07-2026 | antes | [El Gobierno Nacional debe responderle a Quilichao y al Cauca por proyectos inconclusos](https://proclamadelpacifico.com/el-gobierno-nacional-debe-responderle-a-quilichao-y-al-cauca-por-proyectos-inconclusos/) | Contrapeso | Crítica al gobierno: «debe responderle a Quilichao» (en parte atribuida a la exalcaldesa; débil) |
| 50 | 09-08-2026 | después | [Un domingo para mirar de frente lo que ocurrió en Cali](https://proclamadelpacifico.com/un-domingo-para-mirar-de-frente-lo-que-ocurrio-en-cali/) | Izquierda (fiscaliza) | Fiscaliza la posesión de De la Espriella (a partir de una columna de Coronell; leve) |
| 51 | 19-08-2026 | después | [La pobreza del Pacífico pone a prueba a De la Espriella](https://proclamadelpacifico.com/la-pobreza-del-pacifico-pone-a-prueba-a-de-la-espriella/) | Izquierda (fiscaliza) | Fiscaliza sin rótulo: «La pobreza del Pacífico pone a prueba a De la Espriella» |
| 52 | 21-08-2026 | después | [Oficinas de prensa que fabrican semidioses con posesivos y mayúsculas](https://proclamadelpacifico.com/oficinas-de-prensa-que-fabrican-semidioses-con-posesivos-y-mayusculas/) | Izquierda (fiscaliza) | Fiscaliza el lenguaje cortesano de una oficina de prensa del nuevo gobierno |
| 53 | 24-08-2026 | después | [La violencia política que se está ensayando](https://proclamadelpacifico.com/la-violencia-politica-que-se-esta-ensayando/) | Izquierda | Rótulo «gobierno de derecha extrema» solo para el entrante; crítica a dirigentes de derecha |

---

## 3. Recuento

| | I (izquierda) | C (contrapeso) | M (mixta, no cuenta) | Total con postura |
|---|---|---|---|---|
| Antes del 07-08-2026 | **38** | **9** | 2 | 49 |
| Desde el 07-08-2026 | **4** | **0** | 0 | 4 |
| **Total** | **42** | **9** | 2 | **53** |

**Proporción global: 42 a 9, es decir 4,7 a 1.** Sin las 4 piezas de fiscalización a De la Espriella (#48, #50, #51 y #52) queda en 38 a 9 (4,2 a 1). Si además las piezas «débiles» de dirección I (#4, #10, #38) pasaran a M, quedaría en 35 a 9 (3,9 a 1). Las tres lecturas pasan de 3 a 1.

**De qué tratan las 38 I de antes del cambio:**
- **24 son sobre candidaturas:** el CNE frente a Cepeda, la lectura de encuestas y consultas, críticas a De la Espriella, Valencia y Uribe, y la preferencia declarada (#45 y #46). Son el «encuadre asimétrico entre candidatos» que la regla del polo fijo trata como evidencia de primer orden.
- **13 celebran o disculpan al Gobierno Petro:** #1, #4, #6, #8, #11, #12, #13, #16, #30, #33, #34, #36 y #37.
- **1 fiscaliza al presidente electo:** #48, del 07-07-2026.

**La lectura del polo fijo**, que separa fiscalizar a quien manda de lo que no lo es:

| Trato al gobierno **en ejercicio** | Favorables o disculpas | Críticos |
|---|---|---|
| Petro, mientras gobierna (oct. 2025 – 06-08-2026, 10 meses) | **13** | **9** |
| De la Espriella, ya en el poder (07-08 → 09-10-2026, 2 meses) | **0** | **4** |

- **Con Petro**, la casa celebra y disculpa más de lo que critica:
  - frente a Trump, frente al Banco de la República y frente al Consejo de Estado;
  - el salario mínimo;
  - los ministros procesados («No se le acusa de haberse apropiado de un solo peso», #36).

  Pero también lo fiscaliza, y no solo por el Cauca: la Unidad de Víctimas (#17, #18), el Ministerio de la Igualdad (#24) y la gestión de Francia Márquez (#35).
- **Con De la Espriella**, ni una pieza favorable en dos meses. De las 4 críticas:
  - una le pone rótulo ideológico: «El país estrenó el 7 de agosto un gobierno de derecha extrema» (#53). A Petro no se le aplicó ningún rótulo equivalente en las 196 (se buscaron «extrema izquierda», «izquierda radical», «izquierda extrema», «ultraizquierda» y «comunis-»: solo aparecen en citas de candidatos de la derecha);
  - las otras tres son fiscalización sin adjetivo: la pobreza del Pacífico «pone a prueba» al presidente (#51), una oficina de prensa cortesana (#52) y la posesión, leída a partir de una columna de Coronell (#50).
- **La asimetría de la regla está ahí:** a Petro se le celebraba y disculpaba mientras gobernaba; a De la Espriella solo se le fiscaliza, y se le rotula. Pero **la mitad posterior es corta y escasa**. De los 24 editoriales de después del cambio, solo 4 tienen postura nacional. Los demás son locales: la disputa con la Alcaldía de Popayán, Patía, el gobernador y Quilichao.

---

## 4. Contrapesos (lo que contradice la dirección, y cuánto pesa)

1. **La casa fiscaliza al Gobierno Petro mientras gobierna:** 9 piezas en 10 meses.
   - Las más claras: la Unidad de Víctimas como «caja menor de la politiquería corrupta» (#17, 26-01-2026), el Ministerio de la Igualdad, que «permanece silenciado» (#24, 14-03-2026), y la gestión de Francia Márquez, que «no estuvo a la altura del momento histórico» (#35, 25-04-2026).
   - Las demás son reclamos por el Cauca: #7, #40, #41, #44 y #49.
   - **Peso: medio.** Es crítica real y en voz propia, y algunas apuntan a nombramientos del propio Gobierno. Pero por el polo fijo es fiscalizar a quien manda, que por sí sola no sitúa. No compensa las 24 piezas de candidaturas.
2. **Dos piezas mixtas antes del cambio:**
   - #5 (29-11-2025): «una parte del progresismo responde cerrando filas sin autocrítica»;
   - #47 (03-07-2026): sobre el dólar, reprocha a la oposición y a «los defensores del gobierno».
   - **Peso: bajo.**
3. **Tono del director tras la derrota de su opción:**
   - 21-06-2026 (#45): «Aceptaré la decisión oficial, aunque no corresponda a mi preferencia».
   - 27-06-2026 (#46): «Lo nocivo no es tener convicciones; lo perverso es convertir un medio de comunicación en el vocero exclusivo y ciego de una tendencia electoral», y el compromiso de «auditar a sus ministros y confrontar sus promesas con los hechos».
   - Con el entrante, el tono posterior es más medido: #51 no insulta.
   - **Peso: medio para la magnitud.** No cambia la dirección, pero sí explica que después del 07-08 haya fiscalización y no hostilidad sostenida.
4. **No hay recomendación de voto.** Se buscaron en las 196 «votar por Cepeda», «invitamos a votar», «respaldamos», «apoyamos», «nuestro candidato», «recomendamos votar», «votaré por» y «mi voto».
   - Solo aparece el 28-12-2025, en «Votaré solo por candidatos con propuestas pertinentes», que no tiene postura: «yo ya tengo cálculos más o menos precisos sobre cómo será mi voto […] Oportunamente detallaré todos los porqués». En lo leído, no lo detalló antes de las urnas.
   - La víspera de la segunda vuelta (14-06-2026), el editorial pide votar y aceptar el resultado sin nombrar a nadie.
   - **Peso: alto para la magnitud.** Ver el §7 sobre el endoso.
5. **La mitad posterior es corta.** 4 piezas en dos meses, una sola con rótulo.
   - **Peso: alto para la magnitud, no para la dirección.** No hay ni una pieza de después que vaya en sentido contrario, pero 4 es apenas una por encima del mínimo de la regla.
6. **Conflictos de la casa ya declarados en la ficha:** la contratación con la Gobernación del Cauca, los elogios al gobernador y las disputas con Popayán y Patía.
   - **Son locales y no tocan el eje nacional.** No suman ni restan aquí.
   - **Dato para la ficha, sin efecto aquí:** el medio informó el 06-05-2026 que el capítulo Cauca de Colombia Renaciente, el partido con el que fue candidato el gobernador, respaldó a Cepeda ([fuente](https://proclamadelpacifico.com/elias-larrahondo-y-colombia-renaciente-apoyan-candidatura-de-ivan-cepeda/)). Es una declaración del exgobernador Larrahondo y no sitúa al gobernador Guzmán. La laguna de la ficha sobre el partido sigue abierta.

---

## 5. Comprobación complementaria: titulares de noticias (no cuenta)

- **Búsqueda:** sobre las 4.427 entradas descargadas, sin contar la sección Editorial ni las columnas, titulares con Petro, Espriella/Abelardo, Cepeda, Gobierno Nacional, Uribe, Paloma o Pacto Histórico.
- **Resultado:** 191 titulares de noticias, 177 antes y 14 después. Hay otros 34 en columnas, que no cuentan.
- **Qué muestran:** son casi todos atributivos y planos: «Petro responde a Trump…», «De la Espriella anuncia…», «Cepeda lidera intención de voto…», «De La Espriella ganó y Colombia giró a la derecha».
- **Los dos titulares con calificativo** resultaron ser de terceros:
  - «Lo que no se logró en 30 años Petro lo hizo posible…» (04-03-2026) lo firma Carlos Villamil, «Comunicador Social-Periodista»;
  - «Presidente Petro, decisiones firmes para el Cauca» (15-11-2025) es el pronunciamiento del gobernador.
- **Después del cambio:** «62 menores murieron en operaciones durante gobierno Petro» (31-08) y «El nuevo Gobierno pone bajo lupa la administración Petro» (19-08) son informativas y atribuidas. Ninguna noticia elogia ni ataca a De la Espriella en voz propia.
- **Lectura:** la sección informativa es plana y no contradice ni refuerza el editorial. **La dirección está entera en la voz del director.**
- **Límite:** es un barrido de titulares, no de cuerpos.

---

## 6. Veredicto por condición

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | **Sí** | Las 53 piezas son de la sección Editorial firmada por el director, Alfonso José Luna Geller. La regla cuenta lo «firmado por la casa o su director». Se excluyeron 2 entrevistas y 1 nota de rueda de prensa. No cuenta ninguna columna, comunicado ni pieza pagada |
| 2. A los dos lados del cambio (07-08-2026), en 12 meses | **Sí, con la mitad posterior corta** | 49 piezas antes y 4 después. Hay asimetría: con Petro, 13 piezas que celebran o disculpan y 9 que critican; con De la Espriella, 0 y 4, con un rótulo ideológico que no se aplicó al anterior. No es solo fiscalizar a quien manda: antes de las urnas hay 24 piezas de encuadre entre candidatos y una preferencia declarada |
| 3a. ≥10 piezas con postura | **Sí** | 53 |
| 3b. ≥3 a cada lado del cambio | **Sí, por uno** | 49 antes y 4 después. **Aviso:** las 4 de después son 3 de fiscalización y 1 con rótulo. Cuentan como la mitad «fiscalizar a un lado» de la asimetría, igual que en el barrido de El Diario (Pereira) cuentan las críticas a Petro. Si el responsable editorial leyera que la fiscalización de después no es «postura», quedaría 1 y la condición no se cumpliría |
| 3c. Proporción ≥3:1 | **Sí** | 42:9 = 4,7:1 en el global; 38:9 (4,2:1) sin la fiscalización a De la Espriella; 35:9 (3,9:1) si además se pasan las débiles a M. Desde el 07-08 sola, 4:0 |
| 4. Contrapesos escritos | **Sí** | §4, con peso asignado a cada uno |
| 5. Reproducible | **Sí** | La tabla del §2 tiene URL, fecha y clasificación. La consulta exacta está en el §1 |

**Las cinco condiciones se cumplen**, con la 3b en el mínimo. La regla permite mover el número dentro del tope de ±0,30: no hay propiedad documentada con posición (nivel 1), porque los asociados de la EAT no constan, ni endoso explícito (ver abajo).

---

## 7. PROPUESTA (pendiente de la firma del responsable editorial)

**−0,25, izquierda moderada.** Sale de la mixta, pero ahora como conducta medida y no como inclinación de nivel 5 retenida por la regla 3.

### ¿El 21-06-2026 es un endoso explícito que levanta el tope?

**No.** Es una **preferencia declarada** de la casa, que es evidencia de primer orden para la **dirección**, pero no el «endoso explícito» que el protocolo pone al lado de la propiedad para dejar pasar del ±0,30:

1. **Llega después del voto.** Se publicó la noche de la segunda vuelta, con los resultados ya dados: «Ese resultado no era el que personalmente esperaba». Un endoso es pedir el voto antes de la elección. Lo de aquí es reconocer, ya contado el voto, de qué lado se estuvo.
2. **No hay recomendación de voto en todo el año.** La búsqueda del §4.4 no encuentra ninguna. El anuncio del 28-12-2025 («Oportunamente detallaré…») no se cumplió en la sección antes de las urnas. Y la víspera (14-06-2026) se pidió votar sin nombrar a nadie.
3. **La casa enmarca la preferencia como personal.** El 21-06 dice «personalmente» y «mi preferencia». El 27-06 habla de «mis sólidas creencias políticas» y escribe que lo perverso es convertir el medio en «vocero exclusivo y ciego de una tendencia electoral». El «Quienes acompañamos» es plural y puede leerse como la casa. **Esa ambigüedad no se resuelve a favor de levantar un tope:** el protocolo pide un endoso *explícito*, y la regla 2 dice que, ante la duda, se va hacia la mixta.
4. **Compartir el programa de Cepeda «para lectura pública»** (14-03) es difundirlo, no pedir el voto.

**Si el responsable editorial lo leyera como endoso**, el tope dejaría de aplicarse, pero no habría razón para pasar de −0,30. La mitad posterior del barrido es demasiado corta para sostener una magnitud mayor.

### Por qué no 0,00

El barrido no muestra la misma conducta con los dos gobiernos:
- **con Petro:** 13 piezas que celebran o disculpan, frente a 9 críticas;
- **con De la Espriella:** 0 frente a 4, con el rótulo «derecha extrema» que nunca se usó para el otro lado;
- **antes de las urnas:** 24 piezas de encuadre entre candidatos, todas en la misma dirección, y una preferencia declarada.

El 0,00 del 2026-10-08 se sostuvo por la regla 3, y la ficha ya lo decía: «no por ausencia de evidencia». También por coherencia con El Pilón. **La regla nueva se aplica el mismo día a los dos**, así que esa coherencia ya no lo retiene.

### Por qué no −0,30

- **El techo de la regla no está justificado aquí.** Abra Noticias (propuesto en −0,25) no tiene ni una pieza crítica con el Gobierno Petro en 12 meses. Proclama tiene 9, algunas contra nombramientos del propio Gobierno, y dos mixtas.
- **La mitad posterior es la más débil de los casos de la tanda:** 4 piezas, una sola con rótulo, y un tono que el director se comprometió a mantener en la auditoría y no en la hostilidad.
- **Ponerlo más a la izquierda que Abra**, con más contrapesos y menos piezas posteriores, no se sostiene.

### Por qué no −0,20 o −0,15

- **−0,20 es el borde del umbral** de la izquierda moderada. Es el mismo motivo por el que El País España se fijó en −0,25.
- **−0,15 (mixta)** sería contar el barrido y no creerlo. La regla 2 decide entre bandas *ante la duda*, y aquí la duda no está en la dirección, que es la más documentada del catálogo regional: preferencia declarada más seis meses de encuadre. La duda está en la magnitud, y esa se resuelve dentro de la banda, en su parte más cercana a la mixta.

### Por qué −0,25, a la altura de El País España y de Abra Noticias

- **Frente a El País España (−0,25):** El País fiscaliza a los dos gobiernos y adjetiva de forma asimétrica. Proclama hace lo mismo, con más volumen y con una toma de partido electoral más explícita. Pero su voz posterior al cambio es más escasa. Se compensan.
- **Frente a Abra Noticias (−0,25, propuesto):** Proclama tiene más partidismo de campaña (preferencia declarada, programa compartido) y más contrapesos (9 frente a 0). Se compensan.
- **Frente a La Silla Vacía (−0,10):** está claramente más a la izquierda. La Silla no tiene preferencia declarada ni encuadre sostenido entre candidatos en su voz propia.

### Lectura alternativa, que se declara

**0,00, ahora sostenido como «no alcanza».** Es la salida si el responsable editorial lee la condición 3b de forma estricta, es decir, si la fiscalización a De la Espriella no cuenta como «pieza con postura» después del cambio y solo queda #53. En ese caso, la dirección izquierda sigue declarada como tensión en la ficha, igual que hoy, con el barrido como apoyo, y se revisaría cuando la mitad posterior tenga más piezas.

**Lo que el barrido no sostiene** es una dirección derecha, ni un 0,00 descrito como «misma conducta con los dos gobiernos».

### Lo que esta propuesta NO hace

- No hace firmable la ficha.
- No resuelve los asociados de la EAT: falta el certificado de la Cámara de Comercio del Cauca.
- No toca las tensiones locales: la contratación con la Gobernación, los elogios al gobernador y el contrato de «sondeos de opinión».

### Qué la refutaría

- Que en los próximos meses la sección Editorial **elogie** políticas del Gobierno De la Espriella, en seguridad, economía o Paz Total, con la misma frecuencia con que elogió las de Petro.
- O que el **rótulo ideológico** de #53 quede como pieza aislada, y la fiscalización posterior sea tan plana como la que hizo de Petro.

Cualquiera de las dos llevaría el número hacia −0,15 o 0,00.

Si en la próxima elección (2027, regionales) la casa pide el voto con nombre, eso sí sería endoso explícito.

---

## 8. Avisos

- **Una sola lectura.** La clasificación es de un verificador de la misma casa que el autor de la ficha. Las piezas límite se marcaron «débil» (#4, #10, #38, #49) o «leve» (#50). Aunque las débiles de dirección I pasaran a M, el recuento quedaría en 39 a 9, que sigue por encima de 3 a 1.
- **Cloudflare.** El sitio bloquea `/wp-json/` y el listado de usuarios. Se usó la ruta alternativa `?rest_route=`, que el propio WordPress publica, sin forzar nada. Si el medio la cierra, la reproducción tendrá que hacerse por las páginas de la sección (`/tema/noticias-proclama-del-pacifico/editorial-alfonso-j-luna-geller/`, que dio 200).
- **La ficha cita «ocho páginas, 160 títulos del 16-12-2025 al 08-10-2026»** para la sección. La API da 194 en la ventana completa, desde el 09-10-2025. No hay contradicción: son ventanas distintas.
- **Las fechas** son las de la API. Coinciden con las de la ficha para todas las piezas que esta cita.
- **Datos personales.** Este documento no contiene cédulas, teléfonos ni direcciones de personas naturales.
- **Las piezas citadas** se comprobaron literalmente en el texto descargado el 2026-10-09: #15, #23, #27, #28, #29, #36, #43, #45, #46 y #53. Se guardan en el scratchpad de la sesión, no en el repositorio.
