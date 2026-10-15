# Barrido editorial histórico — Vive el Meta (viveelmeta.com)

| | |
|---|---|
| **Medio** | Vive el Meta (`vive-el-meta`), Villavicencio |
| **Fecha del barrido** | 2026-10-09 |
| **Quién lo hizo** | Claude Code (Claude Opus 5.5), a petición del responsable editorial; ciclo 2, tanda 5 |
| **Regla que aplica** | `PROTOCOLO_JUICIO_EDITORIAL.md`, «Evidencia editorial histórica» (condición 5: reproducible) |
| **Resolución de la que sale** | `revision-externa/respuestas/opus-5-5-vive-el-meta.md` |
| **Ficha** | `fichas/vive-el-meta.md` |

Este archivo existe para que cualquiera pueda recontar las piezas y llegar, o
no, al mismo número. Quien lo hizo es de la misma casa que el autor de la
ficha, el revisor y el verificador: que los cuatro coincidan no es aval.

---

## 1. Método

- **robots.txt** de www.viveelmeta.com (2026-10-09): un solo bloque
  `User-agent: *` con `Disallow: /wp-json/` y `Disallow: /?rest_route=`. No
  menciona a ClaudeBot, Claude-Web ni anthropic-ai. **No se usó la API wp-json.**
- **Universo.** Los 9 `post-sitemap` del
  [`sitemap_index.xml`](https://www.viveelmeta.com/sitemap_index.xml): 8.517
  URL el 2026-10-09 (8.513 el 2026-10-08, según la resolución). Se descargaron
  en crudo las 1.121 piezas con ID ≥ 47600, con
  `curl -sL --ssl-no-revoke` y User-Agent de navegador, a razón de una cada
  0,4 s por proceso.
- **Ventana (regla del presente):** del 2026-10-09 hacia atrás 12 meses, es
  decir, piezas publicadas desde el **2025-10-09 00:00 hora de Colombia**:
  **1.083 piezas** (de la 47767, del 14-10-2025, a la 52549, del 09-10-2026).
- **De cada pieza** se sacó: `article:published_time` (UTC, convertido a hora
  de Colombia, UTC−5), `og:title`, `og:description` (la entradilla),
  `articleSection` y `author` del JSON-LD, y el texto del contenedor
  `#continue-reading` sin etiquetas.
- **Cambio de gobierno:** 2026-08-07. «Antes» es hasta el 06-08 inclusive;
  «después», desde el 07-08. La primera pieza posterior es la 51519 (08-08).
- **Selección del barrido (sistemática, por términos sobre toda la ventana).**
  Entran todas las piezas de la ventana cuyo titular o entradilla casa con esta
  expresión regular (sin distinguir mayúsculas), salvo las que casan con
  `ecopetrol|tigres del norte`:

  ```
  cepeda|espriella|abelardo|el tigre|'tigre'|‘tigre’|petro\b|petrista|petrismo|pacto hist|progresista|izquierda|derecha|álvaro uribe|uribismo|paloma valencia|fajardo|presidencial|gobierno nacional|gobierno del cambio|harman|libro de la verdad|juco|isabel zuleta|editorial \|
  ```

  Resultado: **224 piezas, 175 antes y 49 después del cambio.** Se leyeron el
  titular y la entradilla de las 224, y el cuerpo de todas las que tienen
  clasificación distinta de A o F, más las marcadas «(límite)».
- **Voz.** El campo `author` del JSON-LD es «viveelmeta.com» en 1.070 de las
  1.083 piezas de la ventana; las otras 13 las firma Fernando Betancourt, el
  periodista de la página de equipo. **Las columnas firmadas no cuentan como voz
  de la casa.** El texto rotulado «Editorial |» (49617) sí cuenta, aunque sus
  metadatos lo atribuyan a Betancourt: el rótulo lo hace de la casa. El medio
  no nombra director.

## 2. Clasificación

Cada pieza lleva un código. **Solo D y C entran en la cuenta** de la
condición 3.

| Código | Qué es | ¿Cuenta? |
|---|---|---|
| **D** | Postura en voz de la casa (titular, entradilla, análisis o editorial propios, sin atribuir a una fuente) que favorece a la derecha frente a la izquierda: encuadre asimétrico entre candidatos antes del cambio; celebración del gobierno entrante o burla al expresidente, ya sin poder, después | sí, a favor de la dirección |
| **C** | Postura en voz de la casa en sentido contrario a D (crítica propia al candidato o al gobierno de derecha, o favorable a la izquierda) | sí, en contra |
| F | Adversa al gobierno en ejercicio antes del 07-08 (propia o atribuida). Regla del polo fijo: fiscalizar al que manda no es orientación | no |
| A | Atribuida a una fuente (cita, comunicado, encuesta, informe, funcionario) o informativa sin postura propia | no |
| V | Da voz a críticos del gobierno entrante (contrapeso atribuido) | no; se declara |
| N | Política local sin lectura en el eje | no |

«(límite)» marca las piezas que una lectura más amplia pondría en D y esta no
pone. Se dejaron fuera para no inflar la cuenta.

## 3. Resultado y las cinco condiciones

| | Antes del 07-08 | Después del 07-08 | Total |
|---|---|---|---|
| Piezas del barrido | 175 | 49 | **224** |
| **D** (postura propia hacia la derecha) | **7** | **5** | **12** |
| **C** (postura propia en contra) | 1 | 0 | **1** |
| F (fiscalización del gobierno en ejercicio) | 83 | — | 83 |
| A (atribuida o informativa) | 81 | 40 | 121 |
| V (voz a críticos del gobierno entrante) | — | 4 | 4 |
| N (local, sin eje) | 3 | 0 | 3 |

1. **Voz de la casa: se cumple.** Las 13 piezas D y C son titulares,
   entradillas, análisis o el editorial sin firma de autor (todas con `author`
   «viveelmeta.com», salvo el editorial rotulado). No cuenta ninguna columna
   firmada, ninguna pieza que recoja un comunicado ni ninguna cita de terceros.
   Las columnas de Betancourt contra Petro (13-07-2026; 08-10-2025, fuera de la
   ventana) se escribieron con Petro gobernando: son fiscalización y no
   cuentan.
2. **A los dos lados del cambio de gobierno, dentro de 12 meses: se cumple.**
   7 piezas D antes y 5 después. Antes, encuadre asimétrico entre candidatos
   (no fiscalización del gobierno); después, celebración del entrante y burla
   al saliente.
3. **Sostenida: se cumple.** 12 piezas con postura (mínimo 10), 7 y 5 a cada
   lado (mínimo 3) y una proporción de **12 a 1** en la misma dirección
   (mínimo 3 a 1).
4. **Contrapesos escritos: se cumple.** Ver §5.
5. **Reproducible: este archivo.** La tabla completa está en §6.

**Sensibilidad, dicha sin rodeos.** De las 12 piezas D, 8 son inequívocas
(48251, 49617, 50756, 50833, 51519, 51580, 52123 y 52342) y 4 son más tenues
(47876, de una elección local de juventud; 50522; 50775; y 51998, por la
expresión «campaña negra»). **Con solo las 8 inequívocas no se llega al mínimo
de 10.** En sentido contrario, la lectura de la resolución pondría en D otras
cinco que aquí quedan como «(límite)» (51587, 51630, 52298, 52428 y 49621), y
la cuenta subiría a 17. El umbral se cumple con el criterio declarado arriba y
con margen en la lectura amplia, pero no en la más estricta. Quien recuente con
otro criterio debe decirlo.

## 4. Las piezas que cuentan, con su cita

Fechas en hora de Colombia. Citas literales del crudo descargado el 2026-10-09.

**Antes del 07-08 (encuadre entre candidatos y sectores):**

- [47876](https://www.viveelmeta.com/aplastante-derrota-de-los-partidos-progresistas-en-la-eleccion-del-consejo-de-juventud-de-villavicencio-47876/) (20-10-2025), titular: «Aplastante derrota de los partidos progresistas en la elección del Consejo de Juventud de Villavicencio». **D.**
- [48251](https://www.viveelmeta.com/abelardo-de-la-espriella-el-unico-que-podria-tumbar-a-la-izquierda-del-poder-segun-encuesta-del-cnc-48251/) (18-11-2025): De la Espriella «se perfila como la figura con mayor capacidad de tumbar a la izquierda del poder, representada por Petro y su candidato». **D.**
- [49617](https://www.viveelmeta.com/editorial-en-villavicencio-la-oposicion-critica-pero-no-logra-ganar-49617/) (09-03-2026), «Editorial | En Villavicencio la oposición critica, pero no logra ganar»: «Más que construir una alternativa política fuerte, la oposición parece haberse quedado en la crítica permanente» y «Mientras un sector mantiene organización y votantes, el otro aún no logra consolidar un proyecto político que realmente dispute el liderazgo en la ciudad». El sector elogiado es el del alcalde, al que el texto atribuye «el respaldo de Salvación Nacional y el coaval del Centro Democrático y Colombia Justa y Libres». **D.**
- [50522](https://www.viveelmeta.com/cne-suspende-a-atlas-intel-encuestadora-que-dio-al-tigre-como-proximo-presidente-de-colombia-50522/) (20-05-2026): la resolución la firma una magistrada «aparentemente muy cercana al Pacto Histórico». **D.**
- [50756](https://www.viveelmeta.com/mas-constituyente-y-un-discurso-mas-radical-lo-que-revelan-las-433-paginas-del-programa-de-gobierno-de-ivan-cepeda-50756/) (08-06-2026), análisis propio del programa de Cepeda: «¿La segunda etapa del cambio que propone Iván Cepeda traerá soluciones concretas para regiones como el Meta o terminará concentrada, principalmente, en profundizar el discurso ideológico…?». No hay análisis equivalente del programa de De la Espriella en la ventana. **D.**
- [50775](https://www.viveelmeta.com/bomba-politica-orden-judicial-le-prohibe-al-tigre-utilizar-la-bandera-y-la-frase-firmes-por-la-patria-50775/) (09-06-2026): «¡Bomba política!» y «la candidatura de De la Espriella, que sigue fortaleciéndose de cara a la segunda vuelta presidencial». **D.**
- [50833](https://www.viveelmeta.com/cepeda-propone-que-colombia-sea-sede-de-un-mundial-de-futbol-y-estallan-las-redes-va-pa-personero-50833/) (13-06-2026), entradilla: «Los cibernautas no le perdonaron la cuestionada gestión de Gustavo Petro en materia deportiva». **D.**
- [50551](https://www.viveelmeta.com/paloma-valencia-y-abelardo-de-la-espriella-libran-disputa-que-podria-terminar-beneficiando-a-ivan-cepeda-50551/) (22-05-2026): «el discurso radical de De la Espriella podría dificultar la llegada de apoyos desde el centro político». Es crítica propia al candidato que ganó, aunque hecha desde la orilla de Paloma Valencia («la opción más sólida para enfrentar a la izquierda»). **C**, contada en contra para no favorecer la dirección.

**Después del 07-08 (gobierno entrante y expresidente):**

- [51519](https://www.viveelmeta.com/adios-privilegios-de-la-espriella-ordena-trasladar-a-epa-colombia-a-una-carcel-de-mayor-seguridad-51519/) (08-08-2026): «Adiós privilegios: De la Espriella ordena trasladar a ‘Epa Colombia’…». **D.**
- [51580](https://www.viveelmeta.com/gustavo-petro-solicito-permiso-al-senado-para-salir-del-pais-por-un-ano-se-quiere-volar-51580/) (12-08-2026): «…¿Se quiere volar?». **D.**
- [51998](https://www.viveelmeta.com/promueven-campana-negra-contra-avianca-por-negarse-a-transportar-a-gustavo-petro-51998/) (05-09-2026): «Promueven campaña negra contra Avianca por negarse a transportar a Gustavo Petro». **D.**
- [52123](https://www.viveelmeta.com/petro-intento-funar-al-gobierno-pero-le-salio-mal-confundio-a-un-ministro-con-oviedo-ebrio-52123/) (14-09-2026): «Petro intentó funar al Gobierno pero le salió mal…». **D.**
- [52342](https://www.viveelmeta.com/que-bruto-petro-publico-video-de-2021-para-denunciar-supuesta-violencia-policial-en-el-actual-gobierno-52342/) (28-09-2026): «¡Qué bruto!…» y, en el cuerpo, «No es la primera vez que el expresidente intenta atacar al gobierno y se equivoca». **D.**

En dos meses de gobierno nuevo, **ninguna pieza del barrido critica al
gobierno entrante con voz propia.**

## 5. Contrapesos (condición 4)

**Dentro del barrido:**

- **C = 1:** 50551, crítica propia a De la Espriella (arriba). Pesa poco: la
  hace desde la derecha.
- **V = 4**, voz a críticos del gobierno entrante, atribuida:
  [51882](https://www.viveelmeta.com/joven-que-amenazo-con-hacer-invivible-el-pais-a-de-la-espriella-denuncia-amenazas-y-acoso-51882/)
  (la dirigente de la Juco denuncia amenazas),
  [52361](https://www.viveelmeta.com/senadora-petrista-pide-excomulgar-a-de-la-espriella-por-invocar-a-dios-en-medio-de-acciones-militares-52361/)
  (con el rótulo «petrista» en el titular),
  [52500](https://www.viveelmeta.com/abra-las-puertas-de-la-reeleccion-y-me-enfrentara-petro-reta-a-de-la-espriella-a-un-duelo-en-las-urnas-52500/)
  y
  [52529](https://www.viveelmeta.com/de-la-espriella-responde-a-criticas-por-caminar-entre-cuerpos-de-criminales-mas-lo-voy-a-hacer-52529/)
  (las críticas, encuadradas desde la respuesta del presidente). Pesan poco:
  en dos de las cuatro el encuadre lo da el gobierno o un rótulo.
- **40 piezas A después del cambio**: la mayoría de lo que el medio publica
  sobre el gobierno entrante es informativo o atribuido, sin postura propia
  (p. ej. 51605, 51900, 52037, 52071, 52349, 52522). Sobre el expresidente,
  la mayoría de las piezas adversas se apoyan en funcionarios del gobierno
  entrante (Libro de la Verdad, ANT, Dapre, MinTIC), no en voz propia.

**Fuera del barrido (no casan con la expresión regular), con trabajo propio:**

- Fiscalización documental de alcaldías del Meta:
  Acacías ([52008](https://www.viveelmeta.com/extrano-patron-de-precios-en-licitacion-logistica-por-3-867-millones-en-acacias-52008/),
  [52219](https://www.viveelmeta.com/acacias-pagara-mas-de-1-300-millones-por-90-minutos-de-silvestre-dangond-en-el-festival-del-retorno-52219/),
  [52385](https://www.viveelmeta.com/cambia-la-empresa-pero-no-el-beneficiario-corcedef-y-jema-suman-22-324-millones-en-contratos-recibidos-de-carlos-plata-en-acacias-52385/),
  [52432](https://www.viveelmeta.com/relacionan-al-alcalde-carlos-plata-con-loteos-ilegales-en-acacias-por-que-52432/)),
  Restrepo ([52452](https://www.viveelmeta.com/alcalde-de-restrepo-adjudico-a-dedo-5965-millones-a-empresa-recien-creada-52452/),
  [51671](https://www.viveelmeta.com/cuestionan-presunta-titulacion-expres-del-secretario-de-gobierno-de-restrepo-graduado-en-la-u-san-jose-51671/))
  y Mesetas ([51891](https://www.viveelmeta.com/denuncian-penalmente-al-alcalde-de-mesetas-habrian-usado-la-firma-de-una-empresaria-ausente-del-pais-para-limitar-contratos-51891/),
  [51768](https://www.viveelmeta.com/alcaldia-de-mesetas-reconoce-que-camioneta-accidentada-no-registra-mantenimientos-durante-la-actual-administracion-51768/),
  [52402](https://www.viveelmeta.com/alcaldia-de-mesetas-reconoce-que-camioneta-accidentada-no-tenia-mantenimiento-registrado-ni-tecnomecanica-vigente-52402/)),
  y la Gobernación de Casanare
  ([52081](https://www.viveelmeta.com/licitacion-a-la-medida-compra-de-equipos-medicos-de-la-gobernacion-de-casanare-favoreceria-a-un-solo-proponente-52081/)).
  La filiación de esos alcaldes **no consta**, así que no sitúa al medio en el
  eje: muestra que fiscaliza a algunos poderes. *Nota: 52452 publica el
  teléfono y la dirección de una persona natural; aquí no se reproducen.*
- Dos piezas críticas con la Gobernación del Meta, ambas recogiendo a terceros:
  [50693](https://www.viveelmeta.com/docentes-del-meta-amenazan-con-paro-por-incumplimientos-de-la-gobernacion-50693/)
  (02-06-2026, comunicado de ADEM) y
  [50706](https://www.viveelmeta.com/mas-de-339-000-millones-sin-ejecutar-obligan-a-la-gobernacion-del-meta-a-reajustar-su-presupuesto-50706/)
  (03-06-2026, un diputado, con una frase de voz propia: «La crítica apunta a
  que el problema no es cuánto dinero se está incorporando al presupuesto este
  año, sino por qué esos recursos no llegaron oportunamente…»).
- **Cuánto pesan, en conjunto:** muestran oficio de fiscalización local y algo
  de voz a la oposición nacional, pero no contradicen la dirección en el eje:
  no hay ni una pieza propia que favorezca a la izquierda o critique al
  gobierno entrante. Buena parte de la sección «Nacionales» parece reescritura
  de otros medios; la selección y los titulares sí son del medio.

**Lo que tampoco cuenta y se declara:**

- Columnas firmadas por Fernando Betancourt en Opinión:
  [«El ocaso del "jaguar"…»](https://www.viveelmeta.com/opinion-el-ocaso-del-jaguar-el-animal-que-quedo-sin-reino-y-sin-manada-51070/)
  (05-07-2026; alegoría sin nombres, a quién alude no se afirma),
  [«El Agro Ingreso Seguro de Gustavo de Petro»](https://www.viveelmeta.com/opinion-el-agro-ingreso-seguro-de-gustavo-de-petro-51164/)
  (13-07-2026, gobierno en ejercicio) y
  [«Entre torta, políticos y expedientes…»](https://www.viveelmeta.com/entre-torta-politicos-y-expedientes-juan-diego-munoz-soplo-la-vela-y-empezo-a-armar-su-camino-hacia-la-gobernacion-51863/)
  (28-08-2026, local). «Promesas sin obras… el legado de Petro al Meta»
  (47762, 08-10-2025) queda fuera de la ventana.
- [52025](https://www.viveelmeta.com/la-paz-total-dejo-una-factura-de-125-174-millones-y-ningun-acuerdo-con-grupos-ilegales-52025/)
  (07-09-2026, «La ‘Paz Total’ dejó una factura…») es adversa al gobierno
  saliente con voz propia, pero se apoya en cifras de la Consejería de Paz y no
  casa con la expresión regular: no se suma.

## 5 bis. Cobertura de la Agencia para la Infraestructura del Meta (tensión, no orientación)

No entra en la cuenta del eje. Se anota por la línea de contratación pública
de la ficha: el CONTRATO 706 DE 2025 de la Agencia para la Infraestructura del
Meta (AIM) con Grupo La Independencia S.A.S. ($90.000.000, «servicios de
información (hablada; escrita y virtual)») tenía plazo del 18 al 30-12-2025
(SECOP II). En la ventana, 23 piezas nombran a la AIM en el cuerpo; **nueve se
publicaron entre el 23 y el 26-12-2025**, dentro de ese plazo, todas sobre
obras de la AIM y ninguna con rótulo de patrocinio:
[48699](https://www.viveelmeta.com/nueva-torre-del-hospital-de-villavicencio-avanza-583-y-proyectan-otra-para-hospitalizacion-48699/),
[48702](https://www.viveelmeta.com/la-avenida-del-llano-se-alista-para-una-transformacion-urbana-sin-precedentes-en-villavicencio-48702/),
[48710](https://www.viveelmeta.com/nuevo-corredor-humea-la-embajada-acercara-la-region-del-rio-meta-a-villavicencio-48710/),
[48712](https://www.viveelmeta.com/destinan-7-800-millones-para-renovar-la-escuela-gabriela-mistral-en-lejanias-48712/),
[48732](https://www.viveelmeta.com/a-buen-ritmo-avanza-la-via-que-unira-a-san-carlos-de-guaroa-con-altamira-en-puerto-lopez-48732/),
[48735](https://www.viveelmeta.com/la-recuperacion-de-la-via-a-cubarral-comienza-a-saldar-una-deuda-historica-con-el-ariari-48735/),
[48738](https://www.viveelmeta.com/lista-para-inaugurar-la-via-el-rosal-nuevo-eje-de-la-movilidad-rural-en-el-sur-del-meta-48738/)
(«entidad que ha sido garante»),
[48741](https://www.viveelmeta.com/mas-de-4-kilometros-pavimentados-impulsan-la-historica-via-uribe-papamene-en-el-sur-del-meta-48741/)
y
[48743](https://www.viveelmeta.com/intervencion-estructural-atendera-danos-por-sismos-en-colegio-de-san-juanito-meta-48743/).
**Que sean la prestación contratada no consta**: es una coincidencia de fechas,
y se escribe como tal. Ninguna de las nueve menciona el contrato del medio con
la AIM.

## 6. Tabla completa del barrido (224 piezas)

«Voz»: «casa (sin firma)» cuando el `author` es «viveelmeta.com».

| Lado | Fecha | Pieza | Titular | Voz | Clasificación |
|---|---|---|---|---|---|
| antes | 2025-10-20 | [47867](https://www.viveelmeta.com/exfuncionario-de-harman-le-recordo-su-pasado-con-el-acueducto-dejo-perder-17-000-millones-caradura-47867/) | Exfuncionario de Harman le recordó su pasado con el acueducto: "Dejó perder $17.000 millones. Caradura" | casa (sin firma) | F |
| antes | 2025-10-20 | [47876](https://www.viveelmeta.com/aplastante-derrota-de-los-partidos-progresistas-en-la-eleccion-del-consejo-de-juventud-de-villavicencio-47876/) | Aplastante derrota de los partidos progresistas en la elección del Consejo de Juventud de Villavicencio | casa (sin firma) | **D** · titular y entradilla propios: «Aplastante derrota de los partidos progresistas» (elección local de juventud) |
| antes | 2025-10-21 | [47896](https://www.viveelmeta.com/caso-cerrado-alvaro-uribe-fue-declarado-inocente-y-absuelto-de-todos-los-cargos-47896/) | Caso cerrado: Álvaro Uribe fue declarado inocente y absuelto de todos los cargos | casa (sin firma) | A (límite) · «Caso cerrado» sobre un fallo judicial |
| antes | 2025-10-22 | [47904](https://www.viveelmeta.com/petro-anuncia-movilizacion-en-bogota-tras-absolucion-de-alvaro-uribe-vamos-por-el-poder-constituyente-47904/) | Petro anuncia movilización en Bogotá tras absolución de Uribe: “Vamos por el Poder Constituyente” | casa (sin firma) | F |
| antes | 2025-10-24 | [47944](https://www.viveelmeta.com/26x6158-debi-dedicarme-a-las-matematicas-las-cuentas-locas-de-petro-que-desataron-burlas-en-redes-47944/) | “26x6=15,8. Debí dedicarme a las matemáticas”: las cuentas locas de Petro que desataron burlas en redes | casa (sin firma) | F |
| antes | 2025-10-26 | [47958](https://www.viveelmeta.com/la-sombra-de-las-viejas-practicas-de-clientelismo-y-politiqueria-en-la-ant-de-felipe-harman-47958/) | La sombra de las viejas prácticas de clientelismo y politiquería en la ANT de Felipe Harman | casa (sin firma) | F |
| antes | 2025-10-28 | [47984](https://www.viveelmeta.com/alcaldia-de-villavicencio-avanza-en-la-recuperacion-de-obras-que-felipe-harman-dejo-a-medias-47984/) | Alcaldía de Villavicencio avanza en la recuperación de obras que Felipe Harman dejó a medias | casa (sin firma) | F |
| antes | 2025-10-30 | [48036](https://www.viveelmeta.com/gustavo-petro-quedo-en-la-cola-de-ranking-que-mide-a-los-presidentes-sudamericanos-48036/) | Gustavo Petro quedó en la cola de ranking que mide a los presidentes sudamericanos | casa (sin firma) | F |
| antes | 2025-11-04 | [48077](https://www.viveelmeta.com/villavicencio-crece-sin-apoyo-del-gobierno-nacional-alexander-baquero-en-foro-de-semana-48077/) | "Villavicencio crece sin apoyo del Gobierno nacional": Alexander Baquero en foro de Semana | casa (sin firma) | F |
| antes | 2025-11-05 | [48084](https://www.viveelmeta.com/la-via-al-llano-requiere-un-gerente-coviandina-cuestiona-al-gobierno-nacional-por-falta-de-gestion-48084/) | “La vía al Llano requiere un gerente”: Coviandina cuestiona al Gobierno nacional por falta de gestión | casa (sin firma) | F |
| antes | 2025-11-05 | [48088](https://www.viveelmeta.com/piden-a-la-red-social-x-suspender-la-cuenta-de-petro-por-ingreso-a-la-lista-clinton-48088/) | Piden a la red social X suspender la cuenta de Petro por ingreso a la "Lista Clinton" | casa (sin firma) | F |
| antes | 2025-11-07 | [48119](https://www.viveelmeta.com/del-amor-al-odio-daniel-quintero-afirmo-que-el-gobierno-de-petro-ha-sido-muy-flojo-48119/) | ¿Del amor al odio? Daniel Quintero afirmó que el gobierno de Petro ha sido "muy flojo" | casa (sin firma) | F |
| antes | 2025-11-08 | [48140](https://www.viveelmeta.com/acusan-a-felipe-harman-de-usar-la-agencia-nacional-de-tierras-para-hacer-politica-en-el-cesar-48140/) | Acusan a Felipe Harman de usar la Agencia Nacional de Tierras para hacer política en el Cesar | casa (sin firma) | A |
| antes | 2025-11-11 | [48176](https://www.viveelmeta.com/juan-sin-miedo-exige-respetar-plazos-para-definir-candidato-unico-de-la-fuerza-de-las-regiones-48176/) | ‘Juan Sin Miedo’ exige respetar plazos para definir candidato único de La Fuerza de las Regiones | casa (sin firma) | A |
| antes | 2025-11-12 | [48193](https://www.viveelmeta.com/en-su-regreso-a-la-politica-ricardo-jaramillo-buscar-desmarcarse-de-felipe-harman-48193/) | En su regreso a la política, Ricardo Jaramillo se lava las manos por haber respaldado a Felipe Harman | casa (sin firma) | N · política local |
| antes | 2025-11-13 | [48202](https://www.viveelmeta.com/alexander-baquero-culpa-al-gobierno-de-petro-por-la-crisis-del-gas-no-comparto-su-decision-48202/) | Alexander Baquero culpa al Gobierno de Petro por la crisis del gas: "No comparto su decisión" | casa (sin firma) | F |
| antes | 2025-11-13 | [48211](https://www.viveelmeta.com/yo-soy-mas-borracha-que-el-la-respuesta-de-andrea-petro-por-criticas-a-su-papa-48211/) | "Yo soy más borracha que él": la respuesta de Andrea Petro por críticas a su papá | casa (sin firma) | F |
| antes | 2025-11-14 | [48232](https://www.viveelmeta.com/lo-que-mata-no-es-la-edad-sino-el-arma-en-si-mindefensa-48232/) | “Lo que mata no es la edad sino el arma”: Gobierno justifica bombardeo en zona de reclutamiento infantil | casa (sin firma) | F |
| antes | 2025-11-18 | [48240](https://www.viveelmeta.com/van-15-menores-asesinados-en-bombardeos-ordenados-por-petro-confirma-la-defensoria-del-pueblo-48240/) | Van 15 menores asesinados en bombardeos ordenados por Petro, confirma la Defensoría del Pueblo | casa (sin firma) | F |
| antes | 2025-11-18 | [48251](https://www.viveelmeta.com/abelardo-de-la-espriella-el-unico-que-podria-tumbar-a-la-izquierda-del-poder-segun-encuesta-del-cnc-48251/) | Abelardo de la Espriella, el único que podría tumbar a la izquierda del poder según encuesta del CNC | casa (sin firma) | **D** · voz propia: De la Espriella «se perfila como la figura con mayor capacidad de tumbar a la izquierda del poder» |
| antes | 2025-11-21 | [48304](https://www.viveelmeta.com/procuraduria-frena-movida-de-felipe-harman-para-concentrar-en-la-ant-las-decisiones-sobre-tierras-48304/) | Procuraduría frena movida de Felipe Harman para concentrar en la ANT las decisiones sobre tierras | casa (sin firma) | F |
| antes | 2025-11-24 | [48335](https://www.viveelmeta.com/las-explosivas-revelaciones-que-vinculan-a-la-campana-petro-presidente-con-disidencias-de-las-farc-48335/) | Las explosivas revelaciones que vinculan a la campaña Petro Presidente con disidencias de las Farc | casa (sin firma) | F |
| antes | 2025-11-25 | [48342](https://www.viveelmeta.com/ant-de-felipe-harman-adquirio-predio-que-no-sirve-para-proyectos-campesinos-denuncia-la-contraloria-48342/) | ANT de Felipe Harman adquirió predio que no sirve para proyectos campesinos, denuncia la Contraloría | casa (sin firma) | F |
| antes | 2025-11-27 | [48392](https://www.viveelmeta.com/petro-fue-obligado-a-disculparse-por-frase-machista-sobre-el-clitoris-y-el-cerebro-de-las-mujeres-48392/) | Petro fue obligado a disculparse por frase machista sobre el “clítoris y el cerebro” de las mujeres | casa (sin firma) | F |
| antes | 2025-11-27 | [48396](https://www.viveelmeta.com/cne-impone-historica-sancion-a-la-campana-petro-presidente-por-violar-topes-y-recibir-aportes-prohibidos-48396/) | CNE impone histórica sanción a la campaña Petro Presidente por violar topes y recibir aportes prohibidos | casa (sin firma) | F |
| antes | 2025-12-02 | [48450](https://www.viveelmeta.com/el-repertorio-que-tocaran-silvestre-dangond-y-juancho-de-la-espriella-este-fin-de-semana-en-villavicencio-48450/) | El repertorio que tocarán Silvestre Dangond y Juancho de la Espriella este fin de semana en Villavicencio | casa (sin firma) | A |
| antes | 2025-12-04 | [48478](https://www.viveelmeta.com/alexander-baquero-aclara-que-el-paro-taxista-fue-contra-petro-y-no-dirigido-a-su-administracion-48478/) | Alexander Baquero aclara que el paro taxista fue contra Petro y no dirigido a su administración | casa (sin firma) | F |
| antes | 2025-12-09 | [48527](https://www.viveelmeta.com/denuncian-juego-sucio-para-incluir-a-manguito-2-0-en-lista-del-pacto-historico-a-la-camara-por-el-meta-48527/) | Denuncian juego sucio para incluir a 'Manguito 2.0' en lista del Pacto Histórico a la Cámara por el Meta | casa (sin firma) | A |
| antes | 2025-12-09 | [48537](https://www.viveelmeta.com/acusan-a-harman-de-usar-la-ant-para-favorecer-a-circulos-politicos-en-puerto-lopez-48537/) | Acusan a Harman de usar la ANT para favorecer a círculos políticos en Puerto López | casa (sin firma) | F |
| antes | 2025-12-10 | [48540](https://www.viveelmeta.com/tras-16-meses-de-protestas-comunidades-de-villavicencio-logran-traslado-del-peaje-la-libertad-48540/) | Tras 16 meses de protestas, comunidades de Villavicencio logran traslado del peaje La Libertad | casa (sin firma) | F |
| antes | 2025-12-13 | [48588](https://www.viveelmeta.com/cne-estudia-demanda-para-sacar-a-manguito-2-0-de-la-lista-del-pacto-historico-a-la-camara-por-el-meta-48588/) | CNE estudia demanda para sacar a 'Manguito 2.0' de la lista del Pacto Histórico a la Cámara por el Meta | casa (sin firma) | A |
| antes | 2025-12-15 | [48600](https://www.viveelmeta.com/juan-sin-miedo-anuncia-respaldo-a-abelardo-de-la-espriella-es-un-clamor-ciudadano-48600/) | 'Juan Sin Miedo' anuncia respaldo a Abelardo de la Espriella: "Es un clamor ciudadano" | casa (sin firma) | A |
| antes | 2025-12-18 | [48648](https://www.viveelmeta.com/ant-de-felipe-harman-pago-16-000-millones-por-predio-que-no-figura-a-nombre-del-estado-advierte-contraloria-48648/) | ANT de Felipe Harman pagó $16.000 millones por predio que no figura a nombre del Estado, advierte Contraloría | casa (sin firma) | F |
| antes | 2025-12-18 | [48656](https://www.viveelmeta.com/envian-a-prision-a-dos-exministros-de-petro-por-escandalo-de-contratos-para-comprar-congresistas-48656/) | Envían a prisión a dos exministros de Petro por escándalo de contratos para comprar congresistas | casa (sin firma) | F |
| antes | 2025-12-24 | [48720](https://www.viveelmeta.com/sandoval-manguito-2-0-no-dudaria-mucho-como-candidato-a-la-camara-cne-estudia-expulsion-48720/) | Sandoval 'Manguito 2.0' no dudaría mucho como candidato a la Cámara: CNE estudia expulsión | casa (sin firma) | A |
| antes | 2025-12-26 | [48749](https://www.viveelmeta.com/petrismo-inscribe-comite-promotor-de-la-asamblea-nacional-constituyente-que-busca-realmente-48749/) | Petrismo inscribe comité promotor de la Asamblea Nacional Constituyente: ¿Qué busca realmente? | casa (sin firma) | F · constituyente del gobierno en ejercicio |
| antes | 2025-12-29 | [48769](https://www.viveelmeta.com/petro-se-quiere-atornillar-en-el-poder-de-la-espriella-propone-juicio-politico-contra-el-presidente-48769/) | “Petro se quiere atornillar en el poder”: De la Espriella propone juicio político contra el presidente | casa (sin firma) | A |
| antes | 2026-01-05 | [48796](https://www.viveelmeta.com/alexander-baquero-advierte-que-el-aumento-del-salario-minimo-presionara-las-finanzas-municipales-48796/) | Alexander Baquero advierte que el aumento del salario mínimo presionará las finanzas municipales | casa (sin firma) | A |
| antes | 2026-01-06 | [48809](https://www.viveelmeta.com/petro-convoca-manifestaciones-ante-amenazas-de-intervencion-de-estados-unidos-en-colombia-48809/) | Petro convoca manifestaciones ante amenazas de intervención de Estados Unidos en Colombia | casa (sin firma) | F |
| antes | 2026-01-08 | [48843](https://www.viveelmeta.com/de-harman-a-el-tigre-el-salto-politico-con-el-que-ximena-calderon-busca-votos-en-el-meta-48843/) | De Harman a ‘El Tigre’, el salto político con el que Ximena Calderón busca votos en el Meta | casa (sin firma) | N (límite) · política local: desmiente que una aspirante sea candidata de De la Espriella, a quien llama «hoy fenómeno político» |
| antes | 2026-01-13 | [48876](https://www.viveelmeta.com/chaqueta-de-48-millones-contradice-el-discurso-de-petro-sobre-austeridad-y-consumo-nacional-48876/) | Chaqueta de $48 millones contradice el discurso de Petro sobre austeridad y consumo nacional | casa (sin firma) | F |
| antes | 2026-01-13 | [48897](https://www.viveelmeta.com/fuera-manguito-petristas-rechazan-candidatura-de-jose-manuel-sandoval-a-la-camara-por-el-meta-48897/) | "Fuera, Manguito": petristas rechazan candidatura de José Manuel Sandoval a la Cámara por el Meta | casa (sin firma) | A |
| antes | 2026-01-15 | [48918](https://www.viveelmeta.com/desfavorabilidad-de-petro-crece-entre-la-poblacion-joven-segun-encuesta-48918/) | Desfavorabilidad de Petro crece entre la población joven, según encuesta | casa (sin firma) | F |
| antes | 2026-01-17 | [48958](https://www.viveelmeta.com/procuraduria-investiga-uso-de-recursos-publicos-para-defensa-de-petro-por-la-lista-clinton-48958/) | Procuraduría investiga uso de recursos públicos para defensa de Petro por la Lista Clinton | casa (sin firma) | F |
| antes | 2026-01-20 | [48985](https://www.viveelmeta.com/desde-el-meta-alertan-sobre-efectos-adversos-de-la-emergencia-economica-decretada-por-petro-48985/) | Desde el Meta alertan sobre efectos adversos de la Emergencia Económica decretada por Petro | casa (sin firma) | F |
| antes | 2026-01-20 | [48989](https://www.viveelmeta.com/petro-sugiere-que-afectaria-sueldos-de-la-fuerza-publica-si-se-cae-la-emergencia-economica-puede-hacerlo-48989/) | Petro sugiere que afectaría sueldos de la fuerza pública si se cae la Emergencia Económica: ¿puede hacerlo? | casa (sin firma) | A |
| antes | 2026-01-21 | [49014](https://www.viveelmeta.com/presidente-de-la-corte-constitucional-pide-frenar-provisionalmente-la-emergencia-economica-de-petro-49014/) | Presidente de la Corte Constitucional pide frenar provisionalmente la Emergencia Económica de Petro | casa (sin firma) | F |
| antes | 2026-01-23 | [49034](https://www.viveelmeta.com/alvaro-uribe-velez-y-paloma-valencia-haran-una-gira-politica-por-municipios-del-meta-49034/) | Álvaro Uribe Vélez y Paloma Valencia harán una gira política por municipios del Meta | casa (sin firma) | A |
| antes | 2026-01-26 | [49064](https://www.viveelmeta.com/paloma-valencia-propone-un-nuevo-sistema-pensional-pensado-para-trabajadores-informales-49064/) | Paloma Valencia propone un nuevo sistema pensional pensado para trabajadores informales | casa (sin firma) | A |
| antes | 2026-01-27 | [49076](https://www.viveelmeta.com/otorgan-visa-de-solo-cinco-dias-a-petro-para-reunion-con-trump-en-estados-unidos-49076/) | Otorgan Visa de solo cinco días a Petro para reunión con Trump en Estados Unidos | casa (sin firma) | F |
| antes | 2026-01-28 | [49090](https://www.viveelmeta.com/rafaela-cortes-llama-a-petro-y-su-ministra-de-transporte-a-conocer-por-tierra-la-via-al-llano-49090/) | Rafaela Cortés llama a Petro y su ministra de Transporte a conocer por tierra la vía al Llano | casa (sin firma) | F |
| antes | 2026-01-29 | [49114](https://www.viveelmeta.com/la-iglesia-catolica-rechaza-comentarios-sexuales-de-petro-sobre-jesus-y-maria-magdalena-49114/) | La Iglesia Católica rechaza comentarios sexuales de Petro sobre Jesús y María Magdalena | casa (sin firma) | F |
| antes | 2026-02-02 | [49139](https://www.viveelmeta.com/fiscalia-asume-investigacion-por-denuncia-sobre-presunta-red-de-corrupcion-en-la-agencia-nacional-de-tierras-49139/) | Fiscalía asume investigación por denuncia sobre presunta red de corrupción en la Agencia Nacional de Tierras | casa (sin firma) | F |
| antes | 2026-02-03 | [49155](https://www.viveelmeta.com/darwin-castellanos-rechazo-comentarios-de-gustavo-petro-que-atentan-contra-la-fe-cristiana-49155/) | Darwin Castellanos rechazó comentarios de Gustavo Petro que atentan contra la fe cristiana | casa (sin firma) | F |
| antes | 2026-02-04 | [49165](https://www.viveelmeta.com/petro-le-prometio-a-trump-que-en-menos-de-dos-meses-capturaria-a-principales-capos-de-la-mafia-49165/) | Petro le prometió a Trump que en menos de dos meses capturaría a principales capos de la mafia | casa (sin firma) | F |
| antes | 2026-02-04 | [49169](https://www.viveelmeta.com/gobernadora-del-meta-denuncia-falta-de-dialogo-con-el-presidente-y-sus-ministros-la-comunicacion-es-cero-49169/) | Gobernadora del Meta denuncia falta de diálogo con el presidente y sus ministros: "la comunicación es cero" | casa (sin firma) | F |
| antes | 2026-02-06 | [49206](https://www.viveelmeta.com/presidente-petro-en-la-mira-de-la-procuraduria-por-posible-participacion-indebida-en-politica-49206/) | Presidente Petro, en la mira de la Procuraduría por posible participación indebida en política | casa (sin firma) | F |
| antes | 2026-02-09 | [49229](https://www.viveelmeta.com/salida-de-manguito-2-0-deja-al-pacto-historico-roto-y-con-lista-incompleta-a-la-camara-por-el-meta-49229/) | Salida de ‘Manguito 2.0’ deja al Pacto Histórico roto y con lista incompleta a la Cámara por el Meta | casa (sin firma) | A |
| antes | 2026-02-12 | [49277](https://www.viveelmeta.com/gobierno-petro-contrato-14-billones-antes-de-la-ley-de-garantias-advirtio-la-contraloria-49277/) | Gobierno Petro contrató $14 billones antes de la Ley de Garantías, advirtió la Contraloría | casa (sin firma) | F |
| antes | 2026-02-13 | [49283](https://www.viveelmeta.com/eln-declara-objetivo-militar-al-candidato-presidencial-abelardo-de-la-espriella-49283/) | ELN declara objetivo militar al candidato presidencial Abelardo De La Espriella | casa (sin firma) | A |
| antes | 2026-02-16 | [49319](https://www.viveelmeta.com/exministro-de-educacion-de-petro-califica-su-gobierno-como-el-mas-corrupto-en-la-historia-reciente-de-colombia-49319/) | Exministro de Educación de Petro califica su gobierno como el más corrupto en la historia reciente de Colombia | casa (sin firma) | F |
| antes | 2026-02-17 | [49332](https://www.viveelmeta.com/de-la-espriella-pide-mantener-incremento-del-salario-minimo-no-se-puede-decepcionar-asi-a-la-gente-49332/) | De la Espriella pide mantener incremento del salario mínimo: “No se puede decepcionar así a la gente” | casa (sin firma) | A |
| antes | 2026-02-18 | [49351](https://www.viveelmeta.com/divisiones-internas-dejan-en-el-limbo-la-credencial-del-pacto-historico-en-el-meta-49351/) | Divisiones internas dejan en el limbo la credencial del Pacto Histórico en el Meta | casa (sin firma) | A |
| antes | 2026-02-19 | [49368](https://www.viveelmeta.com/darwin-castellanos-culpa-al-gobierno-petro-por-muerte-de-nino-que-no-recibio-medicamentos-de-su-eps-49368/) | Darwin Castellanos culpa al gobierno Petro por muerte de niño que no recibió medicamentos de su EPS | casa (sin firma) | F |
| antes | 2026-02-19 | [49372](https://www.viveelmeta.com/gobierno-petro-gasto-63-billones-mas-de-lo-que-recibio-en-2025-revela-el-comite-de-regla-fiscal-49372/) | Gobierno Petro gastó $63 billones más de lo que recibió en 2025, revela el Comité de Regla Fiscal | casa (sin firma) | F |
| antes | 2026-02-23 | [49422](https://www.viveelmeta.com/indigenas-agredieron-a-un-periodista-durante-concentracion-del-pacto-historico-en-villavicencio-49422/) | Indígenas agredieron a un periodista durante concentración del Pacto Histórico en Villavicencio | casa (sin firma) | A |
| antes | 2026-02-28 | [49517](https://www.viveelmeta.com/gasolina-baja-500-desde-de-marzo-en-villavicencio-se-pagara-15-591-por-galon-49517/) | Gasolina baja $500 desde de marzo: en Villavicencio se pagará $15.591 por galón | casa (sin firma) | F |
| antes | 2026-03-05 | [49585](https://www.viveelmeta.com/llueven-criticas-a-petro-por-millonaria-financiacion-de-pelicula-en-la-que-aparecera-y-para-la-salud-no-hay-plata-49585/) | Llueven críticas a Petro por millonaria financiación de película en la que aparecerá: “Y para la salud no hay plata” | casa (sin firma) | F |
| antes | 2026-03-09 | [49617](https://www.viveelmeta.com/editorial-en-villavicencio-la-oposicion-critica-pero-no-logra-ganar-49617/) | Editorial / En Villavicencio la oposición critica, pero no logra ganar | Fernando Betancourt | **D** · editorial: elogia al sector del alcalde (Salvación Nacional, CD) y desacredita a la oposición del Pacto |
| antes | 2026-03-09 | [49621](https://www.viveelmeta.com/la-derecha-domina-en-el-meta-centro-democratico-lidera-votacion-y-el-pacto-historico-perdio-terreno-49621/) | La derecha domina en el Meta: Centro Democrático lidera votación y el Pacto Histórico perdió terreno | casa (sin firma) | A (límite) · resultado electoral con encuadre «la derecha domina» |
| antes | 2026-03-09 | [49625](https://www.viveelmeta.com/ximena-calderon-paso-sin-pena-ni-gloria-por-las-elecciones-legislativas-de-2026-49625/) | Ximena Calderón pasó 'sin pena ni gloria' por las elecciones legislativas de 2026 | casa (sin firma) | N · política local |
| antes | 2026-03-10 | [49647](https://www.viveelmeta.com/esto-es-lo-que-le-pide-juan-daniel-oviedo-a-paloma-valencia-para-ser-su-formula-vicepresidencial-49647/) | Esto es lo que le pide Juan Daniel Oviedo a Paloma Valencia para ser su fórmula vicepresidencial | casa (sin firma) | A |
| antes | 2026-03-11 | [49661](https://www.viveelmeta.com/proponen-que-un-senador-del-centro-democratico-renuncie-para-que-alvaro-uribe-llegue-al-congreso-49661/) | Proponen que un senador del Centro Democrático renuncie para que Álvaro Uribe llegue al Congreso | casa (sin firma) | A |
| antes | 2026-03-12 | [49680](https://www.viveelmeta.com/medios-estatales-favorecieron-a-la-izquierda-en-elecciones-legislativas-denuncia-la-moe-europea-49680/) | Medios estatales favorecieron a la izquierda en elecciones legislativas, denuncia la MOE Europea | casa (sin firma) | A |
| antes | 2026-03-16 | [49750](https://www.viveelmeta.com/abelardo-de-la-espriella-anuncia-plan-de-seguridad-para-recuperar-el-control-en-el-sur-del-meta-49750/) | Abelardo de la Espriella anuncia plan de seguridad para recuperar el control en el sur del Meta | casa (sin firma) | A |
| antes | 2026-03-17 | [49768](https://www.viveelmeta.com/el-exsenador-manguito-lidera-solicitud-para-declarar-persona-no-grata-a-ivan-cepeda-en-antioquia-49768/) | El exsenador ‘Manguito’ lidera solicitud para declarar persona no grata a Iván Cepeda en Antioquia | casa (sin firma) | A |
| antes | 2026-03-18 | [49772](https://www.viveelmeta.com/alvaro-uribe-acusa-a-ivan-cepeda-de-incitar-asesinatos-y-pide-frenar-la-toma-de-colombia-49772/) | Álvaro Uribe acusa a Iván Cepeda de incitar asesinatos y pide frenar la “toma de Colombia” | casa (sin firma) | A |
| antes | 2026-03-19 | [49806](https://www.viveelmeta.com/antioquia-le-cierra-la-puerta-a-ivan-cepeda-y-lo-declara-persona-no-grata-49806/) | Antioquia le cierra la puerta a Iván Cepeda y lo declara persona no grata | casa (sin firma) | A |
| antes | 2026-03-20 | [49822](https://www.viveelmeta.com/rafaela-cortes-advierte-a-petro-que-liquidar-eps-sin-transicion-pone-en-riesgo-a-millones-de-pacientes-49822/) | Rafaela Cortés advierte a Petro que liquidar EPS sin transición pone en riesgo a millones de pacientes | casa (sin firma) | F |
| antes | 2026-03-20 | [49825](https://www.viveelmeta.com/revelan-en-ee-uu-investigaciones-que-vincularian-a-petro-en-casos-de-narcotrafico-49825/) | Revelan en EE. UU. investigaciones que vincularían a Petro en casos de narcotráfico | casa (sin firma) | F |
| antes | 2026-03-24 | [49846](https://www.viveelmeta.com/petro-recomienda-comprar-vehiculos-electricos-ante-inminente-alza-en-el-precio-de-la-gasolina-49846/) | Petro recomienda comprar vehículos eléctricos ante inminente alza en el precio de la gasolina | casa (sin firma) | F |
| antes | 2026-03-25 | [49861](https://www.viveelmeta.com/accionistas-advierten-presunto-intento-del-gobierno-nacional-de-controlar-la-electrificadora-del-meta-49861/) | Accionistas advierten presunto intento del Gobierno nacional de controlar la Electrificadora del Meta | casa (sin firma) | F |
| antes | 2026-03-28 | [49907](https://www.viveelmeta.com/gobierno-petro-contrato-mas-de-31-billones-a-dedo-con-organizaciones-comunitarias-compra-de-votos-49907/) | Gobierno Petro contrató más de $31 billones a dedo con organizaciones comunitarias: ¿Compra de votos? | casa (sin firma) | F |
| antes | 2026-03-30 | [49915](https://www.viveelmeta.com/fiscalia-confirmo-que-calarca-seguia-delinquiendo-en-medio-de-los-dialogos-con-el-gobierno-petro-49915/) | Fiscalía confirmó que ‘Calarcá’ seguía delinquiendo en medio de los diálogos con el Gobierno Petro | casa (sin firma) | F |
| antes | 2026-04-06 | [49973](https://www.viveelmeta.com/el-regimen-de-petro-me-quiere-asesinar-abelardo-de-la-espriella-hablo-de-un-plan-para-aniquilarlo-49973/) | "El régimen de Petro me quiere asesinar": Abelardo de la Espriella habló de un plan para aniquilarlo | casa (sin firma) | A |
| antes | 2026-04-08 | [50013](https://www.viveelmeta.com/bukele-reta-a-petro-a-recibir-a-todos-los-presos-de-el-salvador-si-no-le-gusta-su-modelo-carcelario-50013/) | Bukele reta a Petro a recibir a todos los presos de El Salvador “si no le gusta” su modelo carcelario | casa (sin firma) | F |
| antes | 2026-04-09 | [50020](https://www.viveelmeta.com/nos-quedan-tres-meses-toca-gastar-petro-acepto-que-varios-ministerios-no-tienen-resultados-para-mostrar-50020/) | “Nos quedan tres meses, toca gastar”: Petro aceptó que varios ministerios no tienen resultados para mostrar | casa (sin firma) | F |
| antes | 2026-04-10 | [50035](https://www.viveelmeta.com/paloma-y-abelardo-derrotarian-con-amplia-ventaja-a-cepeda-en-segunda-vuelta-segun-atlas-intel-50035/) | Paloma y Abelardo derrotarían con amplia ventaja a Cepeda en segunda vuelta, según Atlas Intel | casa (sin firma) | A |
| antes | 2026-04-13 | [50069](https://www.viveelmeta.com/de-la-espriella-como-presidente-buscaria-llevar-a-petro-a-los-estrados-judiciales-no-puede-quedar-impune-50069/) | De la Espriella como presidente buscaría llevar a Petro a los estrados judiciales: “No puede quedar impune” | casa (sin firma) | A |
| antes | 2026-04-14 | [50087](https://www.viveelmeta.com/gobierno-petro-llega-a-su-final-con-el-71-de-promesas-de-campana-sin-cumplir-segun-informe-50087/) | Gobierno Petro llega a su final con el 71 % de promesas de campaña sin cumplir, según informe | casa (sin firma) | F |
| antes | 2026-04-16 | [50110](https://www.viveelmeta.com/alexander-baquero-culpa-al-gobierno-petro-por-crisis-de-seguridad-le-vale-huevo-todo-50110/) | Alexander Baquero culpa al Gobierno Petro por crisis de seguridad: "Le vale huevo todo" | casa (sin firma) | F |
| antes | 2026-04-20 | [50167](https://www.viveelmeta.com/expertos-critican-a-ivan-cepeda-por-no-asistir-a-debates-es-como-ir-a-un-mundial-y-no-jugar-los-partidos-50167/) | Expertos critican a Iván Cepeda por no asistir a debates: "Es como ir a un Mundial y no jugar los partidos" | casa (sin firma) | A |
| antes | 2026-04-21 | [50182](https://www.viveelmeta.com/oso-internacional-telemundo-desmiente-a-petro-por-video-con-el-que-ataco-al-presidente-de-ecuador-50182/) | Oso internacional: Telemundo desmiente a Petro por video con el que atacó al presidente de Ecuador | casa (sin firma) | F |
| antes | 2026-04-24 | [50234](https://www.viveelmeta.com/con-la-seguridad-como-bandera-paloma-valencia-plantea-militarizar-vias-en-el-meta-50234/) | Con la seguridad como bandera, Paloma Valencia plantea militarizar vías en el Meta | casa (sin firma) | A |
| antes | 2026-04-24 | [50244](https://www.viveelmeta.com/petro-lanza-ofensiva-publicitaria-urgente-tras-graves-denuncias-de-funcionaria-de-su-gobierno-50244/) | Petro lanza ofensiva publicitaria urgente tras graves denuncias de funcionaria de su Gobierno | casa (sin firma) | F |
| antes | 2026-04-27 | [50269](https://www.viveelmeta.com/milton-carreno-se-monta-en-la-campana-de-paloma-valencia-tras-diferencias-con-el-uribismo-50269/) | Milton Carreño se monta en la campaña de Paloma Valencia tras diferencias con el uribismo | casa (sin firma) | A |
| antes | 2026-04-28 | [50289](https://www.viveelmeta.com/el-meta-permanece-en-alerta-maxima-ante-riesgo-de-atentados-por-elecciones-presidenciales-50289/) | El Meta permanece en alerta máxima ante riesgo de atentados por elecciones presidenciales | casa (sin firma) | A |
| antes | 2026-04-29 | [50297](https://www.viveelmeta.com/uribe-se-despacho-contra-petro-y-cepeda-por-acusacion-sobre-falsos-positivos-mienten-cobardemente-50297/) | Uribe se despachó contra Petro y Cepeda por acusación sobre falsos positivos: "mienten cobardemente" | casa (sin firma) | A |
| antes | 2026-04-29 | [50306](https://www.viveelmeta.com/denuncian-a-dos-directivos-de-la-ungrd-por-acoso-a-contratistas-pretendia-llevarlas-a-la-cama-50306/) | Denuncian a dos directivos de la UNGRD por acoso a contratistas: "pretendía llevarlas a la cama" | casa (sin firma) | F |
| antes | 2026-04-30 | [50316](https://www.viveelmeta.com/presidente-de-ecuador-acusa-a-petro-de-impulsar-incursion-guerrillera-en-su-territorio-50316/) | Presidente de Ecuador acusa a Petro de impulsar incursión guerrillera en su territorio | casa (sin firma) | F |
| antes | 2026-05-04 | [50339](https://www.viveelmeta.com/paloma-valencia-propone-que-el-estado-asuma-el-soat-de-motos-hasta-250-cc-en-estratos-bajos-50339/) | Paloma Valencia propone que el Estado asuma el SOAT de motos hasta 250 cc en estratos bajos | casa (sin firma) | A |
| antes | 2026-05-04 | [50350](https://www.viveelmeta.com/estudio-revela-que-el-gobierno-petro-registra-la-mayor-presion-delictiva-de-los-ultimos-20-anos-50350/) | Estudio revela que el Gobierno Petro registra la mayor presión delictiva de los últimos 20 años | casa (sin firma) | F |
| antes | 2026-05-05 | [50368](https://www.viveelmeta.com/policia-confirma-que-felipe-harman-si-pago-cinco-dias-de-arresto-por-no-acatar-un-fallo-de-tutela-50368/) | Policía confirma que Felipe Harman sí pagó cinco días de arresto por no acatar un fallo de tutela | casa (sin firma) | A |
| antes | 2026-05-07 | [50393](https://www.viveelmeta.com/petro-tendra-que-retractarse-publicamente-por-llamar-munecas-de-la-mafia-a-mujeres-periodistas-50393/) | Petro tendrá que retractarse públicamente por llamar 'muñecas de la mafia' a mujeres periodistas | casa (sin firma) | F |
| antes | 2026-05-07 | [50401](https://www.viveelmeta.com/ivan-cepeda-acepto-que-hay-corrupcion-en-gobierno-petro-no-ha-sido-perfecto-hay-que-reconocerlo-50401/) | Iván Cepeda aceptó que hay corrupción en el gobierno Petro: "No ha sido perfecto, hay que reconocerlo" | casa (sin firma) | A |
| antes | 2026-05-08 | [50417](https://www.viveelmeta.com/partido-conservador-en-villavicencio-rechazo-versiones-sobre-adhesion-a-ivan-cepeda-estamos-con-paloma-50417/) | Partido Conservador en Villavicencio rechazó versiones sobre adhesión a Iván Cepeda: "Estamos con Paloma" | casa (sin firma) | A |
| antes | 2026-05-11 | [50439](https://www.viveelmeta.com/a-20-dias-de-las-elecciones-de-la-espriella-se-pone-arriba-de-ivan-cepeda-en-polymarket-50439/) | A 20 días de elecciones, De la Espriella se pone arriba de Iván Cepeda en Polymarket | casa (sin firma) | A |
| antes | 2026-05-15 | [50484](https://www.viveelmeta.com/moe-advierte-que-peticion-de-petro-sobre-software-de-escrutinio-afectaria-la-transparencia-electoral-50484/) | MOE advierte que petición de Petro sobre software de escrutinio afectaría la transparencia electoral | casa (sin firma) | F |
| antes | 2026-05-16 | [50487](https://www.viveelmeta.com/rogers-devia-lideraba-campana-de-abelardo-de-la-espriella-en-cubarral-estuvo-recogiendo-publicidad-en-villavicencio-50487/) | Rogers Devia lideraba campaña de Abelardo de la Espriella en Cubarral: “Estuvo recogiendo publicidad en Villavicencio” | casa (sin firma) | A |
| antes | 2026-05-20 | [50522](https://www.viveelmeta.com/cne-suspende-a-atlas-intel-encuestadora-que-dio-al-tigre-como-proximo-presidente-de-colombia-50522/) | CNE suspende a Atlas Intel, encuestadora que dio al 'Tigre' como próximo presidente de Colombia | casa (sin firma) | **D** · voz propia: magistrada «aparentemente muy cercana al Pacto Histórico» suspende a la encuestadora favorable al Tigre |
| antes | 2026-05-22 | [50551](https://www.viveelmeta.com/paloma-valencia-y-abelardo-de-la-espriella-libran-disputa-que-podria-terminar-beneficiando-a-ivan-cepeda-50551/) | Paloma Valencia y Abelardo de la Espriella libran disputa que podría terminar beneficiando a Iván Cepeda | casa (sin firma) | **C** · crítica propia a De la Espriella («discurso radical»), desde la orilla de Paloma Valencia |
| antes | 2026-05-26 | [50588](https://www.viveelmeta.com/denuncian-a-petro-por-presunta-participacion-en-politica-tras-mensajes-sobre-ivan-cepeda-50588/) | Denuncian a Petro por presunta participación en política tras mensajes sobre Iván Cepeda | casa (sin firma) | A |
| antes | 2026-05-27 | [50615](https://www.viveelmeta.com/desarmemos-nuestras-palabras-el-mensaje-de-la-iglesia-a-los-candidatos-presidenciales-50615/) | “Desarmemos nuestras palabras”: el mensaje de la Iglesia a los candidatos presidenciales | casa (sin firma) | A |
| antes | 2026-05-28 | [50624](https://www.viveelmeta.com/westcol-cancelo-transmision-junto-a-paloma-valencia-por-relacion-con-influenciadores-cuestionados-50624/) | WestCol canceló transmisión junto a Paloma Valencia por relación con influenciadores cuestionados | casa (sin firma) | A |
| antes | 2026-05-28 | [50634](https://www.viveelmeta.com/mujer-que-camino-de-la-mano-con-petro-en-panama-se-enriquecio-extranamente-revela-investigacion-50634/) | Mujer que caminó de la mano con Petro en Panamá se enriqueció extrañamente, revela investigación | casa (sin firma) | F |
| antes | 2026-06-02 | [50678](https://www.viveelmeta.com/petro-esta-dando-paso-tras-paso-para-robarse-las-elecciones-abelardo-de-la-espriella-50678/) | “Petro está dando paso tras paso para robarse las elecciones”: Abelardo de la Espriella | casa (sin firma) | A |
| antes | 2026-06-03 | [50699](https://www.viveelmeta.com/donald-trump-se-puso-la-camiseta-para-respaldar-a-el-tigre-en-la-segunda-vuelta-presidencial-50699/) | Donald Trump se puso la camiseta para respaldar a 'El Tigre' en la segunda vuelta presidencial | casa (sin firma) | A |
| antes | 2026-06-03 | [50703](https://www.viveelmeta.com/registraduria-desmonto-una-a-una-las-acusaciones-de-petro-sobre-fraude-electoral-no-es-cierto-50703/) | Registraduría desmontó una a una las acusaciones de Petro sobre fraude electoral :"No es cierto" | casa (sin firma) | F |
| antes | 2026-06-05 | [50734](https://www.viveelmeta.com/proyeccion-de-la-firma-guarumo-pone-a-el-tigre-como-presidente-en-todos-los-escenarios-posibles-50734/) | Proyección de la firma Guarumo pone a 'El Tigre' como presidente en todos los escenarios posibles | casa (sin firma) | A |
| antes | 2026-06-08 | [50756](https://www.viveelmeta.com/mas-constituyente-y-un-discurso-mas-radical-lo-que-revelan-las-433-paginas-del-programa-de-gobierno-de-ivan-cepeda-50756/) | Más constituyente y un discurso más radical: lo que revelan las 433 páginas del programa de gobierno de Iván Cepeda | casa (sin firma) | **D** · análisis propio adverso del programa de Cepeda, sin equivalente para De la Espriella |
| antes | 2026-06-09 | [50770](https://www.viveelmeta.com/esto-se-hace-es-con-dinero-lider-de-campana-de-cepeda-admite-uso-de-recursos-para-movilizar-votantes-50770/) | “Esto se hace es con dinero”: líder de campaña de Cepeda admite uso de recursos para movilizar votantes | casa (sin firma) | A |
| antes | 2026-06-09 | [50775](https://www.viveelmeta.com/bomba-politica-orden-judicial-le-prohibe-al-tigre-utilizar-la-bandera-y-la-frase-firmes-por-la-patria-50775/) | ¡Bomba política! Orden judicial le prohíbe al 'Tigre' utilizar la bandera y la frase "Firmes por la Patria" | casa (sin firma) | **D** · voz propia: «¡Bomba política!» y candidatura «que sigue fortaleciéndose» |
| antes | 2026-06-10 | [50787](https://www.viveelmeta.com/la-suspension-de-petro-es-un-autoatentado-legislativo-abelardo-de-la-espriella-50787/) | “La suspensión de Petro es un autoatentado legislativo”: Abelardo de la Espriella | casa (sin firma) | A |
| antes | 2026-06-11 | [50803](https://www.viveelmeta.com/tonterias-de-perdedores-aliado-de-trump-desestima-supuesta-inhabilidad-por-nacionalidad-del-tigre-50803/) | "Tonterías de perdedores": aliado de Trump desestima supuesta inhabilidad por nacionalidad del 'Tigre' | casa (sin firma) | A |
| antes | 2026-06-11 | [50807](https://www.viveelmeta.com/capturan-por-delitos-ambientales-a-familiares-de-william-aljure-congresista-petrista-del-meta-50807/) | Capturan por delitos ambientales a familiares de William Aljure, congresista petrista del Meta | casa (sin firma) | F |
| antes | 2026-06-12 | [50818](https://www.viveelmeta.com/tener-tres-nacionalidades-no-impide-que-abelardo-de-la-espriella-sea-presidente-aseguran-expertos-50818/) | Abelardo de la Espriella sí puede ser presidente aunque tenga tres nacionalidades, aseguran expertos | casa (sin firma) | A |
| antes | 2026-06-12 | [50823](https://www.viveelmeta.com/ivan-cepeda-enfrenta-criticas-por-el-presunto-origen-de-millonaria-suma-invertida-en-pauta-digital-50823/) | Iván Cepeda enfrenta críticas por el presunto origen de millonaria suma invertida en pauta digital | casa (sin firma) | A |
| antes | 2026-06-13 | [50833](https://www.viveelmeta.com/cepeda-propone-que-colombia-sea-sede-de-un-mundial-de-futbol-y-estallan-las-redes-va-pa-personero-50833/) | Cepeda propone que Colombia sea sede de un mundial de fútbol y estallan las redes: “Va pa personero” | casa (sin firma) | **D** · entradilla propia: «la cuestionada gestión de Gustavo Petro», burla a Cepeda |
| antes | 2026-06-17 | [50856](https://www.viveelmeta.com/lideres-petristas-advierten-que-si-ivan-cepeda-pierde-las-elecciones-se-incendiara-el-pais-50856/) | Líderes petristas advierten que si Iván Cepeda pierde las elecciones se incendiará el país | casa (sin firma) | A |
| antes | 2026-06-17 | [50868](https://www.viveelmeta.com/un-fracaso-mas-del-gobierno-petro-el-ministerio-de-la-igualdad-desapareceria-en-pocos-dias-50868/) | Un fracaso más del gobierno Petro: el Ministerio de la Igualdad desaparecería en pocos días | casa (sin firma) | F · voz propia («Un fracaso más del gobierno Petro»), gobierno en ejercicio |
| antes | 2026-06-18 | [50878](https://www.viveelmeta.com/alcalde-de-villavicencio-cuestiono-visita-de-petro-en-plena-campana-electoral-de-el-no-hemos-recibido-nada-50878/) | Alcalde de Villavicencio cuestionó visita de Petro en plena campaña: “De él no hemos recibido nada” | casa (sin firma) | F |
| antes | 2026-06-19 | [50890](https://www.viveelmeta.com/cero-y-van-dos-fajardo-no-se-decide-por-un-candidato-y-deja-a-un-millon-de-electores-sueltos-50890/) | Cero y van dos: Fajardo no se decide por un candidato y deja a un millón de electores sueltos | casa (sin firma) | A |
| antes | 2026-06-19 | [50899](https://www.viveelmeta.com/exfuncionario-de-petro-lo-considera-nocivo-para-la-campana-de-cepeda-que-se-dedique-a-otras-cosas-50899/) | Exfuncionario de Petro lo considera nocivo para la campaña de Cepeda: "Que se dedique a otras cosas" | casa (sin firma) | A |
| antes | 2026-06-22 | [50920](https://www.viveelmeta.com/peticiones-de-petro-y-cepeda-sobre-reconteo-de-votos-no-proceden-en-esta-etapa-advierte-el-cne-50920/) | Peticiones de Petro y Cepeda sobre reconteo de votos no proceden en esta etapa, advierte el CNE | casa (sin firma) | A |
| antes | 2026-06-23 | [50929](https://www.viveelmeta.com/exgobernador-juan-guillermo-zuluaga-suena-como-ministro-de-defensa-de-abelardo-de-la-espriella-50929/) | Exgobernador Juan Guillermo Zuluaga suena como ministro de Defensa de Abelardo de la Espriella | casa (sin firma) | A |
| antes | 2026-06-23 | [50932](https://www.viveelmeta.com/ivan-cepeda-habria-obtenido-mas-de-360-000-votos-fusil-segun-el-instituto-de-ciencia-politica-50932/) | Iván Cepeda habría obtenido más de 360.000 'votos fusil', según el Instituto de Ciencia Política | casa (sin firma) | A |
| antes | 2026-06-24 | [50941](https://www.viveelmeta.com/juguemos-a-los-congelados-el-pacto-del-gobierno-petro-con-el-clan-del-golfo-que-permitio-su-expansion-50941/) | “Juguemos a los congelados”: el pacto del gobierno Petro con el Clan del Golfo que permitió su expansión | casa (sin firma) | F |
| antes | 2026-06-24 | [50945](https://www.viveelmeta.com/a-poco-de-concluir-los-escrutinios-ivan-cepeda-reconoce-su-derrota-en-segunda-vuelta-presidencial-50945/) | A poco de concluir los escrutinios, Iván Cepeda reconoce su derrota en segunda vuelta presidencial | casa (sin firma) | A |
| antes | 2026-06-24 | [50952](https://www.viveelmeta.com/ivan-cepeda-perdio-400-votos-y-de-la-espriella-recupero-624-tras-los-escrutinios-nacionales-50952/) | Iván Cepeda perdió 400 votos y De la Espriella recuperó 624 tras los escrutinios nacionales | casa (sin firma) | A |
| antes | 2026-06-25 | [50963](https://www.viveelmeta.com/presidente-electo-lanza-ultimatum-a-grupos-criminales-tienen-un-mes-para-organizar-su-sometimiento-al-estado-50963/) | Presidente electo lanza ultimátum a grupos criminales: tienen un mes para organizar su sometimiento al Estado | casa (sin firma) | A |
| antes | 2026-06-30 | [50993](https://www.viveelmeta.com/alcalde-de-villavicencio-buscara-viabilizar-megaproyecto-de-seguridad-con-el-nuevo-gobierno-nacional-50993/) | Alcalde de Villavicencio buscará viabilizar megaproyecto de seguridad con el nuevo Gobierno nacional | casa (sin firma) | F |
| antes | 2026-06-30 | [50998](https://www.viveelmeta.com/ivan-cepeda-amenaza-con-desobediencia-civil-si-de-la-espriella-no-deja-la-idea-de-extraditar-a-petro-50998/) | Iván Cepeda amenaza con desobediencia civil si De la Espriella no deja la idea de extraditar a Petro | casa (sin firma) | A |
| antes | 2026-06-30 | [51001](https://www.viveelmeta.com/denuncian-por-terrorismo-a-joven-petrista-que-llamo-a-hacer-invivible-este-pais-tras-derrota-electoral-51001/) | Denuncian por terrorismo a joven petrista que llamó a "hacer invivible este país" tras derrota electoral | casa (sin firma) | A |
| antes | 2026-07-01 | [51024](https://www.viveelmeta.com/niegan-tutela-que-buscaba-impedir-la-posesion-de-abelardo-de-la-espriella-por-doble-nacionalidad-51024/) | Niegan tutela que buscaba impedir la posesión de Abelardo De La Espriella por doble nacionalidad | casa (sin firma) | A |
| antes | 2026-07-03 | [51051](https://www.viveelmeta.com/contraloria-alerta-por-acelerado-aumento-de-la-deuda-publica-en-el-tramo-final-del-gobierno-petro-51051/) | Contraloría alerta por acelerado aumento de la deuda pública en el tramo final del gobierno Petro | casa (sin firma) | F |
| antes | 2026-07-04 | [51067](https://www.viveelmeta.com/por-derrota-electoral-felipe-harman-echo-de-la-ant-a-uno-de-sus-mas-fieles-colaboradores-51067/) | Por derrota electoral, Felipe Harman echó de la ANT a uno de sus más fieles colaboradores | casa (sin firma) | F |
| antes | 2026-07-06 | [51085](https://www.viveelmeta.com/abelardo-no-gano-las-elecciones-petro-insiste-en-fraude-y-convoca-movilizacion-para-el-20-de-julio-51085/) | "Abelardo no ganó las elecciones": Petro insiste en fraude y convoca movilización para el 20 de julio | casa (sin firma) | F |
| antes | 2026-07-06 | [51089](https://www.viveelmeta.com/petro-asegura-que-por-decision-de-los-colombianos-el-presidente-electo-es-ivan-cepeda-51089/) | Petro asegura que por decisión de los colombianos el presidente electo es Iván Cepeda | casa (sin firma) | A |
| antes | 2026-07-08 | [51121](https://www.viveelmeta.com/alianza-verde-reconoce-a-de-la-espriella-y-le-exige-a-petro-un-empalme-transparente-y-responsable-51121/) | Alianza Verde reconoce a De la Espriella y le exige a Petro un empalme "transparente y responsable" | casa (sin firma) | A |
| antes | 2026-07-09 | [51135](https://www.viveelmeta.com/la-deuda-publica-crecio-mas-de-364-billones-en-el-gobierno-petro-y-sera-la-mayor-de-la-historia-51135/) | La deuda pública creció más de $364 billones en el gobierno Petro y será la mayor de la historia | casa (sin firma) | F |
| antes | 2026-07-10 | [51152](https://www.viveelmeta.com/gobierno-entrante-revisara-la-suspension-general-de-los-permisos-para-portar-armas-en-colombia-51152/) | Gobierno entrante revisará la suspensión general de los permisos para portar armas en Colombia | casa (sin firma) | A |
| antes | 2026-07-10 | [51156](https://www.viveelmeta.com/ivan-cepeda-y-aida-quilcue-incluidos-en-denuncia-penal-por-presiones-armadas-en-las-presidenciales-de-2026-51156/) | Iván Cepeda y Aida Quilcué, incluidos en denuncia penal por presiones armadas en las presidenciales de 2026 | casa (sin firma) | A |
| antes | 2026-07-11 | [51159](https://www.viveelmeta.com/gobernadora-del-meta-ofrece-la-base-aerea-de-apiay-para-la-posesion-de-abelardo-de-la-espriella-51159/) | Gobernadora del Meta ofrece la Base Aérea de Apiay para la posesión de Abelardo de la Espriella | casa (sin firma) | A |
| antes | 2026-07-13 | [51164](https://www.viveelmeta.com/opinion-el-agro-ingreso-seguro-de-gustavo-de-petro-51164/) | El Agro Ingreso Seguro de Gustavo de Petro | Fernando Betancourt | F · columna firmada (Betancourt) contra el gobierno en ejercicio |
| antes | 2026-07-14 | [51175](https://www.viveelmeta.com/sin-resultados-vencio-contrato-por-10-000-millones-para-sacar-a-petro-de-la-lista-clinton-la-platica-se-perdio-51175/) | Sin resultados venció contrato por $10.000 millones para sacar a Petro de la Lista Clinton: ¿la platica se perdió? | casa (sin firma) | F |
| antes | 2026-07-15 | [51187](https://www.viveelmeta.com/petro-confirma-que-no-asistira-a-la-posesion-de-abelardo-no-voy-a-estar-el-7-de-agosto-ni-darle-la-mano-51187/) | Petro confirma que no asistirá a la posesión de Abelardo: “No voy a estar el 7 de agosto, ni darle la mano” | casa (sin firma) | F |
| antes | 2026-07-16 | [51204](https://www.viveelmeta.com/estados-unidos-deportara-hoy-al-activista-beto-coral-aliado-politico-de-gustavo-petro-51204/) | Estados Unidos deportará hoy al activista Beto Coral, aliado político de Gustavo Petro | casa (sin firma) | F |
| antes | 2026-07-16 | [51208](https://www.viveelmeta.com/gobierno-petro-obliga-a-colegios-a-ensenar-sobre-reconocimiento-del-placer-y-diversidad-sexual-51208/) | Gobierno Petro obliga a colegios a enseñar sobre reconocimiento del placer y diversidad sexual | casa (sin firma) | F |
| antes | 2026-07-16 | [51218](https://www.viveelmeta.com/uniamazonia-abre-investigacion-a-profesor-que-rechazo-a-vendedor-de-panela-por-votar-por-de-la-espriella-51218/) | Uniamazonía abre investigación a profesor que rechazó a vendedor de panela por votar por De la Espriella | casa (sin firma) | A |
| antes | 2026-07-17 | [51235](https://www.viveelmeta.com/equipo-de-empalme-del-tigre-denuncia-cuatro-presuntos-casos-de-corrupcion-del-gobierno-petro-51235/) | Equipo de empalme del 'Tigre' denuncia cuatro presuntos casos de corrupción del gobierno Petro | casa (sin firma) | A |
| antes | 2026-07-18 | [51249](https://www.viveelmeta.com/villavicencio-es-de-derecha-alexander-baquero-apoya-que-de-la-espriella-se-posesione-en-apiay-51249/) | "Villavicencio es de derecha": Alexander Baquero apoya que De La Espriella se posesione en Apiay | casa (sin firma) | A |
| antes | 2026-07-21 | [51262](https://www.viveelmeta.com/colombia-no-produce-ni-exporta-carros-electricos-como-afirma-petro-aclara-la-andi-51262/) | Colombia no produce ni exporta carros eléctricos como afirma Petro, aclara la ANDI | casa (sin firma) | F |
| antes | 2026-07-22 | [51282](https://www.viveelmeta.com/nueva-reforma-tributaria-del-gobierno-petro-propone-subir-el-iva-a-la-gasolina-y-al-diesel-hasta-el-19-51282/) | Nueva reforma tributaria del gobierno Petro propone subir el IVA a la gasolina y al diésel hasta el 19 % | casa (sin firma) | F |
| antes | 2026-07-23 | [51290](https://www.viveelmeta.com/gobierno-petro-firmo-6-717-contratos-tras-perder-las-presidenciales-advierte-transparencia-por-colombia-51290/) | Gobierno Petro firmó 6.717 contratos tras perder las presidenciales, advierte Transparencia por Colombia | casa (sin firma) | A |
| antes | 2026-07-24 | [51304](https://www.viveelmeta.com/esta-es-la-millonaria-pension-que-tendra-gustavo-petro-tras-dejar-la-presidencia-de-colombia-51304/) | Esta es la millonaria pensión que tendrá Gustavo Petro tras dejar la Presidencia de Colombia | casa (sin firma) | F |
| antes | 2026-07-27 | [51334](https://www.viveelmeta.com/de-la-espriella-cerrara-14-embajadas-y-cerca-de-15-consulados-para-reducir-el-gasto-publico-51334/) | De la Espriella cerrará 14 embajadas y cerca de 15 consulados para reducir el gasto público | casa (sin firma) | A |
| antes | 2026-07-28 | [51360](https://www.viveelmeta.com/gremios-del-meta-piden-a-de-la-espriella-destinar-10-billones-para-resolver-los-problemas-de-la-via-al-llano-51360/) | Gremios del Meta piden a De la Espriella destinar $10 billones para resolver los problemas de la vía al Llano | casa (sin firma) | A |
| antes | 2026-07-29 | [51386](https://www.viveelmeta.com/posesion-de-abelardo-de-la-espriella-costaria-menos-que-la-de-petro-en-precios-de-2026-51386/) | Posesión de Abelardo De La Espriella costaría menos que la de Petro en precios de 2026 | casa (sin firma) | A |
| antes | 2026-07-30 | [51397](https://www.viveelmeta.com/de-la-espriella-asegura-que-no-saldra-del-pais-durante-su-gobierno-yo-me-quedo-en-las-regiones-51397/) | De la Espriella asegura que no saldrá del país durante su gobierno: "Yo me quedo en las regiones" | casa (sin firma) | A |
| antes | 2026-07-30 | [51401](https://www.viveelmeta.com/compramos-los-tiquetes-de-nuestro-bolsillo-darwin-asumira-sus-gastos-para-ir-a-la-posesion-presidencial-51401/) | “Compramos los tiquetes de nuestro bolsillo”: Darwin asumirá sus gastos para ir a la posesión presidencial | casa (sin firma) | A |
| antes | 2026-07-31 | [51409](https://www.viveelmeta.com/gustavo-petro-termina-su-mandato-con-575-de-desaprobacion-segun-cb-global-data-51409/) | Gustavo Petro termina su mandato con 57,5 % de desaprobación, según CB Global Data | casa (sin firma) | F |
| antes | 2026-08-03 | [51450](https://www.viveelmeta.com/petro-termina-su-gobierno-como-el-presidente-que-mas-viajo-al-exterior-gasto-cerca-de-12-000-millones-51450/) | Petro termina su gobierno como el presidente que más viajó al exterior: gastó cerca de $12.000 millones | casa (sin firma) | F |
| antes | 2026-08-03 | [51455](https://www.viveelmeta.com/esto-es-aberrante-gobierno-de-la-espriella-encontro-un-faltante-de-30-billones-en-presupuesto-de-2027-51455/) | "Esto es aberrante": gobierno De la Espriella encontró un faltante de $30 billones en presupuesto de 2027 | casa (sin firma) | A |
| antes | 2026-08-04 | [51474](https://www.viveelmeta.com/alvaro-uribe-no-asistiria-a-la-posesion-de-abelardo-de-la-espriella-esta-seria-la-razon-51474/) | Álvaro Uribe no asistiría a la posesión de Abelardo de la Espriella: esta sería la razón | casa (sin firma) | A |
| antes | 2026-08-05 | [51495](https://www.viveelmeta.com/gobierno-de-la-espriella-pondra-en-marcha-los-bloques-de-seguridad-urbana-desde-el-8-de-agosto-51495/) | Gobierno De la Espriella pondrá en marcha los Bloques de Seguridad Urbana desde el 8 de agosto | casa (sin firma) | A |
| después | 2026-08-08 | [51519](https://www.viveelmeta.com/adios-privilegios-de-la-espriella-ordena-trasladar-a-epa-colombia-a-una-carcel-de-mayor-seguridad-51519/) | Adiós privilegios: De la Espriella ordena trasladar a ‘Epa Colombia’ a una cárcel de mayor seguridad | casa (sin firma) | **D** · titular propio: «Adiós privilegios» |
| después | 2026-08-12 | [51580](https://www.viveelmeta.com/gustavo-petro-solicito-permiso-al-senado-para-salir-del-pais-por-un-ano-se-quiere-volar-51580/) | Gustavo Petro solicitó permiso al Senado para salir del país por un año: ¿Se quiere volar? | casa (sin firma) | **D** · titular propio con burla: «¿Se quiere volar?» |
| después | 2026-08-12 | [51583](https://www.viveelmeta.com/un-empresario-de-castilla-la-nueva-llego-hasta-la-posesion-presidencial-que-oportunidades-se-abren-para-el-municipio-51583/) | Un empresario de Castilla La Nueva llegó hasta la posesión presidencial: ¿qué oportunidades se abren para el municipio? | casa (sin firma) | A |
| después | 2026-08-12 | [51587](https://www.viveelmeta.com/venezolana-elogia-respuesta-de-de-la-espriella-ante-el-terremoto-nosotros-esperamos-una-semana-51587/) | Venezolana elogia respuesta de De la Espriella ante el terremoto: "Nosotros esperamos una semana" | casa (sin firma) | A (límite) · elogio de una ciudadana elegido como noticia; la cita es de ella |
| después | 2026-08-13 | [51595](https://www.viveelmeta.com/centro-democratico-ayudo-a-gustavo-petro-a-conseguir-permiso-para-salir-del-pais-51595/) | Centro Democrático ayudó a Gustavo Petro a conseguir permiso para salir del país | casa (sin firma) | A |
| después | 2026-08-13 | [51605](https://www.viveelmeta.com/gobierno-alista-decreto-de-retiro-obligatorio-para-funcionarios-que-ya-cumplen-requisitos-de-pension-51605/) | Gobierno alista decreto de retiro obligatorio para funcionarios que ya cumplen requisitos de pensión | casa (sin firma) | A |
| después | 2026-08-14 | [51630](https://www.viveelmeta.com/de-la-espriella-saco-por-las-malas-a-cinco-embajadores-de-petro-que-no-renunciaron-51630/) | De la Espriella sacó por las malas a cinco embajadores de Petro que no renunciaron | casa (sin firma) | A (límite) · «por las malas», coloquial |
| después | 2026-08-18 | [51685](https://www.viveelmeta.com/ant-de-felipe-harman-logro-solo-el-7-de-la-meta-en-tierras-tituladas-segun-el-libro-de-la-verdad-de-de-la-espriella-51685/) | El Libro de la Verdad reveló que la ANT de Harman entregó más de 253.000 hectáreas sin título de propiedad | casa (sin firma) | A |
| después | 2026-08-19 | [51697](https://www.viveelmeta.com/vicepresidente-asegura-que-el-libro-de-la-verdad-es-solo-el-primer-tomo-de-una-enciclopedia-sobre-corrupcion-51697/) | Vicepresidente asegura que El Libro de la Verdad es solo "el primer tomo" de una enciclopedia sobre corrupción | casa (sin firma) | A |
| después | 2026-08-19 | [51701](https://www.viveelmeta.com/el-meta-concentro-el-59-de-bloqueos-al-sector-petrolero-durante-el-gobierno-petro-segun-informe-51701/) | El Meta concentró el 59 % de bloqueos al sector petrolero durante el gobierno Petro, según informe | casa (sin firma) | A |
| después | 2026-08-19 | [51714](https://www.viveelmeta.com/se-llevaron-hasta-los-muebles-conservadores-denuncian-que-petrismo-saqueo-entidades-del-agro-51714/) | “Se llevaron hasta los muebles”: conservadores denuncian que el petrismo saqueó entidades del agro | casa (sin firma) | A |
| después | 2026-08-20 | [51724](https://www.viveelmeta.com/angie-rodriguez-exfuncionaria-de-petro-denuncia-amenazas-y-pide-impedir-su-salida-de-colombia-51724/) | Angie Rodríguez, exfuncionaria de Petro, denuncia amenazas y pide impedir su salida de Colombia | casa (sin firma) | A |
| después | 2026-08-20 | [51735](https://www.viveelmeta.com/el-libro-de-la-verdad-revive-caso-del-centro-potencia-que-el-gobierno-petro-no-construyo-en-villavicencio-51735/) | El ‘Libro de la Verdad’ revive caso del Centro PotencIA que el gobierno Petro no construyó en Villavicencio | casa (sin firma) | A |
| después | 2026-08-21 | [51752](https://www.viveelmeta.com/ministra-de-educacion-acusa-al-gobierno-petro-de-impulsar-ideologia-de-genero-en-colegios-51752/) | Ministra de Educación acusa al gobierno Petro de impulsar “ideología de género” en colegios | casa (sin firma) | A |
| después | 2026-08-24 | [51787](https://www.viveelmeta.com/recursos-de-educacion-habrian-pagado-propaganda-electoral-en-el-gobierno-petro-denuncia-mintic-51787/) | Recursos de educación habrían pagado propaganda electoral en el gobierno Petro, denuncia MinTIC | casa (sin firma) | A |
| después | 2026-08-24 | [51793](https://www.viveelmeta.com/exsenador-alejandro-vega-queda-fuera-de-la-carrera-por-un-cupo-en-el-consejo-nacional-electoral-51793/) | Exsenador Alejandro Vega queda fuera de la carrera por un cupo en el Consejo Nacional Electoral | casa (sin firma) | A |
| después | 2026-08-25 | [51817](https://www.viveelmeta.com/los-resultados-empiezan-a-verse-rafaela-cortes-tras-captura-de-11-milicianos-en-el-meta-51817/) | "Los resultados empiezan a verse": Rafaela Cortés tras captura de 11 milicianos en el Meta | casa (sin firma) | A |
| después | 2026-08-28 | [51882](https://www.viveelmeta.com/joven-que-amenazo-con-hacer-invivible-el-pais-a-de-la-espriella-denuncia-amenazas-y-acoso-51882/) | Joven que amenazó con hacer “invivible” el país a De la Espriella denuncia amenazas y acoso | casa (sin firma) | V · voz a una crítica del gobierno (Juco) |
| después | 2026-08-31 | [51900](https://www.viveelmeta.com/gobierno-nacional-anuncio-congelamiento-de-precios-de-gasolina-y-acpm-durante-septiembre-51900/) | Gobierno nacional anunció congelamiento de precios de gasolina y ACPM durante septiembre | casa (sin firma) | A |
| después | 2026-08-31 | [51909](https://www.viveelmeta.com/medicina-legal-reporta-62-menores-muertos-en-operaciones-militares-durante-gobierno-petro-51909/) | Medicina Legal reporta 62 menores muertos en operaciones militares durante gobierno Petro | casa (sin firma) | A |
| después | 2026-09-01 | [51935](https://www.viveelmeta.com/alexander-baquero-cuestiona-obligacion-que-petro-delego-a-los-municipios-nos-toca-sostener-a-quienes-delinquen-51935/) | Alexander Baquero cuestiona obligación que Petro delegó a los municipios: “Nos toca sostener a quienes delinquen” | casa (sin firma) | A |
| después | 2026-09-02 | [51956](https://www.viveelmeta.com/alexander-baquero-se-niega-a-seguir-asumiendo-gastos-funerarios-de-muertos-en-combate-trasladados-a-villavicencio-51956/) | Alexander Baquero se niega a seguir asumiendo gastos funerarios de muertos en combate trasladados a Villavicencio | casa (sin firma) | A |
| después | 2026-09-04 | [51994](https://www.viveelmeta.com/avianca-revela-en-una-carta-por-que-dejo-a-gustavo-petro-sin-tiquetes-a-mexico-51994/) | Avianca revela en una carta por qué dejó a Gustavo Petro sin tiquetes a México | casa (sin firma) | A |
| después | 2026-09-05 | [51998](https://www.viveelmeta.com/promueven-campana-negra-contra-avianca-por-negarse-a-transportar-a-gustavo-petro-51998/) | Promueven campaña negra contra Avianca por negarse a transportar a Gustavo Petro | casa (sin firma) | **D** · titular propio: «campaña negra» de los afines al expresidente |
| después | 2026-09-07 | [52011](https://www.viveelmeta.com/petro-sabia-donde-estaba-comerciante-secuestrado-en-el-meta-y-no-ordeno-rescatarlo-afirma-de-la-espriella-52011/) | Petro sabía donde estaba comerciante secuestrado en el Meta y no ordenó rescatarlo, afirma De La Espriella | casa (sin firma) | A |
| después | 2026-09-08 | [52033](https://www.viveelmeta.com/contraloria-confirma-hallazgo-fiscal-por-mas-de-370-000-millones-durante-gestion-de-harman-en-la-ant-52033/) | Contraloría confirma hallazgo fiscal por más de $370.000 millones durante gestión de Harman en la ANT | casa (sin firma) | A |
| después | 2026-09-08 | [52037](https://www.viveelmeta.com/atencion-gobierno-de-de-la-espriella-autoriza-nuevamente-el-porte-legal-de-armas-en-colombia-52037/) | ¡Atención! Gobierno de De La Espriella autoriza nuevamente el porte legal de armas en Colombia | casa (sin firma) | A |
| después | 2026-09-10 | [52071](https://www.viveelmeta.com/de-la-espriella-tiene-54-de-imagen-positiva-a-un-mes-de-asumir-el-gobierno-segun-encuesta-52071/) | De la Espriella tiene 54 % de imagen positiva a un mes de asumir el Gobierno, según encuesta | casa (sin firma) | A |
| después | 2026-09-11 | [52091](https://www.viveelmeta.com/nueva-directora-de-la-ant-destapa-multimillonaria-contratacion-de-la-entidad-bajo-la-direccion-de-harman-52091/) | Nueva directora de la ANT destapa multimillonaria contratación de la entidad bajo la dirección de Harman | casa (sin firma) | A |
| después | 2026-09-12 | [52102](https://www.viveelmeta.com/no-solo-juliana-guerrero-otros-24-funcionarios-de-petro-habrian-sido-contratados-con-titulos-falsos-52102/) | No solo Juliana Guerrero, otros 24 funcionarios de Petro habrían sido contratados con títulos falsos | casa (sin firma) | A |
| después | 2026-09-14 | [52123](https://www.viveelmeta.com/petro-intento-funar-al-gobierno-pero-le-salio-mal-confundio-a-un-ministro-con-oviedo-ebrio-52123/) | Petro intentó funar al Gobierno pero le salió mal: confundió a un ministro con Oviedo ebrio | casa (sin firma) | **D** · titular propio: «intentó funar al Gobierno pero le salió mal» |
| después | 2026-09-16 | [52159](https://www.viveelmeta.com/la-presion-esta-dando-resultados-de-la-espriella-por-captura-de-financiador-del-eln-en-villavicencio-52159/) | "La presión está dando resultados": De la Espriella por captura de financiador del ELN en Villavicencio | casa (sin firma) | A |
| después | 2026-09-16 | [52167](https://www.viveelmeta.com/el-dapre-fue-un-contratadero-durante-el-gobierno-petro-denuncia-su-actual-director-52167/) | El Dapre fue un "contratadero" durante el gobierno Petro, denuncia su actual director | casa (sin firma) | A |
| después | 2026-09-17 | [52174](https://www.viveelmeta.com/proyecto-de-ley-busca-que-la-via-al-llano-sea-una-prioridad-permanente-del-gobierno-nacional-52174/) | Proyecto de ley busca que la vía al Llano sea una prioridad permanente del Gobierno nacional | casa (sin firma) | A |
| después | 2026-09-17 | [52181](https://www.viveelmeta.com/contraloria-rastrea-44-billones-de-la-salud-de-los-maestros-girados-sin-soporte-en-el-gobierno-del-cambio-52181/) | Contraloría rastrea $4,4 billones de la salud de los maestros girados sin soporte en el “Gobierno del Cambio” | casa (sin firma) | A |
| después | 2026-09-17 | [52186](https://www.viveelmeta.com/el-pais-va-a-conocer-los-actos-de-corrupcion-de-la-administracion-harman-directora-de-la-ant-52186/) | “El país va a conocer los actos de corrupción de la administración Harman”: directora de la ANT | casa (sin firma) | A |
| después | 2026-09-23 | [52298](https://www.viveelmeta.com/juez-tumbo-tutela-que-le-prohibia-a-de-la-espriella-mostrar-cadaveres-como-trofeos-de-guerra-52298/) | Juez tumbó tutela que le prohibía a De La Espriella mostrar cadáveres como trofeos de guerra | casa (sin firma) | A (límite) · «El Gobierno Nacional ganó la tutela» en el primer párrafo; el titular usa el encuadre crítico («trofeos de guerra») |
| después | 2026-09-24 | [52313](https://www.viveelmeta.com/tarifa-diferencial-que-prometio-petro-en-peajes-del-eje-cafetero-resulto-ser-falsa-una-mentira-mas-del-mentiroso-52313/) | Tarifa diferencial que prometió Petro en peajes del Eje Cafetero resultó ser falsa: "una mentira más del mentiroso" | casa (sin firma) | A · «mentiroso» entre comillas, de un alcalde |
| después | 2026-09-25 | [52329](https://www.viveelmeta.com/funcionarios-de-petro-habrian-ofrecido-prebendas-a-paramilitares-para-atacar-a-de-la-espriella-y-uribe-52329/) | Funcionarios de Petro habrían ofrecido prebendas a paramilitares para atacar a De La Espriella y Uribe | casa (sin firma) | A |
| después | 2026-09-28 | [52342](https://www.viveelmeta.com/que-bruto-petro-publico-video-de-2021-para-denunciar-supuesta-violencia-policial-en-el-actual-gobierno-52342/) | ¡Qué bruto! Petro publicó video de 2021 para denunciar supuesta violencia policial en el actual gobierno | casa (sin firma) | **D** · titular propio: «¡Qué bruto!» y «No es la primera vez que el expresidente intenta atacar al gobierno y se equivoca» |
| después | 2026-09-28 | [52349](https://www.viveelmeta.com/gobierno-de-la-espriella-reporto-caida-de-secuestros-extorsiones-y-homicidios-en-su-primer-mes-52349/) | Gobierno De la Espriella reportó caída de secuestros, extorsiones y homicidios en su primer mes | casa (sin firma) | A |
| después | 2026-09-29 | [52361](https://www.viveelmeta.com/senadora-petrista-pide-excomulgar-a-de-la-espriella-por-invocar-a-dios-en-medio-de-acciones-militares-52361/) | Senadora petrista pide excomulgar a De La Espriella por invocar a Dios en medio de acciones militares | casa (sin firma) | V · voz a una senadora crítica, rotulada «petrista» |
| después | 2026-10-01 | [52419](https://www.viveelmeta.com/lo-noto-asustado-directora-de-la-ant-saco-cuentas-sobre-el-despilfarro-de-felipe-harman-52419/) | "Lo noto asustado": directora de la ANT sacó cuentas sobre presunto despilfarro de Felipe Harman | casa (sin firma) | A |
| después | 2026-10-01 | [52428](https://www.viveelmeta.com/de-la-espriella-ordena-echar-para-atras-el-incremento-en-el-precio-de-la-gasolina-para-octubre-52428/) | De La Espriella ordena echar para atrás el incremento en el precio de la gasolina para octubre | casa (sin firma) | A (límite) · informativa |
| después | 2026-10-05 | [52464](https://www.viveelmeta.com/registrador-exige-a-petro-rectificar-senalamientos-sobre-supuesto-fraude-en-las-elecciones-de-2026-52464/) | Registrador exige a Petro rectificar señalamientos sobre supuesto fraude en las elecciones de 2026 | casa (sin firma) | A |
| después | 2026-10-07 | [52500](https://www.viveelmeta.com/abra-las-puertas-de-la-reeleccion-y-me-enfrentara-petro-reta-a-de-la-espriella-a-un-duelo-en-las-urnas-52500/) | “Abra las puertas de la reelección y me enfrentará”: Petro reta a De la Espriella a un duelo en las urnas | casa (sin firma) | V · voz al expresidente que reta al gobierno |
| después | 2026-10-08 | [52529](https://www.viveelmeta.com/de-la-espriella-responde-a-criticas-por-caminar-entre-cuerpos-de-criminales-mas-lo-voy-a-hacer-52529/) | De La Espriella responde a críticas por caminar entre cuerpos de criminales: "Más lo voy a hacer" | casa (sin firma) | V · críticas al presidente, encuadradas desde su respuesta |
| después | 2026-10-08 | [52533](https://www.viveelmeta.com/oscar-apolinar-descartado-en-la-carrera-por-la-gobernacion-del-meta-en-2027-52533/) | Óscar Apolinar, descartado en la carrera por la Gobernación del Meta en 2027 | casa (sin firma) | A |
| después | 2026-10-09 | [52549](https://www.viveelmeta.com/no-le-corre-sangre-por-esa-jeta-darwin-castellanos-arremete-contra-felipe-harman-52549/) | “No le corre sangre por esa jeta”: Darwin Castellanos arremete contra Felipe Harman | casa (sin firma) | A |

---

Recuento hecho con los datos descargados el 2026-10-09. Si el medio edita o
retira piezas, los enlaces pueden cambiar; los ID numéricos del final de cada
URL sirven para localizarlas en el sitemap.
