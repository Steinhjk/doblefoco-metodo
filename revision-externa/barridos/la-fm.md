# Barrido editorial: La FM

| | |
|---|---|
| **Medio** | La FM, RCN Radio, Organización Ardila Lülle (`la-fm`). Emisora. Voz propia: la sección «Carta del director» (`/carta-del-director`) |
| **Valor vigente** | **+0,35**, firmado en bloque el 2026-10-10 (`reviewedAt: '2026-10-10'`). Razón del registro: «Radio informativa del grupo RCN; línea editorial crítica con gobiernos progresistas». Sus fuentes tratan de la propiedad y del nombramiento del director; ninguna es una pieza del medio. La ficha (`fichas/la-fm.md`) añade cinco piezas de nivel 5 encontradas por un revisor |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus precisiones, entre ellas la del 2026-10-10 (los cuatro casos de un barrido cuando el valor solo se apoya en los niveles 4 y 5) |
| **Ventana** | 2025-10-11 → 2026-10-11 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-11. Es de la misma casa que el autor de la ficha, así que su acuerdo con ella no es aval |
| **Estado** | **FIRMADO el 2026-10-12: +0,25** (antes +0,35), el valor que proponía este barrido. Aplicado en el registro, la ficha y el texto público (`DECISIONES.md`, 2026-10-12). Lo que más abajo dice «propuesta» o «pendiente de firma» es el estado anterior a la firma y se conserva como historia |
| **Resultado** | En la lectura principal **cumple los mínimos**: 12 piezas con postura que cuentan (11 D, 1 C) y 5 mixtas; **8 D antes y 3 D después** del cambio; proporción 11:1. Pero el lado de después **solo llega a 3 contando dos piezas «leves»**: sin las leves de los dos lados quedan 3 D antes y 1 después, y el barrido no llega. **Propuesta: +0,25** (banda moderada, por debajo del tope de ±0,30). Lectura estricta, que se declara: «sin medir» con la dirección derecha como tensión |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas y el método
> están aquí para eso. **La clasificación de cada pieza es el juicio de un solo
> lector**, de la misma casa que el autor de la ficha.

---

## 1. Método

- **robots.txt** de `www.lafm.com.co`, descargado el 2026-10-11 con el User-Agent de abajo: `User-agent: *`, `Allow: /`, `Disallow: /buscar`. Declara cuatro sitemaps (`/sitemapindex`, `/sitemapnews`, `/sitemapindex-videos`, `/sitemapindex-tags`). **No excluye nada de lo que se descargó**: sitemaps, la sección `/carta-del-director`, sus piezas y los feeds `/rss/…`. No se tocó `/buscar`.
- **User-Agent honesto en todas las peticiones**: `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. No se usó en ningún momento el User-Agent de un navegador. Ninguna petición devolvió 403 ni 429: el sitio respondió 200 a las 206 peticiones.
- **Ritmo**: una petición cada 1,5 s, en serie. `curl -s --ssl-no-revoke`.
- **No se tocaron** eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex. No se usó ningún buscador ni Internet Archive: todas las URL salen del propio medio.
- **Cómo se armó la lista.**
  1. `/sitemapindex` enlaza un sitemap de artículos por mes (`/sitemaps/articles_<Mes>_<Año>.xml.gz`). Se bajaron los 13 que cubren la ventana, de octubre de 2025 a octubre de 2026. Juntos traen 31.219 URL (31.207 únicas), repartidas por sección: sociedad 5.950, actualidad 5.258, orden público 4.902, política 4.828, economía 3.122, internacional 3.093, deportes 2.201, entretenimiento 1.441, emisiones 239 y **carta-del-director 185**.
  2. La portada viva de `/carta-del-director` (16 enlaces) añadió **una pieza que no estaba en ningún sitemap** (29-09-2026). `?page=2` devuelve la misma portada: la sección no pagina en el servidor.
  3. El feed de la sección (`/rss/carta-del-director.xml`, 20 ítems) no añadió ninguna. De paso se comprobó lo que dice el registro: **`/rss/rss.xml` y `/rss/politica.xml` existen** (200, `application/xml`, 20 ítems cada uno).
  - Resultado: **186 URL** de la sección, todas descargadas del sitio vivo el 2026-10-11 y leídas enteras. El texto es el cuerpo de `<article>`; la fecha, el `datePublished` del JSON-LD, en UTC (las ediciones que salen de madrugada en UTC son de la noche anterior en Colombia).
- **Qué es la sección.** Desde el 24-10-2025 la «Carta del director» es casi entera **«Las seis de las 6 con Juan Lozano»**: el resumen escrito de los seis temas con los que el director abre la emisión de la mañana. Solo una pieza de la ventana es un editorial clásico en primera persona («Ojo con el populismo incendiario», 24-10-2025), más una lista de «Los 6 retos de Colombia en el 2026» (02-01-2026). Las piezas llevan la firma del director (181) o de «La Fm» (5).
- **Voz de la casa (condición 1).** Cuentan: es el espacio que el medio rotula como carta de su director, y el protocolo admite al «que lo dirige en un espacio que lo compromete». **Con dos avisos que pesan en la magnitud:**
  - el texto es, casi siempre, **un resumen de lo que el director dijo al aire**, redactado por la web y a menudo en tercera persona («Lozano señaló…», «el analista destacó…»). La edición del 12-06-2026 lo declara: «Este contenido fue escrito y producido por una inteligencia artificial bajo revisión y curaduría de un periodista de La FM». La postura que se clasifica es la que el texto atribuye al director, no su frase literal al aire;
  - buena parte de cada edición es un titular sin comentario. Esas líneas no tienen postura y no se clasifican.
- **Lo que no se barrió.**
  - **El audio** de las emisiones (`/emisiones/`, 239 URL de páginas de directo). No hay texto que leer.
  - **Las noticias firmadas por la redacción** (unas 31.000 URL). Sus titulares y entradillas también son voz propia según el protocolo, pero no se pueden barrer sistemáticamente con este método. La ficha cita tres «encuadres informativos» de esa parte (15-03-2026, 08-08-2025, 26-05-2025); no se vuelven a contar aquí.
- **Clases** (las de El Pilón y Razón Pública, adaptadas):
  - **D**, dirección derecha (cuenta): rótulo descalificador contra el Gobierno Petro, la izquierda o sus candidatos; respaldo, elogio o disculpa a De la Espriella, a su programa o a su Gobierno; encuadre asimétrico entre candidatos en la misma dirección.
  - **C**, contrapeso (cuenta): reconocimiento o elogio al Gobierno Petro o a la izquierda; crítica o reparo al Gobierno De la Espriella.
  - **M**, mixta: postura repartida en la misma pieza. No suma.
  - **F**, solo fiscaliza al gobierno en ejercicio. **No suma** (polo fijo y precisión del 2026-10-09). Se declara en §2.3 y se usa en la lectura del polo fijo (§3).
  - **«leve»**: la postura es una frase o un matiz dentro de una edición de otro tema. Cuenta igual en el recuento principal; el §3 da el recuento sin ellas.
- **Descargas y scripts** en la carpeta temporal de la sesión, fuera del repositorio; los scripts en una carpeta distinta de las descargas. No se ha guardado ni se publica el texto completo de ninguna pieza: solo fragmentos breves como evidencia.

### 1.1 Cobertura y huecos

| | Días hábiles (lun-vie) | Con pieza |
|---|---|---|
| 2025-10 (desde el 13) | 15 | 6 |
| 2025-11 | 20 | 15 |
| 2025-12 | 23 | 17 |
| 2026-01 | 22 | 17 |
| 2026-02 | 20 | 20 |
| 2026-03 | 22 | 17 |
| 2026-04 | 22 | 16 |
| 2026-05 | 21 | 17 |
| 2026-06 | 22 | 12 |
| 2026-07 | 23 | 14 |
| 2026-08 | 21 | 12 |
| 2026-09 | 22 | 8 |
| 2026-10 (hasta el 9) | 7 | 4 |
| **Total** | **260** | **175** |

- **186 URL, 185 textos distintos.** La edición del 06-10-2026 (`…-413102`) sirve el mismo cuerpo que la del 29-09-2026 (`…-412351`), palabra por palabra. Se cuenta una sola vez, con la fecha del 29-09.
- **Tres ediciones sin texto** (solo título): 04-12-2025 (`…-384441`), 19-02-2026 (`…-390977`) y 16-03-2026 (`…-393483`).
- **Antes del cambio: 166 URL. Después: 20 URL, 19 textos.**
- **Huecos principales**, que el sitio no ofrece por ninguna de las tres vías:
  - **13 al 23-10-2025**: la sección arranca en la ventana el 24-10;
  - **22-06 al 07-07-2026**: de la segunda vuelta (21-06) al empalme; solo está el 23-06;
  - **07 al 19-08-2026**: **las dos primeras semanas del Gobierno De la Espriella**, con el terremoto del 10-08;
  - **01 al 18-09-2026**, salvo el 03-09;
  - **07 al 09-10-2026**.
- **El lado de después es corto y tiene agujeros justo al principio**: dos meses, 19 textos, y ninguno de la primera quincena de gobierno. Cualquier lectura de esa mitad es frágil.

---

## 2. Piezas clasificadas

Todas las URL son `https://www.lafm.com.co/carta-del-director/` + la ruta. El título es el `<title>` literal de la página (las barras verticales del título se escapan).

### 2.1 Antes del cambio: 2025-10-11 → 2026-08-06 (gobierna Petro)

| # | Fecha | Título literal | Ruta | Clase | Por qué (fragmento) |
|---|---|---|---|---|---|
| 1 | 2025-10-24 | Ojo con el populismo incendiario | `ojo-con-el-populismo-incendiario-380641` | **D** | Editorial en primera persona tras la absolución de Uribe: «los mismos que pedían respeto por el fallo de la juez que condenó a Uribe, ahora se van lanza en ristre»; el rótulo del título va contra ellos |
| 2 | 2026-01-05 | Las seis de las 6 con Juan Lozano \| lunes 5 de enero de 2026 | `las-seis-de-las-6-con-juan-lozano-lunes-5-de-enero-de-2026-387043` | **D leve** | Sobre la captura de Maduro: la polémica viene «especialmente entre quienes guardaron silencio frente a las irregularidades electorales en Venezuela y ahora cuestionan la intervención estadounidense». Rótulo de doble rasero, sin nombre |
| 3 | 2026-03-20 | Las seis de las 6 con Juan Lozano \| viernes 20 de marzo de 2026 | `juan-lozano-noticias-importantes-20-marzo-2026-seis-393988` | **D leve** | Ante la encuesta que da ganador a Cepeda, a De la Espriella y Valencia: «El mensaje es claro: o se unen o se hunden». Consejo de estrategia a un solo lado |
| 4 | 2026-06-10 | seis de las 6 con Juan Lozano: miércoles 10 de junio de 2026 | `seis-de-las-6-con-juan-lozano-miercoles-10-de-junio-2026-401827` | **D leve** | La orden judicial de retirar los símbolos patrios de la campaña de De la Espriella: «Lozano calificó la determinación como una medida inédita» y recoge la «solidaridad y respaldo» de sus seguidores |
| 5 | 2026-06-23 | Seis de las 6 con Juan Lozano \| martes 23 de junio de 2026 | `seis-de-las-6-con-juan-lozano-viernes-23-de-junio-2026-403007` | **D** | Tras la segunda vuelta: «la economía colombiana respira optimismo con los denominados “Abelardonomics”». Sobre el «voto fusil» (voto unánime forzado «por una sola corriente»), el director lo compara con la parapolítica y exige rigor judicial. Es el «voto de fusil» que la ficha cita como editorial |
| 6 | 2026-07-08 | Seis de las 6 con Juan Lozano \| miercoles 8 de julio de 2026 | `seis-de-las-6-con-juan-lozano-miercoles-de-julio-2026-404111` | **D leve** | Da relevancia al mensaje del presidente electo a las Fuerzas Militares «tras la negativa del mandatario saliente a reconocer los resultados» y destaca «la buena recepción» de su ministro de Defensa |
| 7 | 2026-07-23 | Las seis de las 6 con Juan Lozano \| jueves 23 de julio de 2026 | `las-seis-de-las-6-con-juan-lozano-jueves-23-de-julio-de-2026-405707` | **D** | Hace suyo el rechazo del Gobierno electo a la tributaria del saliente: «insistió en que el desafío para la próxima administración será fortalecer la austeridad estatal […] antes de promover nuevas cargas tributarias». La capital alterna «trasciende lo simbólico» |
| 8 | 2026-07-24 | Las seis de las 6 con Juan Lozano \|viernes 24 de julio de 2026 | `las-seis-de-las-6-con-juan-lozano-viernes-24-de-julio-de-2026-405808` | **D leve** | «Destacó las gestiones» del gobierno entrante «para fortalecer la confianza de la banca internacional» |
| 9 | 2026-02-06 | Las seis de las 6 con Juan Lozano \| viernes 6 de febrero de 2026 | `las-seis-de-las-6-con-juan-lozano-viernes-6-de-febrero-de-2026-389777` | **C** | «Visita exitosa de Petro a Washington […] mediante hábil diplomacia […]; pese a posibles peros, el saldo es positivo». La misma edición carga contra la Paz Total (F) |
| 10 | 2026-02-04 | Las seis de las 6 con Juan Lozano \| miércoles 4 de febrero de 2026 | `las-seis-de-las-6-con-juan-lozano-miercoles-4-de-febrero-de-2026-389554` | M | La reunión Petro-Trump, «con un parte satisfactorio para Colombia», sirvió para «rescatar» la relación; y Petro «bajó el tono, dejó atrás insultos previos» |
| 11 | 2026-06-09 | Las seis de las 6 con Juan Lozano \| lunes 9 de junio de 2026 | `las-seis-de-las-6-con-juan-lozano-lunes-9-de-junio-de-2026-401710` | M | Pide proteger a los dos candidatos; reconoce que Cepeda aceptó los resultados de primera vuelta, «un paso que el presidente de la República aún no ha dado» |
| 12 | 2026-06-11 | Seis de las 6 con Juan Lozano \| jueves 11 de junio de 2026 | `seis-de-las-6-con-juan-lozano-jueves-11-de-junio-2026-401954` | M | La suspensión de Petro por una representante, «desde dos perspectivas» (la participación en política y la competencia de quien lo suspende); la orden contra De la Espriella, «de difícil aplicación» |
| 13 | 2026-07-14 | Seis de las 6 con Juan Lozano - martes 14 de julio de 2026 | `seis-de-las-6-juan-lozano-martes-14-julio-2026-404860` | M | El equipo entrante va a Washington «para recuperar la confianza internacional»; de los nuevos ministros, «sus perfiles técnicos, aunque existen inquietudes sobre algunas posturas previas del nuevo ministro de Agricultura» |

### 2.2 Después del cambio: 2026-08-07 → 2026-10-11 (gobierna De la Espriella)

| # | Fecha | Título literal | Ruta | Clase | Por qué (fragmento) |
|---|---|---|---|---|---|
| 14 | 2026-08-31 | Seis de las 6 con Juan Lozano - lunes 31 de agosto de 2026 | `seis-de-las-6-con-juan-lozano-lunes-31-de-agosto-2026-409427` | **D** | «Destacó la decisión del Gobierno de no continuar los diálogos»; «los procesos anteriores terminaron fortaleciendo a algunas organizaciones ilegales». Dentro, exigencias al Gobierno: resultados contra la corrupción, presupuesto «sin acuerdos políticos condicionados», menos burocracia |
| 15 | 2026-09-03 | Seis de las 6 con Juan Lozano jueves 3 de septiembre 2026 | `seis-de-las-6-con-juan-lozano-jueves-3-de-septiembre-2026-409657` | **D leve** | El respaldo de Trump «alimenta las expectativas»; la relación con el Congreso, «en un escenario que busca alejarse de las prácticas asociadas a la llamada "mermelada"». El resto, descriptivo |
| 16 | 2026-09-29 | Las seis de las 6 con Juan Lozano martes 29 de septiembre | `seis-de-las-6-con-juan-lozano-martes-29-de-septiembre-de-2026-412351` | **D leve** | «Destacó el avance de las fuerzas de tarea conjunta»; la alianza Vicepresidencia-Colfuturo «representa un resultado de la gestión». El mismo texto se sirve el 06-10 en `seis-de-las-6-con-juan-lozano-martes-6-de-octubre-2026-413102`; cuenta una vez |
| 17 | 2026-10-05 | Las seis de las 6 con Juan Lozano \| 5 de octubre de 2026 | `las-seis-de-las-6-con-juan-lozano-lunes-5-de-octubre-de-2026-412976` | M | El presidente «asumió una posición contundente frente a la corrupción», y a la vez: presunción de inocencia del alcalde señalado, y «el estándar planteado por el presidente debe aplicarse a todo el Gobierno». Es el único reparo de fondo al Gobierno nuevo en la ventana |

**Ninguna pieza C después del cambio.** Las otras 15 ediciones posteriores (20, 21, 24, 25, 26, 27 y 28-08; 21, 22, 23, 25, 28 y 30-09; 01 y 02-10) son descriptivas: anuncios del Gobierno contados sin comentario propio. Algunas recogen sin contrapunto afirmaciones de ministros (la «campaña woke» del Gobierno anterior, 21-08, atribuida a la ministra de Educación). Al ser atribuidas, no se clasifican.

### 2.3 Fiscalización del Gobierno Petro (F: se declara, no suma)

La mayoría de las ediciones con comentario antes del 07-08 fiscalizan al Gobierno en ejercicio. Una muestra fechada, no exhaustiva, de las que lo hacen con voz propia y no solo citando a otro:

- 28-10-2025: el invierno llega «en el país donde se robaron la Unidad de Gestión del Riesgo».
- 03-12-2025 (`…-384311`): pasaportes, Registraduría.
- 17-12-2025 (`…-385624`): «La llamada paz total terminó confirmándose, para muchos, como violencia total».
- 22-12-2025 (`…-386052`): «Fracaso de la política de paz del gobierno»; el decreto de emergencia «sería inconstitucional».
- 23-12-2025 (`…-386157`): la liberación de soldados deja «la sensación de burla […] por falta de autoridad».
- 24-12-2025: Colfuturo sin recursos; se critica el debilitamiento del ICETEX.
- 09-01, 15-01 y 16-01-2026: deuda «de aire», deuda externa, Nueva EPS.
- 05-02-2026: la UNGRD, «la misma que los corruptos saquearon».
- 17-02, 18-02 y 20-02-2026 (`…-390877`, `…-391119`): el caso de Kevin Acosta, «la actitud de indolencia del gobierno».
- 04-03-2026 (`…-392297`): las dudas de Petro sobre el conteo, «un riesgo de preparar el terreno para desconocer los resultados».
- 19-03-2026 (`…-393724`): Fecode y la USO, «paradoja» por su respaldo al Gobierno.
- 15-05-2026 (`…-399367`): el director pide a las misiones de observación pronunciarse sobre las solicitudes del presidente acerca del código fuente; alarma por los TES. **La ficha la presenta como el editorial firmado más fuerte; por el polo fijo, es fiscalización y no suma.**
- 27-05-2026 (`…-400490`): la participación en política del presidente; «la paquidérmica, muchas veces paralizada Comisión de Acusación».
- 05-08-2026 (`…-406925`): «no existen elementos para sostener que hubo fraude».

**Después del 07-08: ninguna edición fiscaliza al Gobierno De la Espriella.** Los únicos reparos están dentro de #14 y #17.

### 2.4 Leídas y sin postura que cuente (se declaran)

- **02-01-2026**, «Los 6 retos de Colombia en el 2026» (`los-6-retos-de-colombia-en-el-2026-386876`) y su versión larga (`seis-grandes-retos-de-colombia-en-2026-386870`): «Manejo ortodoxo de la macroeconomía», «recortando gasto burocrático» y evitar «más impuestos». Es **programa propio en la dirección D**, como el estudio de hidrocarburos de El Pilón. No es una postura sobre un gobierno ni un candidato.
- **11-12-2025**: «La heroína de América, María Corina Machado». Internacional.
- **11-05 y 12-05-2026**: el homenaje a Vargas Lleras y la frase de su hija contra «Cepeda y sus secuaces», contada como «controversia», sin hacerla suya. Necrológica y cita.
- **Campaña de primera y segunda vuelta** (19-05, 21-05, 25-05, 26-05, 28-05, 29-05, 01-06, 03-06, 05-06, 12-06, 16-06 a 19-06): actividades de los candidatos contadas en paralelo. El 01-06 la segunda vuelta enfrenta «dos modelos económicos opuestos», sin preferencia.
- **No hay endoso.** En ninguna de las 185 piezas el director o la casa piden el voto por un candidato con nombre ni declaran su apoyo a uno.

---

## 3. Recuento

| | D (derecha) | C (contrapeso) | M (mixta, no cuenta) | Con postura que cuenta (D + C) |
|---|---|---|---|---|
| Antes del 07-08-2026 | **8** (3 firmes, 5 leves) | **1** | 4 | 9 |
| Desde el 07-08-2026 | **3** (1 firme, 2 leves) | **0** | 1 | 3 |
| **Total** | **11** | **1** | 5 | **12** |

**Proporción: 11 a 1.** Las piezas con postura son 12, y 17 si se suman las mixtas.

Sensibilidad, para que el lector la recuente:

| Lectura | D antes | D después | C | Proporción | ¿Mínimos? |
|---|---|---|---|---|---|
| Principal (todas las D y C) | 8 | 3 | 1 | 11 : 1 | **Sí**: 12 con postura, 8 y 3 a cada lado |
| Sin las D «leves» | 3 | 1 | 1 | 4 : 1 | **No**: 5 con postura, 1 después |
| Las mixtas #10 y #17 pasan a C | 8 | 3 | 3 | 3,7 : 1 | Sí |
| Las mixtas #10 y #17 pasan a C y sin las D leves | 3 | 1 | 3 | 1,3 : 1 | No |

**La lectura del polo fijo**, que separa fiscalizar a quien manda de lo que no lo es:

| Trato al gobierno **en ejercicio** | Favorables o reconocimientos | Críticos (F) | Mixtos |
|---|---|---|---|
| Petro, mientras gobierna (10 meses, 166 URL) | **1** (#9) | **la mayoría de las ediciones con comentario** (§2.3, muestra de 18) | 2 (#10, #11) |
| De la Espriella, ya en el poder (2 meses, 19 textos) | **3** (#14-#16) | **0** | 1 (#17) |

- **Con Petro**, la sección fiscaliza a diario: seguridad, salud, finanzas, emergencias económicas, el discurso sobre fraude. Lo hace con rótulos propios («violencia total», «indolencia», «paquidérmica») y casi sin reconocimientos: solo la visita a Washington (#9, #10).
- **Con De la Espriella**, en los dos meses que hay, la sección cuenta sus anuncios sin comentario o los destaca (#14-#16). El único reparo es de principio, no a una política (#17). Tampoco aparece la vara que se aplicaba al saliente: la segunda emergencia económica del nuevo Gobierno, por El Niño (23-09), se cuenta sin las dudas de constitucionalidad que acompañaron las de Petro (22-12-2025, 13-02-2026).
- **Esta es la asimetría que el polo fijo admite como evidencia**: fiscalizar con dureza a un lado y pasar a destacar cuando llega el otro. Pero la regla no deja que la fiscalización sume: el número sale solo de las D y C de la tabla de arriba.
- **Sobre las candidaturas, antes de las urnas**: hay un consejo de estrategia a la derecha (#3), una defensa del candidato frente a un juez (#4) y el «Abelardonomics» del día después (#5). **No hay endoso.**

---

## 4. Contrapesos (lo que contradice la dirección, y cuánto pesa)

| Contrapeso | Piezas | Peso |
|---|---|---|
| **Reconocimiento al Gobierno Petro** por la reunión con Trump | #9, #10 | **Bajo-medio.** Es la única política del saliente que la sección elogia en diez meses, y lo hace con peros |
| **Reparo de principio al nuevo presidente**: presunción de inocencia y el mismo estándar para su propio Gobierno | #17 | **Medio-bajo.** Es el único en dos meses, y no toca ninguna política (seguridad, fin de la Paz Total, cierre de embajadas, recortes a la JEP) |
| **Exigencias al nuevo Gobierno** en la pieza que lo elogia: resultados contra la corrupción, presupuesto sin «mermelada», menos burocracia | dentro de #14 | **Bajo.** Son demandas, no críticas a un acto |
| **Defensa institucional en los dos sentidos**: protección para los dos candidatos, Cepeda reconoció resultados, «serenidad y altura técnica de ambos» (Registrador y Petro, 20-02) | #11, #12, 20-02 | **Medio para la magnitud.** La defensa de la Registraduría y del resultado es institucional, aunque en la práctica choque siempre con el mismo lado |
| **Sin endoso** en toda la ventana | §2.4 | **Alto para la magnitud.** Sin endoso ni nivel 1 con posición documentada, el tope es ±0,30 |
| **Formato de resumen** (redacción web, en tercera persona y en parte con IA) | §1 | **Medio.** La postura que se lee es la que el resumen atribuye al director; las «leves» son las más expuestas a esa capa |

**Lo que se declara y no es contrapeso ni nivel 1.** La sección promociona a la casa y a sus socios: la alianza con RCN, El Tiempo y La República en debates y encuestas, y el Hay Festival «con apoyo de RCN, La República y Postobón» (30-01-2026). Postobón es de la misma organización. Va con la tensión de propiedad que la ficha ya tiene abierta.

---

## 5. Veredicto por condición

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | **Sí, con aviso** | Es la «Carta del director», firmada por el director o por «La Fm». Pero es un resumen de la emisión, no su texto literal (§1) |
| 2. A los dos lados del cambio, en 12 meses | **Sí, con asimetría** | Antes: 8 D, 1 C y fiscalización diaria. Después: 3 D, 0 C y ninguna fiscalización |
| 3a. ≥10 piezas con postura | **Sí** | 12 (17 con las mixtas) |
| 3b. ≥3 a cada lado del cambio | **Sí, por la mínima** | 9 antes y 3 después. **Las 3 de después incluyen dos leves**: sin ellas, 1 |
| 3c. Proporción ≥3:1 | **Sí** | 11:1. Sigue por encima de 3:1 aunque dos mixtas pasen a C (3,7:1) |
| 4. Contrapesos escritos | **Sí** | §4, con peso |
| 5. Reproducible | **Sí** | §2 con fecha, título, ruta y clase; §1 con el método, la cobertura y los huecos |

**En la lectura principal se cumplen las cinco.** La 3b es la débil: depende de dos piezas leves, de un lado de dos meses con la primera quincena sin cubrir.

---

## 6. Rama de la precisión del 2026-10-10 y PROPUESTA (pendiente de firma)

**Por qué manda el barrido.** El +0,35 no se apoya en ninguna pieza del medio. Lo sostienen una frase sin fuente («línea editorial crítica con gobiernos progresistas») y la propiedad, que es de nivel 1 pero no documenta una posición: la ficha la tiene «todavía sin cerrar». Es un valor de niveles 4 y 5, así que por la precisión del 2026-10-10 manda el barrido. El +0,35 está además por encima del tope de ±0,30, que sin nivel 1 con posición ni endoso no se puede pasar.

**Rama que se cumple: la primera, «cumple los mínimos».** Corresponde el valor del barrido, con el tope de ±0,30, porque no hay endoso explícito.

**Propuesta: +0,25, derecha moderada.** Es un juicio declarado, razonado contra los vecinos:
- **Por qué no +0,30, el tope**:
  - el lado de después llega a 3 solo con dos leves;
  - los textos son resúmenes y no la voz literal;
  - no hay endoso;
  - hay un reparo de principio al nuevo presidente (#17).

  La regla 2 pide, ante la duda entre dos bandas, la más cercana a la mixta. Al tope llegan hoy Archipiélago Press, La Opinión y El País de Cali (+0,30), y RTVC por la excepción gubernamental.
- **Por qué no +0,20**, como El Pilón o El Heraldo:
  - El Pilón no llega a 3:1 (2,2:1), reconoce cuatro programas del saliente y le pone un reparo de fondo al entrante. Aquí hay un solo reconocimiento al saliente en diez meses y ninguna crítica al entrante en dos;
  - El Heraldo está en +0,20 con un endoso. Esa comparación empuja hacia abajo, y por eso tampoco se sube al tope.
- **A la altura de Noticias RCN (+0,25)**, del mismo dueño y bajo el mismo consejero de medios, y de El Diario de Pereira y Vive el Meta (+0,25). La diferencia de +0,10 con Noticias RCN que la ficha no sabía explicar desaparece. Desaparece por evidencia, no por igualar.

**Lectura estricta, que se declara.** Si las piezas leves no cuentan como postura, el barrido no llega: quedan 5 piezas con postura y 1 después del cambio. La dirección sigue siendo clara: 4 D por cada C, y ninguna crítica al Gobierno nuevo. Esa es la **tercera rama**: **«sin medir» (`bias: null`)**, con la dirección derecha declarada como tensión. **No** sería la rama del 0,00 con evidencia: no hay la misma conducta con los dos gobiernos.

**Lo que esta propuesta NO hace:**
- No cambia el registro, la propiedad, la ficha ni los textos públicos.
- No resuelve el nivel 1 heredado (dueños fallecidos en el MOM, Parklake, Carbe), que sigue abierto en la ficha.
- No barre las noticias de la redacción ni el audio.

**Qué la refutaría:**
- **hacia arriba**: que en los meses siguientes la sección siga sin fiscalizar al Gobierno De la Espriella, y que los «destacó» se vuelvan respaldo explícito a su programa (armas, aspersión aérea, recortes a la JEP), o un endoso con nombre en una próxima elección, que además levantaría el tope;
- **hacia abajo**: que la sección fiscalice al Gobierno nuevo con la frecuencia y los rótulos que usaba con el saliente;
- **en cualquier sentido**: que las ediciones que faltan (sobre todo del 07 al 19-08 y del 01 al 18-09-2026) muevan el lado de después, que es el que decide los mínimos.

---

## 7. Avisos

- **Una sola lectura.** La clasificación es de un verificador de la misma casa que el autor de la ficha. Las piezas límite están marcadas «leve» o «M», y el §3 da el recuento con y sin ellas.
- **Resumen y no transcripción.** Ninguna frase atribuida al director se ha contrastado con el audio. Si el resumen web suaviza o endurece lo dicho al aire, la clasificación lo hereda.
- **Huecos.** 85 de 260 días hábiles sin pieza. Los dos más graves caen en el lado de después.
- **Un texto duplicado.** El 29-09 y el 06-10-2026 sirven el mismo cuerpo; se contó una vez.
- **Datos personales.** No se copia ningún número de documento, teléfono ni dirección. La edición del 09-06-2026 reproduce una lista de presuntos compradores de votos con nombre; no se copia aquí. Las personas nombradas son cargos públicos, candidatos o el director del medio, con su papel.
