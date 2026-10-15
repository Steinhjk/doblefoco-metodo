# RTVC Noticias — ficha de orientación

| | |
|---|---|
| **Medio** | RTVC Noticias · `rtvc` · rtvcnoticias.com |
| **Valor vigente** | **+0,30** · `reviewedAt: '2026-10-10'` · **GUBERNAMENTAL**<br>**Banda (registro):** Derecha moderada |
| **Firma** | ☑ **FIRMADA el 2026-10-10 — el responsable editorial** (firma en bloque tras el ciclo 2; ver DECISIONES.md. Lo que más abajo dice «sin firmar», «no se firma» o «provisional» es el estado anterior a esta firma y se conserva como historia) |
| **Alta** | — |
| **Última revisión** | 2026-10-10 · correcciones de hecho del ciclo 2 aplicadas |
| **Departamento / ámbito** | Nacional |
| **Fuentes de propiedad** | `shared/mediaOwnership.js` (`rtvc`): 15 fuentes; comprobada el 2026-10-10<br>**Propiedad comprobada:** 2026-10-10 (`verifiedAt`) |
| **Recogida** | `https://www.rtvcnoticias.com/noticias/rss.xml` · vía `direct` |
| **Protocolo** | **Regla:** `PROTOCOLO_JUICIO_EDITORIAL.md`, «Medios del Gobierno nacional: excepción al polo fijo» (2026-10-10) |

## Estado

> **MARCA «GUBERNAMENTAL».** RTVC es un medio del Gobierno nacional sin línea
> propia: es oficialista con los dos gobiernos. Por la excepción del protocolo,
> **toma la dirección del gobierno que lo controla, con la magnitud tope**. Hoy
> lo controla el Gobierno De la Espriella, a la derecha, y por eso lleva +0,30.
> **El número no mide una línea del medio: dice hacia dónde empuja hoy.** Cambia
> de signo si cambia el signo del gobierno.
>
> El catálogo no tiene un campo para esta marca. Va escrita al principio del
> `biasRationale` (`shared/mediaRegistry.js`) y aquí. Que la UI la muestre como
> distintivo queda pendiente (ver «Estado»).

**En catálogo, con +0,30 y sin firmar. Marca «gubernamental».** Propiedad
comprobada (`verifiedAt` 2026-10-10).

**Pendiente:**

1. **Mostrar la marca en la UI.** No hay campo para «gubernamental» en
   `mediaRegistry.js` ni en `mediaOwnership.js`; hoy está en el
   `biasRationale` y en esta ficha. Un campo nuevo necesita prueba y lo decide
   el integrador.
2. **Revisión en cada cambio de gobierno** (07-08-2030), y antes si «RTVC
   Ahora» fiscaliza al Gobierno (Refutación, 2).
3. **Vigilancia manual** de `/actualidad/rtvc` y `/actualidad/inravision`
   (mensual) y del RUES (anual). El centinela no puede preguntar a este sitio:
   su buscador está excluido en su robots.txt. Ver `shared/centinela.js`.
4. **Factualidad**: revisar el 0,82 a la luz de la rectificación por tutela.

## Evidencia

### Nivel 1 — Quién lo controla, hoy (comprobado el 2026-10-10)

**Es el único medio público nacional del catálogo.** Sociedad entre entidades
públicas del orden nacional, sometida al régimen de las Empresas Industriales y
Comerciales del Estado. Literal del Decreto 3912 de 2004: «Que Radio Televisión
Nacional de Colombia, RTVC, autorizada mediante Decreto número 3525 de 26 de
octubre de 2004, es una sociedad entre entidades públicas, indirecta, del orden
nacional, sometida al régimen de las Empresas Industriales y Comerciales del
Estado». Se protocolizó por la escritura pública 3138 del 28-10-2004 (Notaría
34 de Bogotá), según las notas del normograma de MinTIC.

**El decreto que autorizó su creación (3525 de 2004) fue declarado nulo** por el
Consejo de Estado, Sección Primera, el 27-01-2011 (exp. 2005-00030-01), según el
normograma de MinTIC. Lo que eso prueba es que la compilación oficial del sector
registra la nulidad; qué efectos tuvo sobre la sociedad no consta, y la
sentencia no se ha leído. La sociedad sigue matriculada y activa.

**Tensión declarada: en el registro mercantil figura como S.A.S.** RUES
(datos.gov.co `c82u-588k`, consultado el 2026-10-10): «INRAVISIÓN - SISTEMA DE
MEDIOS PÚBLICOS DEL ESTADO COLOMBIANO S.A.S», «SOCIEDADES POR ACCIONES
SIMPLIFICADAS SAS», Cámara de Comercio de Bogotá, matrícula 1434314 del
2004-11-29, activa, renovada el 2026-03-30 y actualizada el 2026-08-21. El
propio medio se llama «RTVC - Sistema de Medios Públicos del Estado Colombiano
S.A.S.» el 15-09-2026. No consta el acto que explique la forma SAS, y la
declaración propia vigente (inravision.gov.co, «Quiénes somos») sigue diciendo
«sociedad entre entidades públicas». **No mueve el eje.**

**El Gobierno nombra a su gerente por decreto, y el control pasa por MinTIC.**
La Resolución RTVC 0461 de 2016 dice del gerente de entonces: «nombrado en el
cargo mediante Decreto número 1222 del 4 de junio de 2015».

**Gerente desde agosto de 2026: Ángela María Mora Soto**, nombrada por el
Gobierno De la Espriella. Lo dice el propio medio el 14-08 y el 31-08-2026. Su
predecesor, con el Gobierno Petro, fue Hollman Morris (State Media Monitor lo
sigue dando como gerente: está desactualizado). **No consta director de
noticias desde el 07-08-2026.** El último que consta es el director del
Sistema Informativo de la etapa anterior, citado el 06-08-2026. Desde el
07-10-2026 emite un informativo nuevo, «RTVC Ahora», sin director nombrado.

**Sin aviso de quien dirige.** No consta candidatura ni cargo de elección de la
gerente. Ser gerente de una sociedad pública nombrada por el Gobierno es la
dependencia que ya declara la ficha de propiedad, no el cargo que dispara la
regla. Mismo criterio que en Telecafé.

En 2026 la entidad recuperó su nombre histórico, Inravisión: `rtvc.gov.co`
redirige a `inravision.gov.co` (comprobado el 2026-08-08 y de nuevo el
2026-10-10). **Aquí se le sigue llamando RTVC por decisión del responsable editorial** (2026-08-08):
es el nombre con el que el medio se presenta ante su audiencia. Desde
septiembre el propio medio vuelve a firmar «RTVC - Sistema de Medios
Públicos…» y llama «RTVC Ahora» a su informativo nuevo.

### La previsión del 2026-08-08, contrastada

El 2026-08-08, **antes** de la transición, el responsable editorial dejó anotado en
`mediaOwnership.js`:

> *«PREVISIÓN DECLARADA, no medición: se espera que en los próximos días el medio
> cambie de dirección y pase a cubrir la actualidad desde una posición oficialista
> con el nuevo gobierno. Su valor actual de orientación (−0,35) se fijó bajo el
> gobierno anterior. Se deja escrito ANTES de que ocurra para que el ajuste, si
> llega, se pueda contrastar contra lo que se esperaba, en vez de justificarse
> después.»*

**Contraste, 2026-10-10: la previsión se confirma.** El barrido de 12 meses
muestra postura en voz de la casa a favor del Gobierno Petro antes del 07-08 y a
favor del Gobierno De la Espriella después, sin contrapesos después.

### Voz de la casa — barrido de 12 meses (2026-10-10)

Regla «Evidencia editorial histórica» (2026-10-09). Universo: la sección
«Gobierno» entera (402 piezas en la ventana), `/actualidad/rtvc`,
`/actualidad/inravision`, `/politica` (02-06 a 13-09-2026) y opinión. **622
piezas únicas: 573 antes del 07-08-2026 y 49 después.** La caída de volumen es
en sí un hecho: el 15-08 se cerró la franja informativa.

| | Antes (Petro) | Después (De la Espriella) |
|---|---:|---:|
| Nivel A (firma de la casa): elogio / rótulo / institucional | 14 / 2 / 2 = **18** | 0 / 3 / 1 = **4** |
| Nivel B (titular de periodista de plantilla): elogio / rótulo | 10 / 6 = **16** | 2 / 2 = **4** |
| **Total** | **34** | **8** |
| Dirección | izquierda: a favor del Gobierno Petro y de su candidato | derecha: a favor del Gobierno De la Espriella, contra la etapa anterior |
| Contrapesos | 2 parciales (nivel B) | 0 |

Ejemplos, antes: «100 logros del gobierno Petro…» (30-04-2026), «¡Atención!
RTVC rechaza amenazas intervencionistas de Trump contra Colombia e invita a la
movilización por la soberanía nacional de este miércoles» (06-01-2026), «La ola
Cepeda: artistas, académicos, movimientos sociales e influencers respaldan su
llegada a la Casa de Nariño» (14-06-2026). Después: «Usaron la plata de la
educación para pagar propaganda» (22-08-2026), «RTVC avanza en la
transformación del Sistema de Medios Públicos» («En la Patria Milagro comienza
una nueva etapa para RTVC», 10-09-2026), «Gobierno anuncia conversaciones con el
FMI ante el deterioro recibido de las finanzas públicas» (28-09-2026).

**Lo que no suma y se declara:** la transcripción del Ejecutivo sin contraste,
que es el rasgo más estable del archivo. En «Gobierno», el Ejecutivo es el
sujeto del titular en el 85 % de las piezas antes y en el 63 % después. **La
oposición desaparece del archivo después del cambio**: ninguna de las 49 piezas
posteriores trata de Cepeda ni del Pacto Histórico.

**Resultado:** postura a los dos lados, en sentidos opuestos: a favor de quien
gobierna. Hacia la izquierda, 34 antes y 0 después; hacia la derecha, 0 antes y
8 después. **La condición 3 no se cumple para ninguna dirección.** Las tablas,
pieza por pieza y con URL, están en el [barrido](../revision-externa/barridos/rtvc.md).
La clasificación es juicio de un solo lector, de la misma casa que el autor de
esta ficha.

### Nivel 3 — Registros externos

- **MOE UE, primera vuelta** (declaración preliminar del 02-06-2026, literal):
  «Los medios estatales, que tienen una mayor obligación de neutralidad y
  equilibrio en su cobertura, favorecieron en su mayoría al presidente, al
  Gobierno y a Cepeda, mientras que dedicaron mucho menos tiempo a De la
  Espriella y a Valencia, a menudo en tono negativo». Midió «dos medios
  estatales (el canal de televisión Señal Colombia y Radio Nacional de
  Colombia)», del 30-04 al 30-05-2026.
- **MOE UE, segunda vuelta** (23-06-2026, literal): los medios estatales
  «ampliaron ligeramente la cobertura de Cepeda, en su mayor parte de forma
  neutral, mientras que a De la Espriella se le dedicó menos tiempo y,
  principalmente, en un tono negativo». Y: «Al igual que en la primera vuelta,
  los medios de comunicación estatales favorecieron al presidente y a su
  Gobierno en su cobertura».
- **Rectificación por tutela** (pieza del 2026-08-31, firma «RTVC Noticias»,
  literal): «en cumplimiento de la sentencia de segunda instancia proferida el
  treinta (30) de julio de 2026 por el Tribunal Superior de Bogotá, dentro de la
  acción de tutela instaurada […] en representación de la Fundación La Silla
  Vacía». Se refiere a información «publicada los días 19, 21 y 26 de abril de
  2026». Y: el medio «dejó de emitir el programa Señal Investigativa el 6 de
  agosto de 2026».

Son de la etapa anterior. La MOE mide los canales del sistema, no el sitio.

### Nivel 2 — Conducta medida en nuestro corpus (2026-10-10)

Envío del ciclo 2: **40 días** de corpus (2026-08-31 → 2026-10-10), **214
artículos**, 59 en alguna historia, 66 historias, agenda propia del 14 %. Con 59
piezas en historias **no sostiene nada, en ninguna dirección**, y la compañía
media no mueve un número. Lo que sí hace es desmentir lo que decía esta ficha el
2026-09-09 («seis piezas», «ocho días sin entrar», «hoy no está en el sitio»):
**el silencio era de nuestra vía de ingesta**, Google News, y no del medio.
Desde el 2026-09-09 entra por `/noticias/rss.xml`.

### HECHOS ESTRUCTURALES 2026

Verificados en el sitio del propio medio el 2026-10-10:

| Fecha | Hecho | Fuente |
|---|---|---|
| 15-08-2026 (publicado el 16-08) | **Cierre de la franja informativa y de opinión** y revisión de contenidos y de contratos | «Se acaba el aparato de propaganda en el Sistema de Medios Públicos de Colombia» (firma personal): la ministra TIC y la gerente «definieron un plan de acción inmediato»; «Finalización de la franja noticiosa y de opinión en radio y televisión que hasta el 6 de agosto pasado ocupaba una parte significativa de los recursos humanos y técnicos de Inravisión»; «Revisión inmediata de los contenidos y formatos actualmente al aire»; «En la Patria Milagro se vivirá una nueva etapa para el Sistema de Medios Públicos» |
| 10-09-2026 | **Terminación anticipada de contratos periodísticos** | «RTVC avanza en la transformación del Sistema de Medios Públicos» (firma «RTVC Noticias»): «dar por terminados anticipadamente algunos contratos de prestación de servicios, entre los cuales se encuentran contratos relacionados con actividades periodísticas, de presentación y de gestión de contenidos digitales». Recuerda que «el pasado 15 de agosto se dispuso suspender la franja noticiosa y de opinión que operó hasta el 6 de agosto» |
| 15-09-2026 | **Demanda ante la SIC y denuncia ante la Fiscalía** contra dos excontratistas, por el sitio «RTC Noticias» | Comunicado (firma «RTVC Noticias»): la entidad «presentó ante la Superintendencia de Industria y Comercio una demanda por infracción de derechos de propiedad industrial y, ante la Fiscalía General de la Nación, denuncia penal por la presunta comisión del delito de usurpación de derechos de propiedad industrial». Aquí no se nombra a nadie |
| 06/07-10-2026 | **Vuelve un informativo: «RTVC Ahora»** | «‘RTVC Ahora’ donde pasa, estamos…» (firma «RTVC Noticias», 06-10): «Este miércoles 7 de octubre, el Sistema de Medios Públicos estrenará RTVC Ahora, un nuevo informativo» |

Leídos juntos: cada cambio de gobierno trae otra redacción, y la nueva
administración desmontó la anterior con el lenguaje del nuevo Gobierno
(«aparato de propaganda», «Patria Milagro»). **Es estructura vigente de
dependencia.** Junto con el barrido, es lo que sostiene la marca
«gubernamental».

La «auditoría editorial» anunciada por MinTIC **no entra**: solo la da Pulzo, y
la fuente primaria habla de «revisión inmediata de los contenidos y formatos».

## Barrido de 12 meses

| | |
|---|---|
| **Barrido** | [`revision-externa/barridos/rtvc.md`](../revision-externa/barridos/rtvc.md) |

## Argumento

### ARGUMENTO — por qué +0,30 y la marca «gubernamental»

1. **Es oficialista con los dos gobiernos y no tiene línea propia.** El barrido
   lo muestra: 34 piezas con postura a favor del Gobierno Petro antes del
   07-08-2026 y 8 a favor del Gobierno De la Espriella después, sin contrapesos
   después. La MOE UE lo describió así en la etapa anterior, y los hechos
   estructurales de agosto a octubre lo explican: el Gobierno nombra a la
   gerencia, y la gerencia rehace la redacción.
2. **La regla del polo fijo, sola, daría 0,00**: no hay posición propia que
   sobreviva al cambio, y la regla de evidencia histórica no se activa para
   ninguna dirección (la condición 3 no se cumple). Es lo que proponía la
   resolución.
3. **Pero el protocolo tiene desde el 2026-10-10 una excepción para este
   caso.** Literal: «Un medio que depende del Gobierno nacional y cuya línea
   sigue a la del gobierno de turno —oficialismo con los dos gobiernos, sin
   línea propia— **toma la dirección del gobierno que lo controla**, con la
   magnitud tope (±0,30) y la marca "gubernamental" en su ficha. Se revisa en
   cada cambio de gobierno, y el número cambia de signo si el gobierno lo hace.
   El lector ve así hacia dónde empuja hoy ese medio, y la ficha dice por qué».
4. **RTVC cumple las dos condiciones**: depende del Gobierno nacional (nivel 1:
   gerente nombrado por decreto, control por MinTIC) y su línea sigue a la del
   gobierno de turno (barrido de 12 meses, a los dos lados del cambio).
5. **Hoy lo controla el Gobierno De la Espriella, que está a la derecha.** Por
   eso el valor es **+0,30**, la magnitud tope, y no otra. No es un juicio sobre
   cuánto empuja: es el tope que la excepción fija.
6. **Por qué no se aplica a los canales regionales.** Telecafé, Telemedellín,
   Canal Capital y Telecaribe siguen en 0,00: dependen de gobiernos locales de
   distinto signo a la vez. RTVC depende de uno solo.

**Qué dice el número y qué no.** Dice hacia dónde empuja hoy el medio que
controla el Gobierno nacional. **No dice que RTVC tenga una línea de derecha**:
con el Gobierno Petro empujaba hacia el otro lado, y el número cambiará de signo
el día que lo haga el gobierno.

## El mejor caso en contra

1. **El encuadre pro-Cepeda de la segunda vuelta.** Es lo único del archivo que
   la regla del polo fijo no excluye, y lo que más empuja hacia la izquierda:
   «La ola Cepeda: artistas, académicos, movimientos sociales e influencers
   respaldan su llegada a la Casa de Nariño» (14-06-2026), «Abelardo de la
   Espriella: de abogado de Álex Saab y David Murcia a candidato presidencial»
   (11-06), «El Instituto de Pensamiento Progresista desmiente el mito del "voto
   fusil" promovido por la ultraderecha» (23-06), y la MOE UE. Si eso fuera una
   línea propia, el valor estaría a la izquierda y no a la derecha. **Por qué
   no lo mueve:** el candidato favorecido era el del Gobierno (la MOE lo dice:
   «al presidente, al Gobierno y a Cepeda»), y es **conducta de una redacción
   desmantelada entre el 15-08 y el 10-09-2026** (franja cerrada, «Señal
   Investigativa» fuera del aire, contratos periodísticos terminados). Por la
   regla del presente, ese hecho ya dejó de ser cierto.
2. **La excepción mide al gobierno, que es lo que el polo fijo prohíbe.** La
   prueba del polo fijo («si el gobierno cambiara mañana y el medio mantuviera
   la misma conducta, ¿cambiaría su clasificación?») da «sí» con RTVC, a
   propósito. La excepción lo asume y lo hace visible con la marca: el número
   describe a quién sirve el medio hoy, no una posición propia.
3. **Ocho piezas después del cambio son pocas**, y la mitad son de periodistas
   de plantilla (nivel B). Con el nivel A solo, son 4. Que la dirección actual
   sea la del Gobierno De la Espriella descansa también en los hechos
   estructurales, no solo en el recuento.
4. **«RTVC Ahora» tiene tres días.** Si se quiere medir la redacción nueva y no
   la transición, el número podría esperar unos 30 días. La excepción no lo
   pide: el valor sigue al gobierno que controla el medio, no a su redacción.

## Qué cambiaría el número

| | |
|---|---|
| **Revisión obligada** | En cada cambio de gobierno. La próxima, el 07-08-2030 |

1. **Un cambio de gobierno** (el próximo, el 07-08-2030): se revisa, y el número
   cambia de signo si el gobierno lo hace. Es la revisión obligada de la
   excepción.
2. **Si «RTVC Ahora», en 90 días, fiscaliza al Gobierno De la Espriella como
   fiscalizaría a otro**, con piezas propias críticas: eso rompe el
   oficialismo, la excepción deja de aplicar y la lectura pasa a ser la de
   cualquier medio.
3. **Si en la próxima campaña su encuadre favorece a un candidato que no es el
   del Gobierno**: aparece una posición propia, y deja de ser «gubernamental».
4. **Si cambia el régimen de nombramiento del gerente** (una salvaguarda
   vinculante de independencia editorial): deja de depender del Gobierno
   nacional.

## Tensiones declaradas

### TENSIONES Y PUNTOS A REVISAR (2026-10-10)

1. **Factualidad (0,82), sin tocar.** Hay una sentencia de tutela (Tribunal
   Superior de Bogotá, 30-07-2026) que ordenó rectificar información del 19, 21
   y 26 de abril de 2026, de la que el medio dice que «no está acreditada». Es
   de la redacción anterior. **Queda anotada para revisarla con el criterio de
   factualidad del catálogo**; esta ficha no la mueve.
2. **Contratista del Gobierno que lo nombra.** Hasta el 07-08-2026, once de sus
   catorce contratos de 12 meses fueron con entidades del Gobierno nacional, con
   objetos de divulgación de la propia entidad. Desvelamiento, no acusación.
3. **Forma jurídica.** «Sociedad entre entidades públicas» frente a la S.A.S.
   del RUES, y la nulidad de 2011 del decreto de autorización. Lagunas: la
   sentencia de 2011 y el acto que explique la forma SAS.
4. **Laguna:** el decreto de nombramiento de la gerente (sin fuente primaria) y
   quién dirige «RTVC Ahora».
5. **Pendiente de la UI:** la marca «gubernamental» no tiene campo en el
   catálogo. Hoy vive en el texto. Ver «Estado».

## Contratación pública

Contratación pública (SECOP I y II, NIT 900002583, consultado 2026-10-10): 14
contratos por $30.422 millones **contratados** en los últimos 12 meses
(2025-10-10 → 2026-10-10), todos en SECOP II y **todos firmados antes del
07-08-2026**; 386 por unos $497.000 millones en total desde 2017 (SECOP II: 265
por $389.681 millones; SECOP I: 121 por $107.651 millones), con valores que en
SECOP II pueden incluir adiciones (orden de magnitud, nunca cobrado).
Principales contratantes de los últimos 12 meses: Presidencia de la República
(DAPRE, 3 contratos, $10.680 millones), Ministerio de Educación ($10.600
millones), ICBF ($5.047 millones) y Ministerio de Transporte ($1.390 millones).
**Once de los catorce son de entidades del Gobierno nacional, el mismo que el
medio cubre y que nombra a su gerente**; los otros tres son de la JEP (2) y del
Canal TRO (1). Sus objetos son de producción, emisión y divulgación de la
propia entidad contratante (por ejemplo, el del Ministerio de Educación, «…
PARA DIFUNDIR LAS ACCIONES DEL MINISTERIO DE EDUCACIÓN NACIONAL»). **Con el Gobierno De la Espriella no hay contratos en los que
el medio sea contratista a 2026-10-10.** Es desvelamiento, no acusación.

- **SECOP II** ([`jbjy-vk9h`, últimos 12 meses](https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=nombre_entidad,fecha_de_firma,referencia_del_contrato,estado_contrato,valor_del_contrato,descripcion_del_proceso&$where=documento_proveedor=%27900002583%27%20AND%20fecha_de_firma%3E=%272025-10-10%27);
  [total con fecha de firma](https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=count(id_contrato),sum(valor_del_contrato)&$where=documento_proveedor=%27900002583%27%20AND%20fecha_de_firma%20IS%20NOT%20NULL)):
  265 contratos desde el 2017-04-26, más 6 filas sin fecha de firma que no se
  cuentan. El último de la ventana es el DAPRE 555-26, del 2026-07-27, por
  $2.450 millones. Por entidad: DAPRE (487-25, 390-296 y 555-26), Ministerio de
  Educación (2026-01-29), ICBF, MinTransporte («central de medios»),
  MinHacienda ($857 millones), MinVivienda ($652 millones), Unidad de
  Alimentación Escolar ($600 millones), MinCIT ($297 millones), Superservicios
  ($150 millones), JEP (2 contratos, $103 millones) y Canal TRO ($47 millones).
- **SECOP I** ([`f789-7hwg`](https://www.datos.gov.co/resource/f789-7hwg.json?$select=count(*),sum(cuantia_contrato),min(fecha_de_firma_del_contrato),max(fecha_de_firma_del_contrato)&$where=identificacion_del_contratista%20in(%27900002583%27,%279000025836%27)),
  con y sin dígito de verificación): 121 contratos por $107.651 millones, del
  2017-10-23 al 2022-01-28. **0 en los últimos 12 meses.**
- **Como entidad contratante** (no es la línea del protocolo, pero se declara):
  en SECOP II el NIT aparece como «INRAVISIÓN» (14.163 contratos, el último del
  2026-07-27) y como «INRAVISIÓN - SISTEMA DE MEDIOS PÚBLICOS DEL ESTADO
  COLOMBIANO S.A.S» (1.755, el último del 2026-10-07). El 2026-09-28 firmó
  RTVC-CD-1644-2026, servicios de «toma de fotografía […] del Departamento
  Administrativo de la Presidencia de la República». **La relación de servicio
  con la Presidencia sigue con el nuevo Gobierno.**

## Fuentes

- [Normograma MinTIC — Decreto 3912 de 2004](https://normograma.mintic.gov.co/mintic/compilacion/docs/decreto_3912_2004.htm): naturaleza jurídica. Descargado el 2026-10-10.
- [Normograma MinTIC — Decreto 3525 de 2004](https://normograma.mintic.gov.co/mintic/compilacion/docs/decreto_3525_2004.htm): «Decreto declarado NULO» (Consejo de Estado, 27-01-2011) y escritura 3138 de 2004, en sus notas de vigencia. Descargado el 2026-10-10.
- [Normograma MinTIC — Resolución RTVC 0461 de 2016](https://normograma.mintic.gov.co/mintic/compilacion/docs/resolucion_rtvc_0461_2016.htm): el gerente, nombrado por decreto.
- [RUES, datos.gov.co `c82u-588k`](https://www.datos.gov.co/resource/c82u-588k.json?$select=camara_comercio,matricula,razon_social,organizacion_juridica,estado_matricula,fecha_matricula,ultimo_ano_renovado,fecha_renovacion,fecha_actualizacion&numero_identificacion=900002583), consultado el 2026-10-10.
- SECOP II y SECOP I: las consultas de «Contratación pública», el 2026-10-10.
- RTVC Noticias: [«Sistema de Medios Públicos impulsará la cultura, el deporte y las regiones»](https://www.rtvcnoticias.com/actualidad/inravision/sistema-medios-publicos-impulsara-la-cultura-el-deporte-y-las-regiones) (2026-08-14); [«Se acaba el aparato de propaganda…»](https://www.rtvcnoticias.com/actualidad/inravision/se-acaba-el-aparato-de-propaganda-en-el-sistema-de-medios-publicos) (2026-08-16); [rectificación](https://www.rtvcnoticias.com/actualidad/inravision/rectificacion) (2026-08-31); [«RTVC avanza en la transformación…»](https://www.rtvcnoticias.com/actualidad/rtvc/rtvc-avanza-en-la-transformacion-del-sistema-de-medios-publicos) (2026-09-10); [comunicado sobre la marca](https://www.rtvcnoticias.com/actualidad/rtvc/comunicado-rtvc-uso-indebido-marca) (2026-09-15); [«‘RTVC Ahora’ donde pasa, estamos…»](https://www.rtvcnoticias.com/actualidad/rtvc/rtvc-ahora-donde-pasa-estamos-el-nuevo-informativo-del-sistema-de-medios-publicos) (2026-10-06). Todas descargadas el 2026-10-10.
- MOE UE Colombia 2026: [declaración preliminar de la primera vuelta](https://www.eeas.europa.eu/sites/default/files/2026/documents/Declaracio%CC%81n%20Preliminar%20primera%20vuelta%20MOE%20UE%20Colombia%202026_0.pdf) (02-06-2026) y [de la segunda vuelta](https://www.eeas.europa.eu/sites/default/files/2026/documents/MOE%20UE%20DP%20Segunda%20vuelta%20Colombia%202026%20-23%20JUN.pdf) (23-06-2026). Descargadas el 2026-10-10.
- [State Media Monitor — RTVC](https://statemediamonitor.com/2025/03/radio-y-television-nacional-de-colombia-rtvc-sistema-de-medios-publicos/): «it has no binding editorial-independence safeguard». **Gerente desactualizado** (sigue dando a Hollman Morris). El 2026-10-10 devolvió 403 a la recomprobación; la cita es de la resolución.
- Feed: `https://www.rtvcnoticias.com/noticias/rss.xml` (vivo, ítems del 2026-10-10).
- Barrido: [`revision-externa/barridos/rtvc.md`](../revision-externa/barridos/rtvc.md).

## Historial

### Cabecera anterior (filas superadas)

| | |
|---|---|
| **Valor anterior** | «sin medir» (`bias: null`), del 2026-09-16 al 2026-10-10; antes, −0,35 |
| **Decisión** | el responsable editorial, 2026-10-10: +0,30, sin firmar, marcado «gubernamental» |

### HALLAZGOS DEL CICLO 2 (2026-10-10)

Lo de peso que dejó la revisión externa, comprobado de nuevo en la fuente el
2026-10-10 (curl con UA de navegador; robots.txt leído antes):

- **Oficialista con los dos gobiernos, y sin línea propia.** El barrido de 12
  meses (622 piezas únicas de rtvcnoticias.com, 2025-10-10 → 2026-10-10) da
  **34 piezas con postura a favor del Gobierno Petro antes del 07-08-2026** (18
  con firma de la casa y 16 con titular de periodista de plantilla) y **8 a
  favor del Gobierno De la Espriella después** (4 y 4). Contrapesos: 2
  parciales antes y 0 después. Ninguna dirección cumple «3 a cada lado y 3 a
  1». Es lo que preveía el responsable editorial el 2026-08-08. Fuente: [barrido](../revision-externa/barridos/rtvc.md).
- **Gerente: Ángela María Mora Soto, desde agosto de 2026.** Lo dice el propio
  medio: «Con la llegada de Ángela María Mora Soto a la gerencia, Inravisión
  arranca un ciclo…» (2026-08-14) y «Por instrucciones de la Gerente, Angela
  María Mora Soto…» (2026-08-31). La nombró el Gobierno De la Espriella. El
  número del decreto **no entra** (ver abajo). El cargo es **gerente**, no
  «director general».
- **La norma de constitución que se citaba era otra.** El enlace de Función
  Pública (`i=82339`) carga, pero es el «Concepto Sala de Consulta C.E. 00101 de
  2016», sobre los recursos que la ANTV transfería a RTVC. La sustituye el
  **Decreto 3912 de 2004** del normograma de MinTIC. El **Decreto 3525 de
  2004**, que autorizó la sociedad, figura «declarado NULO por el Consejo de
  Estado, Sección Primera, mediante Sentencia de 27 de enero de 2011» en ese
  normograma. La sentencia no se ha leído.
- **El registro mercantil la inscribe como S.A.S.** (RUES, actualizado el
  2026-08-21). Choca con «sociedad entre entidades públicas». Se declara como
  tensión.
- **Rectificó por orden judicial lo que publicó en abril de 2026.** No es «el
  Estado rectificando a un medio privado», como decía esta ficha: es el medio
  rectificando su propia información del 19, 21 y 26 de abril de 2026, por una
  sentencia de tutela de segunda instancia del Tribunal Superior de Bogotá
  (30-07-2026), a petición de la Fundación La Silla Vacía (pieza del
  2026-08-31).
- **La MOE de la Unión Europea** describió a los medios estatales (Señal
  Colombia y Radio Nacional) favoreciendo «al presidente, al Gobierno y a
  Cepeda» en la primera vuelta (declaración del 02-06-2026), y otra vez al
  presidente y a su Gobierno en la segunda (23-06-2026).
- **Cada cambio de gobierno trae otra redacción.** Cierre de la franja
  informativa y de opinión (15-08-2026), terminación anticipada de contratos
  periodísticos (10-09), demanda ante la SIC y denuncia ante la Fiscalía contra
  dos excontratistas (15-09) y un informativo nuevo, «RTVC Ahora» (07-10). Ver
  «Hechos estructurales».
- **El medio no estaba mudo: era nuestra vía.** Desde el 2026-09-09 entra por
  `/noticias/rss.xml`, que está vivo (ítems del 2026-10-10). El `/rss.xml` sigue
  parado (30-05-2026 y luego junio de 2024).
- **Contratista del Gobierno nacional hasta el cambio**: 14 contratos por
  $30.422 millones en 12 meses, todos firmados antes del 07-08-2026. Ver
  «Contratación pública».

**Lo que NO entra como hecho:**

- **El «Decreto 1196 del 12 de agosto de 2026»** como acto de nombramiento de la
  gerente. Solo lo dan Pulzo (nota marcada como «curada con apoyo de
  inteligencia artificial») e Infobae, sin fuente primaria. Que la nombró el
  Gobierno De la Espriella sí consta: el medio la presenta desde el 14-08 y su
  gerente lo nombra el Ejecutivo por decreto (Resolución RTVC 0461 de 2016).
- **La «auditoría editorial» de MinTIC con retirada de contenidos.** Solo la da
  Pulzo. La fuente primaria (el propio medio, 16-08-2026) dice «Revisión
  inmediata de los contenidos y formatos actualmente al aire», sin «auditoría»
  ni «retirar».
- **Lo que «halló» el Tribunal** en la tutela, citado de Pulzo (nota curada con
  IA). Entra solo lo que dice la rectificación.
- **La vinculación de contratistas recientes con la campaña de De la
  Espriella** (Pulzo, 2026-10-08). No consta en fuente que la acredite, y aquí
  no se nombra a personas naturales.
- **El estudio de La Silla Vacía sobre la cobertura de Cepeda.** Solo se conoce
  por Pulzo; la fuente original no se consulta por las reglas del proyecto.
- **Que la forma «SAS» suponga un cambio de naturaleza jurídica.** No consta el
  acto.
- **Cuántos contratos periodísticos se terminaron.** SECOP II no lo refleja; el
  hecho descansa en el comunicado del 10-09.
- **D1 y D3 a D8 del revisor** como piezas «favorables» al Gobierno De la
  Espriella: son transcripción atribuida de anuncios, igual que cientos de la
  etapa Petro. No suman a ningún lado.

### HISTORIA DE LA FICHA

- **2026-08-08.** Previsión del responsable editorial (oficialismo con el nuevo gobierno) y
  decisión de mantener el nombre RTVC.
- **2026-09-09.** La ficha proponía «no firmar» el −0,35 y marcarlo «sin
  medir». Decía que «no se sabe quién lo dirige», que el medio llevaba «seis
  piezas, y ninguna política» y que la comprobación del cambio «no se puede
  hacer». Lo de la ingesta (Google News, ocho días sin piezas, cadencia
  artificial, ausente del sitio) se resolvió el mismo 2026-09-09 al pasar a
  `/noticias/rss.xml`, aunque la ficha no se actualizó hasta hoy.
- **2026-09-16.** El responsable editorial decide «sin medir» (`bias: null`), aplicado el 09-18.
- **2026-10-10.** Revisión externa del ciclo 2, barrido de 12 meses y decisión
  del responsable editorial: **+0,30, sin firmar, «gubernamental»**, por la excepción nueva del
  protocolo. Errores de la versión anterior, para no repetirlos: la fuente
  `i=82339` no era la norma de constitución; faltaban la nulidad de 2011 y la
  forma SAS del RUES; el cargo es «gerente», no «director general»; la
  rectificación es suya, por tutela, y no a un medio privado; y la refutación
  que pedía mover el número a la derecha «por favorecer al entrante» contradecía
  el polo fijo tal como estaba (hoy lo ordena la excepción, con su marca).

### REVISIÓN EXTERNA

☑ **Ciclo 2 hecho** (Claude Opus 5.5, resuelto el 2026-10-10):
`revision-externa/respuestas/opus-5-5-rtvc.md`. Siete objeciones, todas
aceptadas en lo esencial: la norma de constitución (1), la gerente (2), el
oficialismo a los dos lados (3, con el recuento rehecho en el barrido), la MOE
UE (4), la rectificación (5), el nivel 2 obsoleto (6) y la forma SAS (7). La
resolución proponía 0,00; **el responsable editorial decidió +0,30 con la marca «gubernamental»**,
por la excepción del protocolo del mismo día. El revisor, el verificador y el
autor de esta ficha son de la misma casa: su acuerdo no es aval.
