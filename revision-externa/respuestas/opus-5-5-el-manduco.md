# Respuesta — Claude Opus 5.5 sobre El Manduco

| | |
|---|---|
| **Modelo** | Claude Opus 5.5 |
| **Versión exacta** | `claude-opus-5-5` |
| **Fecha de la consulta** | 2026-10-10 |
| **Quién la hizo** | Claude Code, a petición del responsable editorial (ciclo 2, fase 2, tanda 7; revisor de la misma casa que el autor de las fichas, ver DECISIONES.md 2026-10-07) |
| **¿Tuvo acceso a la red?** | sí |

> **Se pega LITERAL lo que devolvió el modelo, sin editar ni resumir.** Si se
> recorta, se pierde justo lo que pueda incomodar. Los comentarios nuestros van
> al final, en la sección de resolución, claramente separados.
>
> **Edición:** retirados enlaces que pueden mostrar documentos de identidad (PROTOCOLO, Datos personales, 2026-10-10).

---

## RESPUESTA LITERAL

```
DECLARACIÓN PREVIA DE CONFLICTO
Soy Claude Opus 5.5 (claude-opus-5-5), de Anthropic: la misma casa que el modelo que escribió la ficha. Mi acuerdo no debe usarse como aval. Para compensarlo, he buscado sobre todo en fuentes que la ficha NO usa: RUES abierto, SECOP I y SECOP II, la API pública del WordPress del medio, su feed RSS, la página de créditos y la Wayback Machine. Fecha de todas las comprobaciones: 2026-10-10.

MÉTODO Y DÓNDE BUSQUÉ
- robots.txt de elmanduco.com.co (2026-10-10): «User-agent: * / Disallow: /imunify-bot-check» y un bloque Yoast con «Disallow:» vacío. No excluye a ClaudeBot, Claude-Web ni anthropic-ai, así que descargué.
- Descargas con curl -sL y User-Agent de navegador, a t7\manduco-dl:
  - portada https://elmanduco.com.co/
  - https://elmanduco.com.co/feed/
  - https://elmanduco.com.co/wp-json/wp/v2/posts (las 138 entradas: fecha, título, categorías)
  - /wp-json/wp/v2/pages, /wp-json/wp/v2/categories y /wp-json/wp/v2/users
  - la página https://elmanduco.com.co/manduco-media-group/ (créditos) y /radio/
  - el contenido de las categorías Política (20), Editorial (23) y Opinión (10) entre 2025-10-10 y 2026-10-10
  - búsquedas internas de la API (?search=) con estos términos: Guaviare, «San José del Guaviare», Codechocó/Codechoco, DISPAC, «Distribuidora del Pacífico», «Cámara de Comercio», Abelardo, Petro, Cepeda, «De La Espriella»
- Probé la portada y el feed con cuatro User-Agent: curl, python-requests, Feedparser y vacío. Los cuatro dieron HTTP 200.
- Wayback Machine, API CDX (web.archive.org/cdx), de elmanduco.com.co/* desde 2026-08.
- RUES (datos.gov.co c82u-588k): razón social que contenga «MANDUCO»; después, por NIT exacto.
- SECOP II (jbjy-vk9h): documento_proveedor = 901563146, igualdad exacta y sin dígito de verificación. También por documento_proveedor igual al documento del representante legal que da el RUES. Lo comparé por máquina y no lo transcribo. Además busqué por nombre (proveedor_adjudicado) en el departamento del Chocó: «DIAZ CA_ADAS», «GONZALO ANDRES DIAZ», «MARVIN», «DIAZ CARRASCO» y «CARLOS VICENTE DIAZ».
- SECOP I (f789-7hwg): identificacion_del_contratista = 901563146, y el documento del representante legal (RUES), por igualdad exacta.
- Buscador web: una sola consulta, «"El Manduco" periódico Quibdó Chocó», con eltiempo.com, cambiocolombia.com, lasillavacia.com y diariodelsur.com.co excluidos. Estuvo disponible.
- INCIDENCIA QUE DECLARO: descargué por error un PDF de quibdo-choco.gov.co («Listado de medios locales de Quibdó») antes de leer su robots.txt. Ese robots.txt dice «User-agent: *» seguido de «Disallow: /». Borré el archivo sin abrirlo y no uso su contenido. Lo que digo de ese documento sale solo del resumen del buscador, y lo marco como no verificado.
- Cito siempre del HTML o el JSON crudo. Por la Ley 1581 no transcribo cédulas ni la dirección física que el sitio publica: me limito a decir «Quibdó, Chocó».

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré evidencia de ningún cambio. La sociedad editora sale en el RUES (c82u-588k, consultado el 2026-10-10) como MANDUCO MEDIA GROUP S.A.S., NIT 901563146, Cámara de Comercio del Chocó, matrícula 6246212 del 2022-02-07, renovada el 2026-04-21, último año renovado 2026, estado «ACTIVA». El RUES abierto no publica a los accionistas.
  Lo que sí cambió es la plataforma, no el dueño. El WordPress actual empieza en febrero de 2026: la página «sample-page» es del 2026-02-26 y la portada «inicio» del 2026-03-04, según /wp-json/wp/v2/pages. Además, la Wayback guarda URL antiguas (/2020/11/26/…, /2023/02/23/…) que hoy dan 404. Inferencia: en 2026 se rehízo el sitio y se perdió el archivo anterior.
- La persona que la ficha nombra como titular o director, ¿sigue viva y en el cargo? (comprobado el 2026-10-10)
  Los créditos de https://elmanduco.com.co/manduco-media-group/ (página creada el 2026-04-29) dicen hoy: «Director :Gonzalo Díaz García» y «Gerente :Marvin Díaz García».
  El RUES da como representante legal a «GONZALO ANDRES DIAZ GARCIA» (actualización del 2026-04-21).
  «Jhon Diaz C.», el director emérito según los créditos, firma una columna del 2026-10-04. «Gonzalo Diaz Cañada» es el usuario que publica todas las entradas; la última es del 2026-10-06.
  Del fundador, Carlos Díaz Carrasco, no encontré ningún dato sobre su estado actual.
- ¿Quién dirige hoy la redacción?
  Según los créditos, «Jefe de redacción :Carlos Vicente Diaz» (https://elmanduco.com.co/manduco-media-group/, 2026-10-10).
  Un listado de medios locales de la Alcaldía de Quibdó nombra como director a «Jorge Díaz Cañadas». Ese dato viene SOLO del resumen del buscador, sin fecha y sin verificar, por la exclusión de robots descrita arriba. En los créditos actuales del sitio, Jorge Díaz Cañadas figura como «Jefe de publicidad».
- ¿Hay un registro mercantil o un reporte de emisor más reciente que la fuente que la ficha cita?
  Sí. La ficha no cita ningún registro y dice «Falta la sociedad». El RUES la tiene, renovada el 2026-04-21 (ver Objeción 3).

## OBJECIONES

OBJECIÓN 1 — El medio no es del Guaviare: es de Quibdó (Chocó)
- QUÉ afirma la ficha: «El Manduco (San José del Guaviare)», «Departamento | Guaviare — sería el primero del departamento», «En un departamento de 90 000 habitantes», «un medio pequeño de una familia en la Amazonía-Orinoquía». En la refutación propone mirar «la Gobernación del Guaviare y la Alcaldía de San José» y «el certificado de Cámara de Comercio del Guaviare».
- POR QUÉ es incorrecto:
  1) El pie del sitio, en el HTML crudo de la portada y de /manduco-media-group/, dice: «Barrio Obapo - sector Casablanca Quibdó - Chocó - Colombia». Omito la calle.
  2) El RUES registra la sociedad en la «CAMARA DE COMERCIO: CHOCÓ».
  3) De las 138 entradas que da la API, ninguna contiene «Guaviare»: /wp-json/wp/v2/posts?search=Guaviare devuelve []. Las categorías del sitio son «Actualidad Chocó», «Cronicas Chocoanas», «Pacífico» y «Quibdó».
  4) Los diez artículos del feed tratan del Chocó; por ejemplo, «Un chocoano nuevo Magistrado de la Corte Suprema de Justicia» (2026-10-01) y «QUE EL CHOCÓ RESURJA» (2026-09-25).
  5) Todos sus contratos públicos son con entidades del Chocó (Objeción 5).
  Con esto se cae el argumento demográfico de la ficha (90 000 habitantes, Amazonía-Orinoquía), y su plan de refutación apunta a una gobernación, una alcaldía y una cámara de comercio que no son las suyas.
- FUENTES Y FECHAS: https://elmanduco.com.co/ y https://elmanduco.com.co/manduco-media-group/ (descargadas el 2026-10-10); [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (2026-10-10); https://elmanduco.com.co/wp-json/wp/v2/posts?search=Guaviare (2026-10-10).
- NIVEL: propiedad / registro externo (RUES) y declaración del propio medio.

OBJECIÓN 2 — «Sin feed» y «conducta 0»: el medio está vivo y publica; el cero es de la ingesta, no del medio
- QUÉ afirma el expediente: según el contexto del encargo, no tiene feed desde el 2026-09-02, el sitio devolvía HTTP 500 y su última pieza conocida era de marzo de 2026. La conducta medida dice «0 artículos, 0 historias» entre el 2026-08-31 y el 2026-10-10.
- POR QUÉ es incorrecto hoy:
  1) Hoy responde todo con 200: la portada, /feed/ y /wp-json/wp/v2/posts. Las variantes http:// y www. también, porque redirigen a https://elmanduco.com.co/.
  2) El feed trae 10 entradas. La más reciente: «El viacrucis del Largometraje «Tierra Amarga»…», con fecha Tue, 06 Oct 2026 21:50:35 +0000.
  3) La API da X-WP-Total: 138. Por mes: 2026-08: 11, 2026-09: 20, 2026-10: 6. Son 37 entradas desde el 1 de agosto y unas 24 dentro de la ventana medida.
  4) La caída sí existió. La Wayback guarda /radio/ con estado 500 el 20260828154917, pero desde el 20261001 la portada, /feed/ y /radio/ salen con 200.
  5) Hoy responde 200 con los User-Agent curl, python-requests, Feedparser y vacío, así que no parece que el sitio bloquee a los rastreadores.
  Inferencia: hubo una caída real hacia finales de agosto y principios de septiembre, ya superada, y la ingesta no reintentó. No puedo saber si las entradas fechadas en septiembre se publicaron durante la caída o se cargaron con fecha atrasada después.
- FUENTES Y FECHAS: https://elmanduco.com.co/feed/ (2026-10-10); cabecera X-WP-Total de https://elmanduco.com.co/wp-json/wp/v2/posts?per_page=1 (2026-10-10); http://web.archive.org/cdx/search/cdx?url=elmanduco.com.co/*&from=202608 (consultada el 2026-10-10).
- NIVEL: conducta observable. Además invalida el «0 artículos» como dato sobre el medio.

OBJECIÓN 3 — «Falta la sociedad: ni razón social, ni NIT, ni matrícula» es falso
- POR QUÉ: el RUES da razón social «MANDUCO MEDIA GROUP S.A.S.», NIT 901563146, matrícula 6246212, fecha de matrícula 20220207, fecha de renovación 20260421, estado «ACTIVA».
  Actividades CIIU: principal 7310 (publicidad), secundaria 6010 (radio). Representante legal: «GONZALO ANDRES DIAZ GARCIA», que es el «Director» de los créditos.
  El nombre coincide con la página del propio sitio «Manduco Media Group» (/manduco-media-group/). El objeto de sus contratos menciona «las plataformas digitales que conforman MANDUCO MEDIA GROUP».
  Los socios siguen sin estar documentados: el RUES abierto no los publica. Hace falta el certificado de existencia de la Cámara de Comercio del Chocó, no del Guaviare.
- FUENTE Y FECHA: [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (registro actualizado el 2026/04/21; consultado el 2026-10-10).
- NIVEL: propiedad (registro mercantil del presente).

OBJECIÓN 4 — No son «cuatro cargos» ni salen de la «cabecera»: son siete, todos Díaz, en una página de créditos
- QUÉ afirma la ficha: «Los cuatro cargos del medio los ocupan cuatro Díaz». Fuente: «la propia cabecera de elmanduco.com.co».
- POR QUÉ: hoy la portada no muestra los créditos. En el HTML crudo de https://elmanduco.com.co/ no aparecen «Carrasco», «Marvin» ni «Gerente». Están en https://elmanduco.com.co/manduco-media-group/, bajo «CREDITOS», y son siete:
  «Fundador : Carlos Díaz Carrasco / Director hemerito : Jhon Díaz Cañadas / Director :Gonzalo Díaz García / Gerente :Marvin Díaz García / Jefe de publicidad :Jorge Díaz Cañadas / Jefe de redacción :Carlos Vicente Diaz / Comunity manager :Gonzalo Díaz Cañadas».
  La tesis de la ficha (control familiar, sin contrapeso interno) se refuerza: también la redacción y la publicidad están en la familia. Hay que corregir el número de cargos y la URL de la fuente.
  Ojo con una posible confusión. «Gonzalo Díaz García» (director y representante legal) y «Gonzalo Díaz Cañadas» (community manager, autor de las crónicas, usuario «Gonzalo Diaz Cañada» que publica todo) son dos personas distintas en los créditos.
  Que sean parientes es una inferencia por el apellido. No tengo un documento que pruebe el parentesco.
- FUENTE Y FECHA: https://elmanduco.com.co/manduco-media-group/ (página creada el 2026-04-29 según /wp-json/wp/v2/pages; descargada el 2026-10-10).
- NIVEL: declaración del propio medio, con apoyo de la propiedad.

OBJECIÓN 5 — La «comprobación decisiva» que la ficha deja pendiente se puede hacer, y da resultado: la sociedad y su director viven de contratos con entidades públicas del Chocó, y el medio publica a sus contratantes
- QUÉ afirma la ficha: su refutación 1 pide «Comprobar si algún miembro de la familia Díaz tiene o tuvo cargo, contrato o candidatura». El CONTRA supone que el interés estará «en la política local». La conclusión práctica de la ficha («0,00… no sé hacia dónde tira») no registra ningún conflicto.
- HECHOS (SECOP, consultado el 2026-10-10):
  a) La sociedad, MANDUCO MEDIA GROUP (NIT 901563146):
     SECOP II, contratos con EMPRESA DISTRIBUIDORA DEL PACIFICO S.A. E.S.P (DISPAC; NIT de la entidad 818001629; SECOP la clasifica como orden «Territorial», sector «Minas y Energía»):
     - DG-040-2024, firmado el 2024-02-19, 8.800.000 COP.
     - DG-043-2025, firmado el 2025-02-19, 9.020.000 COP.
     - DG-033-2026, firmado el 2026-01-26, 10.332.000 COP, «En ejecución» hasta el 2026-12-31.
     El objeto de los tres es el mismo: «emisión de cuñas y la publicidad de audios; videos; imágenes; flyer y piezas gráficas en las plataformas digitales que conforman MANDUCO MEDIA GROUP; sobre los contenidos estratégicos; informativos y pedagógicos de la empresa DISPAC».
     SECOP I, contratos con la CÁMARA DE COMERCIO DEL CHOCÓ (la misma cámara que lleva su registro mercantil), para difusión:
     - OPS 037 DE 2022, firmado el 2022-09-01, 1.400.000 COP.
     - CPS 001 DE 2025, firmado el 2025-01-02, 8.000.000 COP.
     - Contrato firmado el 2026-01-02 por 9.500.000 COP, publicado con el número «CPS 001 DE 2025» y con objeto la jornada de renovación de 2026.
     Total histórico de la sociedad: 47.052.000 COP. Últimos 12 meses (desde el 2025-10-10): 19.832.000 COP, que son DG-033-2026 más el contrato del 2026-01-02.
  b) El director y representante legal, GONZALO ANDRES DIAZ GARCIA, a título personal. La identidad está comprobada: el documento del proveedor en SECOP II coincide con el del representante legal en el RUES. No lo transcribo.
     SECOP II, CORPORACIÓN AUTÓNOMA REGIONAL PARA EL DESARROLLO SOSTENIBLE DEL CHOCÓ (CODECHOCÓ), 10 contratos entre el 2021-10-08 y el 2026-01-30, por un total de 133.613.000 COP. Todos son de prensa, audiovisual o «manejo de emisoras web».
     El vigente: CPS 070-2026, firmado el 2026-01-30, 32.890.000 COP, «En ejecución» hasta el 2026-12-31. Objeto: «PRESTACIÓN DE SERVICIOS PERSONALES Y DE APOYO A LA GESTIÓN DE UN(A) PERSONA NATURAL CON EXPERIENCIA EN LA EDICIÓN DE VIDEOS Y MANEJO DE EMISORAS WEB…».
     SECOP I, Cámara de Comercio del Chocó: OPS 015 DE 2023, firmado el 2023-01-10, 5.000.000 COP.
     Últimos 12 meses a título personal: 32.890.000 COP. El CPS 124-2025, firmado el 2025-10-01 por 8.541.000 COP, cae nueve días antes de la ventana.
  c) «john diaz cañadas», contratista de DISPAC: orden de servicios No. 010-2020 (2020-04-03, 2.700.000 COP) y CPS-051-2022 (2022-01-28, 3.500.000 COP), con el mismo objeto publicitario que hoy tiene la sociedad. Que sea el director emérito de los créditos es probable, pero no está probado con documento: puede ser un homónimo. Queda fuera de la ventana de 12 meses.
- CONDUCTA OBSERVABLE LIGADA A ESOS CONTRATOS:
  1) «Mejoras programadas por DISPAC para fortalecer el servicio de energía» (2026-03-04, https://elmanduco.com.co/2026/03/04/mejoras-programadas-por-dispac-para-fortalecer-el-servicio-de-energia/) es el comunicado de DISPAC publicado como noticia, en primera persona: «realizaremos trabajos de mantenimiento… nuestro equipo técnico… Importante: este Facebook estará activo hasta el 31 de marzo». Se publicó mientras estaba vigente DG-033-2026, que paga justamente eso.
  2) «Atrato, Cantón de San Pablo, Juradó y Riosucio representarán las subregiones ante el Consejo Directivo de Codechocó» (2026-03-04, https://elmanduco.com.co/2026/03/04/atrato-canton-de-san-pablo-jurado-y-riosucio-representaran-las-subregiones-ante-el-consejo-directivo-de-codechoco/) es una nota institucional de la entidad que contrata a su director.
  3) «UTCH y Señal Memoria de RTVC formalizan alianza…» (2026-08-04), en la categoría «Editorial», celebra «las gestiones del director del Archivo Fotográfico y Fílmico del Chocó, Gonzalo Diaz Cañadas». Es decir, el community manager del medio se cubre a sí mismo en su cargo de la UTCH.
  En el barrido de títulos no encontré ninguna pieza que fiscalice a DISPAC, a CODECHOCÓ ni a la Cámara de Comercio del Chocó.
- POR QUÉ IMPORTA: no mueve el eje izquierda-derecha. La regla 1 del protocolo impide deducir la línea del dueño. Pero contradice dos cosas de la ficha:
  - «basta con que un Díaz tenga un interés»: el interés existe y está documentado, y es de dinero, no de candidatura.
  - el 0,00 sin tensión declarada: según el contexto, la cobertura de quien contrata al dueño es «evidencia de primer orden».
  La ficha debería declarar el conflicto, como se hizo con Diario La Libertad.
  CANDIDATURAS: no las comprobé. No consulté la Registraduría ni Cuéntame; lo declaro como hueco.
- FUENTES Y FECHAS:
  - [enlace retirado: puede mostrar documentos de identidad; ver la resolución]
  - [enlace retirado: puede mostrar documentos de identidad; ver la resolución]
  - SECOP II, consulta por el documento del representante legal (no publico la URL porque contiene la cédula). Entidad CODECHOCÓ, contratos CPS 070-2026, CPS 124-2025, CPS 071-2025, CPS 181-2024, CO1.PCCNTR.5876105, CPS-206-2023, CO1.PCCNTR.4554350, CO1.PCCNTR.3946480, CO1.PCCNTR.3555010 y CO1.PCCNTR.2921877.
  - Todas consultadas el 2026-10-10.
- NIVEL: propiedad (intereses del titular), registro externo (SECOP) y conducta observable.

OBJECIÓN 6 — «Su feed devolvió artículos de hace 66 horas» y «No está ingerido» no son dos fotos de un medio intermitente
Menor, y complementa la Objeción 2. La ficha del 2026-08-09 vio el feed vivo. El expediente actual lo da por muerto desde el 2026-09-02. El ritmo de publicación según la API es estable: 16 en junio, 10 en julio, 11 en agosto y 20 en septiembre de 2026. El problema está en la captura, no en el medio. Si la ingesta se reanuda, la ventana de 90 días podría tener unas 40 piezas, menos de las 60 historias que pide la refutación 3 de la ficha. Esto último es una inferencia a partir del ritmo.
- FUENTE Y FECHA: /wp-json/wp/v2/posts?per_page=100, páginas 1-2 (2026-10-10).
- NIVEL: conducta observable.

## LO QUE NO PUDE VERIFICAR
- Los accionistas de MANDUCO MEDIA GROUP S.A.S. El RUES abierto no los publica y no pedí el certificado de la Cámara de Comercio del Chocó, que es de pago.
- El parentesco entre los siete Díaz de los créditos, y si «john diaz cañadas» (SECOP II, DISPAC 2020 y 2022) es el «Jhon Díaz Cañadas» de los créditos. La identidad solo la comprobé por documento en el caso de Gonzalo Andrés Díaz García.
- Candidaturas o cargos de elección de cualquiera de los Díaz. No consulté la Registraduría.
- Si alguno de los Díaz ocupa un cargo de planta en una entidad pública. La pieza del 2026-08-04 llama a Gonzalo Díaz Cañadas «director del Archivo Fotográfico y Fílmico del Chocó» de la UTCH, pero no lo comprobé en ninguna fuente oficial de la UTCH.
- Busqué por nombre en SECOP II solo en el Chocó: «DIAZ CARRASCO» devuelve contratos de otra persona con la Alcaldía de Quibdó. No figura en los créditos y no pruebo parentesco, así que no lo cuento. «MARVIN» y «CARLOS VICENTE DIAZ» no devuelven nada.
- Cuándo exactamente estuvo caído el sitio: la Wayback solo tiene el 500 del 2026-08-28 y el 200 del 2026-10-01.
- El listado de medios de la Alcaldía de Quibdó, en el que Jorge Díaz Cañadas figuraría como director: lo excluí por robots.
- Las redes sociales que enlaza el sitio (Facebook «manduqueromenor», X «@Manduqueromenor», Instagram «periodicoelmanduco», YouTube «@periodicoelmanduco7331»): no las descargué. El buscador muestra el perfil de X con actividad de octubre de 2026 (la nota del magistrado), pero eso no lo verifiqué en el HTML crudo.

## LO QUE FALTA
- Corregir el departamento a Chocó (Quibdó) y rehacer el plan de refutación: Gobernación del Chocó, Alcaldía de Quibdó, Cámara de Comercio del Chocó.
- La sociedad (Objeción 3) y sus contratos públicos (Objeción 5): DISPAC y la Cámara de Comercio del Chocó para la empresa, CODECHOCÓ para su director. Hay que declararlos como conflicto de interés junto a la ficha.
- Que la conducta medida en 0 se debe a un fallo de ingesta, no a la inactividad del medio. Volver a dar de alta el feed https://elmanduco.com.co/feed/.
- Que existe una extensión radial («RADIO» en el sitio; CIIU 6010 en el RUES).

## EVIDENCIA QUE NO MUEVE EL NÚMERO
Regla de evidencia editorial histórica: NO se cumple, y lo documento.
- Barrido: todas las entradas de las categorías Política, Editorial y Opinión entre el 2025-10-10 y el 2026-10-10 (35 piezas; la lista completa sale de /wp-json/wp/v2/posts?categories=20,23,10), más las búsquedas Petro, Abelardo, Cepeda y «De La Espriella».
- La voz de la casa sobre política nacional casi no existe. Las piezas sin firma o firmadas por la casa con postura son de identidad regional, no de eje izquierda-derecha:
  1) «El Viacrusis de Luis Gilberto Murillo», firmada «Redacción El Manduco», 2026-04-08: encuadre favorable a un candidato presidencial chocoano. https://elmanduco.com.co/2026/04/08/el-viacrusis-de-luis-gilberto-murillo/
  2) «James Mosquera Torres: La fuerza del mandato de las víctimas…», sin firma, 2026-03-14: favorable al representante elegido. https://elmanduco.com.co/2026/03/14/james-mosquera-torres-la-fuerza-del-mandato-de-las-victimas-en-la-camara-de-representantes/
  3) «Luis Enrique Abadía García: una candidatura que pone al Pacífico…», sin firma, 2026-08-10: favorable a un aspirante chocoano a la Contraloría. https://elmanduco.com.co/2026/08/10/luis-enrique-abadia-garcia-una-candidatura-que-pone-al-pacifico-en-el-centro-del-debate-por-el-control-fiscal-de-colombia/
  4) «¿Por qué seguimos escogiendo a los mismos?», de Jhon Diaz C., director emérito, 2026-10-04: «He decidido escribir esta invitación sin mencionar nombres… No es una invitación a votar por alguien». Es anticorrupción local, sin partido. https://elmanduco.com.co/2026/10/04/por-que-seguimos-escogiendo-a-los-mismos-porjhon-diaz/
  Son menos de 10 piezas, ninguna sitúa al gobierno saliente frente al entrante y su eje es el «chocoanismo». No se cumple la regla, y el 0,00 queda donde está.
- Boletines oficiales reproducidos a ambos lados del cambio de gobierno, de forma simétrica:
  - Antes: «Presidente Petro promulga nueva ley…» (2026-03-04) y «El Pacífico tiene CONPES por 12,3 billones…» (2026-03-17, «el Gobierno del presidente Gustavo Petro aprobó el Conpes 4185»).
  - Después: «Ministerio de Minas y Energía y el Grupo Energía Bogotá fortalecen el respaldo eléctrico…» (2026-09-15, enlaza el «Comunicado completo» del GEB).
  Es conducta de boletín, no de postura.
- Columnas de terceros, que no cuentan como voz de la casa pero describen el elenco:
  - Víctor Manuel García Ayala, que se declara «marxista», escribe contra Abelardo De La Espriella y a favor de Iván Cepeda: 2026-05-27, 2026-06-20 («vamos a votar POR LA VIDA, por Iván Cepeda») y 2026-08-07 («la nueva derecha internacional ha impulsado un modelo que diversos analistas denominan ¡tecno fasci…»). El 2026-03-04 publica una sátira contra «camaleones» de la izquierda («Royirius Barreirius y Francíniairis Marquezinius»); que se refiera a Roy Barreras y a Francia Márquez es una inferencia mía.
  - Contrapesos: Yesid Francisco Perea Mosquera, «EL RENACER AZUL» (2026-03-04), a favor del Partido Conservador; Yan Arley Ramos Palacios, «¿Y si en vez de Abelardo o Pablo Pueblo…?» (2026-06-01), contra los dos polos; Olga Garcés (2026-05-13), a favor de Murillo; Astrid Sánchez Montes de Oca, representante, con una columna propia (2026-09-25).
  El elenco es plural y no hay endoso de la casa en la presidencial. No mueve el número.
- No encontré ningún endoso editorial del medio en la elección presidencial de 2026.

## SIN OBJECIÓN
No aplica: presento seis objeciones. Al valor 0,00 en sí no le encontré evidencia de nivel 1-3 que lo mueva en el eje. Lo que sí encontré son errores de hecho en la ficha (departamento, sociedad, cargos, estado del feed) y un conflicto de interés por contratación pública que la ficha debe declarar.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-10. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal: ninguna.** El revisor no copió cédulas, teléfonos, nacionalidades, origen étnico ni lugar de nacimiento de personas naturales. El documento del representante legal, que el RUES devuelve y que se usó solo dentro de las consultas, no aparece en el texto, y el revisor tampoco publica la URL de SECOP que lo contiene. Las cifras largas son el NIT de la sociedad (901563146) y el de DISPAC (818001629), la matrícula, fechas, cuantías e identificadores de contrato. La dirección que cita es la que el medio publica en su pie, y el revisor omite la calle; está a nivel de barrio. Se deja tal cual, pero esta resolución no la traslada a la ficha: basta con «Quibdó (Chocó)».

**Cómo se verificó.**
- **robots.txt**, leído antes de descargar nada (2026-10-10):
  - elmanduco.com.co: «User-agent: * / Disallow: /imunify-bot-check» y un bloque Yoast con «Disallow:» vacío. No excluye a ningún agente de Anthropic.
  - datos.gov.co: `Crawl-delay: 1` y exclusiones de `/browse`. Se usó solo `/resource`, respetando el segundo entre consultas.
  - web.archive.org: su robots.txt responde 404. Se usó la API `cdx`. Las capturas `id_` las bloqueó su filtro antibots, que devolvió una página de bloqueo, y no se insistió.
  - No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co ni **quibdo-choco.gov.co**, que es el dominio de la incidencia del revisor. No hubo buscador web.
- **Sitio**, en crudo con `curl -sL --ssl-no-revoke -A "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/126.0 Safari/537.36"`. Respondieron 200: la portada, `/feed/`, `/manduco-media-group/`, la pieza de DISPAC del 2026-03-04 y las cuatro piezas del barrido que el revisor enlaza.
- **API REST de WordPress:** `/wp/v2/posts?per_page=100&page=1-2` (`X-WP-Total: 138`), `?search=Guaviare`, `?search=DISPAC`, `?search=Codechocó`, `?search=Señal Memoria`, `?slug=` de las piezas de DISPAC y de CODECHOCÓ, `/wp/v2/categories`, `/wp/v2/pages` y `/wp/v2/users`.
- **Registros**, en datos.gov.co:
  - RUES (`c82u-588k`): `nit=901563146`; razón social `like '%MANDUCO%'`; `numero_identificacion` y `num_identificacion_representante_legal` iguales, de forma exacta, al documento del representante legal; y `nit=818001629` (DISPAC).
  - SECOP II (`jbjy-vk9h`): `documento_proveedor` = 901563146 y = documento del representante legal, por igualdad exacta; y `nit_entidad='818001629'` con `proveedor_adjudicado like '%DIAZ CA%'`.
  - SECOP I (`f789-7hwg`): `identificacion_del_contratista` = 901563146 y = documento del representante legal, por igualdad exacta.
- **Ingesta, solo lectura:** `npm run feed:descubrir -- elmanduco.com.co`. Antes de correrlo se leyó `scripts/descubrirFeed.mjs`. Solo hace `fetch`, solo lee del disco los argumentos que sean archivos («elmanduco.com.co» no existe como archivo) y escribe en la consola; no importa nada de la base. Resultado: «elmanduco.com.co 10 art., último hace 93 h [declarado] └─ https://elmanduco.com.co/feed/ … 1 de 1 con feed vivo.», sin el aviso «sin fechas legibles». Usa el User-Agent de la ingesta, `DobleFocoBot/1.0`.
- **Detector del mapa:** `detectarDepartamento` (`shared/geografia.js`) sobre los 138 titulares de la API da Chocó en 64, ninguno en 61, Cundinamarca en 7, Magdalena en 3, y Antioquia, Valle del Cauca y Bogotá en 1 cada uno. **Guaviare: 0.**
- **Repositorio:** `fichas/el-manduco.md`; las entradas `el-manduco` de `shared/mediaRegistry.js`, `shared/mediaOwnership.js` y `shared/centinela.js`; `fichas/choco-7-dias.md`; `fichas/LEEME.md`; `COBERTURA_DEPARTAMENTAL.md`; `MEDIOS_CANDIDATOS_DEPARTAMENTOS.md`; `BARRIDO_NACIONAL.md`; `auditoria/estado.json`, `auditoria/hallazgos.json` y `centinela/estado.json`; el archivo de conducta de `backup/2026-09-01…`; la decisión del 2026-09-02 (commit `b775ee1`; `../MINUTA.md`, líneas 3044-3070 y 3235-3250); y el commit de origen de la candidatura (`e37ca67`, 2026-08-09).

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | El medio es de Quibdó (Chocó), no de San José del Guaviare | sí | sí | **Aceptada.** Pie del sitio, RUES (Cámara del Chocó), 0 de 138 entradas con «Guaviare», 64 titulares que el detector del mapa sitúa en el Chocó y ninguno en el Guaviare. No hay ningún El Manduco del Guaviare en el RUES. **Es un error de geografía del catálogo desde el alta, el 2026-08-09** |
| 2 | El sitio responde, publica y tiene feed; el cero es de la ingesta | sí | sí | **Aceptada, con una precisión.** Feed 200 con 10 ítems, el último del 2026-10-06 21:50:35 UTC; 138 entradas; 11, 20 y 6 en agosto, septiembre y octubre. Wayback: 500 el 2026-08-28 y 200 desde el 2026-10-01. En la ventana caen **26** piezas, no «unas 24». El repositorio ya sabía que el sitio había vuelto (ver abajo) |
| 3 | La sociedad existe: MANDUCO MEDIA GROUP S.A.S. | sí | sí | **Aceptada.** Todas las cifras coinciden. El RUES abierto no tiene campo de municipio; da la cámara (código 29, CHOCÓ) |
| 4 | Siete cargos, no cuatro, y no en la «cabecera» | sí | sí | **Parcial.** Son siete y todos Díaz: exacto. **Pero es falso que la portada no los muestre:** el bloque «CREDITOS» está en el pie de todas las páginas, también en el HTML crudo de la portada descargado hoy. La ficha se equivoca en «cabecera» (es el pie) y en «cuatro»; la URL que cita sí sostiene lo que afirma |
| 5 | Contratación pública de la sociedad y del director; el medio publica a sus contratantes | sí | sí | **Aceptada en los hechos, con dos precisiones.** Cuantías exactas al peso. Dos de los diez contratos con CODECHOCÓ no son de prensa ni de audiovisual por su objeto. Y la regla de la «cobertura del propio accionista» no se extiende a quien contrata: la vía es la línea de contratación del protocolo, más una tensión |
| 6 | El feed no es intermitente; el fallo es de captura | sí | sí | **Parcial.** El ritmo es estable (16, 10, 11 y 20 piezas de junio a septiembre). Pero el cero de la ventana no es un «fallo de captura»: es **la retirada deliberada del feed el 2026-09-02**, tras una caída real que no se revisó cuando el sitio volvió |

### Lo verificado, objeción por objeción

**1 · Departamento.**
- **Pie del sitio**, en el HTML crudo de la portada y de `/manduco-media-group/` (2026-10-10), literal: «Barrio Obapo - sector Casablanca Quibdó - Chocó - Colombia».
- **RUES**, `nit=901563146`, literal: «"codigo_camara":"29"», «"camara_comercio":"CHOCÓ"», «"matricula":"6246212"», «"razon_social":"MANDUCO MEDIA GROUP S.A.S."». El conjunto `c82u-588k` no tiene campo de municipio: el dato registral es la cámara, y la del Chocó es la de ese departamento. El municipio, Quibdó, sale del pie.
- **Contenido:** `/wp/v2/posts?search=Guaviare` devuelve `[]` (la búsqueda de WordPress cubre título y cuerpo). Ningún título de los 138 contiene «Guaviare». Las categorías con contenido incluyen «Actualidad Chocó» (35), «Cronicas Chocoanas» (33), «Pacífico» (6) y «Quibdó» (1). Los diez títulos del feed son del Chocó o del Pacífico: por ejemplo, «Un chocoano nuevo Magistrado de la Corte Suprema de Justicia» (2026-10-01) y «QUE EL CHOCÓ RESURJA. Por:Astrid Sánchez Montes de Oca,Representante a la Cámara por el Chocó» (2026-09-25).
- **Detector del mapa** (`detectarDepartamento`): Chocó 64, Guaviare 0.
- **Antes de 2026:** la Wayback (CDX) guarda la portada con 200 desde el 2020-08-07, y URL antiguas con temas chocoanos, como `/2023/02/23/la-minera-choco-pacifico-y-sus-andanzas-por-bebedo-…`. El contenido de esas capturas no se pudo abrir por el bloqueo antibots.
- **¿Hubo alguna vez un El Manduco del Guaviare?** No se encontró ninguno.
  - RUES por razón social «MANDUCO»: 6 filas, ninguna en el Guaviare. Son MANDUCO BAR Y LICORES LTDA. EN LIQUIDACION (Barranquilla), INVERSIONES MANDUCO Y RAMONA S.A.S. (Montería; antes Urabá), FUNDACION MANDUCO… EN LIQUIDACION (Bogotá), INVERSIONES INMOBILIARIAS MANDUCO SAS (Medellín) y MANDUCO MEDIA GROUP S.A.S. (Chocó).
  - `elmanduco.co` y `periodicoelmanduco.com` no tienen capturas.
  - `elmanduco.com` tiene capturas de 2002, cuyo contenido no se pudo abrir.
  - No consta ningún medio homónimo en el Guaviare.
- **De dónde salió el error.** No consta en el repositorio; esto es lo que se puede reconstruir:
  - La candidatura nace en la investigación del 2026-08-09 (commit `e37ca67`). Su método (`MEDIOS_CANDIDATOS_DEPARTAMENTOS.md:13-26`) comprobaba si el feed respondía y cuán fresco era, **no de dónde era el medio**.
  - La verificación con `detectarDepartamento` del 2026-08-11 (`COBERTURA_DEPARTAMENTAL.md`, sección «Siete departamentos que se pueden cerrar YA») solo se aplicó a los siete departamentos nuevos, no a los ya asignados.
  - La ficha se escribió el mismo día y construyó sobre el departamento asignado («90 000 habitantes», «Amazonía-Orinoquía», Gobernación y Cámara del Guaviare) sin abrir el contenido del medio.
  - `BARRIDO_NACIONAL.md:34` lo repitió («El Manduco publica a diario en el Guaviare»).
  - Hipótesis, no comprobada: el departamento se asignó a partir de una búsqueda por departamento, sin leer el pie ni los titulares. Los datos de 2026-08 ya decían otra cosa: `centinela/estado.json:238-261` guarda URL del medio, todas chocoanas.
- **Qué afecta** (todo con archivo:línea, en la Propuesta, punto D):
  - el Guaviare se queda sin medio propio;
  - el Chocó pasa a tener dos, con Chocó 7 Días;
  - el recuento departamental baja en uno.

  **En el código, el campo `departamento` del registro solo alimenta `alcanceDe` (`shared/mediaOwnership.js:4691-4693`)**, que lo clasifica como «regional» con cualquiera de los dos valores, y el catálogo generado (`src/docs/catalogo_medios.txt`). **El mapa de historias por departamento no usa el registro:** etiqueta cada historia por su titular (`server/services/ingestDaemon.js:1913-1916`). Así que el error no ha mandado noticias al Guaviare. Lo que ha hecho es inflar la cobertura declarada en los documentos.

**2 · El sitio y el feed.**
- `/feed/` (200, 2026-10-10): 10 `<item>`, con `pubDate` del «Fri, 25 Sep 2026 22:57:01 +0000» al «Tue, 06 Oct 2026 21:50:35 +0000». El primer título es «El viacrucis del Largometraje «Tierra Amarga»: Filmada en Quibdó en 1963…». Literal.
- API: `X-WP-Total: 138`, 138 ids únicos, del 2025-11-14 al 2026-10-06. Por mes: 2025-11: 1 · 2026-02: 2 · 03: 43 · 04: 11 · 05: 18 · 06: 16 · 07: 10 · **08: 11 · 09: 20 · 10: 6**. Exacto. **En la ventana del envío (2026-08-31 → 2026-10-10) hay 26**, no «unas 24». El pico de marzo (43, muchas fechadas el 04-03) concuerda con la reconstrucción del sitio que el revisor infiere.
- Wayback CDX desde 2026-07: `/radio/` con **500 el 20260828154917**; desde el 20261001, la portada, `/feed/` y `/radio/` con 200. Literal. Además hay un 404 (no un 500) el 20260923: ese día el servidor respondía.
- **Lo que el revisor no podía ver: el repositorio ya sabía que el sitio había vuelto.**
  - `auditoria/hallazgos.json:432-446`: el hallazgo `el-manduco/fuente/elmanduco.com.co`, «resumen» «500», tiene `primeraVez` y `ultimaVez` del 2026-09-03 y `resueltoEl` del **2026-09-17**.
  - `auditoria/estado.json:3452-3483`: comprobado el 2026-10-08, la fuente da `"status": 200` y `"estado": "sano"`.
  - `centinela/estado.json:231-261`: el centinela lo leyó por la API REST el 2026-10-06 y vio la pieza del 2026-10-04.
  - Nadie descomentó el feed porque la comprobación era «a mano» (`shared/mediaRegistry.js:1224-1226`).
- **La decisión del 2026-09-02 se tomó con dos premisas inexactas.** Constan en el commit `b775ee1`, en `../MINUTA.md:3057-3060` y 3241-3250, y en la nota de `auditoria/hallazgos.json:488`:
  - **«su última pieza conocida es de marzo de 2026» / «lleva medio año sin publicar».** El medio publicó 11 piezas en agosto (API). La ingesta las tuvo: el archivo de conducta del 2026-09-01 (`backup/2026-09-01T04-09-52-063Z/conducta_archivo.ndjson:7005` y `:22227`) registra historias con `source_id` `el-manduco` del 2026-08-17 y del 2026-08-24. El 2026-08-27, la auditoría lo describía como un medio que «publica despacio —una pieza cada 52,6 h—» (`auditoria/hallazgos.json:481`). La «pieza de marzo» salía de Google News.
  - **«cero artículos en la base»** era cierto, pero por la poda de 72 h, no porque el medio callara: es el caso que documenta `ESTUDIO_PUNTOS_CIEGOS.md:390-406`, donde El Manduco da «200 | 10 | 126 h | 0».
  - Lo que sí fue real es la caída: 500 el 2026-08-28 (Wayback) y el 2026-09-03 (auditoría), y ya resuelta el 2026-09-17.
- `npm run feed:descubrir` (hoy, con el User-Agent de la ingesta): 10 artículos, el último hace 93 h, por la vía declarada en el HTML y con fechas legibles. **Se puede reactivar.**
- No se comprobaron otra vez las variantes `http://` y `www.` ni los cuatro User-Agent del revisor; con el de navegador y con `DobleFocoBot` responde.

**3 · Sociedad.** RUES, `nit=901563146` (2026-10-10), literal: «"razon_social":"MANDUCO MEDIA GROUP S.A.S."», «"nit":"901563146"», «"digito_verificacion":"0"», «"cod_ciiu_act_econ_pri":"7310"», «"cod_ciiu_act_econ_sec":"6010"», «"fecha_matricula":"20220207"», «"fecha_renovacion":"20260421"», «"ultimo_ano_renovado":"2026"», «"organizacion_juridica":"SOCIEDADES POR ACCIONES SIMPLIFICADAS SAS"», «"estado_matricula":"ACTIVA"», «"representante_legal":"GONZALO ANDRES DIAZ GARCIA"», «"fecha_actualizacion":"2026/04/21 15:55:07.017000000"». Exacto.
- Por su documento, el representante legal no tiene matrícula propia como persona natural (`numero_identificacion`: 0 filas). Solo representa a esta sociedad (`num_identificacion_representante_legal`: 1 fila).
- El nombre coincide con la página `/manduco-media-group/` y con el objeto de los contratos de DISPAC («las plataformas digitales que conforman MANDUCO MEDIA GROUP»).
- Los accionistas no constan: el RUES abierto no los publica.

**4 · Créditos.**
- HTML crudo de `/manduco-media-group/` **y de la portada** (2026-10-10), bloque «CREDITOS» del pie, literal: «Fundador : Carlos Díaz Carrasco / Director hemerito : Jhon Díaz Cañadas / Director :Gonzalo Díaz García / Gerente :Marvin Díaz García / Jefe de publicidad :Jorge Díaz Cañadas / Jefe de redacción :Carlos Vicente Diaz / Comunity manager :Gonzalo Díaz Cañadas».
- En la portada, «Carrasco», «Marvin» y «Gerente» aparecen una vez cada uno, en ese bloque. La afirmación del revisor de que la portada no los muestra es falsa en la descarga de hoy. No se puede saber si él recibió otra variante de la página.
- `/wp/v2/pages`: `manduco-media-group` creada el 2026-04-29. `/wp/v2/users`: «Admin-principal01» (2 entradas) y «Gonzalo Diaz Cañada» (136).
- Que director y community manager son dos personas distintas lo dicen los propios créditos. **El parentesco no consta**: es una inferencia por apellido.

**5 · Contratación.** Todo es de datos.gov.co, consultado el 2026-10-10.
- **Sociedad, SECOP II** (3 filas): las tres con EMPRESA DISTRIBUIDORA DEL PACIFICO S.A. E.S.P (NIT 818001629; `orden` «Territorial», `sector` «Minas y Energía»).
  - DG-040-2024: 2024-02-19, $8.800.000, «Cerrado».
  - DG-043-2025: 2025-02-19, $9.020.000. SECOP la da «En ejecución» aunque terminó el 2025-12-31.
  - DG-033-2026 (CO1.PCCNTR.9151848): 2026-01-26, $10.332.000, «En ejecución» hasta el 2026-12-31.
  - El objeto, literal en los tres: «…emisión de cuñas y la publicidad de audios; videos; imágenes; flyer y piezas gráficas en las plataformas digitales que conforman MANDUCO MEDIA GROUP; sobre los contenidos estratégicos; informativos y pedagógicos de la empresa DISPAC».
  - En el RUES, DISPAC es «SOCIEDAD ANONIMA», E.S.P., ACTIVA, Cámara del Chocó. Su composición accionaria no se verificó aquí.
- **Sociedad, SECOP I** (3 filas): las tres con la CÁMARA DE COMERCIO DEL CHOCÓ.
  - OPS 037 DE 2022: 2022-09-01, $1.400.000, difusión de sus elecciones de junta. Constancia 22-4-13432762.
  - CPS 001 DE 2025: 2025-01-02, $8.000.000, jornada de renovación de 2025. Constancia 25-4-14289961.
  - Firmado el 2026-01-02 con el número de proceso «CPS 001 DE 2025»: $9.500.000, jornada de renovación «DE 2026». Constancia 26-4-14596220.
- **Totales de la sociedad:** $47.052.000 en 6 contratos; **$19.832.000 en 2 en los últimos 12 meses**. Exacto.
- **Director a título personal.** La consulta se hizo con el mismo documento que da el RUES, por igualdad exacta, así que **no es homonimia**. El documento no se escribe.
  - SECOP II: **10 contratos con CODECHOCÓ por $133.613.000**, del 2021-10-08 al 2026-01-30, todos con el proveedor «GONZALO ANDRES DIAZ GARCIA».
  - Vigente: **CPS 070-2026** (CO1.PCCNTR.9259070), 2026-01-30, $32.890.000, «En ejecución» hasta el 2026-12-31. Objeto literal: «…EDICIÓN DE VIDEOS Y MANEJO DE EMISORAS WEB; EN EL MARCO DE LA IMPLEMENTACIÓN DEL PLAN DE ACCIÓN INSTITUCIONAL 2024-2027».
  - CPS 124-2025: 2025-10-01, $8.541.000, nueve días antes de la ventana. Exacto.
  - SECOP I: OPS 015 DE 2023 con la Cámara de Comercio del Chocó, 2023-01-10, $5.000.000. Constancia 23-4-13451884.
  - **Total personal: 11 contratos, $138.613.000, de 2021 a 2026. En los últimos 12 meses, $32.890.000.**
- **Precisión 1:** «Todos son de prensa, audiovisual o "manejo de emisoras web"» es inexacto. Hay dos que no lo son por su objeto:
  - CO1.PCCNTR.5876105 (2024-02-05, $25.000.000): «ACTIVIDADES PROPIAS DE LA GESTIÓN AMBIENTAL…».
  - CO1.PCCNTR.3555010 (2022-02-03, $10.000.000): «PROYECTO GESTIÓN DE LA CULTURA Y EDUCACIÓN AMBIENTAL…».
  - Los otros ocho sí son de prensa, audiovisual, divulgación o emisoras.
- **«john diaz cañadas» con DISPAC:** orden de servicios No. 010-2020 (2020-04-03, $2.700.000) y CPS-051-2022 (2022-01-28, $3.500.000). Exacto. No se comprobó por documento, así que no entra: es homonimia posible y está fuera de los 12 meses.
- **La pieza de DISPAC.** https://elmanduco.com.co/2026/03/04/mejoras-programadas-por-dispac-para-fortalecer-el-servicio-de-energia/ (200). API: autor 2, categoría 7 («Actualidad Chocó»), sin etiquetas. Cuerpo literal: «Con el objetivo de seguir optimizando la calidad del servicio eléctrico, realizaremos trabajos de mantenimiento… mientras nuestro equipo técnico ejecuta las labores… Importante: este Facebook estará activo hasta el 31 de marzo. Desde ya puedes empezar a seguirnos en nuestra nueva cuenta oficial: DISPAC SA ESP…».
  - **¿Declara el medio que es contenido institucional? No.** El HTML y el JSON de la pieza no contienen «comunicado», «institucional», «patrocin», «publirreportaje» ni «contenido pagado». Las dos apariciones de «publicidad» son el pie («Jefe de publicidad», «Politica de Publicidad»).
  - Se publicó como noticia, en la primera persona de la empresa, con DG-033-2026 vigente, que paga «contenidos estratégicos; informativos y pedagógicos» de DISPAC. Es la única entrada que nombra a DISPAC (`?search=DISPAC`: 1).
- **La pieza de CODECHOCÓ.** https://elmanduco.com.co/2026/03/04/atrato-canton-de-san-pablo-jurado-y-riosucio-representaran-las-subregiones-ante-el-consejo-directivo-de-codechoco/. Categorías 11 y 13, sin firma visible en la API, sin rótulo. Literal: «se aprobaron los Estados Financieros, que reflejan un manejo responsable, transparente y eficiente de los recursos públicos». Se publicó con CPS 070-2026 del director vigente. Las otras cinco entradas que devuelve `?search=Codechocó` son crónicas o columnas que solo mencionan a la entidad.
- **La pieza de la UTCH** (2026-08-04, categorías 7, 8 y **23 «Editorial»**), literal: «Gracias a las gestiones del director del Archivo Fotográfico y Fílmico del Chocó, Gonzalo Díaz Gonzalo Diaz Cañadas…». El cargo en la UTCH no se verificó en fuente oficial.
- **Precisión 2, sobre el alcance de la regla.** El envío habla de «la cobertura del propio **accionista**» como evidencia de primer orden. DISPAC y CODECHOCÓ no son accionistas: son contratantes. Para eso el protocolo tiene su propia vía («CONTRATACIÓN PÚBLICA», `PROTOCOLO_JUICIO_EDITORIAL.md:180-210`): **desvelamiento, no acusación**, y «si los editoriales elogian a quien contrata, eso se declara como tensión». Así entra. No mueve el eje.
- **¿Aviso de quien dirige?** No procede (`PROTOCOLO_JUICIO_EDITORIAL.md:212-240`). Un contrato de prestación de servicios con CODECHOCÓ no es un cargo público en ejercicio. El precedente es Diario de Cundinamarca (DECISIONES.md 2026-10-10): «vínculo contractual de su director», como tensión. El supuesto cargo del community manager en la UTCH no dispararía el aviso aunque se probara, porque no dirige la redacción; y no está probado.

**6 · Captura.** Ritmo por mes: exacto (ver 2). «El fallo es de captura» no describe lo que pasó, que fue:
- (a) caída real del sitio a finales de agosto y principios de septiembre;
- (b) **retirada del feed por decisión, el 2026-09-02**, con premisas inexactas;
- (c) vuelta del sitio, que la auditoría registró el 2026-09-17 y nadie trasladó al registro.

Desde el 2026-09-02 la ingesta no lo pide, y por eso no lo captura. La estimación de unas 40 piezas en 90 días es una inferencia razonable a ~0,4 piezas al día, y deja la refutación 3 de la ficha (más de 60 historias) fuera de alcance por mucho tiempo.

**Barrido de la voz de la casa (comprobación parcial).**
- Las piezas de 12 meses en las categorías Política, Editorial y Opinión (ids 20, 23 y 10) son **35**. Exacto.
- La categoría Editorial (id 23) tiene **2** entradas: la de Murillo y la de la UTCH.
- Las cuatro URL del revisor responden 200.
- «El Viacrusis de Luis Gilberto Murillo» lleva la firma literal «Redacción El Manduco».
- La columna del 2026-10-04 contiene, literal, «He decidido escribir esta invitación sin mencionar nombres» y «No es una invitación a votar por alguien».
- **No se rehízo el barrido de cuerpos.** Con 2 editoriales en 12 meses y voz propia de eje regional, no hay base para acercarse al mínimo (10 piezas con postura, 3 por lado). La regla de evidencia editorial histórica no se cumple, y el 0,00 se queda por las reglas 2 y 3: **sigue siendo «no sabemos»**.

### Motivo de cada rechazo

No se rechaza entera ninguna objeción. Se rechazan o corrigen estas partes:
- **Obj. 4: «hoy la portada no muestra los créditos. En el HTML crudo de https://elmanduco.com.co/ no aparecen "Carrasco", "Marvin" ni "Gerente"».** Falso en la descarga de hoy: aparecen una vez cada uno, en el bloque «CREDITOS» del pie de la portada.
- **Obj. 5: «Todos son de prensa, audiovisual o "manejo de emisoras web"».** Ocho de diez. Dos tienen objetos de gestión ambiental genéricos.
- **Obj. 5: «la cobertura de quien contrata al dueño es "evidencia de primer orden"».** El envío dice «del propio accionista». La de los contratantes entra por la línea de contratación y como tensión, no como evidencia de eje.
- **Obj. 2: «unas 24 dentro de la ventana medida».** Son 26.
- **Obj. 6: «el fallo es de captura».** El cero es la retirada deliberada del feed, no un fallo de la ingesta.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente.** Todas las URL comprobadas resuelven, las citas del medio son literales y las cifras del RUES y de SECOP coinciden al peso. Hay una afirmación falsa sobre el HTML de la portada (obj. 4) y las precisiones de arriba. El dato de la Alcaldía de Quibdó (Jorge Díaz Cañadas como director) viene solo del resumen de un buscador, de un dominio que excluye a todos los agentes. El propio revisor lo marca como no verificado. **No entra en nada**, y aquí no se tocó ese dominio.

**Errores de la propia ficha, para no repetirlos:**
- **El departamento** (`fichas/el-manduco.md:1`, `:9`, `:32`, `:49`, `:55`, `:69`, `:71` y `:74`), y con él todo el argumento demográfico: «90 000 habitantes», «Amazonía-Orinoquía», y una Gobernación, una Alcaldía y una Cámara del Guaviare como plan de refutación.
- **«la propia cabecera»** (`:24`): es el bloque «CREDITOS» del pie.
- **«Los cuatro cargos»** (`:26`): son siete. Faltan Jefe de publicidad, Jefe de redacción y Community manager.
- **«Falta la sociedad: ni razón social, ni NIT, ni matrícula»** (`:35`): está en el RUES desde 2022, ACTIVA.
- **«No está ingerido. Su feed devolvió artículos de hace 66 horas»** (`:7` y `:39`): estuvo en la ingesta del 2026-08-09 al 2026-09-02, y está fuera desde entonces por decisión.
- **«basta con que un Díaz tenga un interés»** (`:58`): el interés existe y está documentado. Es contractual, no electoral.
- **`shared/mediaRegistry.js:1203-1227`**: «última pieza conocida es de marzo de 2026» y «el Guaviare era suyo y solo suyo» son inexactos (ver 2 y 1).
- **Lo que la ficha sí tenía bien:** los cuatro nombres con sus cargos, que el medio es de una sola familia de apellido (hoy, siete Díaz) y que la estructura «dice quién manda, no hacia dónde tira».

---

**Propuesta para la firma**

**A. Valor: 0,00, provisional y no firmable. Sin cambios.**
- **Regla 3:** el nivel 1 no tiene posición (sociedad y representante legal conocidos, socios no), y no hay nivel 3. El nivel 2 es 0 en la ventana, porque el feed estaba retirado.
- **Evidencia editorial histórica:** no se cumple (2 editoriales en 12 meses; voz propia de eje regional, «chocoanismo»).
- **Regla 2:** la banda mixta. Sigue siendo «no sabemos», ahora con la sociedad, sus contratos y los del director a la vista.

**B. Departamento: `Chocó`.** En `shared/mediaRegistry.js:1199`, `departamento: 'Guaviare'` → `departamento: 'Chocó'`. Para el `group` (`'Regional Guaviare'`) hay dos opciones; decide el responsable editorial (punto 2 de abajo):
- `'Manduco Media Group'`, el nombre de la casa, como en `'Corporación El Morichal'` (`:1239`);
- `'Regional Chocó'`, que compartiría con Chocó 7 Días, como El Heraldo y La Libertad comparten `'Regional Caribe'`.

  `group` no fija la propiedad (`scripts/checkRegistry.mjs:495-545` cruza por `controlGroup`), pero se enseña en el mapa de medios y se usa al buscar.

**C. Feed: reactivarlo.** En `shared/mediaRegistry.js:1228`, descomentar `feed: { url: 'https://elmanduco.com.co/feed/', via: 'direct', category: 'Política' }` y sustituir el comentario de `:1202-1227` por:

```
/*
 * FEED REACTIVADO EL 2026-10-10 (ciclo 2, tanda 7; decisión del responsable editorial).
 *
 * Estuvo fuera de la ingesta del 2026-09-02 al 2026-10-10. El sitio cayó de
 * verdad a finales de agosto (HTTP 500: Wayback 2026-08-28, auditoría
 * 2026-09-03) y la auditoría lo vio sano otra vez el 2026-09-17, pero nadie
 * descomentó esta línea. Dos premisas de aquella retirada eran inexactas: su
 * última pieza no era de marzo (publicó 11 en agosto y 20 en septiembre, según
 * su API), y el «cero en la base» era la poda de 72 h sobre un medio que publica
 * una pieza cada dos o tres días.
 *
 * Comprobado el 2026-10-10: /feed/ responde 200 con 10 ítems y fechas legibles,
 * el último del 2026-10-06 (`npm run feed:descubrir -- elmanduco.com.co`).
 *
 * Es de Quibdó (Chocó), no del Guaviare: el catálogo lo tuvo en el Guaviare
 * desde el alta del 2026-08-09 por un error de geografía, y por eso aquel
 * comentario decía que el Guaviare «era suyo». El Guaviare no tiene medio
 * propio en el catálogo. Ver fichas/el-manduco.md.
 */
```

  También: añadir a `auditoria/hallazgos.json:488` (la nota de `el-manduco/feed`), o a la próxima pasada, que el feed vuelve el 2026-10-10.

**D. Textos a corregir, con archivo:línea.**

*La ficha, `fichas/el-manduco.md`:*
1. `:1` → «# El Manduco (Quibdó) — ficha de orientación».
2. `:7` → «2026-08-09 (candidatura); revisada el 2026-10-10 (ciclo 2, tanda 7)».
3. `:9` → «Chocó — segundo medio del departamento en el catálogo, con Chocó 7 Días. Hasta el 2026-10-10 figuró por error en el Guaviare».
4. **Tabla del nivel 1 (`:13-24`):** los siete cargos del bloque «CREDITOS» (fuente: «el pie de elmanduco.com.co y la página /manduco-media-group/, 2026-10-10»). Se añaden filas:
   - «Sociedad | **MANDUCO MEDIA GROUP S.A.S.**, NIT 901563146, Cámara de Comercio del Chocó, matrícula 6246212 del 07-02-2022, renovada el 21-04-2026, ACTIVA; CIIU 7310 (publicidad) y 6010 (radio) | RUES, datos.gov.co c82u-588k, 2026-10-10»;
   - «Representante legal | **Gonzalo Andrés Díaz García**, el Director de los créditos | RUES (actualizado el 21-04-2026)»;
   - «Socios | no constan: el RUES abierto no los publica».
5. `:26` → «**Los siete cargos del medio los ocupan siete personas de apellido Díaz.**». Añadir: «Que sean una familia es inferencia por apellido; no hay documento de parentesco». Y retirar `:31-32` («En un departamento de 90 000 habitantes, esa frase pesa»).
6. `:35` («Falta la sociedad»): retirar.
7. **Sección nueva «CONTRATACIÓN PÚBLICA»**, en el formato del protocolo:

   > Contratación pública (SECOP I y II, NIT 901563146, consultado 2026-10-10): 2 contratos por $19.832.000 contratados en los últimos 12 meses (2025-10-10 → 2026-10-10); 6 por $47.052.000 en total desde 2022. Principales contratantes: Empresa Distribuidora del Pacífico S.A. E.S.P. (DISPAC; SECOP II, 3 por $28.152.000, 2024-2026, «emisión de cuñas y la publicidad… sobre los contenidos estratégicos; informativos y pedagógicos» de DISPAC; DG-033-2026, $10.332.000, en ejecución hasta el 31-12-2026) y Cámara de Comercio del Chocó (SECOP I, 3 por $18.900.000, 2022-2026, difusión de sus elecciones y de sus jornadas de renovación). DISPAC es la distribuidora de energía que el medio cubre. La Cámara es una entidad privada con funciones públicas.
   >
   > A nombre personal de su director y representante legal, Gonzalo Andrés Díaz García (identificado por el mismo documento que en el RUES): 11 contratos por $138.613.000 entre 2021 y 2026, 1 por $32.890.000 en los últimos 12 meses. SECOP II, 10 con la Corporación Autónoma Regional para el Desarrollo Sostenible del Chocó (CODECHOCÓ) por $133.613.000, de prensa, audiovisual y emisoras web en su mayoría; el vigente es el CPS 070-2026 (30-01-2026, $32.890.000, edición de videos y manejo de emisoras web, en ejecución hasta el 31-12-2026). SECOP I, 1 con la Cámara de Comercio del Chocó (OPS 015 de 2023, $5.000.000). Es desvelamiento, no acusación: no mueve el número ni dispara el aviso de quien dirige, porque un contrato de prestación de servicios no es un cargo público.
8. **Sección nueva «TENSIÓN DECLARADA: publica a quien la contrata, sin rótulo»:**

   > El 04-03-2026 publicó como noticia, en la primera persona de la empresa y sin rótulo de comunicado ni de publicidad, un aviso de DISPAC («realizaremos trabajos de mantenimiento… nuestro equipo técnico…»), con el contrato DG-033-2026 vigente. El mismo día publicó una nota institucional de CODECHOCÓ, entidad que contrata a su director, que presenta sus estados financieros como «un manejo responsable, transparente y eficiente de los recursos públicos». En 12 meses no consta ninguna pieza que fiscalice a DISPAC, a CODECHOCÓ ni a la Cámara de Comercio del Chocó. La pieza del 04-08-2026, en la categoría «Editorial», atribuye una alianza de la UTCH a «las gestiones» de su propio community manager, Gonzalo Díaz Cañadas; ese cargo en la UTCH no está verificado.
9. **Nivel 2 (`:37-39`)** → «0 artículos en la ventana del 31-08 al 10-10-2026, porque el feed estuvo retirado de la ingesta del 02-09 al 10-10 (`shared/mediaRegistry.js`). El medio publicó 26 piezas en esa ventana (API de WordPress, 2026-10-10). No hay nivel 2 que aportar todavía.»
10. **ARGUMENTO (`:43-49`):** retirar «en la Amazonía-Orinoquía» y escribir «un medio pequeño de una familia en Quibdó, editado por una S.A.S. cuyo representante legal es su director». Añadir el resultado del barrido: «Política, Editorial y Opinión: 35 piezas en 12 meses, 2 editoriales; la voz propia es de identidad regional, no de eje izquierda-derecha. No se cumple la regla de evidencia editorial histórica».
11. **CONTRA (`:55-58`):** retirar «en un departamento de 90 000 habitantes». Sustituir «basta con que un Díaz tenga un interés para que el medio lo tenga» por: «el interés ya consta: la sociedad vende publicidad a DISPAC y a la Cámara de Comercio del Chocó, y el director es contratista vigente de CODECHOCÓ. El medio publica a las dos primeras y a CODECHOCÓ sin rótulo».
12. **REFUTACIÓN (`:68-74`):**
    - 1 → «Candidaturas o cargos públicos de los Díaz en el Chocó (Registraduría; no consultada). Los contratos ya constan»;
    - 2 → «El certificado de existencia de la Cámara de Comercio del Chocó (matrícula 6246212), por los socios»;
    - 3 → «A los 90 días con más de 60 historias: su cobertura de la Gobernación del Chocó, la Alcaldía de Quibdó, DISPAC y CODECHOCÓ. Al ritmo actual (~0,4 piezas al día) no llegará en mucho tiempo».

*`shared/mediaOwnership.js`, entrada `el-manduco` (`:2598-2611`):*

13. `ownerType` (`:2599`): **`null`**, que es la recomendación, o `'familiar'` con la salvedad escrita. Decide el responsable editorial (punto 3 de abajo).
14. `holdings[0]` (`:2601`) → «Lo edita MANDUCO MEDIA GROUP S.A.S., NIT 901563146, Cámara de Comercio del Chocó, matrícula 6246212 del 07-02-2022, renovada el 21-04-2026, ACTIVA; CIIU 7310 y 6010 (RUES, datos.gov.co c82u-588k, consultado el 2026-10-10). Representante legal: Gonzalo Andrés Díaz García, el Director de los créditos. El RUES abierto no publica accionistas.» Y un `holdings[1]` → «Los siete cargos del bloque CREDITOS del sitio (2026-10-10) los ocupan personas de apellido Díaz: Carlos Díaz Carrasco (fundador), Jhon Díaz Cañadas (director emérito), Gonzalo Díaz García (director), Marvin Díaz García (gerente), Jorge Díaz Cañadas (jefe de publicidad), Carlos Vicente Diaz (jefe de redacción) y Gonzalo Díaz Cañadas (community manager). El parentesco es inferencia por apellido.»
15. `notes[0]` (`:2604`) → retirar «No consta la sociedad que lo edita» y escribir «Se conocen la sociedad y su representante legal, no sus socios.» `notes[1]` (`:2605`) → retirar «En un departamento de unos 90 000 habitantes» y escribir: «No hay ninguna estructura interna que contrapese un interés de la familia que lo dirige. Eso no dice hacia dónde tira su línea; dice de quién depende.» Añadir dos `notes`: la línea de contratación del punto 7, sin documento, y la tensión del punto 8.
16. `sources` (`:2607-2609`): añadir
    - `https://elmanduco.com.co/manduco-media-group/`
    - `https://www.datos.gov.co/resource/c82u-588k.json?$select=razon_social,sigla,nit,camara_comercio,matricula,organizacion_juridica,estado_matricula,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,fecha_cancelacion,cod_ciiu_act_econ_pri&nit=901563146`
    - `https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=id_contrato,nombre_entidad,proveedor_adjudicado,fecha_de_firma,valor_del_contrato,modalidad_de_contratacion,objeto_del_contrato,estado_contrato&documento_proveedor=901563146`
    - `https://www.datos.gov.co/resource/f789-7hwg.json?$select=numero_de_constancia,nombre_entidad,nom_razon_social_contratista,fecha_de_firma_del_contrato,cuantia_contrato,valor_total_de_adiciones,detalle_del_objeto_a_contratar,estado_del_proceso&identificacion_del_contratista=901563146`
    - la pieza de DISPAC y la de CODECHOCÓ.

    **Las consultas por el documento del director no se enlazan.** Se citan los identificadores (CPS 070-2026 / CO1.PCCNTR.9259070, etc.).
17. `verifiedAt` (`:2610`): **sigue `null`**, porque no constan los socios. Así sigue valiendo `shared/mediaOwnership.test.js:295`, que usa a El Manduco como «ficha sin fecha»; si se le pusiera fecha, habría que cambiar ese test. Añadir `buscadoEn` y `falta` como en las demás entradas (RUES, SECOP I y II, API de WordPress, Wayback; y que falta el certificado de la matrícula 6246212).

*`shared/mediaRegistry.js`:*

18. `biasRationale` (`:1201`) → «Digital de Quibdó (Chocó), editado por MANDUCO MEDIA GROUP S.A.S. (NIT 901563146, ACTIVA), cuyo representante legal es su director. Los siete cargos de sus créditos son de apellido Díaz, y no constan los socios. La sociedad vende publicidad a DISPAC y a la Cámara de Comercio del Chocó, y el director es contratista vigente de CODECHOCÓ. El medio publica a los dos primeros y a CODECHOCÓ sin rótulo, y eso queda como tensión declarada. 0,00 por ausencia de evidencia: su voz propia es de identidad regional y no cumple la regla de evidencia editorial histórica — ver fichas/el-manduco.md.»
19. `fichas/choco-7-dias.md:11` → «Chocó — uno de los dos medios del departamento en el catálogo, con El Manduco». `shared/mediaRegistry.js:1194`: retirar «el único vivo del Chocó en el catálogo».

*`shared/centinela.js`, entrada `el-manduco` (`:237-245`):*

20. `vigila` (`:242`) → «Que los siete cargos de los créditos sigan en personas de apellido Díaz y que Gonzalo Andrés Díaz García siga como director. Toda la ficha descansa en esa coincidencia de apellido y en los contratos de la sociedad (DISPAC, Cámara de Comercio del Chocó) y del director (CODECHOCÓ).» Opcional: una consulta «Codechocó» o «DISPAC» que vigile cómo cubre a sus contratantes.

*Cobertura departamental: lo que cambia por el error de geografía.*

21. `COBERTURA_DEPARTAMENTAL.md`:
    - `:4` («El catálogo pasa a 30 de 33») y `:44-46` («29 de los 33… Faltan cuatro», que eran Amazonas, Guainía, Vaupés y Sucre): esos recuentos contaban al Guaviare. Nota fechada arriba del todo: «2026-10-10: El Manduco es de Quibdó (Chocó), no del Guaviare. Todos los recuentos de este archivo cuentan un departamento de más: el Guaviare nunca tuvo medio propio en el catálogo. Con LeticiaHoy, son 29 de 33, y el Guaviare se suma a los huecos».
    - `:87-92` (la lista de los 18 vivos y «El más rezagado del grupo es El Manduco (Guaviare)») se deja como foto del 2026-08-11, cubierta por la nota.
    - **Pista para el Guaviare, sin verificar:** el mismo archivo, `:22`, dice que `marandua.com.co` «es una emisora de Guaviare». `BARRIDO_NACIONAL.md:136` recoge que el censo de la FLIP visitó el Guaviare.
22. `MEDIOS_CANDIDATOS_DEPARTAMENTOS.md`:
    - `:61` y `:368`: «Guaviare» → «Chocó (por error, Guaviare hasta el 2026-10-10)»;
    - `:194`: la fila pasa a «Chocó | El Manduco | 0,00 provisional, sin firmar · S.A.S. en el RUES, contratista de DISPAC y de la Cámara del Chocó; su director, de CODECHOCÓ · ciclo 2, 2026-10-10»;
    - `:324-326` («El Manduco (Guaviare)… 90 000 habitantes»): una nota de corrección;
    - `:30-37` («8 → 28», «Eran 29»): la misma nota que en el punto 21.
23. `BARRIDO_NACIONAL.md:34` («El Manduco publica a diario en el Guaviare») → «en el Chocó».
24. `src/docs/catalogo_medios.txt:203-208` sale de `scripts/generateCatalogDoc.mjs`: regenerarlo después de cambiar el registro, no editarlo a mano.
25. `fichas/LEEME.md`: **sin cambios**; no nombra a El Manduco ni al Guaviare.
26. `../MINUTA.md:3044-3070` y `:3235-3250` es historia: no se reescribe. Si acaso, una entrada nueva que diga que la retirada del 2026-09-02 se deshace y por qué.

**Lo que NO entra como hecho:**
- el parentesco entre los siete Díaz;
- que «john diaz cañadas» (DISPAC, 2020 y 2022) sea el director emérito;
- que Jorge Díaz Cañadas dirija el medio (solo un resumen de buscador, de un dominio excluido);
- el cargo de Gonzalo Díaz Cañadas en la UTCH;
- que la sociedad sea «familiar» como hecho de propiedad;
- la composición accionaria de DISPAC;
- que las piezas de DISPAC y de CODECHOCÓ sean entregables pagados: el contrato de DISPAC paga «contenidos… informativos», pero cuál pieza lo es no consta.

**Decisiones para el responsable editorial:**
1. **Departamento.** Recomendación: **Chocó**, con la nota de corrección en los documentos de cobertura (puntos 21-23). Guaviare vuelve a ser un hueco declarado.
2. **`group`.** Recomendación: **`'Manduco Media Group'`**, el nombre de la casa, como El Morichal. Así no se mezcla en el mismo cubo con Chocó 7 Días, que tiene otro dueño. La otra opción, `'Regional Chocó'`, tiene el precedente de `'Regional Caribe'`.
3. **`ownerType`.** Recomendación: **`null`**, con el criterio de DECISIONES.md 2026-10-09 («así no se afirma un carácter "familiar" que no consta»): la sociedad tiene socios desconocidos, y el parentesco es inferencia. Lo familiar queda dicho en `holdings` como lo que es: siete cargos con el mismo apellido. Alternativa: mantener `'familiar'` con esa salvedad escrita.
4. **Feed.** Recomendación: **reactivarlo** (punto C) y anotar en DECISIONES.md que la retirada del 2026-09-02 se deshace. Que la auditoría viera el sitio sano el 2026-09-17 y nadie lo trasladara al registro indica que hace falta enlazar «fuente resuelta» con «feed retirado», el mismo defecto que ya anotaba `../MINUTA.md:3068-3072`.
5. **Contratos del director y piezas sin rótulo.** Recomendación: **constan** como desvelamiento (punto 7) y **tensión** (punto 8), sin documento y sin enlaces que lo lleven, con «no mueve el número» escrito. Es el criterio de DECISIONES.md 2026-10-10.
6. **Valor.** Recomendación: **mantener 0,00**, provisional y sin firmar.

**Avisos:**
- El revisor declaró haber bajado un PDF de `quibdo-choco.gov.co` (robots «Disallow: /») y haberlo borrado sin abrirlo. Aquí no se tocó ese dominio, y nada de lo que se propone usa ese documento.
- La Wayback bloqueó las capturas `id_` por su filtro antibots; solo se usó la API CDX.
