# Barrido de la voz de la casa — Chocó 7 Días

| | |
|---|---|
| **Medio** | Chocó 7 Días (`choco7dias.com`), Quibdó |
| **Regla** | «Evidencia editorial histórica», `PROTOCOLO_JUICIO_EDITORIAL.md` (2026-10-09) |
| **Ventana** | 2025-10-09 → 2026-10-09 (12 meses; regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Gustavo Petro → Abelardo de la Espriella |
| **Hecho por** | Claude Code (Claude Opus 5.5), 2026-10-09, a petición del responsable editorial |
| **Ficha** | `fichas/choco-7-dias.md` |
| **Resolución de origen** | `revision-externa/respuestas/opus-5-5-choco-7-dias.md` |

**Para qué sirve.** Para que cualquiera pueda recontar las piezas y llegar, o
no, al mismo número. Cada fila lleva su URL, su fecha, de quién es la voz, de
qué gobierno habla y cómo se clasificó.

---

## Método

**Fuente.** La API REST pública de WordPress del propio medio
(`https://choco7dias.com/wp-json/wp/v2/`), consultada el 2026-10-09 con
`curl -sL --ssl-no-revoke`, un User-Agent de navegador y 21 s entre peticiones.
El `robots.txt` del sitio dice «User-agent: * / Crawl-Delay: 20», sin
exclusiones. Las fechas son el campo `date` de la API, que el sitio da en hora
de Colombia.

**Universo.** Todas las entradas de la ventana que contienen alguno de estos
términos, en título o texto, salvo los edictos (categoría «EDICTOS»):

| Término | Entradas | Nota |
|---|---|---|
| `Petro` | 28 | |
| `Espriella` | 11 | |
| `gobierno nacional` | 100 + página 2 | la API da 100 por página; se pidió la segunda |
| `presidente` | 62 | |
| `Ministerio` | 100 + página 2 | ídem |

**La búsqueda de la API sí filtra.** Con un término sin sentido (`zzqxwv`)
devuelve `[]`. El revisor del ciclo 2 creyó lo contrario, y por eso no encontró
la muerte del propietario ni los textos que nombran a quien coordina el medio.

Se añadieron **las 56 entradas de «Columnistas» y «Opinión»** de la ventana. En
total son 263 entradas distintas, todas leídas en texto completo. De ellas, 47
mencionan al gobierno nacional al menos dos veces, y esas se leyeron una a una
para clasificarlas.

**Qué cuenta como voz de la casa** (condición 1 de la regla):

- las piezas sin firma publicadas con la cuenta del medio, sin «Tomado de»,
  «Fuente:» ni categoría «Remitidos»;
- las firmadas por **Jorge Salgado**, que según el propio medio dirige (2021) y
  coordina (2023) el medio.

**Qué NO cuenta, y se declara aparte:**

- las columnas de terceros;
- las reimpresiones («Tomado de Consonante», «Fuente: Mongabay», «Tomado de
  Unicef», El Guarengue, La Sal en la Herida);
- los comunicados reescritos o en «Remitidos»;
- las piezas cuya valoración es de una fuente nombrada (personero, Defensoría,
  Comité Cívico, una periodista de Semana).

**Clasificación:**

- **fiscaliza**: la casa critica con voz propia una decisión o un resultado del
  gobierno nacional;
- **favorable**: la casa celebra o disculpa a ese gobierno;
- **neutra**: lo cuenta en plano;
- **posición**: la casa toma partido en el eje, sin hablar de un gobierno.

---

## 1. Piezas que cuentan: voz de la casa con postura

| # | Fecha | Pieza | Voz | Gobierno | Clasificación | Cita |
|---|---|---|---|---|---|---|
| 1 | 2025-10-17 | [El Chocó sufrió una reducción de recursos de inversión del 10,52% en el presupuesto 2026…](https://choco7dias.com/el-choco-sufrio-una-reduccion-de-recursos-de-inversion-del-1052-en-el-presupuesto-2026-en-relacion-al-presupuesto-2025/) | casa | Petro (presupuesto 2026) | fiscaliza | «Otro garrotazo al Chocó»; «Una suma pírrica» |
| 2 | 2025-11-08 | [Chocó 2025: departamento con mayor confinamiento y cuarto en desplazamiento](https://choco7dias.com/choco-2025-departamento-con-mayor-confinamiento-y-cuarto-en-desplazamiento/) | casa (entradilla propia sobre un informe de la Defensoría) | Petro | fiscaliza | «el fracaso total de la política de "paz total" del gobierno Petro» |
| 3 | 2025-12-05 | [Gobierno nacional continúa absurda persecución a los pequeños mineros del Chocó](https://choco7dias.com/gobierno-nacional-continua-absurda-persecucion-a-los-pequenos-mineros-del-choco/) | casa | Petro | fiscaliza | «El gobierno Petro ha ejecutado una irracional política antiminera, similar a la de los gobiernos anteriores» |
| 4 | 2025-12-10 | [Hace dos años el gobierno nacional anunció el mejoramiento del aeropuerto de Bahía Solano…](https://choco7dias.com/hace-dos-anos-el-gobierno-nacional-anuncio-el-mejoramiento-del-aeropuerto-de-bahia-solano-pero-solo-se-ha-ejecutado-un-dos-por-ciento-del-proyecto/) | casa (sobre una denuncia del personero) | Petro | fiscaliza | «¡Dos años después del anuncio con bombos y platillos […] sólo se ha ejecutado un insignificante dos por ciento!» |
| 5 | 2026-01-12 | [Aumenta absurda persecución del gobierno nacional a los pequeños mineros del Chocó](https://choco7dias.com/aumenta-absurda-persecucion-del-gobierno-nacional-a-los-pequenos-mineros-del-choco/) | casa | Petro | fiscaliza | «El gobierno Petro ha ejecutado una irracional política en el tema minero» |
| 6 | 2026-04-12 | [Charlatanería interoceánica](https://choco7dias.com/charlataneria-interoceanica/) | Jorge Salgado | Petro | fiscaliza | «Petro se lavó las manos como Poncio Pilatos»; «¿Charlatán que vende humo…?» |
| 7 | 2026-04-14 | [Exorbitantes aumentos de avalúos catastrales en zonas rurales de nueve municipios del Chocó](https://choco7dias.com/exorbitantes-aumentos-de-avaluos-catastrales-en-zonas-rurales-de-nueve-municipios-del-choco/) | casa | Petro (PND 2022-2026, IGAC) | fiscaliza | «la metodología que privilegia los precios de la especulación inmobiliaria» |
| 8 | 2026-05-22 | [El hambre y el hambre extrema crecieron de manera dramática en el Chocó en el año 2025](https://choco7dias.com/el-hambre-y-el-hambre-extrema-crecieron-de-manera-dramatica-en-el-choco-en-el-ano-2025/) | casa | Petro | fiscaliza | «se debe a la reducción de recursos e inversiones del gobierno Petro en el Chocó» |
| 9 | 2026-06-17 | [Continúa absurda persecución del gobierno nacional a los pequeños mineros del Chocó](https://choco7dias.com/continua-absurda-persecucion-del-gobierno-nacional-a-los-pequenos-mineros-del-choco/) | casa | Petro | fiscaliza | «irracional política antiminera, similar a la de los gobiernos anteriores» |
| 10 | 2026-06-20 | [Rumbo al fracaso otro contrato del gobierno Petro en el Chocó…](https://choco7dias.com/rumbo-al-fracaso-otro-contrato-del-gobierno-petro-en-el-choco-pavimentacion-y-ampliacion-de-pista-de-aterrizaje-del-aeropuerto-de-bahia-solano/) | casa | Petro | fiscaliza | «con bombos y platillos, el Presidente Petro […] colocó la "primera piedra"» |
| 11 | 2026-07-29 | [Ovidio Garrido Córdoba, séptimo interventor del hospital San Francisco de Asís en el gobierno Petro](https://choco7dias.com/ovidio-garrido-cordoba-septimo-interventor-del-hospital-san-francisco-de-asis-en-el-gobierno-petro/) | casa | Petro | fiscaliza | «En el errático gobierno Petro»; «ha sido un fracaso total» |
| — | — | **07-08-2026: cambio de gobierno** | | | | |
| 12 | 2026-08-09 | [Con Petro, otros cuatro años de retroceso del Chocó](https://choco7dias.com/con-petro-otros-cuatro-anos-de-retroceso-del-choco/) | Jorge Salgado | Petro (balance del saliente) | fiscaliza | «Similar al balance de los anteriores gobiernos, con Petro el Chocó sufrió otros cuatro años de retroceso general» |
| 13 | 2026-09-19 | [Otro golpe al Chocó: nuevo recorte de recursos de inversión en el Presupuesto Nacional 2027](https://choco7dias.com/otro-golpe-al-choco-nuevo-recorte-de-recursos-de-inversion-en-el-presupuesto-nacional-2027/) | casa | De la Espriella (proyecto de presupuesto 2027) | fiscaliza | «Otro golpe al Chocó»; «baja a 1,45 billones en el proyecto 2027 del gobierno De La Espriella» |
| 14 | 2026-10-04 | [En El Dos, Unión Panamericana, siguen esperando la reconstrucción del colegio tras el terremoto](https://choco7dias.com/en-el-dos-union-panamericana-siguen-esperando-la-reconstruccion-del-colegio-tras-el-terremoto/) | casa | De la Espriella | fiscaliza | «un doloroso ejercicio de retórica política»; «resulta un insulto para un pueblo incomunicado» |
| 15 | 2026-10-05 | [A casi dos meses del terremoto, no hay cifra oficial de cuántos damnificados del Chocó han recibido ayudas](https://choco7dias.com/a-casi-dos-meses-del-terremoto-no-hay-cifra-oficial-de-cuantos-damnificados-del-choco-han-recibido-ayudas/) | casa | De la Espriella (Gobierno nacional, UNGRD) | fiscaliza | «la pregunta central sigue sin respuesta oficial» |
| 16 | 2026-07-20 | [A propósito del 20 de julio](https://choco7dias.com/a-proposito-del-20-de-julio-2/) | Jorge Salgado | ninguno | **posición** (izquierda nacionalista) | «Colombia se ha trastocado en una vergonzosa y miserable neocolonia del imperio norteamericano»; contra el TLC |

**Nota sobre la pieza 16.** Su identificador en WordPress (45286) es de 2024 y
su URL lleva el sufijo `-2`, así que puede ser una reedición de un texto
anterior. No se comprobó. Cuenta igual, porque el medio la publicó en la
ventana.

### El recuento, contra las condiciones de la regla

| Condición | Mínimo | Chocó 7 Días | ¿Cumple? |
|---|---|---|---|
| 1. Voz de la casa | — | 15 piezas sin firma o firmadas por quien coordina el medio, más 1 de posición | sí |
| 2. A los dos lados del 07-08-2026, dentro de 12 meses | — | 11 antes y 4 después: 3 sobre el gobierno entrante y 1 balance del saliente | sí |
| 3. Piezas con postura | ≥ 10 | 16 | sí |
| 3. A cada lado del cambio | ≥ 3 | 11 / 4 | sí, **al mínimo** del lado posterior (3 sobre De la Espriella) |
| 3. Dirección | ≥ 3 a 1 | no hay dirección: la misma conducta con los dos gobiernos | sostiene el **0,00**, no lo mueve |
| 4. Contrapesos escritos | — | sección 3 de este archivo y la ficha | sí |
| 5. Reproducible | — | este archivo | sí |

**La lectura.** La conducta es la misma con el gobierno de izquierda saliente y
con el de derecha entrante:

- la casa fiscaliza al que manda con adjetivos propios y no celebra a ninguno;
- el ritmo es parecido, con 11 piezas en unos diez meses de Petro (≈ 1,1 al
  mes) y 3 en dos meses de De la Espriella (≈ 1,5 al mes);
- la comparación más limpia es la misma pieza con los dos gobiernos: el recorte
  del presupuesto de inversión del Chocó. Con Petro, el 17-10-2025, fue «Otro
  garrotazo al Chocó» (pieza 1). Con De la Espriella, el 19-09-2026, fue «Otro
  golpe al Chocó» (pieza 13).

Contado por el eje sería otra cosa: 12 piezas contra un gobierno de izquierda y
3 contra uno de derecha. Pero eso es lo que la regla del polo fijo prohíbe leer,
porque fiscalizar a quien manda no es orientación. El desequilibrio sale de la
exposición (diez meses frente a dos), no de un trato distinto.

**Qué sostiene y qué no.** El barrido **cumple las cinco condiciones para
sostener el 0,00 como evidencia**, y no como valor por defecto. Del lado
posterior al cambio lo cumple justo en el mínimo: tres piezas sobre el gobierno
entrante en dos meses. Si en los próximos meses la casa dejara de fiscalizar a
De la Espriella, o lo celebrara, el 0,00 dejaría de estar sostenido.

---

## 2. Piezas sobre el gobierno nacional que NO cuentan, y por qué

**Comunicados en plano, favorables al gobierno saliente (no cuentan: comunicado
reescrito o remitido):**

| Fecha | Pieza | Por qué no cuenta |
|---|---|---|
| 2025-12-11 | [Con histórica inversión: Planeación Nacional impulsa transformación de municipios PDET en Chocó](https://choco7dias.com/con-historica-inversion-planeacion-nacional-impulsa-transformacion-de-municipios-pdet-en-choco/) | Comunicado del DNP reescrito, sin rótulo: «el Gobierno nacional demuestra una vez más…» |
| 2026-01-09 | [Gobierno del Cambio ha invertido más de $511 mil millones para fortalecer la educación en el Chocó](https://choco7dias.com/gobierno-del-cambio-ha-invertido-mas-de-511-mil-millones-para-fortalecer-la-educacion-en-el-choco/) | Comunicado del Ministerio de Educación, sin rótulo; cierra con «Mejor Estudiar con recursos bien invertidos» |
| 2026-07-24 | [Empalme ante el pueblo: Los legados del presidente Gustavo Petro para la educación pública](https://choco7dias.com/empalme-ante-el-pueblo-los-legados-del-presidente-gustavo-petro-para-la-educacion-publica/) | Categoría «Remitidos» |

**Anuncios del gobierno entrante, en plano (no cuentan: neutras):**

| Fecha | Pieza | Clasificación |
|---|---|---|
| 2026-06-30 | [Quince chocoanos forman parte del equipo de empalme del nuevo gobierno nacional](https://choco7dias.com/quince-chocoanos-forman-parte-del-equipo-de-empalme-del-nuevo-gobierno-nacional/) | neutra |
| 2026-09-04 | [Gobierno deroga Distrito Minero Especial del San Juan en Chocó](https://choco7dias.com/gobierno-deroga-distrito-minero-especial-del-san-juan-en-choco/) | neutra: da la versión del ministerio |
| 2026-09-07 | [José Leonidas Tobón Torreglosa, gerente especial para la reconstrucción del Chocó](https://choco7dias.com/jose-leonidas-tobon-torreglosa-gerente-especial-para-la-reconstruccion-del-choco/) | neutra: el «Plan Marshall» sin adjetivos |
| 2026-09-08 | [David Vélez, de Nubank, anuncia compromisos en bancarización…](https://choco7dias.com/david-velez-de-nubank-anuncia-compromisos-en-bancarizacion-e-inversion-en-educacion-en-el-choco/) | neutra |

**Valoración atribuida a una fuente nombrada (no cuentan: no es la voz de la
casa):**

| Fecha | Pieza | De quién es la valoración |
|---|---|---|
| 2025-10-22 | [Bahía Solano: denuncian otro incumplimiento del gobierno nacional a comunidades indígenas](https://choco7dias.com/bahia-solano-denuncian-otro-incumplimiento-del-gobierno-nacional-a-comunidades-indigenas/) | el personero |
| 2026-01-11 | [Recorte al Chocó de $43.486 millones por mala planeación del gobierno nacional](https://choco7dias.com/recorte-al-choco-de-43-486-millones-por-mala-planeacion-del-gobierno-nacional/) | Edward Torres Ruidiaz, firmada |
| 2026-01-16 | [Comité Cívico del Chocó convoca paro cívico para el 12 de febrero](https://choco7dias.com/comite-civico-del-choco-convoca-paro-civico-para-el-12-de-febrero/) | el Comité Cívico |
| 2026-07-15 | [Consejo Comunitario del Chocó protesta por incumplimientos del gobierno de Petro](https://choco7dias.com/consejo-comunitario-del-choco-protesta-por-incumplimientos-del-gobierno-de-petro/) | Cocomopoca |
| 2026-08-14 | [Inconformidad de líderes comunitarios, alcaldes y habitantes del Chocó por la falta o retraso de ayudas tras el terremoto](https://choco7dias.com/inconformidad-de-lideres-comunitarios-alcaldes-y-habitantes-del-choco-por-la-falta-o-retraso-de-ayudas-tras-el-terremoto/) | alcaldes y líderes citados |
| 2026-08-20 | [Gobierno nacional suspendió la programación de las Emisoras de Paz de Bojayá y Riosucio](https://choco7dias.com/gobierno-nacional-suspendio-la-programacion-de-las-emisoras-de-paz-de-bojaya-y-riosucio/) | «ha sido considerada como violatoria…»: atribuida |
| 2026-09-28 | [«De La Espriella, pare bolas»…](https://choco7dias.com/de-la-espriella-pare-bolas-periodista-cuestiona-el-malecon-espejo-en-quibdo-y-pide-priorizar-necesidades-basicas/) | Salud Hernández-Mora (Semana) |
| 2026-10-08 | [Docente de la UTCH radica derecho de petición al Presidente de la República…](https://choco7dias.com/docente-de-la-utch-radica-derecho-de-peticion-al-presidente-de-la-republica-y-a-la-ministra-de-educacion/) | el docente |

**Reimpresiones de otros medios sobre el terremoto:** Consonante (14-08 y
12-09-2026), Unicef (18-08-2026), Defensoría (29-08-2026) y Mongabay
(29-09-2026). No cuentan.

---

## 3. Columnas de la ventana (no mueven el número)

**56 entradas en «Columnistas»**, todas de la ventana. «Opinión» no tiene
ninguna desde agosto de 2025, y el medio **no tiene categoría de editoriales**.

| | Antes del 07-08-2026 | Desde el 07-08-2026 | Total |
|---|---|---|---|
| Reimpresas de El Guarengue (Julio César Uribe Hermocillo, «Tomado de El Guarengue») | 28 | 5 | **33** |
| Firmadas por Jorge Salgado (quien coordina el medio) | 2 | 0 | 2 |
| Firmadas por otros columnistas | 18 | 2 | 20 |
| Otras reimpresiones (La Sal en la Herida) | 1 | 0 | 1 |
| **Total** | 49 | 7 | 56 |

Las dos de Salgado (12-04 y 20-07-2026) están en la tabla 1: son la voz de
quien coordina el medio, no de un tercero.

**El Guarengue, tensión de nivel 5 que no cuenta.** Es una reimpresión semanal
de un blog de terceros. Casi todo es crónica e historia de Quibdó. Las columnas
con posición política nacional son pocas, y casi todas caen en el mes
electoral:

- [«Dos textos electorales…»](https://choco7dias.com/dos-textos-electorales/),
  01-06-2026: la fábula de «Tío Tigre», la mañana después de la primera vuelta.
  Leerla como alusión al ganador es interpretación, apoyada en la del 22-06.
- [«Elecciones, intuiciones, decisiones…»](https://choco7dias.com/elecciones-intuiciones-decisiones/),
  08-06-2026: alegoría de la victoria liberal de 1930.
- [«Tocando fondo»](https://choco7dias.com/tocando-fondo/), 15-06-2026: «más de
  siete mil asesinatos de civiles», «no estarían recogiendo café».
- [«Ante la tragedia nacional, dignidad regional»](https://choco7dias.com/ante-la-tragedia-nacional-dignidad-regional/),
  22-06-2026: «las mismas tristes razones que la votación en el Plebiscito», la
  «cacareada tigritud» del ganador, y una región «donde masivamente nadie votó
  por él».
- [«Free Angela Davis»](https://choco7dias.com/free-angela-davis/),
  02-03-2026: memoria personal con epígrafe feminista.

Después del 07-08-2026, ninguna de las cinco de El Guarengue trata del gobierno
nuevo: tres son sobre el terremoto, una es un obituario y otra recuerda a
Yolanda Cerón.

**Otros columnistas con posición:** «Soberanía en juego: Estados Unidos y
Venezuela» (Eduardo Xavier Moreno Mosquera, 09-01-2026), contra la «injerencia»
de Washington. No hay columnistas de derecha. Las columnas firmadas se declaran
y no cuentan (condición 1).

---

## 4. Fuera de la ventana: la serie de quien coordina el medio (historia, no cuenta)

Por la regla del presente, nada de esto cuenta hoy. Se deja escrito porque
muestra la misma conducta con un tercer gobierno y un segundo cambio de signo
(Duque → Petro en 2022). Todas son piezas firmadas «Por Jorge Salgado»:

- 16-01-2021, [«Lo que el Presidente Duque ocultó o distorsionó en el Chocó»](https://choco7dias.com/lo-que-el-presidente-duque-oculto-o-distorsiono-en-el-choco/);
- 08-09-2021, [«Récord de mentiras del gobierno Duque sobre acuerdos con el Chocó»](https://choco7dias.com/record-de-mentiras-del-gobierno-duque-sobre-acuerdos-con-el-choco/);
- 14-10-2021, [«En el presupuesto nacional 2022 se reducen recursos al Chocó»](https://choco7dias.com/en-el-presupuesto-nacional-2022-se-reducen-recursos-al-choco/):
  la misma pieza del recorte, ahora con Duque;
- 26-10-2021, [«Gobierno nacional sigue negándose a dialogar con los mineros del Chocó»](https://choco7dias.com/gobierno-nacional-sigue-negandose-a-dialogar-con-los-mineros-del-choco/)
  («el gobierno de Iván Duque sigue negándose»);
- 06-08-2023, [«Chocó: un año del gobierno Petro, otro año de retroceso»](https://choco7dias.com/choco-un-ano-del-gobierno-petro-otro-ano-de-retroceso/);
- 02-02-2024, [«La comedia de Petro con el acueducto de Quibdó»](https://choco7dias.com/la-comedia-de-petro-con-el-acueducto-de-quibdo/);
- 17-09-2025, [«La intervención de EPQ, otra intervención fracasada del gobierno nacional»](https://choco7dias.com/la-intervencion-de-epq-otra-intervencion-fracasada-del-gobierno-nacional/).

---

## Para recontar

```
curl -sL --ssl-no-revoke -A "<UA de navegador>" \
  "https://choco7dias.com/wp-json/wp/v2/posts?search=Petro&after=2025-10-09T00:00:00&per_page=100&_fields=id,date,link,title,author,categories"
```

Lo mismo con `Espriella`, `gobierno%20nacional`, `presidente` y `Ministerio`
(con `&page=2` donde salgan 100). Para las columnas, `categories=41,36`. El
texto completo se pide con `include=<ids>&_fields=id,date,link,title,content`.
Respétese el `Crawl-Delay: 20`.
