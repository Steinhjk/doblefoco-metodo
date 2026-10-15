# Barrido editorial — The Archipielago Press (`archipielago-press`)

| | |
|---|---|
| **Para qué** | Condición 5 («reproducible») de la regla «Evidencia editorial histórica» de `PROTOCOLO_JUICIO_EDITORIAL.md` (2026-10-09) |
| **Ficha** | `fichas/archipielago-press.md` |
| **Resolución de origen** | `revision-externa/respuestas/opus-5-5-archipielago-press.md` (barrido de 873 títulos, 2026-10-08) |
| **Recontado** | 2026-10-09 (hora de Colombia), por Claude Code, sobre el sitio |
| **Resultado** | **Cumple las cinco condiciones.** 26 piezas con postura en voz de la casa en la misma dirección (22 antes del cambio de gobierno y 4 después), más 2 del propio 07-08-2026; 2 en contra, ambas después. Proporción 13 a 1 |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas y el método
> están aquí para eso. **La clasificación de cada pieza es juicio de un solo
> lector**, de la misma casa que el autor de la ficha y que el revisor.

---

## Método

1. **robots.txt** de `www.thearchipielagopress.co`, leído el 2026-10-09: solo
   `Disallow: /wp-admin/`. No menciona a ClaudeBot ni a anthropic-ai.
2. **Universo:** todas las entradas publicadas desde el 2025-10-08 (regla del
   presente), por la API pública de WordPress:
   `https://www.thearchipielagopress.co/wp-json/wp/v2/posts?after=2025-10-08T00:00:00&per_page=100&page=1…9`
   (`X-WP-Total: 873`), descargadas el 2026-10-09 con `curl -sL --ssl-no-revoke`
   y User-Agent de navegador. **698 antes del 07-08-2026 y 175 desde ese día**
   (la última, del 05-10-2026). Las fechas son el `date` de la API, en hora de
   Colombia.
3. **Filtro de términos** sobre los 873 títulos: `petro`, `espriella`,
   `abelardo`, `cepeda`, `presidente`, `ministr`, `gobierno nacional`,
   `uribe`, `pacto hist`, `centro democr` (276 títulos), y una segunda pasada
   por `petrism`, `izquierd`, `mamert`, `progresis`, `tigre`, `derecha`,
   `dictad`, `paz total`, `gobierno del cambio`, `santos`, `farc`. Más la
   sección «Editorial» entera (6 piezas en 12 meses).
4. **Lectura uno por uno** de esos títulos, y del cuerpo de las piezas que
   entran en la cuenta o la discuten.
5. **Qué cuenta como voz de la casa** (condición 1): el editorial sin firma,
   lo firmado por el director, y los **titulares, entradillas y análisis
   propios no atribuidos** a una fuente. Muchas notas del medio llevan el
   cuerpo de otro medio («De EL TIEMPO», «Fuente: El Colombiano»); en esas
   **solo cuenta el titular**, cuando el calificativo es del medio y no está
   entre comillas ni atribuido. **No cuentan:** columnas firmadas por
   terceros, reimpresiones, comunicados reescritos, citas atribuidas en el
   titular («…: Ministro de Hacienda») ni contenido comercial.
6. **Dirección:** «derecha» = hostil a Petro, al petrismo o a Cepeda con
   calificativo propio, o favorable a De la Espriella. «En contra» = hostil
   a De la Espriella o a su Gobierno, o favorable a Petro o a Cepeda, en
   voz de la casa.

**Límite que se declara:** con Petro en el poder, una parte de la hostilidad
es fiscalización, que por sí sola no sitúa a nadie (regla del polo fijo). Lo
que sitúa es la asimetría: el mismo calificativo hostil cuando Petro ya no
manda, y la celebración del lado contrario antes y después. Por eso se da
también la cuenta sin las piezas de fiscalización (ver «Recuento»).

---

## Antes del cambio de gobierno (2025-10-08 → 2026-08-06): 22 en la dirección

| Fecha | Pieza | Voz | Clasificación |
|---|---|---|---|
| 11-10-2025 | [Representante a la Cámara, Jorge Méndez Hernández confirma las denuncias hechas por The Archipiélago Press este fin de semana sobre la menti…](https://www.thearchipielagopress.co/representante-a-la-camara-jorge-mendez-hernandez-confirma-las-denuncias-hechas-por-the-archipielago-press-este-fin-de-semana-sobre-la-mentira-publica-del-presidente-gustavo-petro-respecto-a-la-supues/) | casa (titular; denuncia propia) | crítica a Petro con calificativo propio («la mentira pública del presidente») |
| 12-10-2025 | [¿Está celoso? Presidente Petro arremete contra María Corina Machado tras su premio Nobel de Paz y cuestiona carta de 2018 en la que pidió ay…](https://www.thearchipielagopress.co/esta-celoso-presidente-petro-arremete-contra-maria-corina-machado-tras-su-premio-nobel-de-paz-y-cuestiona-carta-de-2018-en-la-que-pidio-ayuda-a-benjamin-netanyahu/) | casa (titular; cuerpo de El Tiempo) | crítica a Petro con calificativo propio («¿Está celoso?») |
| 12-10-2025 | [Gobierno convirtió la prevención de un plan criminal entre dos exraditables presos en gesto de paz con cumbre presidencial e intervención de…](https://www.thearchipielagopress.co/gobierno-convirtio-la-prevencion-de-un-plan-criminal-entre-dos-exraditables-presos-en-gesto-de-paz-con-cumbre-presidencial-e-intervencion-de-senadora-oficialista-y-ministros-cuando-lo-que-ameritaba-er/) | casa (titular; cuerpo de Noticias RCN) | crítica al Gobierno Petro con juicio propio («cuando lo que ameritaba era un control penitenciario») |
| 30-10-2025 | [Proyecto de Asamblea constituyente de Gustavo Petro busca una dictadura constituyente que eliminará la oposición, la democracia y el orden c…](https://www.thearchipielagopress.co/proyecto-de-asamblea-constituyente-de-gustavo-petro-busca-una-dictadura-constituyente-que-eliminara-la-oposicion-la-democracia-y-el-orden-constitucional/) | casa (titular y entradilla) | hostil a Petro («dictadura constituyente») |
| 30-10-2025 | [Petro el super tuitero: en vez de gobernar, el mandatario solo parece dedicarse a pontificar de lo divino y lo humano y a echar vainazos. En…](https://www.thearchipielagopress.co/petro-el-super-tuitero-en-vez-de-gobernar-el-mandatario-solo-parece-dedicarse-a-pontificar-de-lo-divino-y-lo-humano-y-a-echar-vainazos-en-un-solo-dia-publico-75-mensajes/) | casa (titular) | hostil a Petro («Petro el super tuitero… echar vainazos») |
| 22-12-2025 | [Congresistas de izquierda firmaron carta de respaldo a favor de 11 terroristas que han sembrado caos haciéndolo pasar como protesta social](https://www.thearchipielagopress.co/congresistas-de-izquierda-firmaron-carta-de-respaldo-a-favor-de-11-terroristas-que-han-sembrado-caos-haciendolo-pasar-como-pr/) | casa (titular) | hostil a la izquierda («11 terroristas… haciéndolo pasar como protesta social») |
| 12-01-2026 | [En pocos minutos el petrismo pasó de quemar la bandera y el rostro de Donald Trump, al jubilo y la adulación al presidente norteamericano po…](https://www.thearchipielagopress.co/en-pocos-minutos-el-petrismo-paso-de-quemar-la-bandera-y-el-rostro-de-donald-trump-al-jubilo-y-la-adulacion-a/) | casa (titular) | hostil al petrismo («júbilo y la adulación») |
| 13-01-2026 | [A través de los impuestos, todos los colombianos estamos pagando abogados de 10.000 millones para que Gustavo Petro se defienda jurídicament…](https://www.thearchipielagopress.co/a-traves-de-los-impuestos-todos-los-colombianos-estamos-pagando-abogados-de-10-000-millones-para-que-gustavo-petro-se-defienda-juridicamente-luego-de-haber-sido-incluido-en-la-lista-clinton/) | casa (titular; cuerpo de El Colombiano) | hostil a Petro («todos los colombianos estamos pagando») |
| 28-01-2026 | [¿A qué juega el presidente? Faltando una semana de su anunciada reunión con Donald Trump en la Casa Blanca, Gustavo Petro lanza críticas con…](https://www.thearchipielagopress.co/a-que-juega-el-presidente-faltando-una-semana-de-su-anunciada-reunion-con-donald-trump-en-la-casa-blanca/) | casa (titular; cuerpo, un trino de tercero) | hostil a Petro («¿A qué juega el presidente?») |
| 28-01-2026 | [Sin pandemia, cuarentena, huracanes, ni paro nacional, Petro se ha gastado en 3 años y medio de gobierno 87 billones mas que el gobierno de …](https://www.thearchipielagopress.co/sin-pandemia-cuarentena-huracanes-ni-paro-nacional-petro-se-ha-gastado-en-3-anos-y-medio-de-gobierno-87-billones-mas-que-el-gobierno-de-duque/) | casa (titular) | hostil al Gobierno Petro (gasto frente a Duque) |
| 03-02-2026 | [Las razones que alegaba el petrismo como causales para reformar la salud se han triplicado en este gobierno; quejas y tutelas por falta de a…](https://www.thearchipielagopress.co/las-razones-que-alegaba-el-petrismo-como-causales-para-reformar-la-salud-se-han-triplicado-en-este-gobierno-quejas-y-tutelas-por-falta-de-atencion-y-medicamentos-arreciaron/) | casa (titular; cuerpo de El Colombiano) | hostil al petrismo («se han triplicado en este gobierno») |
| 17-03-2026 | [Nunca antes ningún gobierno acumuló tanta deuda nueva como el gobierno de Petro, ni siquiera en pandemia: en 3 años Petro endeudó a Colombia…](https://www.thearchipielagopress.co/nunca-antes-ningun-gobierno-acumulo-tanta-deuda-nueva-como-el-gobierno-de-petro-ni-siquiera-en-pandemia-en-3-anos-petro-endeudo-a-colombia-en-400-billones-de-pesos/) | casa (titular) | hostil al Gobierno Petro («Nunca antes ningún gobierno…») |
| 30-03-2026 | [A Gustavo Petro no le gusta la solución que Bukele le dio a la criminalidad en El Salvador donde bajó la delincuencia casi a cero.](https://www.thearchipielagopress.co/a-gustavo-petro-no-le-gusta-la-solucion-que-bukele-le-dio-a-la-criminalidad-en-el-salvador-donde-bajo-la-delincuencia-casi-a-cero/) | casa (titular) | hostil a Petro, elogio implícito a Bukele |
| 07-04-2026 | [El asalto político del gobierno Petro al Banco de la República](https://www.thearchipielagopress.co/el-asalto-politico-del-gobierno-petro-al-banco-de-la-republica/) | casa (titular y entradilla) | hostil al Gobierno Petro («El asalto político») |
| 14-04-2026 | [Aunque no tiene facultades para hacerlo, el 'dictador' Petro amenaza con destituir alcaldes por el paro nacional contra el impuesto confisca…](https://www.thearchipielagopress.co/aunque-no-tiene-facultades-para-hacerlo-el-dictador-petro-amenaza-con-destituir-alcaldes-por-el-paro-nacional-contra-el-impuesto-confiscatorio-predial/) | casa (titular) | hostil a Petro («el 'dictador' Petro», «impuesto confiscatorio») |
| 24-05-2026 | [El Malecón del Río tuvo un multitudinario lleno del candidato a la presidencia de la república Abelardo de la Espriella.](https://www.thearchipielagopress.co/el-malecon-del-rio-tuvo-un-multitudinario-lleno-del-candidato-a-la-presidencia-de-la-republica-abelardo-de-la-espriella/) | casa (titular y cuerpo) | favorable a De la Espriella («multitudinario lleno», «puro fervor popular» citado) |
| 01-06-2026 | [El fenómeno político de Abelardo de la Espriella: ganó la primera vuelta con 10,3 millones de votos y derrotó a las encuestadoras que lo ubi…](https://www.thearchipielagopress.co/el-fenomeno-politico-de-abelardo-de-la-espriella-gano-la-primera-vuelta-con-103-millones-de-votos-y-derroto-a-las-encuestadoras-que-lo-ubicaban-detras-de-sus-rivales/) | casa (titular; cuerpo de La Silla Vacía) | favorable a De la Espriella («El fenómeno político») |
| 05-06-2026 | [‘Fraude’ electoral que denunció Petro es un montaje ¿de quién?](https://www.thearchipielagopress.co/fraude-electoral-que-denuncio-petro-es-un-montaje-de-quien/) | casa (titular; cuerpo de El Colombiano) | hostil a Petro («‘Fraude’… es un montaje ¿de quién?») |
| 15-06-2026 | [Iván Cepeda Castro afianza su rol de acusador de sus oponentes políticos y anuncia nueva denuncia penal contra Abelardo de la Espriella por …](https://www.thearchipielagopress.co/ivan-cepeda-castro-afianza-su-rol-de-acusador-de-sus-oponentes-politicos-y-anuncia-nueva-denuncia-penal-contra-abelardo-de-la-espriella-por-supuesta-corrupcion-en-di/) | casa (titular) | hostil a Cepeda («afianza su rol de acusador») |
| 15-06-2026 | [Abelardo de la Espriella asumió una postura más presidencial al adoptar un tono más moderado y menos confrontacional](https://www.thearchipielagopress.co/abelardo-de-la-espriella-asumio-una-postura-mas-presidencial-al-adoptar-un-tono-mas-moderado-y-menos-confrontacional/) | casa (titular y cuerpo) | favorable a De la Espriella («postura más presidencial») |
| 15-06-2026 | [Apoteósico cierre de campaña tuvieron Abelardo de la Espriella y José Manuel Restrepo en la ciudad de Buga, Valle del Cauca este domingo 14 …](https://www.thearchipielagopress.co/apoteosico-cierre-de-campana-tuvieron-abelardo-de-la-espriella-y-jose-manuel-restrepo-en-la-ciudad-de-buga-valle-del-cauca-este-domingo-14-de-junio/) | casa (titular) | favorable a De la Espriella («Apoteósico cierre») |
| 27-06-2026 | [¿Cerco mediático y administración de los tiempos políticos en el periodismo colombiano?: Las preguntas sobre el papel de una parte de la pre…](https://www.thearchipielagopress.co/cerco-mediatico-y-administracion-de-los-tiempos-politicos-en-el-periodismo-colombiano-las-preguntas-sobre-el-papel-de-una-parte-de-la-prensa-tradicional-en-la-campana-presidencial-de-ivan-cepe/) | director (sección Editorial, «Por César A. Pizarro B.») | favorable a De la Espriella frente a la prensa que habría favorecido a Cepeda |

**En contra, en voz de la casa: 0.** Las críticas a De la Espriella de ese
periodo están todas atribuidas a terceros (Claudia López, 09-11-2025; la
denuncia de Cepeda, 11-06-2026; la carta de Karol G, 02-07-2026; Uribe,
18-07-2026). Y la denuncia de Cepeda del 15-06 entra con un titular propio
en contra del denunciante (fila del 15-06-2026, arriba).

## El día del cambio (07-08-2026): 2, que no se asignan a ningún lado

| Fecha | Pieza | Voz | Clasificación |
|---|---|---|---|
| 07-08-2026 | [Petro propone guardias libertadoras que cuide al pueblo de la policía y el ejército: ¿sería el nacimiento de una nueva modalidad de paramili…](https://www.thearchipielagopress.co/petro-propone-guardias-libertadoras-que-cuide-al-pueblo-de-la-policia-y-el-ejercito-seria-el-nacimiento-de-una-nueva-modalidad-de-paramilitarismo/) | casa (titular), 12:03, antes de la posesión | hostil a Petro (insinúa «una nueva modalidad de paramilitarismo») |
| 07-08-2026 | [El Gobierno de Gustavo Petro llegó a su fin, y estos fueron los escándalos más grandes que nos dejó su mandato](https://www.thearchipielagopress.co/el-gobierno-de-gustavo-petro-llego-a-su-fin-y-estos-fueron-los-escandalos-mas-grandes-que-nos-dejo-su-mandato/) | casa (análisis propio), 13:04 | hostil al Gobierno saliente («los escándalos más grandes que nos dejó») |

## Después del cambio (2026-08-08 → 2026-10-05): 4 en la dirección

| Fecha | Pieza | Voz | Clasificación |
|---|---|---|---|
| 04-09-2026 | [Petro vetado por Avianca para viajar en sus aviones por hacer parte de la Lista Clinton.](https://www.thearchipielagopress.co/petro-vetado-por-avianca-para-viajar-en-sus-aviones-por-hacer-parte-de-la-lista-clinton/) | casa (cierre del cuerpo) | hostil a Petro ya fuera del poder, débil («comenzó a cerrarle las puertas en todos lados») |
| 08-09-2026 | [La indignación de los indignados](https://www.thearchipielagopress.co/la-indignacion-de-los-indignados/) | casa (sección Editorial, sin firma) | favorable al Gobierno De la Espriella; descalifica a «la mamertaría colombiana» |
| 14-09-2026 | [El desastre económico que hoy sufre Colombia es producto del despilfarro y la corrupción de Gustavo Petro.](https://www.thearchipielagopress.co/el-desastre-economico-que-hoy-sufre-colombia-es-producto-del-despilfarro-y-la-corrupcion-de-gustavo-petro/) | casa (titular y frase de entrada; el resto, comunicado) | hostil a Petro ya fuera del poder («La corrupción fue la especialización del gobierno de Petro.») |
| 05-10-2026 | [Por orden del presidente de la República, Abelardo de la Espriella, el convicto Juan Guillermo Monsalve fue trasladado a la cárcel de máxima…](https://www.thearchipielagopress.co/por-orden-del-presidente-de-la-republica-abelardo-de-la-espriella-el-convicto-juan-guillermo-monsalve-fue-trasladado-a-la-carcel-de-maxima-seguridad-de-combita-boyaca-y-dejo-de-gozar-de-placeres-pe/) | casa (titular; cuerpo, nota con el trino del presidente) | celebra una orden del presidente («el convicto… dejó de gozar de placeres penitenciarios») |

Sin la de Avianca, que es débil, quedan **3**: el mínimo exacto de la regla.

## Contrapesos (condición 4): 2 en contra y 1 neutral, todos después

| Fecha | Pieza | Voz | Lado | Clasificación y peso |
|---|---|---|---|---|
| 18-08-2026 | [La inexcusable actitud del Ministro de Vivienda de irse de playa cuando todos sus compañeros de gobierno, comenzando por el propio president…](https://www.thearchipielagopress.co/la-inexcusable-actitud-del-ministro-de-vivienda-de-irse-de-playa-cuando-todos-sus-companeros-de-gobierno-comenzando-por-el-propio-presidente-han-estado-ocupados-atendiendo-la-emergencia-sin-descanso/) | casa (titular) | después | mixta: critica a un ministro del Gobierno entrante, pero elogia al presidente en el mismo titular. Se cuenta como contrapeso |
| 26-08-2026 | [¿Quién controla el cielo y vecindario del Presidente? ¿Un dron expuso su esquema de seguridad en el Batallón Paraíso?](https://www.thearchipielagopress.co/quien-controla-el-cielo-y-vecindario-del-presidente-un-dron-expuso-su-esquema-de-seguridad-en-el-batallon-paraiso/) | director (firmada) | después | escrutinio técnico de la seguridad del presidente entrante; concluye que el vídeo «no demuestra espionaje ni una falla concreta» |
| 08-09-2026 | [De la Espriella cumple su primer mes en la Presidencia: seguridad, terremoto y un Gobierno que busca imponer su sello](https://www.thearchipielagopress.co/de-la-espriella-cumple-su-primer-mes-en-la-presidencia-seguridad-terremoto-y-un-gobierno-que-busca-imponer-su-sello/) | casa (análisis sin firma) | después | neutral: balance del primer mes que recoge las críticas de derechos humanos a la operación con «seis menores de edad» muertos |

**Contrapesos que no son del eje nacional, pero cuentan como conducta:** el
medio fiscaliza con dureza al poder local. Persigue las «maniobras
dilatorias» del gobernador anulado Nicolás Gallardo (16-10-2025, 27-10-2025,
11-11-2025 y 26-02-2026), recoge la denuncia de un veedor contra el Gobierno
Departamental por un hueco vial que causó un accidente mortal (17-11-2025),
y publica una columna firmada contra la Gobernación (23-09-2026, Neme
Bustillo Bowie: «En la isla es claro que no hay un gobierno funcional sino
una máquina gubernamental de extracción de recursos públicos para pasarlas a
manos privadas»). **La resolución contaba también la pieza del incendio de
Magic Garden (08-09-2026) como crítica al Gobierno Departamental; no lo es:**
el cuerpo reproduce el parte del propio Gobierno Departamental y de los
bomberos, en tono institucional.

## Declaradas, pero que no cuentan

| Fecha | Pieza | Voz | Lado | Por qué no cuenta |
|---|---|---|---|---|
| 14-09-2026 | [La tiranía de la tutela](https://www.thearchipielagopress.co/la-tirania-de-la-tutela/) | firmada por tercero («Dylan Pizarro Torregroza», «* Abogado»), en Editorial | después | favorable al Ejecutivo frente a los jueces, con contrapeso de principio interno. No cuenta (columna de tercero) |
| 05-10-2026 | [Fuerte editorial de director de RCN Radio, Juan Lozano: proceso de paz de Juan Manuel Santos solo buscó un premio Nobel de paz.](https://www.thearchipielagopress.co/fuerte-editorial-de-director-de-rcn-radio-juan-lozano-proceso-de-paz-de-juan-manuel-santos-solo-busco-un-premio-nobel-de-paz/) | reproducción (vídeo de RCN Radio) en Editorial | después | titular calificativo («Fuerte editorial»), contra el proceso de paz de Santos. No cuenta (reimpresión) |
| 04-09-2026 | [La apuesta del Presidente de la República, Abelardo de la Espriella: entregar una Colombia en paz y con autoridad.](https://www.thearchipielagopress.co/la-apuesta-del-presidente-de-la-republica-abelardo-de-la-espriella-entregar-una-colombia-en-paz-y-con-autoridad/) | comunicado (discurso del presidente en primera persona) | después | favorable al Gobierno entrante. No cuenta (comunicado) |
| 29-09-2026 | [Presidente Abelardo de la Espriella confirma inversión de US$1.000 millones de Pepsico en Colombia para los próximos cinco años](https://www.thearchipielagopress.co/presidente-abelardo-de-la-espriella-confirma-inversion-de-us1-000-millones-de-pepsico-en-colombia-para-los-proximos-cinco-anos/) | anuncio oficial reproducido (con data line «Bogotá, 28 de septiembre de 2026») | después | logro del Gobierno entrante (Pepsico). No cuenta (comunicado) |
| 29-09-2026 | [«Colombia debe saber la verdad de la grave crisis en que el gobierno Petro dejó al país: en 4 años derrocharon el erario en viajes, embajada…](https://www.thearchipielagopress.co/colombia-debe-saber-la-verdad-de-la-grave-crisis-en-que-el-gobierno-petro-dejo-al-pais-en-4-anos-derrocharon-el-erario-en-viajes-embajadas-lagartos-patos-y-contratos-leoninos-ministro-de-haci/) | cita atribuida (ministro de Hacienda) | después | hostil a Petro. No cuenta (atribuida) |
| 19-05-2026 | [El gobierno del cambio navega hacia los territorios: libros, memoria y herramientas digitales transforman la educación en San Andrés, Provid…](https://www.thearchipielagopress.co/el-gobierno-del-cambio-navega-hacia-los-territorios-libros-memoria-y-herramientas-digitales-transforman-la-educacion-en-san/) | comunicado del Ministerio de Educación («Así cumple el Gobierno del Cambio») | antes | favorable al Gobierno Petro. No cuenta (comunicado); muestra que el medio también reproducía comunicados del Gobierno saliente |
| 12-12-2025 | [El gobierno avanza en el fortalecimiento del Registro Nacional de Turismo con diálogo y participación](https://www.thearchipielagopress.co/el-gobierno-avanza-en-el-fortalecimiento-del-registro-nacional-de-turismo-con-dialogo-y-participacion/) | comunicado del Gobierno nacional | antes | favorable al Gobierno Petro (turismo). No cuenta (comunicado) |
| 03-03-2026 | [¿Puede alguno de los candidatos punteros ganar en primera vuelta? Los antecedentes indican que solo Álvaro Uribe Vélez lo logró dos veces.](https://www.thearchipielagopress.co/puede-alguno-de-los-candidatos-punteros-ganar-en-primera-vuelta-los-antecedentes-indican-que-solo-alvaro-uribe-velez-lo-logro-dos-veces/) | casa (sección Elecciones 2026) | antes | neutral; la única pieza de esa sección |

---

## Recuento

| | Antes | Después | Día del cambio | Total |
|---|---|---|---|---|
| En la dirección (derecha) | 22 | 4 (3 sin la débil) | 2 | 26 (28 con el día del cambio) |
| En contra | 0 | 2 | 0 | 2 |
| Neutrales anotadas | 1 | 1 | 0 | — |

**Las cinco condiciones:**

1. **Voz de la casa.** Sí: titulares y análisis propios, un editorial sin
   firma (08-09-2026) y una pieza del director en la sección Editorial
   (27-06-2026). Quedan fuera la columna de «La tiranía de la tutela», el
   vídeo de Lozano y los comunicados.
2. **A los dos lados del 07-08-2026.** Sí: 22 antes y 4 después (3 sin la
   débil). **El lado de después está en el mínimo**, y se dice.
3. **Sostenida.** Sí: 26 piezas con postura (mínimo 10), al menos 3 a cada
   lado, y una proporción de 26 a 2, **13 a 1** (mínimo 3 a 1). Con el
   cálculo más estricto (sin la pieza débil y contando como contrapeso
   también el balance neutral del primer mes), queda 25 a 3, más de 8 a 1.
   **Sin las piezas que podrían leerse como fiscalización de Petro en el
   poder**, quedan 7 antes (96654, 98041, 98145, 98269, 98284, 98290 y
   98365: contra la izquierda o Cepeda, o a favor de De la Espriella) y las
   4 de después, que ya no fiscalizan a quien manda: 11 a 2.
4. **Contrapesos escritos.** Sí: arriba, con su peso. El más claro es el
   balance del primer mes, que es información sin juicio propio.
5. **Reproducible.** Este archivo.

**Magnitud.** No hay propiedad documentada con posición conocida ni endoso
formal: el tope es ±0,30. El valor exacto es juicio declarado, en la ficha.

---

## Otras cifras del mismo volcado (2026-10-09)

- 175 piezas desde el 07-08-2026, publicadas en **15 días distintos**; 111
  desde el 31-08-2026.
- 42 piezas en la categoría «Comercial» en los 12 meses (118 en total) y 19
  títulos con «Cajasai».
- **0 títulos en inglés** en los 873. La página y el feed declaran `es`.
