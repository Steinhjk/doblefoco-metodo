# Barrido editorial — Abra Noticias (abranoticias.com)

| | |
|---|---|
| **Para qué** | Comprobar las cinco condiciones de «Evidencia editorial histórica» (`PROTOCOLO_JUICIO_EDITORIAL.md`, §1, añadida el 2026-10-09) antes de mover el 0,00 de la ficha |
| **Fecha** | 2026-10-09 (hora de Colombia) |
| **Quién** | Claude Code (Claude Opus 5.5), a petición del responsable editorial. Es de la misma casa que el autor de la ficha, que el revisor y que quien escribió la resolución: el acuerdo con ellos no es aval |
| **Resultado** | **No se cumplen las cinco condiciones.** En la lectura estricta hay **7 piezas con postura en voz de la casa** (3 antes y 4 después del 07-08-2026), las 7 a la izquierda y 0 a la derecha. El mínimo es 10. **El número no se mueve: 0,00** |
| **Ficha** | [`fichas/abra-noticias.md`](../../fichas/abra-noticias.md) |
| **Resolución** | [`respuestas/opus-5-5-abra-noticias.md`](../respuestas/opus-5-5-abra-noticias.md) |

---

## 1. Método, para poder repetirlo

**robots.txt** de abranoticias.com, leído el 2026-10-09 antes de descargar nada:
«User-agent: * / Allow: /». No excluye ninguna ruta ni ningún agente.

**Archivo de 12 meses, desde la API pública de WordPress del propio medio:**

```
https://abranoticias.com/wp-json/wp/v2/posts?per_page=100&page=1…8&after=2025-10-09T00:00:00
  &_fields=id,date,link,title,content,author,categories
X-WP-Total: 752
```

- Las 752 entradas van del 2025-10-13 al 2026-10-09; entre el 09-10 y el 13-10-2025 no hay ninguna.
- 517 son anteriores al 07-08-2026 y 235 son de ese día en adelante.
- Fechas: el campo `date` de la API, en hora de Colombia.
- La resolución contó 751 (518 + 233) con la ventana del 2025-10-08 al 2026-10-08. La diferencia es solo de ventana.
- Todas las entradas tienen `author` 2: la cuenta «ABRA NOTICIAS», slug `atisbernal`.

**Qué se leyó.**
1. **Los 752 titulares**, uno por uno.
2. **El cuerpo entero de 97 piezas.** Son todas las que tratan de política nacional o de los actores del eje: las que nombran a Petro, De la Espriella, Cepeda, Uribe, el Pacto Histórico o el Centro Democrático, a la «derecha» o la «izquierda», al gobierno o al presidente de la República, a candidatos o al Congreso. También 14 de las 18 entradas de Opinión de la ventana.
   Las otras 4 son columnas firmadas largas, de historia y de crónica (05-07, 06-07, 17-07 y 28-07-2026): se leyó su arranque y se rastrearon por términos. Ninguna toma partido en el eje.
3. **Fragmentos de contexto de otras 35** que solo mencionaban «gobierno», «presidente» o «derecha» de pasada: secretarías de gobierno municipales, presidentes de juntas comunales, «la mano derecha» de un cabecilla. Ninguna tiene postura.
4. **Una búsqueda por términos sobre los 752 cuerpos**, para no dejar fuera rótulos sueltos: `petris|desgobierno|gobierno del cambio|progresis|oligarq|ultra derech|extrema derech|fascis|arrodill|uribis|zurd|mamert|castrochav|comunis|neoliberal|élite|burgues|fantoche|payaso|tirano|dictador`. Todas las piezas que devuelve están clasificadas abajo.

**Cómo se clasificó.** Se aplicó el protocolo al pie de la letra.

Solo cuenta la **voz de la casa**:
- las piezas de Opinión sin firma;
- la narración propia de las noticias, que todas salen sin firma de la cuenta «ABRA NOTICIAS»;
- los titulares y entradillas propios.

**No cuentan:**
- las columnas firmadas por terceros;
- las reimpresiones («Tomado de…»);
- las cartas y los comunicados que se publican enteros;
- las declaraciones de terceros que la pieza recoge;
- la **fiscalización de una medida concreta**, que la regla del polo fijo excluye.

**Se marcan como dudosas** las piezas en las que no se puede saber si la frase es de la casa o de la fuente que reescribe, y las que no están en el eje colombiano. Las dudosas se cuentan aparte.

La clasificación es de este barrido. Cualquiera puede repetir la consulta y volver a contar.

---

## 2. Piezas contadas: postura en voz de la casa (lectura estricta)

| # | Fecha | Lado | Pieza | Voz | Clasificación y cita literal |
|---|---|---|---|---|---|
| 1 | 31-10-2025 | antes | [Petro canceló contrato con empresa estadounidense…](https://abranoticias.com/petro-cancelo-contrato-con-empresa-estadounidense-que-no-abastecio-combustible-al-avion-presidencial/) | narración propia (Nación) | **Izquierda (débil):** defiende a Petro frente a Trump: «Es decir, el presidente gringo no aprobado sin ninguna documentación lo dicho en días anteriores contra Petro». Es la más floja de las siete: es una disputa diplomática, no un rótulo ideológico |
| 2 | 06-02-2026 | antes | [«Peñuela debe hablar mal de su adversario para pescar votos en Nariño»](https://abranoticias.com/penuela-debe-hablar-mal-de-su-adversario-para-pescar-votos-en-narino/) | narración propia (Noticias), antes de citar a «los internautas» | **Izquierda:** a los congresistas que votaron contra las reformas los presenta así: «se fueron en contra del Gobierno, donde votaron negativamente a las reformas. Es decir, no fue en contra del mandatario sino de todo un pueblo» |
| 3 | 02-06-2026 | antes | [Por esta declaración internautas se le fueron con toda a exalcaldesa de Policarpa](https://abranoticias.com/por-esta-declaracion-internautas-se-le-fueron-con-toda-a-exalcaldesa-de-policarpa/) | narración propia (Noticias) | **Izquierda:** «se declaró en apoyo a la extrema derecha», «Hoy se volvió al lado de la extrema derecha», y en voz propia: «El candidato presidencial Abelardo de la Espriella, son bastantes polémicas sus propuestas, que hasta dijo que va a destripar a la izquierda radical, habrá fraking, bajará el salario mínimo…» |
| 4 | 01-09-2026 | después | [Abelardo de la Espriella comenzó a censurar medios de comunicación como lo hizo Hugo Chávez en el 2004](https://abranoticias.com/abelardo-de-la-espriella-comenzo-a-censurar-medios-de-comunicacion-como-lo-hizo-hugo-chavez-en-el-2004/) | **Opinión sin firma** | **Izquierda (la más fuerte):** «ayudaron a elegir a un fantoche presidente de la oligarquía», «no puede ser apagado por un presidente fantoche y payaso» y la absolución expresa del gobierno saliente: «Ese cuento la extrema derecha quiso amilanar al gobierno progresista, a quien lo acusaron de llegar al poder censuraría a la prensa […] lo cual nunca sucedió» |
| 5 | 04-09-2026 | después | [Mataron a líder social juvenil que participó en un evento con Petro…](https://abranoticias.com/mataron-a-lider-social-juvenil-que-participo-en-un-evento-con-petro-vuelve-la-violencia-contra-lideres-sociales/) | narración propia (Nación) | **Izquierda:** «El homicidio de la joven líder social juvenil es una advertencia más de que el actual gobierno abandonará a todos los dirigentes que quedan a merced de sus enemigos de la extrema derecha» y «en este gobierno se recrudeció la violencia contra los líderes sociales en el país» |
| 6 | 10-09-2026 | después | [Frenan a periodistas del establecimiento y les dicen que son vampiros del periodismo en Colombia](https://abranoticias.com/frenan-a-periodistas-del-establecimiento-y-les-dicen-que-son-vampiros-del-periodismo-en-colombia/) | titular y entradilla propios | **Izquierda:** defiende al expresidente y descalifica a otros medios: «dos periodistas del Blu Radio y El Tiempo, medios arrodillados al establecimiento» |
| 7 | 12-09-2026 | después | [UNP le quitó esquema de seguridad a influencer](https://abranoticias.com/unp-le-quito-esquema-de-seguridad-a-influencer/) | entradilla y narración propias | **Izquierda:** «Al parecer ser crítico del actual gobierno, le mandaron a quitar la seguridad» y «por ser un reconocido crítico de los políticos de la extrema derecha en Colombia». La pieza recoge también la versión de la UNP (auditoría general de esquemas) |

**Postura en voz de la casa a la derecha** (contra Petro, el Pacto o la izquierda, o a favor de la derecha como bando): **0**, a los dos lados del 07-08-2026.

**Ninguna pieza de la casa critica al gobierno Petro mientras gobernó** (13-10-2025 → 06-08-2026), ni al expresidente después. Las únicas críticas a ese gobierno que aparecen son de terceros que el medio recoge: el director de Corpocarnaval, «El Gobierno actual no cumplió» ([22-07-2026](https://abranoticias.com/en-pasto-se-realizara-el-onomastico-y-carnaval-de-negros-y-blancos-2027-esto-dicen-los-concejales/)); el comunicado de un frente de las Farc ([14-04-2026](https://abranoticias.com/las-farc-declara-objetivo-militar-al-presidente-gustavo-petro/)); y la columna del Eln sobre la «Paz Total» ([26-04-2026](https://abranoticias.com/explosivo-ataque-del-eln-contra-alvaro-uribe-velez-miedo-electoral/)).

---

## 3. Dudosas: no entran en la lectura estricta

| Fecha | Lado | Pieza | Por qué es dudosa |
|---|---|---|---|
| 18-02-2026 | antes | [El 'niño' rico que no quiere a su pueblo](https://abranoticias.com/el-nino-rico-que-no-quiere-a-su-pueblo/) (Opinión sin firma) | Insulta al presidente de Ecuador, Daniel Noboa («niño caprichoso, arrogante y desobediente»), por los aranceles a Colombia. **No está en el eje colombiano**: defiende el interés de la frontera, no a un bando |
| 30-05-2026 | antes | [Noboa metido en política de otro país…](https://abranoticias.com/noboa-medito-en-politica-de-otro-pais-y-ecuador-con-la-peor-crisis-de-seguridad/) | En voz propia contra Noboa («show mediático de un niño gomelo») porque se reunió con el candidato De la Espriella: «debe ser investigado, por intervenir en política de otra nación». Toca el eje solo de lado |
| 30-06-2026 | antes | [En Pasto seguidoras del presidente electo «te vamos a estripar» a defensora de DDHH](https://abranoticias.com/en-pasto-seguidoras-del-presidente-electo-te-vamos-a-estripar-a-defensora-de-ddhh/) | La frase «Tras la llegada de la extrema derecha al poder, han comenzado a surgir las amenazas de muerte contra los dirigentes» va sin atribución, pero justo después de «Así lo escribió el medio», dentro de una nota que reescribe al portal Al Punto. **No se puede saber si es de la casa** |
| 08-07-2026 | antes | [«Se configura un gobierno paramilitar», Cepeda a Abelardo](https://abranoticias.com/se-configura-un-gobierno-paramilitar-cepeda-a-abelardo/) | «el elector presidente de la extrema derecha» aparece dentro de una nota que parafrasea a Cepeda de principio a fin. Puede ser paráfrasis suya |
| 14-09-2026 | después | [«Abelardo busca engañar su propia incapacidad…», dice Petro al presidente](https://abranoticias.com/abelardo-busca-enganar-su-propia-incapacidad-de-gobernar-a-colombia-dice-petro-al-presidente/) | La entradilla propia es asimétrica en intensidad («el presidente de la ultra derecha en Colombia Abelardo de la Espriella contra el expresidente de la izquierda Gustavo Petro»), pero rotula a los dos. El resto es el texto de Petro |

---

## 4. Fiscalización de medidas: no cuenta (regla del polo fijo)

Todas son del gobierno entrante. Se anotan porque, en los 517 artículos anteriores al cambio, **no hay ni una pieza equivalente sobre el gobierno Petro**. Esa ausencia ya está contada en la sección 2.

| Fecha | Pieza | Qué critica |
|---|---|---|
| 25-08-2026 | [Iniciarán operativos con migrantes ilegales…](https://abranoticias.com/iniciaran-operativos-con-migrantes-ilegales-en-colombia-asi-lo-anuncio-el-presidente/) | «muchos afirman que es una simple vil copia del presidente de los Estados Unidos Donal Trump». Lo atribuye a «muchos» y recoge el respaldo de «un sector» |
| 21-08-2026 | [GOLPE SILENCIOSO A LA PROTECCIÓN LABORAL EN COLOMBIA…](https://abranoticias.com/golpe-silencioso-a-la-proteccion-laboral-en-colombia-dejan-sin-efecto-11-circulares/) | La derogación de 11 circulares del Ministerio del Trabajo («un golpe silencioso pero certero contra la clase trabajadora») |
| 03-09-2026 | [Policías que prestaron seguridad al expresidente Petro los trasladaron a zonas de conflicto armado](https://abranoticias.com/policias-que-prestaron-seguridad-al-expresidente-petro-los-trasladaron-a-zonas-de-conflicto-armado/) | El traslado de los escoltas. Da también la explicación oficial («reforzar las operaciones») |
| 09-09-2026 | [Presidente firmó decreto del porte de armas y estudiante ingresó armado…](https://abranoticias.com/presidente-firmo-decreto-del-porte-de-armas-y-estudiante-ingreso-armado-para-matar-a-su-docente/) | El titular junta el decreto y el tiroteo. El cuerpo cita a Isabel Zuleta y a un internauta que dice: «No podemos afirmar que una cosa haya provocado la otra» |
| 09-09-2026 | [Congresista tumba imágenes del presidente que se paseó en medio de cadáveres](https://abranoticias.com/congresista-tumba-imagenes-del-presidente-que-se-paseo-en-medio-de-cadaveres/) | Las imágenes del presidente entre abatidos: «como si fueran un trofeo» |

---

## 5. Contrapesos en voz de la casa

| Fecha | Lado | Pieza | Qué contradice la dirección |
|---|---|---|---|
| 04-02-2026 | antes | [Campañas de insultos…](https://abranoticias.com/campanas-de-insultos-politicos-se-sacan-los-trapitos-al-sol/) (Opinión sin firma) | Reparte por igual: «Las campañas de hoy, no son transparentes ni de propuestas sino se han convertido en un tema de ataques». La única pieza de Opinión sin firma con tema político nacional antes del cambio no toma partido |
| 22-07-2026 | antes | [Atribuyen a grupo armado del homicidio de líder social y periodista](https://abranoticias.com/atribuyen-a-grupo-armado-del-homicidio-de-lider-social-y-periodista/) | Pone distancia con lo que dice Petro: «las autoridades competentes no han confirmado públicamente la autoría del crimen» |
| 13-08-2026 | después | [Primera dama anunció este beneficio gratuito…](https://abranoticias.com/primera-dama-anuncio-este-beneficio-gratuito-para-familias-que-perdieron-a-sus-seres-queridos-en-el-terremoto/) | Trato favorable a la esposa del presidente entrante: «una de las gestiones que se destaca» |
| 04-09-2026 | después | [Los cogieron durmiendo a 'Bendito Menor' y a 'La Bebecita'…](https://abranoticias.com/los-cogieron-durmiendo-a-bendito-menor-y-a-la-bebecita-fueron-abatidos-en-operativo-policial/) | Un resultado de seguridad del nuevo gobierno contado como «un contundente golpe» |
| 08-09-2026 | después | [La Fuerza Pública le estarían cerrando el cerco a cabecillas del Eln y disidencias](https://abranoticias.com/la-fuerza-publica-le-estarian-cerrando-el-cerco-a-cabecillas-del-eln-y-disidencias/) | Hace suya la ofensiva: «Tras la orden de Abelardo, la cacería militar no se detiene» |
| 11-09-2026 | después | [Ordenan retirar elementos de las cárceles. «Se les acabó el 'hotel'»](https://abranoticias.com/ordenan-retirar-elementos-de-las-carceles-se-les-acabo-el-hotel/) | Aprueba la medida en voz propia: «Se acaba los privilegios en los centros penitenciarios», «Los internos no deben tener es nada.» |
| 12-09-2026 | después | [¿En Colombia se acaba el negocio de las fotomultas?…](https://abranoticias.com/en-colombia-se-acaba-el-negocio-de-las-fotomultas-esta-fue-la-orden-del-presidente/) | Presenta sin reparos la revisión de las fotomultas ordenada por el presidente |
| 12-09-2026 | después | [Tras señalamientos del presidente contra gobernador de Nariño, Petro llama apoyar a Escobar a las calles](https://abranoticias.com/tras-senalamientos-del-presidente-contra-gobernador-de-narino-petro-llama-apoyar-a-escobar-a-las-calles/) | Choque entre Petro y De la Espriella contado con las dos versiones y sin rótulos |
| 14-09-2026 | después | [«La universidad es conocimiento, de ideas, debate y no refugio del terrorismo», dijo el presidente](https://abranoticias.com/la-universidad-es-conocimiento-de-ideas-debate-y-no-refugio-del-terrorismo-dijo-el-presidente/) | Transmite el ultimátum sin reparos, con el contexto de los daños de las protestas |
| 24-09-2026 | después | [Integrantes de las disidencias se entregó a unidades militares](https://abranoticias.com/integrantes-de-las-disidencias-se-entrego-a-unidades-militares/) | Recoge sin reparos el balance del presidente |

**Cuánto pesan.** Las dos piezas de antes del cambio pesan poco: una reparte críticas sin ideología, la otra matiza a Petro. Las de después son reales pero de un solo tipo. Aprueban medidas de seguridad y orden, y ninguna celebra al gobierno entrante como proyecto político ni le aplica un rótulo favorable. Contradicen la idea de una oposición total al nuevo gobierno. **No equilibran los rótulos ideológicos, que van solo en un sentido.**

Las columnas firmadas que hacen de contrapeso están en la sección 7.

---

## 6. Relevos, reimpresiones y comunicados: no cuentan

El medio elige qué recoge, y el patrón se declara. Pero no es voz de la casa.

- **A favor de Petro, Cepeda o el Pacto, o contra la derecha** (13):
  - [16-10-2025](https://abranoticias.com/celag-dice-que-gustavo-petro-mejor-presidente-de-la-historia-de-colombia/), CELAG: **«Tomado de: RTVC NOTICIAS»**, es una reimpresión. La resolución trataba como «subtítulo propio» su «Presidente Petro, el mejor presidente de la historia»; ver la sección 8;
  - [19-11-2025](https://abranoticias.com/la-dura-respuesta-de-petro-a-ivan-mordisco/), trino de Petro;
  - [23-11-2025](https://abranoticias.com/asi-respondio-sargento-a-abelardo-de-la-espriella-por-saludo-militar/), carta de un sargento a De la Espriella;
  - [25-11-2025](https://abranoticias.com/condenan-en-segunda-instancia-a-santiago-uribe-velez-a-mas-de-28-anos-de-prision/) y [04-06-2026](https://abranoticias.com/ratifican-condena-a-28-anos-de-carcel-a-santiago-uribe-estos-fueron-los-delitos/), condena de Santiago Uribe, «Tomado de: RTVC» y «Tomado de: Radio Nacional»;
  - [14-03-2026](https://abranoticias.com/ella-es-yira-castro-mama-del-candidato-ivan-cepeda/), semblanza de la madre de Cepeda, «Texto Facebook: Iván Gallo»;
  - [26-04-2026](https://abranoticias.com/explosivo-ataque-del-eln-contra-alvaro-uribe-velez-miedo-electoral/), columna del Eln contra Uribe, amplificada con signos de admiración («¡ACUSACIÓN DIRECTA Y SIN PRECEDENTES!»);
  - [01-06-2026](https://abranoticias.com/la-contundente-respuesta-de-petro-tras-un-ataque-del-tigre-abelardo/), texto de Petro;
  - [28-07-2026](https://abranoticias.com/solo-atacare-a-angie-penalmente-porque-ha-decidido-el-camino-de-la-calumnia-petro-a-rodriguez/), texto de Petro;
  - [04-08-2026](https://abranoticias.com/las-5-demandas-que-buscan-tumbar-a-abelardo-de-la-espriella/), demandas de nulidad en primera persona del demandante;
  - [06-08-2026](https://abranoticias.com/que-dice-la-carta-que-escribio-un-sargento-r-al-presidente-gustavo-petro/), carta de agradecimiento a Petro;
  - [24-07-2026](https://abranoticias.com/congresista-tumaqueno-dice-que-no-asistira-a-posesion-de-abelardo/), congresista que no irá a la posesión;
  - [16-08-2026](https://abranoticias.com/fallecio-exalcalde-el-parapolitico-nando-diaz/), texto firmado por un activista en el exilio.
- **Contra el gobierno De la Espriella, de terceros** (6):
  - [27-08-2026](https://abranoticias.com/esta-es-la-razon-de-la-manifestacion-de-estudiantes-de-la-universidad-de-narino-en-pasto/), comunicado estudiantil;
  - [27-08-2026](https://abranoticias.com/congresistas-del-pacto-historico-recusan-a-ministra-de-salud-y-piden-apartarla-de-la-definicion-de-recursos-para-las-eps-en-2027/), recusación del Pacto;
  - [22-09-2026](https://abranoticias.com/el-discurso-de-odio-y-mentiroso-del-irresponsable-presidente-le-dicen-congresistas-a-abelardo-tras-paro-armado/), congresistas;
  - [23-09-2026](https://abranoticias.com/identifican-a-presuntos-integrantes-de-la-banda-criminal-abelardo-mataste-a-mi-hijo-voy-a-denunciarte/), madre de un abatido;
  - [25-09-2026](https://abranoticias.com/en-putumayo-a-defensor-de-derechos-humanos-lo-torturaron-y-le-quitaron-la-vida/), comunidad de Villagarzón;
  - [14-09-2026](https://abranoticias.com/abelardo-busca-enganar-su-propia-incapacidad-de-gobernar-a-colombia-dice-petro-al-presidente/), texto de Petro.
- **Contra el gobierno Petro, de terceros** (3): las tres de la sección 2 (Corpocarnaval, Farc y Eln).

---

## 7. Opinión: 18 entradas en la ventana, firmadas o no

| Fecha | Firma | Pieza | Lectura |
|---|---|---|---|
| 04-11-2025 | Rober Atis Bernal | [Se juntan los viejitos canosos, ¿Temen a Iván Cepeda?](https://abranoticias.com/se-juntan-los-viejitos-canosos-temen-a-ivan-cepeda/) | Toma partido en plena campaña («La extrema derecha que por más de 200 años ha gobernado a Colombia…», «Y temen que nuevamente les gane el poder la izquierda con […] Iván Cepeda»). **No cuenta como voz de la casa:** está firmada por una persona y no consta que dirija el medio. Si constara, sería la octava pieza antes del cambio |
| 04-02-2026 | sin firma | Campañas de insultos | Contrapeso (sección 5) |
| 18-02-2026 | sin firma | El 'niño' rico… | Dudosa, fuera del eje (sección 3) |
| 30-06, 03-07, 05-07, 09-07, 24-07, 28-07 y 24-08-2026 | Pablo Emilio Obando A. (siete; la del 03-07 abre «Po: …») | Nariño, Ley de Fronteras, Bernardo de la Espriella, juventud, Pasto | **Contrapesos firmados.** Desmiente un bulo contra el «presidente electo, doctor Abelardo de la Espriella» (03-07) y elogia la carta del gobernador al presidente electo: «Nariño no puede darse el lujo de permanecer distante del Gobierno Nacional» (09-07) |
| 04-07, 10-07, 17-07, 31-07 y 16-08-2026 | Fernando Alexis Jiménez / Alexis Fernando Jiménez | Crónicas | Contrapeso firmado el 10-07: «Hay un nuevo presidente electo, nos guste o no» y la petición de un «Acuerdo Nacional». El resto no toca el eje |
| 06-07-2026 | Enrique Herrera Enríquez | De la caída de un corcel al poder | Historia; fuera del eje |
| 01-09-2026 | sin firma | Abelardo de la Espriella comenzó a censurar… | **Contada** (sección 2, n.º 4) |
| 08-10-2026 | Harold Ruiz | [LA NUEVA DERECHA VS LA IZQUIERDA](https://abranoticias.com/la-nueva-derecha-vs-la-izquierda/) | Militante («le corresponde a las fuerzas progresistas y de izquierda, salir del impacto de la pasada derrota electoral…»). Columna de un tercero: no cuenta |

Fuera de la ventana, la categoría tiene otras 5 entradas (2024). Entre ellas, la otra columna firmada por Rober Atis Bernal, [«¿En Ipiales todo es culpa de Amilcar?»](https://abranoticias.com/en-ipiales-todo-es-culpa-de-amilcar/) (09-11-2024, publicada desde la cuenta «adminabra»), y la única firmada «Por: ABRA NOTICIAS» (10-05-2024). Total de la categoría: `X-WP-Total: 23`.

---

## 8. Las cinco condiciones, con los números

| Condición | ¿Se cumple? | Números |
|---|---|---|
| 1. Voz de la casa | se aplicó | Solo cuentan las piezas sin firma de la cuenta «ABRA NOTICIAS» y sus titulares y entradillas. Columnas, reimpresiones y relevos aparte |
| 2. A los dos lados del cambio de gobierno, en 12 meses | **sí, por poco** | 3 antes y 4 después. Las 3 de antes incluyen la del 31-10-2025, la más débil: Petro contra Trump, sin rótulo ideológico |
| 3. Sostenida: ≥10 piezas, ≥3 por lado, ≥3:1 | **NO** | **7 piezas** (no llega a 10). Proporción 7:0, que sí la cumple |
| 4. Contrapesos escritos | sí | Sección 5: 2 antes y 8 después. Más las columnas de Obando y Jiménez (sección 7) |
| 5. Reproducible | sí | Este archivo |

**Qué haría falta para llegar a 10.** Habría que contar como voz de la casa piezas que el protocolo excluye o en las que la duda es real:

| Lectura | Antes | Después | Total | ¿≥10? |
|---|---|---|---|---|
| Estricta (sección 2) | 3 | 4 | **7** | no |
| + las dos dudosas más defendibles (Noboa-De la Espriella, 30-05; entradilla del 14-09) | 4 | 5 | 9 | no |
| + las dos frases sin atribución clara dentro de notas que reescriben a otros (30-06, 08-07) | 6 | 5 | 11 | sí, contando las cuatro dudas a favor de la dirección |
| + los titulares de fiscalización (25-08 y los dos del 09-09) | 6 | 8 | 14 | sí, pero contra la regla del polo fijo |

Para pasar el umbral hay que resolver cuatro dudas, y las cuatro a favor de la dirección. **La regla 2 manda la banda más cercana a la mixta.** El 0,00 se queda, ya no como valor por defecto sino con la dirección escrita como tensión.

**Lo que este barrido corrige de la resolución del 2026-10-08:**
- **La pieza CELAG (16-10-2025) es una reimpresión** («Tomado de: RTVC NOTICIAS»). No es «voz de la casa con subtítulo propio».
- **El 04-06-2026 (barristas)** dice «la segunda vuelta presidencial que quiere continuar con el segundo mandato del gobierno progresista». Es descriptivo: no se cuenta como postura.
- **El 30-06 y el 08-07-2026** quedan como dudosas, por la atribución.
- **Se añade el 06-02-2026 (Peñuela)**, que la resolución no tenía.
- La resolución hablaba de «unas 20 piezas con postura en 751». Con el filtro de voz de la casa son **7 seguras y 4 dudosas**. El resto son relevos, columnas o fiscalización.
- **«Relevos en contra de Petro: 0» no es exacto.** Hay al menos uno de un tercero no armado: Corpocarnaval, 22-07-2026.
- La cuenta «adminabra» publicó hasta el **18-04-2025**, no hasta marzo. La cuenta «ABRA NOTICIAS» empieza el 26-04-2025. Totales a 2026-10-09: 754 y 910; 1.664 entradas en el archivo.

---

## 9. Otras comprobaciones del mismo día (2026-10-09)

- **`/wp-json/wp/v2/users`:** `{"id":2,"name":"ABRA NOTICIAS",…,"link":"https://abranoticias.com/author/atisbernal/","slug":"atisbernal"}`. La cuenta 1 es «adminabra».
- **Páginas:** `/wp-json/wp/v2/pages` devuelve `[]`; `/quienes-somos/` y `/contacto/` dan 404.
- **Portada en crudo:**
  - una aparición de cada dato de plantilla: «555-0156», «Miller Court», «Hagerstown» y «[correo omitido]»;
  - el pie «Copyright &copy; Todos los derechos reservados.»;
  - 0 enlaces a facebook.com, twitter.com, x.com, instagram o tiktok.
  - Una pieza del 03-09-2026 incrusta un trino de «ABRA-NOTICIAS (@AbraNoticias)»: hay una cuenta en X que la portada no enlaza.
- **Feed:** 10 ítems, 0 `enclosure`, 0 `media:content`, los 10 con `dc:creator` «ABRA NOTICIAS».
- **datos.gov.co.** robots.txt pide `Crawl-delay: 1` y excluye solo rutas `/browse`. Resultados:
  - RUES (`c82u-588k`) por razón social «ABRA…NOTICIA», «ABRANOTICIA» y «ATIS…BERNAL»: **0**;
  - SECOP I (`f789-7hwg`) y SECOP II (`jbjy-vk9h`) por «ABRA NOTICIA» / «ABRANOTICIA»: **0 contratos a nombre del medio**.
  - Por «ATIS BERNAL» aparecen dos personas naturales distintas, con dos números de identificación distintos. **Ninguno se escribe aquí**, y no se atribuye al medio ni a la firma del sitio ningún contrato: homonimia no descartada.
