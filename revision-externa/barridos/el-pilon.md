# Barrido editorial: El Pilón

| | |
|---|---|
| **Medio** | El Pilón, Valledupar, Cesar (`el-pilon`) |
| **Valor vigente** | +0,20, provisional de alta, sin firmar, «por la banda regional». Dirección declarada en la ficha: derecha (seguridad, minería, apoyo al Gobierno De la Espriella). La resolución del ciclo 2 dejó un hueco: no se había leído nada de enero a mayo de 2026 |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09) |
| **Ventana** | 2025-10-09 → 2026-10-09 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5 (`claude-opus-5-5`), a petición del responsable editorial, el 2026-10-09. Es de la misma casa que el autor de la ficha y que quien escribió la resolución del ciclo 2: su acuerdo no es aval |
| **Estado** | **DECIDIDO el 2026-10-09: se queda en +0,20** (no llega a la proporción de 3 a 1), por el responsable editorial; firmado en bloque el 2026-10-10 (`DECISIONES.md`, «2026-10-09 · Reexamen de cinco fichas cerradas con la regla nueva»). Lo que más abajo dice «propuesta» o «pendiente» es el estado anterior a la decisión y se conserva como historia |
| **Decisión (2026-10-09)** | el responsable editorial: **se queda en +0,20.** El barrido no llega a 3 a 1 (2,2 a 1), y un barrido que no llega conserva el valor que había (`DECISIONES.md`, «Reexamen de cinco fichas cerradas con la regla nueva»; ver la ficha) |

---

## 1. Método

- **robots.txt** de elpilon.com.co (descargado el 2026-10-09): `User-Agent: * / Allow: /` y `Sitemap: https://elpilon.com.co/sitemap-index.xml`. No excluye a ningún agente ni ninguna ruta.
- **No se tocaron** eltiempo.com, cambiocolombia.com ni lasillavacia.com. No hubo buscador web.
- **Descarga.** `curl -sL --ssl-no-revoke` con el UA de un navegador (Chrome 126 en Windows), el 2026-10-09. El sitio es Next.js con muro de registro: el texto completo viaja en el HTML, en los campos `previewHtml` + `hiddenHtml` del flujo RSC. Se leyó de ahí. La fecha de cada pieza es el primer `dateTime` ISO de la página, y coincide con la fecha impresa.
- **Cómo se armó la lista de piezas.** La paginación de las secciones no funciona en el servidor, así que se juntaron todas las fuentes de URL disponibles y cada URL se descargó **del sitio vivo**:
  1. **Los 170 sitemaps** (`sitemap-index.xml` → `sitemap/0..169.xml`): 162.469 entradas, **50.038 URL únicas**. Solo traen **50** editoriales en `/opinion/editoriales/` (los más recientes) y 1.694 del archivo antiguo `/editorial/`, que es de 2009-2016. **Los sitemaps no cubren enero-agosto de 2026**, al contrario de lo que se esperaba: el `lastmod` es la fecha de regeneración (casi todo dice 2026-10), no la de publicación.
  2. **El índice CDX de Internet Archive** (`web.archive.org/cdx`), por prefijo y desde 2025-09, para `elpilon.com.co/editorial/`, `/opinion/editoriales/` y `/editoriales/`, con y sin `www`. Solo se usó para descubrir URL. El texto que se cita no sale del archivo, sale de elpilon.com.co.
  3. **La sección `/editorial` viva** (6 enlaces de junio de 2026) y **cinco instantáneas de junio** de las portadas de opinión y de editorial (Internet Archive), para tapar el mes con menos capturas.
  - Resultado: 550 URL descargadas; **305 piezas únicas** fechadas entre el 2025-10-09 y el 2026-10-09 (deduplicadas por título; varias se sirven en las dos rutas).
  - **Hallazgo de paso.** El servidor sirve en `/opinion/editoriales/` todo el año, no solo desde el 13-08. La sección vigente tiene editoriales desde octubre de 2025; lo que se corta en 50 es el sitemap.
- **Voz de la casa.** Los editoriales de El Pilón no llevan firma y hablan como «EL PILÓN», «desde estas líneas», «apoyamos». Cuentan todos (condición 1).
- **Excluidas de las 305 (15)**, porque no son voz de la casa aunque estén bajo `/editorial/`:
  - **11 columnas firmadas** colgadas en junio de 2026 bajo la ruta de editorial («Por: …»): Castilla-Tobías (05-06), Ruiz Ditta (05-06, 19-06), Castro Araújo (05-06), Verano de la Rosa (07-06), Ariza (07-06), Ortega Vergara (09-06), «Carta a los tibios…» (09-06, «el autor»), Cotes (09-06), Indalecio Dangond (19-06) y Araújo Calderón (19-06). Hay columnas a favor de De la Espriella («El Tigre y el despertar de una nueva derecha») y en contra («De ‘papucho’ a tigre», «¿Llegó el fascismo a Colombia?»). Se declaran y no cuentan.
  - **4 notas informativas** (FELVA, sismo, avenida El Edén, elecciones cafeteras).
- **Quedan 290 piezas en voz de la casa**: 236 antes del 07-08-2026 y 54 desde ese día.
- **Cobertura.** Faltan 29 días hábiles (lunes a sábado) de 313. Por mes, se encontraron entre 16 y 27 editoriales, con un hueco en **junio de 2026: 17 encontrados, 11 días hábiles sin pieza**, entre ellos el 22-06, día siguiente a la segunda vuelta. El 20-06, víspera de la segunda vuelta, sí está, y es cultural. Los días que faltan: 10, 11, 13 y 28-10-2025; 25-12; 1, 2 y 10-01-2026; 16-02; 09-03; 3 y 4-04; 22, 26 y 29-05; 1, 2, 3, 8, 11, 15, 16, 22, 26 y 29-06; 17 y 29-07; 04-08; 16-09.
- **Filtro de las 290.**
  - Primero se buscaron en el texto completo términos nacionales: Petro, Gobierno nacional, gobierno del cambio, presidente, De la Espriella/Abelardo, Cepeda, Pacto Histórico, Centro Democrático, izquierda/derecha, paz total, ministr-, reforma, candidat-, elecci-, Uribe, Duque, ELN.
  - Las 147 con algún término se leyeron por sus frases con esos términos. Las que tenían postura o la rozaban se leyeron enteras (unas 45).
  - Las demás se leyeron por título. Son locales (Alcaldía de Valledupar, Gobernación, Emdupar, UPC, el río Guatapurí), culturales (Festival Vallenato, FELVA), viales o internacionales.
- **Qué se clasificó.** Solo las piezas con postura sobre el Gobierno nacional, las candidaturas presidenciales o el presidente electo.
  - **D, dirección derecha:**
    - critica o fiscaliza al Gobierno Petro o a su política (se marca, para leerla con el polo fijo del §3);
    - favorece la candidatura o el programa de De la Espriella;
    - celebra, apoya o disculpa al presidente electo o a su Gobierno.
  - **C, contrapeso:**
    - reconoce al Gobierno Petro, a sus programas o al Pacto Histórico;
    - critica o pone reparos al Gobierno De la Espriella.
  - **M, mixta:** tiene postura, pero reparte a los dos lados en medida parecida. No cuenta en la proporción.
  - **«leve»:** la postura existe, pero es una frase o un matiz dentro de un editorial de otro tema. Cuenta igual en el recuento principal; el §3 da también el recuento sin ellas.
  - **Fuera del recuento:** editoriales locales aunque nombren a un ministerio; electorales de procedimiento; internacionales sin Gobierno colombiano (Venezuela, 12-12-2025 y 05-01-2026); necrológicas (Vargas Lleras, 11-05-2026); y las que no tienen postura (ver §2.3).
- **Scripts y descargas** en la carpeta temporal de la sesión, fuera del repositorio. No se ha guardado ni se publica el texto completo de ninguna pieza: solo fragmentos breves como evidencia.

---

## 2. Tabla de piezas que cuentan (voz de la casa)

Todas las URL son `https://elpilon.com.co` + la ruta.

### 2.1 Antes del cambio: 2025-10-09 → 2026-08-06 (gobierna Petro)

| # | Fecha | Ruta | Clas. | Por qué |
|---|---|---|---|---|
| 1 | 2025-10-14 | `/opinion/editoriales/hay-que-madrugarles-a-las-alertas-electorales-tempranas` | D | Las alertas de la Defensoría «han sido subestimadas por el alto gobierno»: Petro y sus ministros reconocen 104 municipios en riesgo y no 649 |
| 2 | 2025-12-11 | `/opinion/editoriales/palomino-linan-y-socarras-los-relevos-van-pa-atras` | D leve | Los relevos de interventores «por parte del gobierno Petro» generan «suspicacias» en época preelectoral. Concede que el argumento oficial «tendría un argumento válido» |
| 3 | 2026-01-28 | `/opinion/editoriales/una-buena-intencion-produciendo-estragos` | D | El «desproporcionado incremento del salario mínimo» produce «efectos perversos». No nombra al Gobierno, pero la decisión es suya |
| 4 | 2026-03-12 | `/opinion/editoriales/se-quedo-en-anuncio-la-zona-especial-de-logistica-de-bosconia` | D leve | «Se le debe pedir explicación» a Petro por la ZEL de Bosconia |
| 5 | 2026-03-16 | `/opinion/editoriales/por-que-antioquia-saco-la-cara-frente-al-pais` | D | El Gobierno de Petro, «poco dado a trabajar, en un equivocado criterio, con gobiernos políticamente opuestos»; Antioquia no esperó a «un gobierno como el de Petro» |
| 6 | 2026-04-07 | `/opinion/editoriales/hasta-cuando-la-crisis-de-la-salud` | D leve | La crisis hospitalaria del Cesar, porque «los recursos del Gobierno nacional no llegan de manera oportuna» |
| 7 | 2026-04-15 | `/opinion/editoriales/vuelve-el-paro-un-problema-de-mas-de-50-anos-y-aun-sin-solucion` | D | «Todo sigue igual en el ‘gobierno del cambio’», aunque reconoce «buena voluntad del actual gobierno» |
| 8 | 2026-04-20 | `/opinion/editoriales/bloqueo-vial-de-bosconia-necesitamos-de-los-cesarenses-amigos-del-gobierno` | D leve | Pide a «esos que son amigos del presidente Gustavo Petro» que intervengan en Bosconia |
| 9 | 2026-05-08 | `/opinion/editoriales/pero-quien-reclama-por-el-cesar` | D | «El presidente Petro nunca consideró prioritario» al Cesar; los proyectos «se mantuvieron engavetados durante los cuatro años» |
| 10 | 2026-05-13 | `/opinion/editoriales/vuelve-la-incertidumbre-energetica` | D leve | Falta un mensaje claro del ministro de Minas sobre el riesgo de apagón |
| 11 | 2026-05-28 | `/opinion/editoriales/el-gobierno-petro-ha-trabado-los-servicios-publicos-de-valledupar` | D | Tesis en el título. Matiza: «no todo lo malo [...] es responsabilidad del Gobierno nacional actual» |
| 12 | 2026-06-19 | `/opinion/editoriales/de-la-espriella-y-cepeda-sin-proyectos-para-la-region` | D | Reprocha a los dos candidatos, pero con asimetría: la paz de Cepeda, sin seguridad, «palabra que evita la izquierda», es «un ingenuo banderazo»; con De la Espriella habría «un presidente costeño después de 140 años». Dentro, un contrapeso: la reforma agraria logró un avance «muy notable» |
| 13 | 2026-07-15 | `/opinion/editoriales/valledupar-y-el-cesar-tambien-merecen-una-sede-del-gobierno-nacional` | D | La sede alterna que estudia el presidente electo es «una buena señal [...] de una nueva forma de gobernar»; Petro «nunca realizó una visita oficial al departamento» |
| 14 | 2026-07-16 | `/opinion/editoriales/posible-apagon-prioridad-para-la-agenda-regional-con-el-nuevo-gobierno-nacional` | D leve | Ironía sobre el ministro Palma: tarifas «costosas», «a pesar de» que dijo que bajaron un 28 % |
| 15 | 2026-07-25 | `/opinion/editoriales/que-barranquilla-representando-a-la-region-caribe-sea-sede-del-gobierno-nacional` | D | Hace suya la iniciativa del presidente electo; «la ausencia del Gobierno nacional durante los últimos cuatro años» |
| 16 | 2026-08-03 | `/opinion/editoriales/la-frustrada-gobernadora-y-la-nueva-oportunidad` | D | La gobernadora, «frustrada con el gobierno de Gustavo Petro»; De la Espriella «ha prometido acertadamente cambiar»; el Pacto Funcional del «gobierno del antecesor Iván Duque» |
| 17 | 2025-10-27 | `/opinion/editoriales/jep-en-valledupar` | C | La mesa del Gobierno con los exjefes de las AUC: «es buena la idea», con escepticismo por el momento. Cierra: la consulta del Pacto Histórico fue «positivo para la democracia», una «justa aspiración» |
| 18 | 2026-01-08 | `/opinion/editoriales/alentadoras-expectativas-rurales-para-el-cesar-en-2026` | C | Los proyectos de la ADR del Gobierno saliente son «alentadores»; pide que el próximo Gobierno «le dé continuidad» |
| 19 | 2026-03-23 | `/opinion/editoriales/de-subsidios-a-paneles-solares-gratis-2` | C leve | «Ha despertado buenas expectativas» el programa Colombia Solar de Minenergía, con reservas |
| 20 | 2026-04-13 | `/opinion/editoriales/prever-no-mas-humo-de-lena-en-hogares-urbanos` | C leve | Elogia el convenio de gas domiciliario con Minenergía y pide que el próximo presidente lo continúe |
| 21 | 2026-07-02 | `/opinion/editoriales/quien-responde-por-la-entrega-de-tierras-en-el-empalme-con-el-nuevo-gobierno` | C | Defiende la continuidad de la entrega de tierras del Gobierno saliente frente al entrante: «no puede depender de los calendarios electorales» |
| 22 | 2025-12-09 | `/opinion/editoriales/mientras-aplauden-megaobra-vial-del-caribe-bosconia-sigue-bloqueado` | M | Reconoce la Variante de Ciénaga («debemos reconocer la importancia») y a la vez: «el gobierno saca pecho [...] pese a que fue proyectada [...] en anteriores administraciones» |
| 23 | 2025-12-22 | `/opinion/editoriales/el-nuevo-terrorismo-que-al-cesar-tambien-llego` | M | «Resulta alentador el anuncio del Gobierno nacional» (antidrones), y «hay que exigirle mayor compromiso» |
| 24 | 2026-04-18 | `/opinion/editoriales/el-cesar-tierra-prometida-campo-empobrecido` | M | Cuestiona los resultados de la reforma agraria con el IPM, pero pide «darle un compás de espera» y reparte la culpa con la Gobernación |
| 25 | 2026-05-12 | `/opinion/editoriales/programa-de-tierras-debe-ser-con-mejor-comunicacion-regional` | M | Critica la comunicación de la ANT y trata la recuperación de predios como «actos de justicia histórica y construcción de paz» |

### 2.2 Después del cambio: 2026-08-07 → 2026-10-09 (gobierna De la Espriella)

| # | Fecha | Ruta | Clas. | Por qué |
|---|---|---|---|---|
| 26 | 2026-08-13 | `/opinion/editoriales/nombramientos-que-generan-esperanzas-para-el-cesar` | D | Celebra los nombramientos de cesarenses en el nuevo Gobierno: «una ventana de oportunidades» |
| 27 | 2026-08-24 | `/opinion/editoriales/balones-al-arco-de-la-reconstruccion` | D | Disculpa al presidente ante el «ruidoso cotarro» por los balones a niños del terremoto: «podría resultar siendo un gesto plausible» |
| 28 | 2026-08-31 | `/opinion/editoriales/hay-que-dimensionar-el-robo-de-hidrocarburos-en-el-cesar` | D leve | «Compartimos las inquietudes del presidente De La Espriella» |
| 29 | 2026-09-04 | `/opinion/editoriales/un-nino-que-asusta-hay-que-agilizar-el-plan-de-minagricultura` | D leve | Respalda el plan del ministro Dangond y pide agilizarlo |
| 30 | 2026-09-15 | `/opinion/editoriales/el-cesar-en-medio-de-la-campana-contra-el-eln-y-la-fuerza-urano` | D | «El gobierno de Abelardo De la Espriella está cumpliendo con su principal promesa [...]. Apoyamos esa tarea». Pide «reconsiderar las estrategias» tras la masacre de Simaña |
| 31 | 2026-10-05 | `/opinion/editoriales/abelardo-de-la-espriella-a-ritmo-de-puya-vallenata` | D | La seguridad, «un propósito que apoyamos»; programa propio (minería, hidrocarburos, menos «restricciones ambientales injustificadas» y «gravosos y desiguales tributos»); Petro «prometidas y nunca ejecutadas» frente a Duque «obras trascendentales». Un reparo: el «látigo» de la puya «genera tormentas sin fin» |
| 32 | 2026-08-11 | `/opinion/editoriales/llegan-mas-presos-senor-presidente-atienda-el-pedido-del-alcalde-de-valledupar` | C | Fiscaliza el traslado de presos de alto perfil decidido por el nuevo Gobierno: «un tema de mucho cuidado», respalda al alcalde y a la senadora que lo cuestionan |
| 33 | 2026-08-22 | `/opinion/editoriales/el-nuevo-eje-del-gobierno-sera-el-pacifico-y-no-el-caribe-ambos-viven-un-terremoto-social` | C leve | El nuevo Gobierno «ya no está pensando de la misma manera en el Caribe» |
| 34 | 2026-09-11 | `/opinion/editoriales/ojo-con-la-cultura-del-arma-en-la-region` | C leve | Ante el decreto de porte de armas, advierte el riesgo de «combinar arma, licor, celebración» y pide una política diferencial. No pide derogarlo |
| 35 | 2026-10-03 | `/opinion/editoriales/un-informe-para-pararle-oreja` | C leve | El nuevo Gobierno «no puede empezar de cero ni limitarse a la elaboración de nuevos diagnósticos» |
| 36 | 2026-10-09 | `/opinion/editoriales/ahorrar-energia-si-pero-sin-castigar-la-necesidad-del-servicio` | C leve | Los recargos de la CREG son «necesarios», pero castigan en el Caribe el consumo por calor |
| 37 | 2026-08-10 | `/opinion/editoriales/cuando-llegara-el-bloque-anticorrupcion-de-de-la-espriella-al-cesar` | M | «Apoyamos esas inquietudes», y advierte que combatir la corrupción no es «aprovechar eso para hacer persecuciones políticas» |
| 38 | 2026-09-07 | `/opinion/editoriales/reactivan-las-emisoras-publicas-en-el-cesar-el-tema-esta-en-mora` | M | «Muy acertada la decisión del Gobierno nacional» de reactivar las Emisoras de Paz: elogia al entrante en una política nacida del Acuerdo de 2016. **La ficha la lee como contrapeso; aquí es M** |
| 39 | 2026-10-07 | `/opinion/editoriales/del-arroz-y-otras-crisis-y-por-que-no-una-mision-animar-2` | M | Discute la frase del ministro Dangond a los arroceros y a la vez lo avala como «experto» |

### 2.3 Leídas y sin postura (se declaran, no cuentan)

- **2026-05-25**, [«¿Está bien que los medios o periodistas tomen partido?»](https://elpilon.com.co/opinion/editoriales/esta-bien-que-los-medios-o-periodistas-tomen-partido): a propósito del endoso de El Heraldo a De la Espriella (24-05), la casa declara que su junta directiva adoptó en 2010 unas «políticas editoriales» por las que **«no apoyará oficialmente (en editorial) ninguna campaña electoral»**. Es la prueba de que **no hay endoso**.
- **2026-06-23**, `/editorial/ceso-la-tempestad-electoral-ahora-toca-con-cabeza-fria-por-el-cesar`: conciliador, «remar todos para el mismo lado».
- **2026-07-10** (carta del Caribe al presidente electo), **2026-08-07** («llegó la hora de la verdad») y **2026-08-08** («Ahora le toca al nuevo Gobierno»): expectativa sin inclinación. El 08-08 pide «una oposición que pueda ejercer su función» y gobernar «incluidos quienes no votaron por él».
- **2026-10-06**, «¿Termoeléctrica propia?»: el reparo es a la propuesta de los alcaldes, no al Gobierno. **La ficha la lee como contrapeso; aquí no cuenta.**
- **2026-09-05**, «Hidrocarburos: el aporte…»: hace suyo el estudio de los gremios petroleros. Es programa, coherente con la dirección D, pero no es una postura sobre el Gobierno.
- **2025-10-15** (conflicto arhuaco: exhorta a Petro sin calificarlo), **2026-03-03** («fuga de votos» al Senado) y **2026-03-10** (nuevo Congreso): sin inclinación nacional.

---

## 3. Recuento

| | D (derecha) | C (contrapeso) | M (mixta, no cuenta) | Total con postura |
|---|---|---|---|---|
| Antes del 07-08-2026 | **16** | **5** | 4 | 25 |
| Desde el 07-08-2026 | **6** | **5** | 3 | 14 |
| **Total** | **22** | **10** | 7 | **39** |

**Proporción global: 22 a 10, es decir 2,2 a 1. No llega a 3 a 1.**

Sensibilidad, para que el lector la recuente:

| Lectura | D | C | Proporción |
|---|---|---|---|
| Principal (todas las D y C) | 22 | 10 | **2,2 : 1** |
| Las «leves» de los dos lados pasan a M (8 D, 6 C) | 14 | 4 | 3,5 : 1 |
| Solo las D «leves» pasan a M | 14 | 10 | 1,4 : 1 |
| Solo las C «leves» pasan a M | 22 | 4 | 5,5 : 1 |

Solo pasa de 3 a 1 si se descartan los contrapesos leves. La lectura principal no lo hace, y la regla 2 pide, ante la duda, quedarse en lo más cercano a la mixta.

**La lectura del polo fijo**, que separa fiscalizar a quien manda de lo que no lo es:

| Trato al gobierno **en ejercicio** | Favorables o reconocimientos | Críticos | Mixtos |
|---|---|---|---|
| Petro, mientras gobierna (10 meses) | **5** (#17-#21) | **15** (#1-#11, #13-#16) | 4 |
| De la Espriella, ya en el poder (2 meses) | **6** (#26-#31) | **5** (#32-#36) | 3 |

- **Con Petro**, la casa critica tres veces más de lo que reconoce. La crítica es sobre todo de **relación con el territorio** (abandono del Cesar, proyectos engavetados, Emdupar, Bosconia), con dos excursiones al **modelo**: el salario mínimo (#3) y el criterio político con gobiernos opuestos (#5). Ningún rótulo ideológico al Gobierno («extrema izquierda» y similares no aparecen).
- **Con De la Espriella**, apoya tanto como reparos pone. Pero el peso no es igual:
  - dos «apoyamos» explícitos a su bandera, la seguridad (#30, #31), una disculpa ante una polémica (#27) y un programa económico hecho propio (#31);
  - de los 5 reparos, solo uno es de fondo (#32, los presos). Los otros cuatro son leves y **ninguno critica una política central de su programa** (seguridad, armas, fracking, minería). El decreto de armas recibe pedagogía, no oposición (#34).
- **Sobre las candidaturas, antes de las urnas:** asimetría de encuadre (#12) y entusiasmo por el presidente electo (#13, #15, #16). Pero **ningún endoso**: la casa lo prohíbe por política desde 2010 (25-05-2026), reprocha a los dos candidatos que vengan «sin proyectos para la región» y la víspera de la segunda vuelta publica un editorial cultural.
- **La asimetría de la regla está, pero es moderada:** se fiscaliza más al saliente que al entrante, y al entrante se le apoya en su bandera. No es el patrón de El Diario de Pereira (0 piezas favorables a Petro frente a 52 críticas): aquí hay 5 reconocimientos a programas de Petro, 4 mixtas y un reparo de fondo a De la Espriella.

---

## 4. Contrapesos (lo que contradice la dirección, y cuánto pesa)

| Contrapeso | Piezas | Peso |
|---|---|---|
| **Reconocimiento de programas del Gobierno Petro y petición de continuidad**: ADR, gas domiciliario, Colombia Solar, entrega de tierras | #18, #19, #20, #21 | **Medio.** Son cuatro piezas a lo largo del año y piden expresamente que el Gobierno entrante no los corte. #21 lo pide en pleno empalme |
| **La reforma agraria del saliente, «muy notable»**, dicho en el editorial más asimétrico de la campaña | #12 (dentro), #24, #25 | **Medio-bajo.** Reconoce el avance, pero lo condiciona («compás de espera», comunicación) |
| **Consulta del Pacto Histórico, «positivo para la democracia»** | #17 | **Bajo.** Es procedimental, de octubre de 2025 |
| **Fiscalización de una decisión del nuevo Gobierno**: el traslado de presos | #32 | **Medio.** Es la única crítica de fondo a De la Espriella en dos meses, y se apoya en un alcalde y una senadora del Cesar |
| **Reparos leves al nuevo Gobierno**: el Caribe relegado, el porte de armas, «no puede empezar de cero», recargos de la CREG | #33-#36 | **Bajo.** Son matices regionales. Ninguno cuestiona la seguridad, el fracking ni la minería |
| **Política de no endoso desde 2010** y equidistancia formal en campaña | 25-05-2026; #12; 23-06-2026 | **Alto para la magnitud.** No cambia la dirección, pero es la razón de peso para no ponerlo por encima de El Heraldo, que sí endosó |
| **Matices dentro de las propias piezas D** | #2, #7, #11, #30, #31 | **Bajo.** «No todo lo malo [...] es responsabilidad del Gobierno nacional actual» (#11); «buena voluntad del actual gobierno» (#7); el «látigo» que «genera tormentas» (#31) |
| **Pluralidad en las columnas de junio** colgadas en la ruta de editorial, a favor y en contra de De la Espriella | §1 | **No cuenta.** Son terceros |

**Proximidad que se declara (no es contrapeso, ni nivel 1):** el ministro de Agricultura de De la Espriella, Indalecio Dangond, «escribió décadas en nuestras páginas» (#39). La casa lo llama «muy nuestro» (#13) y publicó su columna de campaña el 19-06-2026. Dos de las piezas posteriores al cambio tratan de su ministerio (#29, #39). Es afinidad con un miembro del Gobierno, no propiedad ni endoso. Va a TENSIONES si el responsable editorial lo considera.

---

## 5. Veredicto por condición

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | **Sí** | Las 39 piezas son editoriales sin firma que hablan como la casa. Se excluyeron 11 columnas firmadas y 4 notas colgadas bajo `/editorial/` |
| 2. A los dos lados del cambio (07-08-2026), en 12 meses | **Sí, con asimetría moderada** | Con Petro, 15 críticas y 5 reconocimientos. Con De la Espriella, 6 apoyos y 5 reparos (uno de fondo). No es solo fiscalizar a quien manda: al entrante se le apoya en su bandera |
| 3a. ≥10 piezas con postura | **Sí** | 39 |
| 3b. ≥3 a cada lado del cambio | **Sí** | 25 antes y 14 después. En la dirección D: 16 y 6 |
| 3c. Proporción ≥3:1 | **No** | 22:10 = **2,2:1**. Solo llega (3,5:1) si se descartan los contrapesos leves de los dos lados. Desde el 07-08 es 6:5 |
| 4. Contrapesos escritos | **Sí** | §4, con peso |
| 5. Reproducible | **Sí** | §2 con ruta, fecha y clasificación; §1 con el método y los días que faltan |

**Falla la condición 3c en la lectura principal.** Por la regla, «por debajo de eso es nivel 5 y no mueve el número».

---

## 6. PROPUESTA (pendiente de la firma del responsable editorial)

**+0,20, derecha moderada. Se mantiene.** El barrido no activa la regla nueva, así que el número sigue siendo, por la regla 3, el provisional de alta que era. Lo que cambia es que **ya no descansa solo en el parecido con la banda**: un barrido de 290 editoriales dice que la dirección es la correcta y que la magnitud no es mayor. Sigue sin firmarse.

**Por qué no bajar a 0,00.** El 0,00 con evidencia exige la misma conducta con los dos gobiernos, y no la hay:
- con Petro, 15 críticas y 5 reconocimientos; con De la Espriella, 6 apoyos y solo 1 crítica de fondo;
- dos «apoyamos» explícitos a la seguridad del entrante (#30, #31), ninguno equivalente a una política del saliente;
- programa propio en la dirección D: salario mínimo (#3), minería, hidrocarburos, menos restricciones ambientales y tributos (#31, 05-09);
- encuadre asimétrico entre candidatos (#12) y entre gobiernos (Petro frente a Duque, #16 y #31).

Bajar sería mover el número con un nivel 5 contra su propia dirección.

**Por qué no subir a +0,25 (Vive el Meta y El Diario de Pereira, propuestos hoy):**
- la proporción no llega a 3 a 1 (2,2:1);
- El Diario tiene 0 piezas favorables a Petro frente a 52 críticas y editoriales de campaña contra «la opción de izquierda». El Pilón reconoce cuatro programas de Petro, pide su continuidad y no toma partido en campaña;
- después del cambio, el apoyo al entrante (6) apenas supera a los reparos (5).

**Por qué no por encima de El Heraldo (+0,20, firmado).** El Heraldo endosó a De la Espriella en editorial (24-05-2026). El Pilón se negó a hacerlo por política escrita y lo dijo al día siguiente. Ponerlo por encima sería premiar con más magnitud al que no endosó. Mucho menos llega a Archipiélago Press (+0,30, propuesto) o a El Colombiano (+0,35, con propiedad con posición).

**Lectura alternativa, que se declara.** Si el responsable editorial considera que las piezas «leves» no tienen postura, y las quita de los dos lados (8 D y 6 C), el recuento queda 14:4 = 3,5:1 y las cinco condiciones se cumplen. **El valor sería el mismo, +0,20, pero ahora con evidencia** (nivel 2 por la regla nueva), por las mismas razones de vecindad: por debajo de Vive el Meta y El Diario, y a la altura de El Heraldo sin su endoso. Las dos lecturas dan el mismo número. Solo cambia si el +0,20 es evidencia o sigue siendo provisional.

**Una cuestión que no resuelve este barrido.** DECISIONES (2026-10-09) dice que los medios de la tanda 5 «se quedan en 0,00» si el barrido no alcanza. Aquí se lee «se quedan» como «se quedan donde estaban», y El Pilón estaba en +0,20. Si el responsable editorial entiende que un valor de banda sin barrido suficiente debe volver a 0,00, la decisión afecta a la vez a todos los regionales que están en su banda por parecido (El Universal, La Patria, Vanguardia, La Opinión, El País de Cali). No se puede tomar solo para El Pilón.

**Lo que esta propuesta NO hace:**
- No hace firmable la ficha: la junta y el accionariado siguen sin registro (falta el certificado de la Cámara de Valledupar).
- No toca las tensiones locales (FELVA y edictos contratados por la Alcaldía, Corpocesar), que siguen declaradas.
- No cambia nada de la ficha. Las correcciones que sugiere este barrido (#38 y 06-10 no son contrapesos; el hueco de enero a mayo está cubierto; `/opinion/editoriales/` tiene el año entero) se aplicarían solo si el responsable editorial lo decide.

**Qué la refutaría:**
- hacia arriba: que en los próximos meses los reparos al Gobierno De la Espriella desaparezcan y los «apoyamos» se extiendan a su programa (armas, fracking, Paz Total), o un endoso con nombre en la próxima elección, que además levantaría el tope de ±0,30;
- hacia abajo: que la casa critique de fondo la seguridad o la política minera del entrante con la frecuencia con la que criticó al saliente;
- o que los editoriales de junio de 2026 que no se encontraron (11 días hábiles, en plena segunda vuelta) cambien el recuento.

---

## 7. Avisos

- **Una sola lectura.** La clasificación es de un verificador de la misma casa que el autor de la ficha. Las piezas límite están marcadas «leve» o «M», y el §3 da el recuento con y sin ellas.
- **El hueco de junio de 2026.** Es el mes de la segunda vuelta y el de peor cobertura (17 editoriales, 11 días hábiles sin pieza). El 22-06, día siguiente a la segunda vuelta, falta. La política de no endoso (25-05) y el editorial cultural del 20-06 hacen improbable un endoso en esos días, pero no se ha comprobado.
- **Internet Archive solo sirvió para encontrar URL.** Todo el texto citado sale de elpilon.com.co, descargado el 2026-10-09. El índice CDX estuvo intermitente («Temporarily Offline») y algunas consultas se repitieron.
- **El lado de después es corto:** dos meses y 54 editoriales, frente a diez meses y 236. Cualquier lectura de la mitad posterior es frágil.
- **El 07-08-2026** se publicó «Como dice un vallenato: llegó la hora de la verdad», sin inclinación. Si se pasa al lado de antes, nada cambia.
- **Datos personales.** No se copia ningún número de documento, teléfono ni dirección. Las personas nombradas son cargos públicos o columnistas, con su papel.
