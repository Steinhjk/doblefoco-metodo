# Cambio — ficha de orientación

| | |
|---|---|
| **Medio** | Cambio · `cambio` · cambiocolombia.com |
| **Valor vigente** | **sin medir de forma permanente desde el 2026-10-12** (`bias: null`, `reviewedAt: null`) — decisión del responsable editorial: no autoriza la lectura por IA y no habrá lectura humana (`DECISIONES.md`, «2026-10-12 · Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Firma** | — (sin medir de forma permanente desde el 2026-10-12; la firma en bloque del 2026-10-10 recaía sobre el valor anterior, ver DECISIONES.md) |
| **Alta** | 2026-09-08 |
| **Última revisión** | — |
| **Departamento / ámbito** | Nacional |
| **Fuentes de propiedad** | `shared/mediaOwnership.js` (`cambio`): 11 fuentes; comprobada el 2026-10-07 |
| **Recogida** | `https://cambiocolombia.com/feeds/articulos/` · vía `direct` |
| **Protocolo** | `PROTOCOLO_JUICIO_EDITORIAL.md` |

## Estado

> **SIN MEDIR DE FORMA PERMANENTE DESDE EL 2026-10-12** (decisión del
> responsable editorial; `DECISIONES.md`, «2026-10-12 · Veinte medios: barridos
> firmados, sin medir permanente para quien no autoriza la IA, y feeds que se
> mantienen»). DobleFoco ubica a los medios leyendo sus piezas con sistemas
> automáticos; este medio no autoriza esa lectura por IA en su robots.txt, así
> que no tiene lugar en el eje. DobleFoco se actualiza de forma 100 % automática
> y **no habrá lectura humana**: la promesa de la decisión de la mañana se
> retira, y la plantilla `revision-externa/lectura-humana/` se borró el mismo
> día. Si el medio autoriza la lectura, se medirá: se le pedirá permiso por
> correo tras el lanzamiento. **El feed se mantiene**
> (`cambiocolombia.com/feeds/articulos/`), por decisión del responsable
> editorial, como ejercicio de transparencia, y se vigila: sus titulares siguen
> en el agregador con enlace.
>
> **Historia — la decisión de la mañana del 2026-10-12, que lo anterior
> sustituye.** **SIN MEDIR DESDE EL 2026-10-12 (decisión del responsable editorial;
> `DECISIONES.md`, «Cambio y La Silla Vacía, sin medir hasta una lectura
> humana»).** El −0,40 pasa a `bias: null` y `reviewedAt: null`. **Motivo:** el
> robots.txt de cambiocolombia.com excluye a ClaudeBot (consta abajo, en el
> nivel 1, desde el 2026-10-07), así que el barrido de 12 meses que exige la
> regla «Evidencia editorial histórica» no lo puede hacer un revisor con IA. El
> proyecto respeta esa negativa a la lectura por IA **también sobre lo que ya
> entra por su feed**: no se reconstruye el barrido con los titulares de la
> ingesta. Y las piezas que hay no sostienen el número: esta misma ficha
> concluía que la evidencia del presente no saca a Cambio de la banda mixta.
> Se preveía una lectura humana de 12 meses con una plantilla
> (`revision-externa/lectura-humana/`, retirada el mismo día: no habrá lectura
> humana). El agregador sigue
> mostrando sus titulares con enlace por su feed: eso no cambia. **Lo que sigue
> es historia y se conserva**: donde dice «valor actual −0,40» o «propuesta», es
> el estado anterior.
>
> **Efecto en el modelo:** al salir del reparto, Cambio deja de contar en la
> tasa de la izquierda (ver «El efecto sobre el modelo», abajo). Sigue contando
> en la cobertura de cada historia.

> **Es el medio de la banda de izquierda con más peso en el corpus:** 1305
> artículos y 310 historias en 37 días (envío del 2026-10-07). **Su valor es el
> que más mueve la tasa de la izquierda**, que es la `q` sobre la que se apoya el
> modelo de puntos ciegos. Si este número está mal, el modelo está mal.

| | |
|---|---|
| **Propuesta** | **NO FIRMAR −0,40 todavía.** La evidencia del presente apunta a la banda mixta, pero falta re-medir el nivel 2 |

**2026-10-12, SIN MEDIR DE FORMA PERMANENTE.** `bias: null` y `reviewedAt:
null`. Este medio no autoriza la lectura por IA en su robots.txt, DobleFoco es
100 % automático y no habrá lectura humana: no tiene lugar en el eje. Si el
medio autoriza la lectura, se medirá (se pedirá permiso por correo tras el
lanzamiento). El feed se mantiene, por decisión del responsable editorial, como
ejercicio de transparencia, y se vigila.

**Historia — mañana del 2026-10-12, SIN MEDIR.** Decisión del responsable editorial: `bias: null` y
`reviewedAt: null` hasta una lectura humana de 12 meses, con una plantilla
(`revision-externa/lectura-humana/`, retirada el mismo día). Motivo: el robots.txt de cambiocolombia.com
excluye a ClaudeBot y el proyecto respeta esa negativa, también sobre su feed; y
la evidencia que hay no sostenía el −0,40. Sus titulares siguen en el agregador.

**Historia — 2026-10-10:** firmada en bloque en −0,40 (ver la tabla de arriba).

**Historia — 2026-10-07, CORREGIDA Y SIN FIRMAR.** El responsable editorial aprobó aplicar las correcciones de
hecho del ciclo 2 (DECISIONES.md, «Ciclo 2, tanda 1»). **El valor sigue en −0,40,
no se firma** y `reviewedAt` sigue en null: espera a que se re-mida el
expediente.

## Evidencia

| | |
|---|---|
| **Nivel 2** | `npm run expediente -- --medio=cambio`, medido el 2026-09-08. **Caducado:** las cifras vigentes son las del envío del ciclo 2 (2026-10-07). Hay que volver a correrlo antes de firmar |

### Nivel 1 — Propiedad, vigente y declarada

> **CORREGIDO EL 2026-10-07 (ciclo 2, tanda 1), sin firmar.** Cada corrección
> lleva la fuente que verificó la resolución de
> `revision-externa/respuestas/opus-5-5-cambio.md`. La ficha daba a Coronell como
> presidente y a Armitage como accionista vigente, y callaba a quien dirige,
> preside y más acciones tiene. Ninguna corrección mueve el valor.
> **cambiocolombia.com no se consultó**: su robots.txt excluye a ClaudeBot. Lo
> que solo consta allí queda como «no verificable por exclusión de robots.txt».

La revista **se relanzó como medio digital en febrero de 2022**, después de que
un grupo de inversionistas comprara los derechos de publicación en 2021.

**Quién la dirige y preside.** Lo dirige y preside **Federico Gómez Lara**,
director general y presidente (Valora Analitik, 08-04-2025; El Tiempo,
09-04-2025). Sigue como director en junio de 2026. La FLIP (18-06-2026): «le
escribió al director de Cambio, Federico Gómez Lara». La Silla Vacía
(17-06-2026): «Federico Gómez, director de Cambio, le respondió que no
iban a rectificar». **Daniel Coronell fue su presidente hasta agosto de 2023**
(La Silla Vacía, 31-08-2023: «Me tengo que apartar de la presidencia de Cambio»)
y sigue como accionista: 22 % en 2024 (La República) y «socio» en 2025
(Las2Orillas).

**Composición publicada más reciente** (La República, 05-07-2024, literal):
«Daniel Coronell (22%), Federico Gómez Lara (22%), Patricia Lara (16%), Maurice
Armitage (16%), Inversiones Zimmerman (12%), Gabriel Silva (8%) y Diego Carvajal
(4%)». Ya en 2022 los dos mayores accionistas eran Gómez Lara y Coronell, al 25 %
cada uno (La Silla Vacía, 04-02-2022), y esta ficha no los nombraba como dueños.

**La salida de Armitage.** En abril de 2025 **Maurice Armitage vendió su
participación** y renunció a la junta directiva; sus acciones las compró Gómez
Lara (Valora Analitik, 08-04-2025; El Tiempo, 09-04-2025: «dejó de ser
accionista de la revista Cambio»). Valora habla en futuro («serán adquiridas»);
que la compra se cerró solo consta en El Tiempo, y no hay primario mercantil.
Armitage se retiró **antes** de su precandidatura presidencial, que abandonó el
12-03-2026 tras completar «los trámites de inscripción ante la Registraduría»
(Infobae). Hoy no hay ningún accionista candidato.

**Resultado: la familia Lara–Gómez (Patricia Lara Salive y su hijo Federico
Gómez Lara) controla ≈54 %.** Es una **suma** de las cifras de 2024 (22 + 16 +
16), no un certificado. Las2Orillas (09-04-2025) da el mismo 54 %, pero con
porcentajes individuales distintos (18 % a cada uno), y dice tomarlos de la
infografía de La República, cuyo texto los contradice. No hay extracto mercantil
público.

**MDIF.** El fondo Media Development Investment Fund firmó con Cambio un acuerdo
de **deuda convertible por 500.000 dólares** (La República, 05-07-2024; MDIF,
15-07-2024: «MDIF has invested in Colombian news outlet Cambio»). El matiz que
cuenta, según La República:
- el acuerdo «aún no se ha ejecutado» en julio de 2024;
- convertir la deuda en acciones es **opción de los socios de Cambio**, que
  pueden «pagar esa deuda y seguir con la composición accionaria como está hoy»;
- el plazo de dos años desde junio de 2024 es «un plazo inicial que puede
  extenderse».

**Su estado actual no está documentado.** No consta que se convirtiera. Gómez
Lara, sobre el fondo: «No se meten en nada editorial, sino solamente
estratégico» (nivel 4, declaración del propio medio).

**Silva.** Gabriel Silva Luján tenía el 8 % en 2024. Fue ministro de Defensa de
Álvaro Uribe (2009-2010) y embajador en EE. UU. con Santos (2010-2012), según
Wikipedia. Eso es historia. La Silla Vacía (2022) lo llama «exministro de Juan
Manuel Santos»: es un error de esa fuente, que esta ficha citaba sin advertirlo.
Del presente, una posición pública: el 07-01-2026 escribió en X que «Petro quiere
meter a Colombia en una guerra con los Estados Unidos para suspender las
elecciones y quedarse en el poder» (Infobae). **Fue un mensaje en X, no una pieza
de Cambio.** Si sigue siendo columnista de Cambio no es verificable por
exclusión de robots.txt. Es política de un accionista minoritario: se declara
como propiedad y no entra en el número.

**Cargos públicos.** Hoy **ningún accionista** ocupa un cargo público ni es
candidato. Armitage, exalcalde de Cali, salió antes de lanzarse. Silva fue
ministro, pero eso es historia.

**Regla de quien dirige.** No consta candidatura ni cargo público vigente de
Federico Gómez Lara. **No salta el aviso, tampoco por la vía estatutaria**:
dirección y presidencia recaen en la misma persona. Los estatutos no son
consultables. Que sea hijo del exfiscal Alfonso Gómez Méndez consta (La Silla
Vacía, 2022), pero la regla excluye expresamente el parentesco con un político.

- [Valora Analitik — Maurice Armitage vendió participación accionaria en revista Cambio](https://www.valoraanalitik.com/maurice-armitage-vendio-participacion-accionaria-en-revista-cambio-ante-posible-aspiracion-politica-para-2026/) · 08-04-2025
- [El Tiempo — Maurice Armitage vendió su participación accionaria en la revista Cambio](https://www.eltiempo.com/politica/partidos-politicos/maurice-armitage-vendio-su-participacion-accionaria-en-la-revista-cambio-por-posible-candidatura-a-la-presidencia-3443133) · 09-04-2025
- [La Silla Vacía — Por segunda vez, Daniel Coronell será el presidente de Noticias Univision](https://www.lasillavacia.com/en-vivo/por-segunda-vez-daniel-coronell-sera-el-presidente-de-noticias-univision/) · 31-08-2023
- [La República — acuerdo entre el Media Development Investment Fund y revista Cambio](https://www.larepublica.co/empresas/acuerdo-entre-el-media-development-investment-fund-y-revista-cambio-3900902) · 05-07-2024
- [MDIF — MDIF invests in Colombian news outlet Cambio](https://www.mdif.org/news/mdif-invests-in-colombian-news-outlet-cambio/) · 15-07-2024
- [Las2Orillas — quiénes quedaron como dueños de la revista Cambio](https://www.las2orillas.co/quienes-quedaron-como-duenos-de-la-revista-cambio-tras-el-retiro-del-empresario-maurice-armitage/) · 09-04-2025
- [Infobae — Maurice Armitage renunció a la carrera presidencial](https://www.infobae.com/colombia/2026/03/12/maurice-armitage-renuncio-a-la-carrera-presidencial-el-empresario-caleno-anuncio-que-no-participara-en-las-elecciones/) · 12-03-2026
- [FLIP — Abelardo de la Espriella y su campaña profundizan su discurso hostil contra la prensa](https://flip.org.co/pronunciamientos/abelardo-de-la-espriella-y-su-campana-profundizan-su-discurso-hostil-contra-la-prensa) · 18-06-2026
- La Silla Vacía — «Abogado de Abelardo hace acusaciones a Cambio sin prueba alguna» · 17-06-2026
- [Infobae — Gabriel Silva Luján: «Petro quiere meter a Colombia en una guerra…»](https://www.infobae.com/colombia/2026/01/07/exministro-de-defensa-gabriel-silva-lujan-aseguro-petro-quiere-meter-a-colombia-en-una-guerra-con-los-estados-unidos/) · 07-01-2026
- [Wikipedia — Gabriel Silva Luján](https://es.wikipedia.org/wiki/Gabriel_Silva_Luj%C3%A1n)
- [LatAm Journalism Review — «Los accionistas no son los dueños de la información», dice Daniel Coronell](https://latamjournalismreview.org/es/articles/los-accionistas-no-son-los-duenos-de-la-informacion-dice-daniel-coronell-presidente-de-la-resucitada-revista-colombiana-cambio/) · 13-10-2021, anterior al relanzamiento: no sirve para cargos vigentes
- [La Silla Vacía — Así resucita la revista Cambio en la era digital](https://www.lasillavacia.com/historias/silla-nacional/asi-resucita-la-revista-cambio-en-la-era-digital/) · 04-02-2022
- [Wikipedia — Cambio (revista)](https://es.wikipedia.org/wiki/Cambio_(revista))

> **ATENCIÓN A LA REGLA DEL PRESENTE, Y AQUÍ MUERDE DE VERDAD.** La *Cambio*
> anterior —la que relanzó García Márquez con sus socios (Abrenuncio, 1998) y la
> que la Casa Editorial El Tiempo compró en 2006 y cerró en 2010 (Wikipedia)—
> **no es este medio**. **No la publicó Semana**, como decía esta ficha, y García
> Márquez figura como socio, no como director. Hay un hilo entre las dos: la
> marca la puso Patricia Lara Salive (La Silla Vacía, 2022). Pero la empresa de
> hoy es de 2021, y cualquier evidencia de su línea anterior a 2021 es historia,
> exactamente como el caso Semana que zanjó la discusión en el protocolo.

### Nivel 2 — Conducta medida en nuestro corpus

> **CIFRAS SUSTITUIDAS EL 2026-10-07.** Las del 2026-09-08 (381 artículos, 116
> historias, 30 días) caducaron, y su ventana contenía entera el terremoto del
> 10-08. Las vigentes son las del envío del ciclo 2. **Falta re-medir** con
> `npm run expediente -- --medio=cambio`, fuera de la ventana del terremoto.

| | |
|---|---|
| Ventana | 37 días, medida el 2026-10-07 |
| Artículos | 1305 |
| Historias en las que entra | 310 |
| Historias compartidas con otro medio | 254 |
| Agenda propia (historias en solitario) | 18 % |
| Compañía media | 0,154 |

**Trabaja la agenda común.** Un 18 % de historias en solitario es menos que el
22 % de Semana en el ciclo 2. Ya con las cifras del 08-09 eran 33 de 116 (28 %):
la frase «no tiene agenda propia medible» que tenía esta ficha estaba mal escrita
desde el origen, y se retira.

> **RETIRADA EL 2026-10-07 la tabla de elevaciones** (con quién coincide más de lo
> esperable). Se leía con el sesgo **declarado** de los socios, que es la misma
> circularidad que el CONTEXTO desautoriza para la compañía media. Además, los
> socios de mayor elevación tenían una base de 8 a 13 historias comunes, dentro
> de la ventana del terremoto.

**En qué se aparta de la agenda común** (medición del 08-09, **no recalculada**;
solo describe formato):

| Tema | Suyo | Corpus | Se aparta |
|---|---:|---:|---:|
| Cultura | 10,6 % | 4,3 % | 2,5× |
| Conflicto y paz | 13,1 % | 7,8 % | 1,7× |
| Derechos y sociedad | 5,4 % | 3,1 % | 1,7× |
| Justicia | 17,9 % | 13,9 % | 1,3× |
| Desastres y accidentes | 4,2 % | 9,7 % | 0,4× |
| Deportes | 2,6 % | 10,9 % | 0,2× |

Perfil de revista de fondo: mucha justicia, conflicto y cultura; poco suceso y
poco deporte. Eso describe **formato**, no posición.

### Nivel 2 — Sus titulares, literales, del 08-09-2026

- «Un niño murió por negligencia, y después expusieron su historia clínica sin permiso: exministro de salud del gobierno Petro, citado a responder»
- «"Un 5 por ciento para la doctora": los nuevos detalles del presunto entramado de corrupción heredado del gobierno anterior que denunció Minsalud»
- «El último ajuste del gobierno Petro al giro directo en salud sale a la luz un mes después de su gobierno»
- «Gobierno De la Espriella levanta suspensión al porte de armas de fuego: ¿qué cambia y cuáles serán las condiciones?»
- «Así cayó el recaudo tributario en Colombia según la OCDE: va en contravía del resto de países»

### Nivel 5 — Hechos de los últimos 12 meses, con fuente de terceros

Ninguno se leyó en el sitio del medio: no es verificable por exclusión de
robots.txt. Constan por terceros que los citan.

- **12-04-2026 — Cepeda.** Cambio publicó «¿Quién es Iván Cepeda?», perfil
  firmado por Felipe López Caballero. Según Infobae (13-04-2026) y El Colombiano
  (*fact check*, 14-04-2026), dice: «Las cuentas de su campaña para la consulta
  de la izquierda resultaron fraudulentas. De los 964 millones de pesos que
  reportó como gastos ante el Consejo Nacional Electoral, 609 provinieron de una
  empresa fantasma y 106 de un individuo que negó haber dado un solo peso».
  Cepeda lo calificó de «falaz». (Infobae fecha la consulta en 2026; fue en
  2025.)
- **16-06-2026 — De la Espriella.** Investigación de redacción: «Campaña de
  Abelardo de la Espriella registró pagos por 1.299 millones a una empresa
  fantasma» (FLIP, 18-06-2026; Infobae, 18-06-2026). El abogado de la campaña
  respondió que «la Revista Cambio se ha perfilado por tener unos periodistas
  activistas ideológicos». La FLIP lo trató como estigmatización. Cambio no
  rectificó (La Silla Vacía, 17-06-2026).
- **07-10-2026 — Fondo Milagro, ya con el gobierno De la Espriella.** El País
  (Cali): «La información fue conocida por la revista Cambio, tras un derecho de
  petición enviado por la representante Catherine Juvinao, donde se dejaba en
  claro como este anuncio quedaba en más palabras del presidente que en hechos».

- [FLIP — pronunciamiento del 18-06-2026](https://flip.org.co/pronunciamientos/abelardo-de-la-espriella-y-su-campana-profundizan-su-discurso-hostil-contra-la-prensa)
- [Infobae — la FLIP alertó por estigmatización de Abelardo de la Espriella](https://www.infobae.com/colombia/2026/06/18/la-flip-alerto-por-estigmatizacion-de-abelardo-de-la-espriella-contra-periodistas-y-medios-tras-investigaciones-sobre-su-campana/) · 18-06-2026
- Infobae, 13-04-2026, y El Colombiano, 14-04-2026, sobre el perfil de Cepeda
- El País (Cali), 07-10-2026, sobre el Fondo Milagro

**Lo que esto dice:** en campaña aplicó el **mismo encuadre de financiación
irregular a los dos candidatos**, a Cepeda dos meses antes que a De la Espriella.
Y fiscaliza al gobierno entrante igual que al saliente.

> **DESMENTIDO EL INDICIO DE ASIMETRÍA ENTRE CANDIDATOS.** El revisor del ciclo 2
> propuso uno: investigación propia sobre la financiación de De la Espriella y
> «ninguna equivalente» sobre Cepeda. La premisa es falsa. La pieza del
> **12-04-2026** sobre Cepeda existe y la citan Infobae y El Colombiano. El indicio
> no se sostiene en la dirección que le dio. Tampoco prueba simetría: ver
> TENSIONES.

## Argumento

### ARGUMENTO — y no sostiene el −0,40

El valor de hoy no tiene detrás ninguna evidencia de nivel 1-3 que lo sitúe a
−0,40. Lo que queda en pie del presente es:

1. **Fiscaliza a los dos gobiernos, sin giro a celebrar.** Los titulares del
   08-09 sobre la corrupción heredada del gobierno Petro; la investigación del
   16-06 sobre la campaña de De la Espriella; el Fondo Milagro del 07-10, ya con
   él en el gobierno. **La regla del polo fijo dice expresamente que eso no es
   evidencia de orientación**: es el oficio.
2. **En campaña aplicó el mismo encuadre a los dos candidatos** (nivel 5): Cepeda
   el 12-04 y De la Espriella el 16-06. No se encontró endoso, con la reserva de
   que el sitio no se pudo leer.
3. **Trabaja la agenda común.** Un 18 % de historias en solitario, por debajo del
   22 % de Semana. No dice nada de orientación; solo que no hay en el nivel 2 un
   perfil de agenda que lo separe del resto.

> **RETIRADO EL 2026-10-07 el antiguo argumento 2** («su co-cobertura de mayor
> elevación es con la mixta y la derecha»). Leía la elevación con el sesgo
> declarado de los socios, que el protocolo no admite, y su ventana contenía el
> terremoto. **El antiguo argumento 3** («no tiene agenda propia medible») se
> reescribe arriba: lo que cae es la redacción, no el fondo.

Nada de esto prueba que sea de derecha —no lo es— ni que sea simétrico. Prueba
que **la evidencia del presente no sostiene una posición fuera de la banda
mixta.** La regla 2 del protocolo dice que, ante la duda entre dos bandas, se
elige la más cercana a la mixta, porque el error de clasificar de más acusa. Pero
lo que sostiene moverlo es esa regla de duda, no una medición, y así hay que
decirlo.

**Propuesta: revisar −0,40 → un valor de la banda mixta**, con el número exacto
a decidir por quien firma, **después de re-medir el nivel 2**. La ficha no
propone cifra para no disfrazar de medición lo que sería juicio.

## El mejor caso en contra

### CONTRA — el mejor caso a favor de mantener −0,40

**Y hay que tomarlo en serio, porque toca los límites de lo que mide el nivel 2.**

1. **La co-cobertura mide qué se cubre, no cómo.** Un medio puede compartir toda
   la agenda y encuadrarla al revés, y el encuadre es justamente lo que este
   proyecto **no** analiza, por decisión escrita.
2. **Coronell y Lara son firmas con trayectoria pública reconocible**, y la
   sección de opinión, que es donde el protocolo manda mirar primero, no es
   verificable por exclusión de robots.txt. Que Silva fuera ministro de Uribe
   **no es argumento** en ningún sentido: es historia.
3. **La regla del polo fijo también protege de sobre-corregir.** Que fiscalice a
   los dos gobiernos y aplique el mismo encuadre a dos candidatos no prueba
   simetría: habría que medir la **dureza** relativa, y dos piezas de distinta
   naturaleza no son una muestra. Bajar el valor a la mixta por ausencia de
   evidencia es defendible; hacerlo afirmando simetría no lo es.
4. **La regla 3 dice que sin evidencia de nivel 1-3 no se mueve el número**, y la
   que hay para salir de −0,40 es sobre todo de nivel 5. Ver TENSIONES.

## Qué cambiaría el número

### REFUTACIÓN — qué observación concreta cambiaría el número

- **Si en la re-medición su co-cobertura de mayor elevación pasa a ser con
  medios de la banda de izquierda**, leída sin el sesgo declarado de los socios,
  el −0,40 recupera apoyo.
- **Si se documenta un endoso editorial** —no fiscalización: endoso— a favor de
  una candidatura o de un lado, el valor se mueve hacia ahí con evidencia de
  primer orden.
- **Si entra o sale un accionista**, es revisión extraordinaria por el punto 7 del
  protocolo. **La conversión de la deuda de MDIF lo sería.**
- **Si al medir la dureza relativa hacia los dos gobiernos o los dos candidatos
  apareciera asimetría sostenida**, eso sí sería orientación y no oficio. Hoy no
  se mide.

## Tensiones declaradas

### TENSIONES — declaradas el 2026-10-07, ciclo 2, tanda 1

Lo que la revisión del ciclo 2 dejó abierto. Ninguna mueve el valor hoy.

1. **Regla 2 frente a regla 3.** La regla 2 lleva a la mixta ante la duda. La
   regla 3 dice que sin evidencia de nivel 1-3 no se mueve el número. La
   evidencia para salir de −0,40 es de nivel 5 (hechos de terceros) más una FLIP
   (nivel 3) que acredita la fiscalización a De la Espriella, no la simetría.
   **Lo decide el responsable editorial.**
2. **No hay medición de dureza relativa.** Las dos piezas sobre financiación son
   de distinta naturaleza (perfil firmado por un autor externo frente a
   investigación de redacción), y dos casos no son una muestra. Ni la simetría ni
   la asimetría están medidas.
3. **El archivo del propio medio es inaccesible** a este proceso, por el
   robots.txt: sección de opinión, Los Danieles, si Silva sigue de columnista,
   posibles editoriales o endosos. «No se encontró endoso» no equivale a ausencia
   comprobada.
4. **La composición accionaria posterior a abril de 2025 es inferida**, y las dos
   fuentes de prensa no cuadran en los porcentajes individuales. El estado de la
   deuda de MDIF y el titular de Inversiones Zimmerman (12 %) no constan.
5. **La posición pública de un accionista minoritario** (Silva, 07-01-2026, en X)
   se declara en la propiedad como desvelamiento, sin efecto en el número.
6. **El peso de Cambio en la tasa de la izquierda** (abajo): mover este valor
   cambia la `q` del modelo de puntos ciegos.
7. **Pregunta abierta para el responsable editorial, no corrección:** si `ownerType: 'independiente'`
   sigue siendo el tipo correcto para un medio controlado en ≈54 % por una
   familia, con un fondo extranjero como acreedor convertible.

**Qué falta para firmar:** re-medir el nivel 2 fuera de la ventana del
terremoto, y que el responsable editorial resuelva la tensión 1.

### EL EFECTO SOBRE EL MODELO, QUE ES POR LO QUE ESTA FICHA IMPORTA

Con la medición del 08-09, Cambio aportaba 381 de las ~644 piezas de toda la
banda de izquierda en el corpus; con las cifras del envío su peso es mayor.
**Si su valor se mueve a la mixta, la tasa base de la izquierda —el 3,29 % sobre
el que se calcula cada punto ciego— baja de golpe**, y con ella cambia qué
historias se marcan y cuáles no.

No es un motivo para dejar el número donde está: es un motivo para no decidirlo
deprisa, y para que la Etapa 3.2 vuelva a medirse el día que se firme.

## Historial

### Cabecera anterior (filas superadas)

| | |
|---|---|
| **Valor vigente (histórico, mañana del 2026-10-12)** | sin medir hasta una lectura humana (plantilla en `revision-externa/lectura-humana/`, **retirada el mismo 2026-10-12**) |
| **Valor anterior** | **−0,40**, firmado en bloque el 2026-10-10 |
| **Valor actual (histórico, antes del 2026-10-12)** | **−0,40** · `reviewedAt: null` |
| **Corrección** | El conteo de artículos de este expediente salió inflado un 9,3 %: `expedienteDeMedio.mjs` contaba una fila por historia. Corregido el 2026-09-09; al firmar hay que volver a correrlo |
| **Correcciones de hecho** | **2026-10-07, ciclo 2, tanda 1, aprobadas por el responsable editorial. NO es una firma:** el valor sigue en −0,40 y `reviewedAt` no cambia. Corregidos quién dirige y preside, Coronell, Armitage, la composición accionaria, MDIF, la Cambio anterior y Silva; sustituidas las cifras del nivel 2; retirados el argumento 2 y la redacción del 3. Espera a la re-medición |

### REVISIÓN EXTERNA

Va al circuito con la instrucción de **argumentar EN CONTRA de bajar el valor**,
que es la dirección que propone esta ficha. Si los modelos coinciden conmigo, la
ficha no gana nada.

| Modelo | Versión | Fecha | Objeción | Resolución |
|---|---|---|---|---|
| Claude Opus 5.5 | claude-opus-5-5 | 2026-10-07 | Ciclo 2, tanda 1: ocho objeciones. Coronell, Armitage, la omisión de Gómez Lara y del ≈54 %, MDIF, la Cambio anterior, la conducta medida, una asimetría entre candidatos y Silva | **Aceptadas las de hecho; rechazados el dato de Gómez Méndez como aviso, la «refutación» del argumento 3 y el indicio de asimetría** (premisa falsa: pieza del 12-04-2026 sobre Cepeda). Correcciones de hecho aplicadas el 2026-10-07, sin firmar. Detalle en `revision-externa/respuestas/opus-5-5-cambio.md`. Quien resolvió es de la misma casa que el revisor y el autor: la coincidencia no es aval |
