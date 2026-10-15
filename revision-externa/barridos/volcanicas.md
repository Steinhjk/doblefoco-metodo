# Barrido editorial: Volcánicas (volcanicas.com)

| | |
|---|---|
| **Medio** | Volcánicas (`volcanicas`), no noticioso, fuera del mapa. Proyecto de la Fundación Hoja Blanca ONG (`fichas/volcanicas.md`) |
| **Valor vigente** | **−0,50**, sin firmar, puesto en el alta del 2026-08-08 solo con su misión declarada (nivel 4) |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus dos precisiones |
| **Ventana** | 2025-10-10 → 2026-10-10 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Resolución de origen** | `revision-externa/respuestas/opus-5-5-volcanicas.md` (revisor: 12 piezas con postura, todas a la izquierda, 6 antes y 6 después) |
| **Quién lo hizo** | Claude Opus 5.5 (`claude-opus-5-5`), verificador del ciclo 2, tanda 8, a petición del responsable editorial, el 2026-10-10. Es de la misma casa que el autor de la ficha y que el revisor: su acuerdo no es aval |
| **Estado** | **DECIDIDO el 2026-10-10: −0,25** (antes −0,50), por el responsable editorial, contando las leves de después del 07-08 que se declaran dudosas; firmado en bloque el mismo día (`DECISIONES.md`, «2026-10-10 · Tandas 8 y 9 del ciclo 2: el barrido manda sobre los números sin evidencia»). Lo que más abajo dice «propuesta», «recomendada» o «pendiente» es el estado anterior a la decisión y se conserva como historia |
| **Resultado** | **Llega a los mínimos solo si se cuentan las piezas leves.** Lectura amplia: 17 piezas con postura a la izquierda (12 antes del cambio y 5 después), frente a 3 contrapesos parciales: 5,7 a 1. Lectura estricta, sin las leves: 8 piezas (6 y 2), 2,7 a 1, y **no llega**. Sin endoso. La dirección no está en duda; lo que está en el límite es el después |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas, el
> fragmento y el método están aquí para eso. **La clasificación de cada pieza
> es juicio de un solo lector**, de la misma casa que el autor de la ficha y
> que el revisor.

---

## 1. Método

- **robots.txt** de `volcanicas.com` (descargado el 2026-10-10): bloque de Yoast, `User-agent: *` con `Disallow:` vacío. No veta nada ni nombra a ClaudeBot, Claude-Web ni anthropic-ai.
- **Descarga:** `curl -sL --ssl-no-revoke` con User-Agent de navegador (Chrome 126), con pausa entre peticiones.
- **Universo, sin muestreo:** la API pública de WordPress,
  `https://volcanicas.com/wp-json/wp/v2/posts?after=2025-10-10T00:00:00&per_page=100&page=1..3`.
  Devuelve **267 piezas** (`X-WP-Total: 267`), del 2025-10-10 al 2026-10-09. Las 267 se descargaron enteras, en HTML.
- **Quién firma.** El autor de WordPress no es la firma visible: el sitio usa PublishPress Authors, y la firma está en `<meta name="author">`. Leída en las 267:
  - **«Volcánicas»: 196 piezas.** Es la voz de la casa.
  - **Catalina Ruiz-Navarro, directora: 3 piezas, y 1 más firmada con la editora general.** La regla cuenta lo «firmado por la casa o su director», como en el barrido de Archipiélago Press. Cuentan las dos de política nacional (§2).
  - **Ita María, editora general: 4 piezas**, ninguna de política nacional con postura que cuente; una (2026-07-25, «Fascismo-core») habla del «candidato de ultraderecha». No es la directora, así que **no cuenta**. Se declara.
  - **Firmas de terceras: 62 piezas** (columnas, cartas, reportajes de colaboradoras). **No cuentan.** Muchas de política nacional se inclinan a la izquierda (por ejemplo, 2026-05-29 «El riesgo de una alianza de derechas Ecuador-Colombia» o 2026-06-08 «La institucionalidad está en juego»), y se declaran sin contarlas.
- **Sección Editorial** (categoría 953): **5 piezas en todo el sitio**, 4 dentro de la ventana (2025-10-18 a 2025-11-08): Bullrich (Argentina), Israel (dos) y la absolución del exabogado de Uribe que demandó al medio. Ninguna toma postura sobre el gobierno ni sobre un candidato colombiano. Fuera.
- **Filtro.** Sobre el texto completo de las 196 de la casa y las 4 de la directora: Petro, Espriella/Abelardo, Cepeda, Paloma Valencia, Pacto Histórico, Uribe/uribis-, Centro Democrático, Fajardo, Quilcué, Francia Márquez, Benedetti, Hollman; y una segunda pasada por rótulos: ultraderech-, extrema derecha, fascis-, neofascis-, ultraconserv-, antiderechos/anti-derechos, fundamentalis-, ultrauribis-. **Las 38 piezas con nombres nacionales y las 44 con rótulos se leyeron**; las de después del 07-08 con contenido nacional, enteras.
- **Clases**, las mismas que en El Informador, con el signo cambiado:
  - **I, dirección izquierda** (cuenta): rótulo ideológico o descalificador en voz propia contra la derecha, sus candidatos o el Gobierno De la Espriella («ultraderechista», «fundamentalista», «neofascista», «anti-derechos»); elogio de candidatos o del gobierno de la izquierda; **encuadre asimétrico entre candidatos** (perfil laudatorio de unos y de escándalos de otros), que la regla del polo fijo trata como evidencia de primer orden.
  - **I (leve)** (cuenta en la lectura amplia, se marca): la postura existe pero es lateral, suelta o va dentro de una pieza que sobre todo informa o fiscaliza.
  - **F, solo fiscaliza a quien manda** (no cuenta, se declara): crítica a hechos de gestión del gobierno en ejercicio, sin rótulo ni toma de partido. **Precisión del responsable editorial del 2026-10-09: no suma para el mínimo por lado.**
  - **C, contrapeso:** crítica o reparo al Gobierno Petro, a su gente o a la izquierda colombiana; reconocimiento a la derecha.
  - **T, temática** (no cuenta, se declara): rótulo «antiderechos» a legisladores o concejales por su voto sobre aborto o diversidad, sin relación con el gobierno ni con la elección.
  - **Fuera:** internacionales (Ortega, Milei, Bukele, Perú, Honduras…), locales, servicio, emergencias y las nacionales descriptivas (M).

---

## 2. Tabla de piezas que cuentan

Todas las URL son `https://volcanicas.com/<slug>/`. El fragmento se comprobó por programa contra el HTML de cada página (2026-10-10).

### 2.1 Antes del cambio: 2025-10-10 → 2026-08-06 (gobierna Petro)

| # | Fecha | Pieza | Firma | Clase | Fragmento literal (breve) |
|---|---|---|---|---|---|
| 1 | 2025-10-27 | [ivan-cepeda-el-candidato-del-pacto-historico](https://volcanicas.com/ivan-cepeda-el-candidato-del-pacto-historico/) | Volcánicas | I (leve) | «con un estilo pragmático y más prudente y conciliador que el del actual presidente». El resto es perfil descriptivo |
| 2 | 2025-12-18 | [hay-festival-la-cultura-no-es-apolitica](https://volcanicas.com/hay-festival-la-cultura-no-es-apolitica/) | Volcánicas | I (leve) | «El candidato presidencial de ultraderecha, Abelardo de la Espriella». La pieza es sobre todo internacional |
| 3 | 2026-03-11 | [paloma-valencia-la-candidata-de-derecha](https://volcanicas.com/paloma-valencia-la-candidata-de-derecha/) | Volcánicas | I | «ha dejado claras sus posturas de derechas, antifeministas y antiderechos y su fidelidad al uribismo» |
| 4 | 2026-03-12 | [aida-quilcue-la-formula-vicepresidencial-de-ivan-cepeda](https://volcanicas.com/aida-quilcue-la-formula-vicepresidencial-de-ivan-cepeda/) | Volcánicas | I | Bajada: «ratifica la apuesta social del Pacto Histórico»; «refuerza la alianza entre el proyecto político del Pacto Histórico y los movimientos indígenas». Perfil laudatorio, publicado el día siguiente al de Valencia |
| 5 | 2026-03-14 | [asi-quedaron-las-formulas-presidenciales-…](https://volcanicas.com/asi-quedaron-las-formulas-presidenciales-para-las-elecciones-de-2026-en-colombia/) | Volcánicas | I (leve) | «En la extrema derecha se ubica la candidatura del abogado Abelardo de la Espriella»; «la campaña securitista del ultraderechista». A Quilcué, en la misma pieza, «una voz crucial» |
| 6 | 2026-05-11 | [el-asesinato-del-periodista-mateo-perez-rueda](https://volcanicas.com/el-asesinato-del-periodista-mateo-perez-rueda/) | Volcánicas | I (leve) | «el candidato de ultraderecha Abelardo de la Espriella no se pronunció» |
| 7 | 2026-05-27 | [que-es-el-centro-politico](https://volcanicas.com/que-es-el-centro-politico/) | **Catalina Ruiz-Navarro, directora** | I | «la nueva derecha fascista encarnada en Abelardo de la Espriella»; «Cepeda no está en la “extrema izquierda”»; «nada del gobierno de Petro ha mostrado que esté yendo contra la empresa privada» |
| 8 | 2026-06-03 | [abelardo-de-la-espriella-para-dummies](https://volcanicas.com/abelardo-de-la-espriella-para-dummies/) | Volcánicas | I | «construyó su fortuna y su red de poder en los bordes donde la ley y el crimen se tocan». Perfil de escándalos, entre las dos vueltas |
| 9 | 2026-07-02 | [defensora-de-derechos-humanos-es-atacada-por-ultraderechistas-en-pasto](https://volcanicas.com/defensora-de-derechos-humanos-es-atacada-por-ultraderechistas-en-pasto/) | Volcánicas | I (leve) | «ganador al ultraderechista Abelardo de la Espriella» |
| 10 | 2026-07-06 | [el-gabinete-de-abelardo-de-la-espriella-los-nunca](https://volcanicas.com/el-gabinete-de-abelardo-de-la-espriella-los-nunca/) | Volcánicas | I | «Viviane Morales, la exfiscal fundamentalista»; «la ultrauribista Paola Holguín». Presidente electo, todavía no gobierna |
| 11 | 2026-07-16 | [marcha-del-orgullo-y-yo-marcho-trans](https://volcanicas.com/marcha-del-orgullo-y-yo-marcho-trans/) | Volcánicas | I | «la llegada del ultraderechista Abelardo de la Espriella al poder»; «la elección de un gobierno que amenaza las garantías y los derechos de las personas LGBT+» |
| 12 | 2026-07-20 | [nuevo-caso-de-homofobia-en-el-centro-comercial-andino](https://volcanicas.com/nuevo-caso-de-homofobia-en-el-centro-comercial-andino/) | Volcánicas | I (leve) | «ad portas de un gobierno abiertamente antiderechos y anti LGBT+ en Colombia» |

**Antes: 12 (6 I + 6 leves).**

### 2.2 Después del cambio: 2026-08-07 → 2026-10-10 (gobierna De la Espriella)

| # | Fecha | Pieza | Firma | Clase | Fragmento literal (breve) |
|---|---|---|---|---|---|
| 13 | 2026-08-14 | [emergencia-por-incendios-forestales-en-colombia-…](https://volcanicas.com/emergencia-por-incendios-forestales-en-colombia-340-municipios-en-alerta-roja/) | Volcánicas | I (leve) | «El Gobierno de Petro dejó activada una estrategia para 12 meses»; el giro del nuevo gobierno «podría tensionar algunas de las políticas de protección de ecosistemas» del anterior. Contraste favorable al saliente |
| 14 | 2026-08-17 | [abelardo-de-la-espriella-debuta-como-presidente-…](https://volcanicas.com/abelardo-de-la-espriella-debuta-como-presidente-e-improvisa-en-la-emergencia-por-el-terremoto/) | Volcánicas | I (leve) | Sobre todo F. Lo que suma: Petro pidió transmitir el empalme «en un gesto de transparencia con el país ante la constante narrativa de fraude del gobierno entrante» |
| 15 | 2026-08-19 | [la-nueva-directora-del-icbf-…](https://volcanicas.com/la-nueva-directora-del-icbf-pide-dejar-de-nombrar-a-las-ninas-y-estigmatiza-al-colectivo-infantil-resistencia-chiquita/) | Volcánicas | I (leve) | Sobre todo F. Lo que suma: la «batalla cultural», «la bandera con que el gobierno de Abelardo de la Espriella se hizo elegir y busca retroceder en materia de derechos» |
| 16 | 2026-08-26 | [361-dias-de-desigualdad](https://volcanicas.com/361-dias-de-desigualdad/) | **Catalina Ruiz-Navarro, directora** | I | «un gobierno neofascista como el de Abelardo» |
| 17 | 2026-09-03 | [sale-viviane-morales-y-entra-ilva-myriam-hoyos-…](https://volcanicas.com/sale-viviane-morales-y-entra-ilva-myriam-hoyos-la-exprocuradora-anti-derechos-ahora-sera-ministra-de-educacion/) | Volcánicas | I | Titular: «La exprocuradora anti-derechos»; cuerpo: «la ultraconservadora Ilva Myriam Hoyos» |

**Después: 5 (2 I + 3 leves).** Las 3 leves son las dudosas del barrido: dos van dentro de piezas que sobre todo fiscalizan.

---

## 3. Contrapesos

| Fecha | Pieza | Peso | Qué hace |
|---|---|---|---|
| 2025-11-15 | [siete-menores-muertos-en-operativo-militar-en-el-guaviare](https://volcanicas.com/siete-menores-muertos-en-operativo-militar-en-el-guaviare/) | Parcial | Fiscaliza al Gobierno Petro mientras gobierna: «Este nuevo caso, ahora bajo un mandato progresista, revive la deuda»; «no es negociable bajo ningún gobierno». Lleva un atenuante (la comparación con el bombardeo de 2019, «una ofensiva militar planeada —no una acción defensiva reactiva—»), por eso no es pleno |
| 2026-03-24 | [metoo-yo-te-creo-colega-…](https://volcanicas.com/metoo-yo-te-creo-colega-nueva-ola-de-denuncias-en-el-periodismo-colombiano-que-sigue/) | Parcial | Presión sobre «el gerente de RTVC», Hollman Morris, nombrado por el Gobierno Petro, por su pleito contra una denunciante |
| 2026-04-22 | [fiscalia-desarchiva-denuncia-contra-hollman-morris-…](https://volcanicas.com/fiscalia-desarchiva-denuncia-contra-hollman-morris-por-acto-sexual-violento/) | Parcial | Sigue la denuncia contra el mismo funcionario del Gobierno Petro |

Los tres son de antes del cambio y son fiscalización del gobierno afín, que es lo que el barrido de El Informador contó como contrapeso en el sentido contrario. Ninguno es pleno: el primero se atenúa y los otros dos son sobre una persona y por el eje de género, no sobre la política del gobierno.

**No cuentan como contrapeso, y se declaran:**
- 2026-07-20, [Ortega](https://volcanicas.com/daniel-ortega-entierra-las-elecciones-en-nicaragua-y-consolida-la-dictadura-familiar/): «sentenció el dictador». Internacional.
- 2026-08-04, [JEP, macrocasos 10 y 11](https://volcanicas.com/historico-primera-imputacion-de-la-jep-en-el-marco-de-los-macrocasos-10-y-11/): «la crueldad de este gobierno guerrillero», sobre las FARC. Es un grupo armado, no un actor del eje electoral.
- La propia directora, dentro de la pieza 7: «Desde la izquierda se le puede exigir a la misma izquierda, tener valores feministas, garantizar los derechos humanos, no ser corrupta y no ser autoritaria». Es una declaración, no una pieza que critique a la izquierda.
- **No hay ningún reconocimiento a la derecha colombiana ni a su gobierno** en voz de la casa en los 12 meses.

---

## 4. Lo que no cuenta, y se declara

**F, solo fiscaliza al Gobierno De la Espriella** (no suma, por la precisión del 2026-10-09):

| Fecha | Pieza | Nota |
|---|---|---|
| 2026-08-08 | [abelardo-de-la-espriella-defendio-al-pastor-gamez-…](https://volcanicas.com/abelardo-de-la-espriella-defendio-al-pastor-gamez-denunciado-por-abusar-sexualmente-de-23-mujeres-y-4-ninas/) | Su pasado como abogado |
| 2026-08-29 | [salvia-sistema-atencion-violencias-genero-gobierno-de-la-espriella](https://volcanicas.com/salvia-sistema-atencion-violencias-genero-gobierno-de-la-espriella/) | Futuro de un sistema público |
| 2026-08-31 | [abelardo-de-la-espriella-respalda-bombardeo-…](https://volcanicas.com/abelardo-de-la-espriella-respalda-bombardeo-que-deja-tres-menores-muertos-en-guaviare-otro-menor-de-edad-murio-en-el-bombardeo-del-10-de-agosto/) | Ver abajo, «el verbo» |
| 2026-09-01 | [censura-a-la-prensa-en-gobierno-de-abelardo-de-la-espriella-…](https://volcanicas.com/censura-a-la-prensa-en-gobierno-de-abelardo-de-la-espriella-erosiona-la-democracia/) | Libertad de prensa: «Desde Volcánicas rechazamos estas medidas» |
| 2026-09-07 | [primer-mes-de-gestion-de-abelardo-de-la-espriella](https://volcanicas.com/primer-mes-de-gestion-de-abelardo-de-la-espriella/) | Cronología: «la imagen de un presidente que se pasea entre cadáveres para mostrar resultados». Descalificador, pero sobre un hecho documentado (los videos que un juzgado ordenó ocultar) |

Más 2 F con un elemento leve que sí se cuentan (piezas 14 y 15).

**El verbo de los bombardeos (31-08-2026).** El revisor lo da como «encuadre asimétrico», y el dato es literal: «Tres menores de edad fueron asesinados» con De la Espriella, «durante el gobierno de Gustavo Petro han muerto entre 62 y 68 menores» y, con Duque, «367 personas fueron asesinadas». Pero la misma pieza dedica una sección entera a los bombardeos de Petro, con su frase en X y su petición de perdón, y la de noviembre de 2025 fiscalizó a Petro por el mismo hecho. **Es fiscalización de los tres gobiernos con una asimetría léxica dentro**, no una disculpa. Se declara y no suma.

**La intensidad de la fiscalización.** En 10 meses de Gobierno Petro, la casa le dedica 1 pieza de fiscalización de su política (Guaviare) y 2 sobre un funcionario suyo. En 2 meses de Gobierno De la Espriella, 7 (5 F y 2 F con leve). No suma por la precisión del 2026-10-09, pero es la asimetría que la regla del polo fijo describe («fiscalizaba al saliente y sigue con el entrante» no es lo que se ve). Se declara como tensión.

**T, temáticas** (rótulo «antiderechos» por el voto sobre aborto o diversidad):
- 2026-02-10, [la congresista y pastora Milagros Jáuregui](https://volcanicas.com/maternidades-forzadas-de-ninas-de-10-a-13-anos-en-la-casa-del-padre-el-albergue-de-congresista-y-pastora-milagros-jauregui/): «una congresista y pastora abiertamente antiderechos».
- 2026-07-30, [bancada antiderechos](https://volcanicas.com/bancada-antiderechos-radica-nuevo-proyecto-para-prohibir-el-aborto/): «la bancada antiderechos radicó en el Congreso de Colombia».
- 2026-02-06, [Concejo de Bogotá](https://volcanicas.com/concejo-de-bogota-aprueba-proyecto-antiderechos/). Local.

**M y fuera** (informativas, servicio, locales o internacionales): Córdoba (2026-02-12; cita a Petro de forma favorable sobre Urrá: «Incluso el presidente Gustavo Petro […] criticó públicamente» la represa), Arturo Calle y el voto de sus empleados (2026-06-18, investigación sobre un empresario), la bala perdida de Calamar (2026-06-24), el obispo de la posesión (2026-08-07), el terremoto (08-10, 08-11, 08-12), la gobernadora del Chocó (2026-08-20, elogio de una gobernadora que la propia pieza presenta como «candidata del Partido Liberal» en 2023; local), tutelas y Consejo de Estado (08-29), los líderes de Cajibío (09-03), Samuel Adrián (09-13, fact-check que corrige que la captura fuera «ordenada por Gustavo Petro» y rotula a un ideólogo extranjero), paro armado en Santa Marta (09-23), Donovan Balanta (09-25), las dos piezas del aborto (09-28 y 09-29) y Olivia Rodrigo (08-30, «gobiernos autoritarios de corte neofascista», genérico y sin nombre).

**Ninguna pieza de la casa ni de la directora pide el voto** por nadie. Se buscó «votar por», «vote por», «votaremos», «nuestro voto», «llamamos/invitamos a votar» en las 267: el único resultado es una cita ajena en la columna de la directora del 26-08. La casa no publicó nada en voz propia sobre el resultado de la primera ni de la segunda vuelta. **Sin endoso.**

---

## 5. Lo que el revisor contó, pieza por pieza

| Revisor | Pieza | Aquí | Por qué |
|---|---|---|---|
| L1 | Cepeda, 27-10-2025 | I (leve) | El encuadre favorable es una frase; el resto, perfil |
| L2 | Guaviare, 15-11-2025 | **C parcial** | Fiscaliza a Petro mientras gobierna. El atenuante existe, pero la pieza recoge las críticas y la moción de censura. No es «indulgente» |
| L3 | Quilcué, 12-03-2026 | I | De acuerdo |
| R1 | Valencia, 11-03-2026 | I | De acuerdo |
| R2 | De la Espriella, 03-06-2026 | I | De acuerdo: candidato, no gobernante |
| R3 | Gabinete, 06-07-2026 | I | De acuerdo: presidente electo |
| R4 | Debut, 17-08-2026 | I (leve) | Sobre todo F; suma solo por el elogio a Petro |
| R5 | ICBF, 19-08-2026 | I (leve) | «Estigmatiza» describe un acto: F. Suma solo por la frase sobre la «batalla cultural» |
| R6 | Bombardeos, 31-08-2026 | **F** | Ver §4, «el verbo» |
| R7 | Censura, 01-09-2026 | **F** | Libertad de prensa frente al gobierno de turno |
| R8 | Hoyos, 03-09-2026 | I | De acuerdo |
| R9 | Primer mes, 07-09-2026 | **F** | Cronología de gestión |

De sus 12, **suman aquí 8** (5 claras: L3, R1, R2, R3 y R8; 3 leves: L1, R4 y R5) **y 4 no** (L2 pasa a contrapeso; R6, R7 y R9 son fiscalización). Le faltan las 2 de la directora, 5 leves de antes (Hay Festival, fórmulas, Mateo Pérez, Pasto y Andino), la de la marcha (16-07) y la de los incendios (14-08). Su «12:0» pasa por alto los 3 contrapesos, y su «6 después» se queda en 1 clara y 2 leves.

---

## 6. Veredicto por condición

| Condición | Lectura amplia (I + leves) | Lectura estricta (solo I) |
|---|---|---|
| 1. Voz de la casa | **Sí.** Firma «Volcánicas» o de la directora | **Sí** |
| 2. A los dos lados del 07-08-2026, en 12 meses | **Sí** | **Sí** |
| 3a. ≥10 piezas con postura | **Sí: 17** | **No: 8** |
| 3b. ≥3 a cada lado, sin fiscalización | **Sí: 12 y 5** (3 de las 5 son leves) | **No: 6 y 2** |
| 3c. Proporción ≥3:1 | **Sí: 17:3 = 5,7:1** | **No: 8:3 = 2,7:1** |
| 4. Contrapesos escritos | **Sí** (§3) | **Sí** |
| 5. Reproducible | **Sí** (§1 y §2) | **Sí** |

**Cumple en la lectura amplia y no en la estricta.** El precedente se parte en dos:
- El Informador (2026-10-10) contó las leves, pero allí la regla se cumplía igual sin ellas (58 y 28).
- Abra Noticias (2026-10-09) no contó las dudosas, y por la regla 2 se quedó en 0,00.

Aquí las 6 leves de antes son rótulos claros en voz propia («ultraderechista», «extrema derecha»), sueltos dentro de piezas informativas: son leves en el sentido de El Informador, no dudosas. **Las 3 leves de después sí se parecen a las dudosas de Abra**: dos van dentro de piezas que sobre todo fiscalizan. Sin ellas, el lado de después tiene 2 piezas, y 1 es de la directora.

---

## 7. Magnitud: ¿sigue el tope de ±0,30?

**El texto del protocolo:**
- §1, «Cuánto mueve»: «Sin propiedad documentada con posición conocida (nivel 1) ni endoso explícito, **la magnitud no pasa de ±0,30**, la banda moderada. El valor exacto es un juicio declarado […]. La regla 2 sigue en pie».
- §5, regla 3, con la precisión del 2026-10-10: «mueve como mucho hasta ±0,30, **salvo endoso explícito o nivel 1 con posición conocida**».
- §2, la tabla: nivel 1 es «**Propiedad documentada** — Quién controla la empresa, con fuente citable y persona natural».

**Endoso:** no hay (§4).

**¿La posición declarada de la directora es «nivel 1 con posición conocida»?** Aquí no:
1. El nivel 1 es **propiedad o control** («quién controla la empresa»). De la directora consta el cargo, que sí es nivel 1. **Su posición, en cambio, sale de una columna de opinión**, y eso es voz de la casa (cuenta en este mismo barrido, piezas 7 y 16) o declaración (nivel 4). Contarla además como nivel 1 sería contar dos veces la misma pieza.
2. Los precedentes de «nivel 1 con posición conocida» son estructurales: el **control orgánico del PCC sobre la Fundación Semanario VOZ** (DECISIONES 2026-10-07) y la pregunta por un **vínculo orgánico de El Nuevo Siglo con el Partido Conservador** (2026-09-22). Son dueños o controladores que son actores políticos, y eso se comprueba en un registro, no en una columna.
3. La regla de quien dirige (§1) excluye de su aviso la «opinión publicada» de quien dirige: «lo demás es orientación —y la orientación se mide con corpus, no con biografía—». Es la misma idea.
4. La fundación que controla el medio se declara «no partidista. No apoya a ningún candidato ni partido político» (/nosotras/, 2026-10-10).

**Lectura.** Si el barrido cuenta, el tope rige y el valor no pasa de −0,30. Si no cuenta, la regla 3 deja el número que había (−0,50), pero ese número se apoya solo en nivel 4, que el §2 no admite como única base. **Es una incoherencia del protocolo que esta ficha destapa:** con menos evidencia el número queda más lejos de la mixta que con más. La decisión es del responsable editorial.

---

## 8. PROPUESTA (pendiente de la firma del responsable editorial)

**−0,25, izquierda moderada.** Es juicio declarado, no medición.

**Por qué en la banda moderada y no en 0,00:**
- La dirección no está en duda. Hay encuadre asimétrico entre candidatos en la campaña (Cepeda y Quilcué con perfil laudatorio; Valencia y De la Espriella con perfil de escándalos), la directora se sitúa a la izquierda en su propio medio y en voz de la casa no hay ni un reconocimiento a la derecha.
- La regla del polo fijo trata ese encuadre entre candidatos como evidencia de primer orden, fuera de la exclusión de la fiscalización.

**Por qué −0,25 y no el tope de −0,30:**
- Archipiélago Press llegó a +0,30 con 26 piezas y holgura a los dos lados. Aquí son 17 en la lectura amplia y 8 en la estricta, y el lado de después se sostiene con 2 piezas claras.
- El Diario (Pereira), en +0,25, tiene 80 piezas, pero un después mezclado (9 a 7). Diario La Libertad, en +0,20, tiene 27 piezas a 3,5:1.
- La regla 2, en su espíritu: el barrido cumple solo contando leves.

**Lecturas alternativas, que se declaran:**
- **−0,30**, el tope, si el responsable editorial pesa más el encuadre entre candidatos y las dos piezas de la directora que la delgadez del después.
- **−0,50 provisional, sin firmar e incompleta**, si el responsable editorial lee el barrido en estricto (como en Abra) y aplica «un barrido que no llega no deshace nada». La ficha tendría que decir que su magnitud no tiene base admisible.
- **−0,50** también si el responsable editorial decide que la posición declarada de la directora es nivel 1 con posición conocida. No se recomienda (§7).

**Lo que el barrido no sostiene:** la derecha, ni un 0,00 «con evidencia».

**Qué la refutaría:**
- que, en lo que queda de 2026, la casa critique en voz propia al Gobierno De la Espriella solo por hechos de gestión, sin rótulos, y a la vez publique fiscalización de la izquierda en el Congreso o en la oposición;
- o un endoso en voz propia en una elección futura, que levantaría el tope.

**Se aplica a la vez** («Lo que NO cambia», §1): la misma pregunta —un valor puesto por la misión, por encima de ±0,30 y sin barrido que lo sostenga— está abierta en Colombia Informa (−0,55) y en CasaMacondo (−0,35 entonces; desde el 2026-10-10, 0,00 con evidencia).
