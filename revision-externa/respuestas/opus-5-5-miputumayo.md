# Respuesta — Claude Opus 5.5 sobre MiPutumayo

| | |
|---|---|
| **Modelo** | Claude Opus 5.5 |
| **Versión exacta** | `claude-opus-5-5` |
| **Fecha de la consulta** | 2026-10-08 |
| **Quién la hizo** | Claude Code, a petición del responsable editorial (ciclo 2, fase 2, tanda 4; revisor de la misma casa que el autor de las fichas, ver DECISIONES.md 2026-10-07) |
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
Soy Claude Opus 5.5 (claude-opus-5-5), de Anthropic: la misma casa que el modelo que escribió la ficha. Mi acuerdo con ella no vale como aval independiente. Para compensarlo he buscado sobre todo en fuentes que la ficha NO usa (RUES, SECOP I y II, páginas «Paute Aquí», «Colaboradores» y «Términos de uso» del medio, su buscador interno y artículos de agosto-octubre de 2026). Solo he leído el archivo del envío; ningún otro archivo del repositorio.

MÉTODO Y DÓNDE BUSQUÉ
Fecha de la comprobación: 2026-10-08, hora de Colombia (las cabeceras del servidor marcan 2026-10-09 00:51 GMT).
- robots.txt de miputumayo.com.co (leído antes de descargar nada): «User-agent: * / Allow: /wp-admin/admin-ajax.php ...». Solo bloquea Amazonbot, Bytespider, SemrushBot, MJ12bot, AhrefsBot y PetalBot. No excluye a ClaudeBot, Claude-Web ni anthropic-ai, así que descargué.
- La fuente que «no responde» (https://miputumayo.com.co/quienes-somos/) NO está rota. Vive en la misma URL y devuelve HTTP 200 con el texto que cita la ficha. Lo que falla es el servidor de origen del medio, que va a ratos: detrás de Cloudflare me dio varias veces «error code: 525» (fallo de SSL entre Cloudflare y el origen) o se agotó el tiempo, y después respondió en un reintento. En mi entorno, además, curl en Windows (schannel) fallaba hasta que añadí --ssl-no-revoke. Es probable que el centinela viera alguno de esos dos fallos. Recomendación: reintentar antes de declarar rota una fuente de este dominio.
- Todo lo citado del sitio sale del HTML crudo, descargado con curl -sL y User-Agent de Chrome. Páginas: portada, /quienes-somos/, /paute-aqui/, /colaboradores/, /terminos-de-uso/, /contactenos/, 9 artículos y 5 búsquedas internas (?s=Petro, ?s=De+la+Espriella, ?s=elecciones+presidenciales, ?s=uribe, ?s=gobernador). No me cargaron sitemap.xml, sitemap-pages.xml ni wp-json (siempre tiempo agotado o 525).
- RUES abierto (datos.gov.co c82u-588k): razón social con LIKE '%CHAMORRO BURBANO%', '%MIPUTUMAYO%' y '%MI PUTUMAYO%'. Luego igualdad exacta por el NIT hallado.
- SECOP II (jbjy-vk9h, documento_proveedor = NIT, igualdad exacta y sin DV) y SECOP I (f789-7hwg, identificacion_del_contratista = NIT, igualdad exacta). También por nombre (proveedor_adjudicado / nom_razon_social_contratista) y por objeto que contenga «MIPUTUMAYO» en SECOP II.
- Wikipedia en español, solo por /wiki/: https://es.wikipedia.org/wiki/Guillermo_Rivera_Fl%C3%B3rez
- Buscador web: disponible. Hice 1 consulta («"MiPutumayo" "Chamorro" Mocoa medio digital») y no aportó nada utilizable: solo una nota de las2orillas.co sin fecha visible sobre un taller de la FLIP, que es historia. No toqué eltiempo.com ni cambiocolombia.com. Algunas piezas que cito replican contenido de El Tiempo, pero las leí en miputumayo.com.co.
- NIT: el medio no publica razón social ni NIT. Por RUES encontré una matrícula de persona natural a nombre del director (ver objeción 1). Ese NIT es su número de cédula, así que NO lo escribo (Ley 1581). Lo usé solo para las consultas.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré nada de eso. No hay una sociedad que pueda venderse o fusionarse: en RUES no aparece sociedad alguna con «MiPutumayo» en la razón social. Lo único que encontré con ese nombre son entidades sin ánimo de lucro ajenas al medio («ASOCIACION ARTESANOS POR MI PUTUMAYO», «FUNDACIÓN DEPORTIVA SUEÑA MI PUTUMAYO»; no hay nada que las ligue a él). El único hecho corporativo del año es una expansión, no un cambio de propiedad. El 2026-10-02 el medio anunció un portal nuevo: «MiPutumayo.com.co anuncia el lanzamiento oficial de su nueva plataforma de información y servicios: enputumayo.com.co . Esta nueva herramienta digital nace como un directorio integral...» (https://miputumayo.com.co/2026/10/02/miputumayo-com-co-lanza-enputumayo-com-co-el-nuevo-directorio-comercial-y-de-servicios-de-la-region/, publicado 2026-10-02T14:46:19+00:00, autor en metadatos: «director»).

- La persona que la ficha nombra como titular o director, ¿sigue viva y en el cargo? (fecha de la comprobación)
  Sí, según el propio medio, comprobado el 2026-10-08. La página https://miputumayo.com.co/quienes-somos/ termina con «Luis Carlos Chamorro Burbano Director». La de /colaboradores/ dice «Director Luis Carlos Chamorro Burbano». Aviso: las dos páginas tienen datePublished 2011-02-07 en su JSON-LD, así que el dato es antiguo aunque siga publicado. Hay actividad reciente bajo el usuario «director»: artículos del 2026-10-02, 05, 07 y 08 firmados así en metadatos. Eso prueba que alguien publica con ese usuario, no quién es. No encontré necrológica ni noticia de relevo, pero no busqué expresamente obituarios fuera del sitio por el cupo del buscador.

- ¿Quién dirige hoy la redacción?
  Luis Carlos Chamorro Burbano, según las páginas institucionales del medio. No encontré un nombre distinto de «jefe de redacción». /colaboradores/ dice «Editores Sandra Martínez». Es una página de 2011 y no sé si sigue vigente.

- ¿Hay un registro mercantil o un reporte de emisor más reciente que la fuente que la ficha cita?
  Sí, y lo que dice es relevante. Es el registro RUES de la Cámara de Comercio del Putumayo (ver objeción 1): matrícula de persona natural CANCELADA el 2021-04-29, con última fecha de actualización 2021-06-19. No encontré ninguna matrícula activa.

## OBJECIONES

OBJECIÓN 1 — «Razón social / NIT: no constan» y «Una persona, ninguna sociedad»
- QUÉ afirma la ficha: que no constan razón social ni NIT. En «Refutación» pide buscarlos en la Cámara de Comercio del Putumayo, como si no estuvieran a mano.
- POR QUÉ: el RUES abierto tiene una matrícula mercantil de persona natural a nombre del director, en la cámara del Putumayo, abierta 4 meses después de la fundación declarada del medio y con actividades de portales web. Pero está cancelada desde 2021. Hoy no consta ninguna matrícula mercantil activa que respalde la explotación comercial del medio, que vende publicidad (objeción 2). El registro, literal (omito número de identificación y DV):
  «"camara_comercio":"PUTUMAYO","matricula":"24541","razon_social":"CHAMORRO BURBANO LUIS CARLOS","clase_identificacion":"CEDULA DE CIUDADANIA", ... "cod_ciiu_act_econ_pri":"6820","cod_ciiu_act_econ_sec":"6311", ... "fecha_matricula":"20040727","fecha_renovacion":"20160926","ultimo_ano_renovado":"2016", ... "fecha_cancelacion":"20210429", ... "organizacion_juridica":"PERSONA NATURAL", ... "estado_matricula":"CANCELADA","fecha_actualizacion":"2021/06/19 18:45:32.200000000"»
  (Código CIIU 6311: procesamiento de datos, alojamiento y actividades relacionadas, que incluye portales web. Código 6820: actividades inmobiliarias a cambio de una retribución o por contrato.)
  Homonimia: NO está probada documentalmente que sea la misma persona que dirige el medio. Lo hace muy probable que coincidan nombre completo, cámara (Putumayo), año 2004 y actividad de portales web. En RUES hay otra matrícula con el mismo nombre en Bogotá (matrícula 827553, 1997-1999, cancelada el 2011-12-29) cuyo número de identificación NO coincide con el de la matrícula del Putumayo: ahí sí hay homonimia o, como mínimo, otro documento.
  Hecho: la matrícula existe y está cancelada. Inferencia: el medio funciona hoy sin matrícula mercantil activa del director ni de una sociedad.
- FUENTE Y FECHA: datos.gov.co, RUES abierto c82u-588k. Consulta del 2026-10-08: [enlace retirado: puede mostrar documentos de identidad; ver la resolución]. Fecha del registro: actualizado el 2021-06-19, cancelación el 2021-04-29.
- NIVEL: registro externo / propiedad.

OBJECIÓN 2 — «No declara ni financiación ni sociedad» y «sin financiación declarada»
- QUÉ afirma la ficha: que el medio no declara de qué se financia. Lo llama «la pregunta central».
- POR QUÉ: el medio publica hoy una tarifa de publicidad y una sección de avisos de empresas de servicios públicos. Eso responde en parte la pregunta (fuentes de ingreso por publicidad), aunque no dice quién paga ni cuánto.
  a) /paute-aqui/ (datePublished 2014-09-23, dateModified 2024-01-12), literal: «Diseño de Piezas Publicitarias 3 tamaños Inversión : $ 60,000=: Publicidad en MiPutumayo.com.co y Portales Aliados Mensual / Aleatorio : $ 200,000= Fijo : $ 1,000,000= 1000 impresiones $ 20,000=». Además de la venta directa, declara una red de «Portales Aliados».
  b) Categoría «Publicaciones» con avisos legales de prestadores de servicios públicos. Ejemplo: «La empresa HELIOS ENERGÍA S.A. E.S.P , dando cumplimiento a las disposiciones de ley, informa a todos sus usuarios los costos tarifarios para la prestación del servicio público de energía, que se aplicarán durante el mes de Septiembre de 2026...» (https://miputumayo.com.co/2026/09/22/helios-energia-sas-esp-publicacion-de-tarifas-septiembre-2026/, 2026-09-22; «Categorías Publicaciones»). La portada del 2026-10-08 enlaza también «emevasi-tarifas-del-servicio-septiembre-de-2026» (2026-09-23) y «edicto-pago-prestaciones-sociales-de-milton-javier-gomez-lopez-aguas-mocoa» (2026-09-24), y muestra un banner «Helios-2024» (src=https://miputumayo.com.co/wp-content/uploads/2023/12/Helios-2024-300x131.webp).
  c) La red de publicidad «Publimayo»: los artículos están salpicados de bloques «Publimayo», con el logo «Logo de Publimayo» enlazado a publimayo.com.co. No pude abrir publimayo.com.co (tiempo agotado), así que no sé quién la opera.
  Hecho: hay tarifa publicitaria pública y avisos legales de empresas de servicios públicos. Inferencia NO probada: que esos avisos sean pagados. Es la práctica habitual de las publicaciones legales, pero no tengo factura ni contrato. En SECOP no aparece ningún contrato con el NIT del director (ver «Lo que no pude verificar»).
  La pregunta de financiación tiene, pues, una respuesta parcial y comprobable. Los anunciantes visibles (una E.S.P. de energía solar, EMEVASI, Aguas Mocoa, Tránsito del Putumayo) son sobre todo prestadores de servicios públicos y entidades locales: ese es el riesgo de dependencia que la ficha intuye en «CONTRA», ahora con nombres.
- FUENTE Y FECHA: https://miputumayo.com.co/paute-aqui/ (modificada el 2024-01-12, consultada el 2026-10-08); el artículo de Helios del 2026-09-22; la portada https://miputumayo.com.co/ consultada el 2026-10-08.
- NIVEL: declaración del propio medio (tarifa) + conducta observable (avisos de los últimos 12 meses).

OBJECIÓN 3 — «Una persona, ninguna sociedad» como única estructura de control. La declaración de nivel 4 es de 2011.
- QUÉ afirma la ficha: que el control es de una sola persona. Su nivel 4 se apoya solo en «Quiénes somos».
- POR QUÉ: «Quiénes somos» tiene "datePublished":"2011-02-07T23:01:39+00:00", sin fecha de modificación. Es la declaración vigente porque sigue publicada, pero el texto tiene 15 años. La página hermana /colaboradores/ (datePublished 2011-02-07) describe una estructura mayor que «una persona». Incluye editora y una red de corresponsales, columnistas con seudónimo y oficinas de prensa de instituciones y de dos políticos como «colaboradores institucionales». Literal: «Institucional Oficina de Prensa Alcaldía de Puerto Asís Oficina de Prensa Brigada de Selva 27 – Institucional Oficina de Prensa Policía Nacional – Institucional Oficina de Prensa Fuerza Naval del Sur – Institucional Corpoamazonía – Institucional, Medio Ambiente SENA Putumayo – ... Gobernación del Putumayo Oficina de Prensa Luis Fernando Ochoa – Institucional, Gestión Cámara de Representantes Oficina de Prensa Guillermo Rivera – Institucional, Gestión Cámara de Representantes Editores Sandra Martínez Defensor del Lector Director Luis Carlos Chamorro Burbano».
  Según Wikipedia, Guillermo Rivera «Fue Representante a la cámara por el departamento de Putumayo entre 2002 y 2014 por el Partido Liberal». La misma página le atribuye hoy el Partido Alianza Verde y el cargo de embajador ante Brasil del 13 de enero de 2023 al 3 de julio de 2025. Así que la lista describe un acuerdo de hace más de 10 años. Por la regla del presente, el vínculo con esas oficinas de prensa NO es evidencia vigente de alineamiento, y no lo uso para mover el número. Lo que sí objeto: la ficha presenta como «lo que declara HOY» una página de 2011, sin marcar su antigüedad, cuando el propio medio publica una página de la misma fecha que describe otro modelo de trabajo, el de sindicar material institucional. Hechos del día de hoy, ese modelo sigue siendo visible: se publican comunicados de Ecopetrol, Policía, Fiscalía y Tránsito (ver «Evidencia que no mueve el número»). «Defensor del Lector» aparece sin nombre: el texto es ambiguo y no puedo afirmar que tenga titular.
- FUENTE Y FECHA: https://miputumayo.com.co/colaboradores/ (publicada el 2011-02-07, consultada el 2026-10-08); https://miputumayo.com.co/quienes-somos/ (publicada el 2011-02-07, consultada el 2026-10-08); https://es.wikipedia.org/wiki/Guillermo_Rivera_Fl%C3%B3rez (consultada el 2026-10-08).
- NIVEL: declaración del propio medio. Para Rivera, registro externo de tercer orden (Wikipedia).

(Ninguna de las tres objeciones aporta evidencia que lleve el valor fuera de la banda mixta. Corrigen los datos de propiedad y financiación y la antigüedad de la autodeclaración.)

## LO QUE NO PUDE VERIFICAR

- Contratación pública. SECOP II (jbjy-vk9h, documento_proveedor = NIT de la matrícula RUES del director, igualdad exacta, sin DV): 0 registros. SECOP I (f789-7hwg, identificacion_del_contratista = mismo NIT, igualdad exacta): 0 registros. Sin contratos en los últimos 12 meses ni en ningún otro periodo, así que no aplica lo de valor_pagado = 0. Búsqueda por nombre en SECOP II: solo sale un homónimo de segundo apellido distinto («LUIS CARLOS CHAMORRO ENRIQUEZ»: obras para el Centro de Salud Guachaves ESE, en Nariño), que NO es el director. Por nombre en SECOP I: solo otras personas con apellidos «Chamorro Burbano» (médico y profesional ambiental en Nariño), sin relación probada con el medio. Por objeto con «MIPUTUMAYO» en SECOP II: 0. Límite: si el medio factura por medio de un tercero (Publimayo, otra persona o una sociedad que no conozco) o por contratación directa no publicada, estas consultas no lo ven. Tampoco cubren a Ecopetrol, que contrata por régimen propio.
- Si los avisos de Helios, EMEVASI, Aguas Mocoa y Tránsito son pagados y por cuánto. No encontré facturas, contratos ni declaración del medio.
- Quién opera publimayo.com.co y chamorro.com.co (el web personal que enlaza «Quiénes somos»). Ambos dominios dieron tiempo agotado y no pude ni leer su robots.txt. No los descargué.
- Si los titulares de las piezas replicadas son los originales o los reescribió el medio (por ejemplo, «El aumento del presupuesto para la Amazonía se debe a Petro», que reproduce a La Silla Vacía). No comparé con los originales para no gastar descargas en terceros.
- Editorial de la casa o endoso en la elección presidencial de 2026: el menú del sitio no tiene sección de editoriales («Colaboradores · Paute Aquí · Quienes Somos · Contactenos · Términos de Uso»). Las búsquedas internas «elecciones presidenciales», «Petro», «De la Espriella» y «uribe» no muestran ninguna pieza firmada por la dirección que pida el voto. No es un barrido completo: solo vi la primera página de resultados de cada búsqueda y no pude cargar el sitemap.
- Sitemaps y API REST de WordPress: tiempo agotado o 525 en todos los intentos. No pude hacer un barrido completo del archivo.
- Fallecimiento o relevo del director fuera del sitio: no lo busqué en prensa externa por el cupo del buscador.

## LO QUE FALTA

1. El registro RUES (matrícula 24541 del Putumayo, cancelada en 2021). La ficha debería citarlo y decir que hoy no consta matrícula activa ni sociedad. Es la mejor respuesta disponible a su punto 2 de «Refutación».
2. La tarifa publicitaria de /paute-aqui/, la categoría «Publicaciones» con avisos de prestadores de servicios públicos y la red «Publimayo / Portales Aliados». Contestan en parte su punto 1 («de qué se financia»).
3. El lanzamiento de enputumayo.com.co (2026-10-02): hecho corporativo de los últimos 12 meses que amplía el negocio del mismo titular.
4. Para el nivel 2: buena parte de la cobertura nacional NO es propia. Son reproducciones acreditadas a otros medios y publicadas con el usuario «director»: El Heraldo (De la Espriella y el CRIC, 2026-10-07), Infobae (MOE y Cepeda, 2026-07-15), La Silla Vacía (presupuesto Amazonía, 2026-09-24), El Tiempo (el «libro de la verdad», 2026-08-19), Caracol Radio (campesinos y fumigación, 2026-10-07). El protocolo de 90 días y 60 historias que propone la ficha tiene que separar lo propio de lo replicado. En un medio así, la señal de orientación está sobre todo en QUÉ medios elige replicar y con qué titular, no en la redacción.
5. Que «Quiénes somos» y «Colaboradores» son de 2011. Hay que fecharlas en la ficha.

## EVIDENCIA QUE NO MUEVE EL NÚMERO

Toda es de los últimos 12 meses, citable, y deja el 0,00 donde está.

- Continuidad frente al cambio de gobierno (agosto de 2026). Antes y después, el medio da voz a los dos lados y replica fuentes de ambos extremos del espectro. No encontré que celebre la llegada de un gobierno.
  · Campaña: «en-el-putumayo-estarian-amenazando-a-la-gente-para-que-solo-voten-por-ivan-cepeda-denuncio-alvaro-uribe-a-sangre-y-fuego» (2026-02-23) junto a «ivan-cepeda-acuso-a-alvaro-uribe-de-agudizar-la-guerra-arancelaria-con-ecuador-con-su-visita-a-la-frontera-metodos-sucios» (2026-04-16), «uribe-denuncia-presion-electoral-en-regiones-la-orden-es-votar-por-cepeda» (2026-05-06) y «ivan-cepeda-rechazo-convocatorias-de-grupos-armados-...» (2026-05-15). Fuente: búsquedas internas https://miputumayo.com.co/?s=uribe y ?s=elecciones+presidenciales, consultadas el 2026-10-08.
  · Antes del cambio, ante el gobierno saliente: «s-o-s-en-putumayo-gobernador-jhon-gabriel-molina-urge-al-presidente-petro-la-reapertura-de-la-frontera-con-ecuador» (2026-01-28).
  · Después del cambio, sobre el balance del gobierno saliente: reproduce a El Tiempo, que es crítico con Petro. Literal: «En esa publicación, el equipo de De La Espriella presenta su propio empalme y concluye que la pasada administración incurrió en nueve 'pecados'...» (https://miputumayo.com.co/2026/08/18/sector-por-sector-el-critico-balance-de-la-era-petro-que-denuncia-el-libro-de-la-verdad-elaborado-por-el-gobierno-de-de-la-espriella/, 2026-08-19). En sentido contrario, reproduce a La Silla Vacía: «mucho del presupuesto no lo asignó De la Espriella, sino que lo dejó amarrado Petro a través de vigencias futuras» (https://miputumayo.com.co/2026/09/24/el-aumento-del-presupuesto-para-la-amazonia-se-debe-a-petro/, 2026-09-24).
  · Ante el gobierno entrante: reproduce sin comentario propio la advertencia del presidente al CRIC (El Heraldo, 2026-10-07): «De la Espriella fue enfático al señalar que en su Gobierno no se permitirán los bloqueos ni las vías de hecho» (https://miputumayo.com.co/2026/10/07/presidente-de-la-espriella-lanza-advertencia-al-cric-ante-posibles-protestas-no-permitiremos-bloqueos-de-ninguna-clase/).
- Tema decisivo según la propia ficha (coca, erradicación, sustitución), después de agosto de 2026. Lo registro como candidato a eje del nivel 2, no como prueba de signo:
  · Pieza sin crédito externo visible, del 2026-09-08: «El Gobierno del presidente Abelardo de la Espriella anunció de manera oficial la reanudación de la aspersión aérea ... A pesar de la determinación gubernamental, la puesta en marcha definitiva no es automática ni inmediata. Para que estas operaciones se extiendan, el Gobierno nacional está obligado a sortear el estricto marco legal impuesto por la Corte Constitucional» (https://miputumayo.com.co/2026/09/08/gobierno-de-de-la-espriella-reactiva-la-aspersion-aerea-con-plan-piloto-en-putumayo-bajo-estricta-lupa-de-la-corte-constitucional/). Encuadre explicativo y fiscalizador. Por la regla del polo fijo, no es evidencia de orientación.
  · Réplica de Caracol Radio que da voz a los campesinos cocaleros: «Estas comunidades le piden al Gobierno Nacional que llegue al territorio y hable con los campesinos para poder encontrar una ruta diferente que no sea la fumigación aérea» (https://miputumayo.com.co/2026/10/07/campesinos-en-putumayo-piden-ser-escuchados-antes-de-fumigar-los-cultivos-de-coca/, 2026-10-07).
  · Columna firmada (Alexander Africano): «el documento rechaza la aspersión aérea y la erradicación forzada, pero simultáneamente expresa la voluntad de las comunidades de avanzar hacia una sustitución concertada» (https://miputumayo.com.co/2026/10/05/putumayo-no-esta-pidiendo-que-le-dejen-la-coca-esta-proponiendo-como-salir-de-ella/, 2026-10-05). Es opinión de un colaborador. Los Términos de uso dicen: «El contenido de los artículos firmados y las opiniones vertidas son de estricta responsabilidad de sus autores/as, y no necesariamente reflejan la posición editorial de Miputumayo.com.co» (https://miputumayo.com.co/terminos-de-uso/, publicada el 2010-03-01, consultada el 2026-10-08).
  · Al mismo tiempo publica material corporativo y de la fuerza pública sin filtro aparente: «Ecopetrol entregó al Departamento de Policía Putumayo dos camionetas...» (https://miputumayo.com.co/2026/09/02/ecopetrol-apoya-el-fortalecimiento-institucional-y-la-seguridad-en-putumayo/, 2026-09-02), más otras tres piezas de Ecopetrol en agosto y septiembre de 2026 y comunicados de Policía y Fiscalía en portada.
  Lectura: hasta donde vi, el enfoque territorial (voz campesina contra la aspersión) convive con comunicados de Ecopetrol y de la fuerza pública y con réplicas de medios de signos distintos. Que esto se incline hacia un lado solo lo puede decir el nivel 2 medido, separando lo propio de lo replicado.
- Autodeclaración vigente, confirmada literalmente el 2026-10-08: «es un magazín informativo imparcial, neutral e independiente que ofrece sus espacios a la comunidad en el Putumayo» (https://miputumayo.com.co/quienes-somos/).
- No encontré endoso electoral de la casa en 2026 (ver los límites del barrido arriba).

## SIN OBJECIÓN
No aplica: hay tres objeciones. Ninguna trae evidencia que saque el valor 0,00 de la banda mixta. Que yo no haya encontrado esa evidencia no la descarta ni avala el número.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-08. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal: ninguna.** El revisor no escribió ningún número de cédula, teléfono ni dirección particular: dice expresamente que omite el número de identificación y el DV de la matrícula del director. El texto va íntegro. Esta resolución tampoco escribe ninguno: el documento del director y el de la representante legal de Publimayo SAS (ver abajo) se usaron solo para consultar, y las coincidencias entre registros se comprobaron por igualdad, sin copiarlos.

**Cómo se verificó.**
- **El medio.** Se descargaron en crudo, el 2026-10-08, con `curl -sL --ssl-no-revoke -A "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/126.0 Safari/537.36"`: la portada, `/quienes-somos/`, `/colaboradores/`, `/paute-aqui/`, `/terminos-de-uso/`, `/contactenos/`, `/category/publicaciones/`, las cinco búsquedas internas que cita el revisor, los nueve artículos que cita, el de Infobae sobre la MOE (2026-07-15) y los tres avisos de la portada (EMEVASI, Aguas Mocoa y Tránsito). **Todas respondieron 200.** Las citas se buscaron literalmente en el texto extraído (el HTML sin etiquetas). Las fechas son el `datePublished` del JSON-LD de cada página.
- **Sitios ligados que el revisor no pudo abrir:** `publimayo.com.co`, `www.chamorro.com.co` (la página personal que enlaza «Quiénes somos») y `enputumayo.com.co`. Los tres respondieron 200 aquí.
- **Registros, en datos.gov.co:**
  - RUES (`c82u-588k`): por razón social `like '%CHAMORRO BURBANO%'`, `'%MIPUTUMAYO%'`, `'%MI PUTUMAYO%'` y **`'%PUBLIMAYO%'`**.
  - SECOP I (`f789-7hwg`), con `identificacion_del_contratista` = el documento de la matrícula 24541 y = `901152998`; SECOP II (`jbjy-vk9h`), con `documento_proveedor` igual a los mismos dos valores. **Igualdad exacta, sin DV.** También por nombre («PUBLIMAYO», «CHAMORRO BURBANO», «LUIS CARLOS CHAMORRO») y por objeto que contenga «MIPUTUMAYO» o «PUBLIMAYO».
  - SECOP I y II por las entidades que publican avisos en el medio (Aguas Mocoa, EMEVASI, Helios, Tránsito del Putumayo), buscando a Publimayo, al director o al medio entre sus contratistas.
- **Wikipedia:** solo rutas `/wiki/` (`Guillermo_Rivera_Fl%C3%B3rez` y `Luis_Fernando_Ochoa_Zuluaga`).
- **El armador:** se leyó `scripts/armarEnvio.mjs` y se reprodujo su comprobación con Node (`fetch`, mismo User-Agent, mismo tiempo límite).
- **Buscador web: no se usó** en esta verificación. Lo que dependería de prensa de terceros queda como laguna.

**robots.txt, comprobado aquí antes de descargar:**
- miputumayo.com.co: `User-agent: *` con `Allow : /wp-admin/admin-ajax.php` (así, con espacio antes de los dos puntos), `Allow: /wp-content/uploads/`, `Disallow: /wp-content/plugins/` y `Disallow: /wp-admin/`. Bloquea por completo solo a Amazonbot, Bytespider, SemrushBot, MJ12bot, AhrefsBot y PetalBot. No menciona a ClaudeBot, Claude-Web ni anthropic-ai, y no excluye las búsquedas internas (`?s=`). La cita del revisor es correcta en lo sustancial: omite con «...» los dos `Disallow`, que no afectan a nada de lo descargado.
- publimayo.com.co y enputumayo.com.co: `User-agent: *`, `Disallow: /wp-admin/`. Sin exclusión para Claude.
- www.chamorro.com.co y publimayo.com: `robots.txt` devuelve 404, es decir, no hay exclusión.
- datos.gov.co: solo `Crawl-delay: 1` y exclusiones de `/browse` y similares.
- es.wikipedia.org: no menciona a ClaudeBot, Claude-Web ni anthropic-ai; las rutas `/wiki/` usadas no están vetadas.
- No se tocaron eltiempo.com ni cambiocolombia.com. Las piezas replicadas de El Tiempo se leyeron en miputumayo.com.co, como hizo el revisor.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | «Razón social / NIT: no constan»: el RUES tiene una matrícula de persona natural del director, cancelada en 2021 | sí | sí | **Aceptada en el hecho**: la matrícula existe y la ficha no la cita. **Rechazadas con motivo** dos partes: la «homonimia» de Bogotá, que es falsa (mismo número de identificación), y la inferencia de que el medio funciona «sin matrícula mercantil activa del director ni de una sociedad», que también es falsa (Publimayo SAS, activa y ligada al director; ver abajo) |
| 2 | La ficha dice que el medio no declara de qué se financia, pero publica tarifa, avisos de servicios públicos y la red Publimayo | sí | sí | **Aceptada**, con correcciones: el aviso de Tránsito no está en «Publicaciones»; faltan dos empresas de energía; y Publimayo no es solo una «red»: es una SAS registrada que vende banners y contenido patrocinado en el medio. Que los avisos sean pagados **sigue sin probar** |
| 3 | El nivel 4 se apoya en una página de 2011 sin fecharla, y «Colaboradores», de la misma fecha, describe otra estructura | sí | sí | **Aceptada** en lo de fechar las dos páginas. La lista de colaboradores es literal. Las oficinas de prensa de Rivera y Ochoa **no entran como evidencia** (regla del presente), como el propio revisor concluye |

### Lo verificado, objeción por objeción

**1 · La matrícula del director.**
- RUES, matrícula **24541**, Cámara del **Putumayo**, literal en los campos que cita el revisor: «CHAMORRO BURBANO LUIS CARLOS», CEDULA DE CIUDADANIA, CIIU principal 6820 y secundario 6311, matriculada el 20040727, renovada el 20160926, último año renovado 2016, cancelada el 20210429, PERSONA NATURAL, CANCELADA, actualizada el 2021/06/19. **Exacto.**
- El revisor omite con «...» otros dos campos de actividad del mismo registro: `ciiu3` **7310** y `ciiu4` 7912. Según la CIIU Rev. 4 A.C., 7310 es «Publicidad» y 7912 «Actividades de operadores turísticos» (las denominaciones no se cotejaron en línea en esta sesión). Para un medio que vende publicidad, el 7310 es el código más pertinente del registro, y el revisor no lo menciona.
- **CIIU 6311 no es «portales web».** En la CIIU Rev. 4 A.C., 6311 es procesamiento de datos y alojamiento (*hosting*); los portales web son el **6312** (misma reserva: no cotejado en línea). El revisor escribe que la matrícula tiene «actividades de portales web» y que el 6311 «incluye portales web». Es una precisión menor, pero la usa para atar la matrícula al medio.
- **La «homonimia» de Bogotá es falsa.** La matrícula 827553 de Bogotá (1997-10-14, último año renovado 1999, cancelada el 2011-12-29) tiene **el mismo `numero_identificacion`** que la 24541 del Putumayo. Se comprobó por igualdad, sin escribirlo. El revisor dice que «NO coincide». Lo más probable es que comparara el campo `nit`, que el registro de Bogotá no trae. Es la misma persona con dos matrículas sucesivas, no un homónimo.
- RUES por «MIPUTUMAYO»: 0. Por «MI PUTUMAYO»: las dos ESAL que cita el revisor (ASOCIACION ARTESANOS POR MI PUTUMAYO, 2013; FUNDACIÓN DEPORTIVA SUEÑA MI PUTUMAYO, 2025), sin nada que las ligue al medio. **Exacto.**
- **Lo que tumba la inferencia del revisor** («el medio funciona hoy sin matrícula mercantil activa del director ni de una sociedad»): el RUES por «PUBLIMAYO» devuelve, literal, **«PUBLIMAYO-COMUNICACIONES PUBLICIDAD Y MERCADEO SAS»**, sigla «PUBLIMAYO SAS», NIT **901152998**, DV 5, Cámara del **Putumayo**, matrícula **65530**, matriculada el 20180207, **renovada el 20260507**, último año renovado **2026**, SOCIEDADES POR ACCIONES SIMPLIFICADAS SAS, **ACTIVA**, CIIU principal 7310 y secundario **6391** (agencias de noticias), con 6311 y 6312 como tercera y cuarta actividad. Representante legal: **MARTINEZ DELGADO SANDRA JANNETH**, actualizado el 2026/05/07. El vínculo con el medio y con el director está en el apartado de identidad, abajo.
- La frase del revisor sobre una matrícula activa «que respalde la explotación comercial del medio» insinúa una irregularidad que no se ha documentado. No entra.

**2 · Financiación.**
- `/paute-aqui/`: `datePublished` 2014-09-23 y `dateModified` 2024-01-12. Literal: «Diseño de Piezas Publicitarias 3 tamaños Inversión : $ 60,000=: Publicidad en MiPutumayo.com.co y Portales Aliados Mensual / Aleatorio : $ 200,000= Fijo : $ 1,000,000= 1000 impresiones $ 20,000=». **Exacto.**
- Helios, 2026-09-22T21:32:02, categoría «Publicaciones», autor en metadatos «director». Literal: «La empresa HELIOS ENERGÍA S.A. E.S.P , dando cumplimiento a las disposiciones de ley, informa a todos sus usuarios los costos tarifarios para la prestación del servicio público de energía, que se aplicarán durante el mes de Septiembre de 2026». Sigue: «para los Sistemas Solares Fotovoltaicos Individuales-SSFVI». **Exacto.**
- EMEVASI (2026-09-23) y el edicto de Aguas Mocoa (2026-09-24): los dos en «Publicaciones», autor «director». El de EMEVASI empieza: «LA EMPRESA DE ENERGIA DEL VALLE DE SIBUNDOY S.A. E.S.P., En cumplimiento del inciso segundo del artículo 125 de la Ley 142 de 1994…». Banner `Helios-2024-300x131.webp` (subido en 2023/12) en la portada. **Exacto.**
- **Tránsito NO es un aviso de «Publicaciones».** La pieza del 2026-10-08 («Tránsito del Putumayo publica listado de presuntos infractores y los cita a audiencia») está en la categoría **«Otras Noticias»** y cuenta que el Departamento Administrativo de Tránsito y Transporte del Putumayo «publicó un aviso». Incluirlo entre «los anunciantes visibles» es una deformación.
- **Lo que el revisor omite de «Publicaciones»** (primera página de 37): tarifas de la **Empresa de Energía del Bajo Putumayo S.A. E.S.P.** (2026-09-20) y de la **Empresa de Energía del Putumayo** (2026-09-22), y avisos de corte de energía (2026-09-14 y 09-15). También hay una venta de lote y una convocatoria académica. Los prestadores de energía son el grupo más numeroso.
- **Publimayo, visto por dentro** (el revisor no pudo abrirlo):
  - Su sitio se titula «Publimayo SAS – Comunicaciones, Publicidad y Mercadeo» y dice, literal: «Mostramos su Empresa / Marca al Mundo Por medio de Banners (Publicidad) y Comunicados de prensa y artículos con Contenido Patrocinado en MiPutumayo.com.co y Portales Aliados». Entre sus servicios está «Prensa y Comunicaciones Noticias y publicación de información institucional». Pie: «© 2022 Publimayo SAS • MiPutumayo.com.co».
  - En MiPutumayo, el bloque «Visitar Publimayo» lleva el logo a `publimayo.com.co`, y los banners se sirven desde `publimayo.com/banners/www/delivery/…`, un servidor de anuncios.
  - **Ninguna de las piezas revisadas lleva marca de contenido patrocinado**: ni los avisos de Helios, EMEVASI y Aguas Mocoa ni la de Ecopetrol del 2026-09-02. Lo único marcado como «Patrocinado» / «Publicidad» en la portada son espacios de anuncio. Esto **no prueba** que esas piezas estén pagadas. Prueba que la sociedad ligada al medio vende «artículos con contenido patrocinado» en él, y que el lector no tiene cómo distinguirlos.
- **Contratación pública:** recalculada aquí con igualdad exacta.
  - Del director como persona natural, por su documento: **0 en SECOP II y 0 en SECOP I**. Coincide con el revisor.
  - **De Publimayo SAS (NIT 901152998), que el revisor no consultó:** **6 contratos en SECOP I por $6.520.500, todos con la Cámara de Comercio del Putumayo** (NIT 891224106). Cuatro son de hosting, dominios y web de la Cámara: 2018-06-29, $1.844.500; 2019-01-31, $2.500.000; 2020-01-01, $1.300.000; 2020-09-01, $400.000. Dos son de publicidad «MEDIANTE BANNER (FORMATO PUBLICITARIO DE INTERNET; UNA PIEZA GRaFICA EN DISTINTOS PORTALES)»: 2024-09-26 y 2024-11-19, $238.000 cada uno. **0 en SECOP II. 0 en los últimos 12 meses.** La misma búsqueda por nombre «PUBLIMAYO» da los mismos 6 y 0.
  - Por objeto con «MIPUTUMAYO» o «PUBLIMAYO»: 0 en SECOP I y II.
  - **Las entidades de los avisos no contratan con el medio por otra vía, hasta donde muestra SECOP:**
    - Aguas Mocoa: 145 registros en SECOP II y 238 en SECOP I. EMEVASI: 48 en SECOP I.
    - En ninguno aparecen Publimayo, el documento del director o el medio. Sus contratos de comunicación van a personas naturales sin relación con el medio.
    - Helios no está en SECOP; es una E.S.P. privada.
    - No se encontró en SECOP ninguna entidad «Tránsito» del Putumayo con ese nombre.
    - Límite: SECOP no ve la pauta pagada fuera de contrato ni la de entidades de régimen privado (Helios, Ecopetrol).

**3 · Las páginas institucionales de 2011.**
- `/quienes-somos/`: `datePublished` 2011-02-07T23:01:39, **sin `dateModified`**. Literal: «MiPutumayo.com.co – Magazín Informativo Digital del Putumayo, fundado el 17 de Marzo de 2004 por Luis Carlos Chamorro Burbano (www.chamorro.com.co)», «es un magazín informativo imparcial, neutral e independiente que ofrece sus espacios a la comunidad en el Putumayo», y cierra con «Luis Carlos Chamorro Burbano Director». El pie dice «© 2023». **Exacto.**
- `/colaboradores/`: `datePublished` 2011-02-07T23:22:45, sin `dateModified`. Empieza: «MiPutumayo.com.co en su nueva versión cuenta con los siguientes colaboradores». **El tramo que cita el revisor es literal**, incluido «Oficina de Prensa Luis Fernando Ochoa – Institucional, Gestión Cámara de Representantes Oficina de Prensa Guillermo Rivera – Institucional, Gestión Cámara de Representantes Editores Sandra Martínez Defensor del Lector Director Luis Carlos Chamorro Burbano». «Defensor del Lector» aparece sin nombre: la lectura ambigua del revisor es correcta.
- **Rivera**, en Wikipedia, literal: «Fue Representante a la cámara por el departamento de Putumayo entre 2002 y 2014 por el Partido Liberal». La ficha lo da como embajador ante Brasil del «13 de enero de 2023-3 de julio de 2025» y como del Partido Alianza Verde (en la ficha técnica). **Exacto.**
- **Ochoa** (el revisor no lo comprobó): `es.wikipedia.org/wiki/Luis_Fernando_Ochoa_Zuluaga` lo registra como «Representante a la Cámara por Putumayo 2010-2014», con Apertura Liberal y Partido Social de Unidad Nacional. Que sea la misma persona que la «Oficina de Prensa Luis Fernando Ochoa» de la lista es probable, pero no está probado. Si lo es, la lista describe el periodo 2010-2014, en el que los dos eran representantes por el Putumayo, de partidos distintos. En cualquier caso es **historia**: no entra como evidencia de orientación, ni en un sentido ni en otro.
- «Editores Sandra Martínez» no permite saber si hay hoy una editora. No consta.

**«Lo que falta» y «Evidencia que no mueve el número».** Todo lo que el revisor cita está en el HTML, con la fecha que dice:
- **Lanzamiento de enputumayo.com.co.** 2026-10-02T14:46:19, categoría «Varios». Literal: «MiPutumayo.com.co anuncia el lanzamiento oficial de su nueva plataforma de información y servicios: enputumayo.com.co . Esta nueva herramienta digital nace como un directorio integral…».
  - Matiz: el mismo texto dice que el registro de anuncios es «completamente gratuito».
  - En el directorio figura «Publimayo SAS – Comunicaciones, Publicidad y Mercadeo, Mocoa».
- **«Libro de la verdad»** (2026-08-19T03:35:26), crédito «ElTiempo» y enlace al original. La cita es literal salvo las comillas tipográficas: ‘pecados’.
- **Presupuesto de la Amazonía** (2026-09-24), crédito «LaSillaVacia» y enlace a lasillavacia.com: «mucho del presupuesto no lo asignó De la Espriella, sino que lo dejó amarrado Petro a través de vigencias futuras». Literal.
- **Advertencia al CRIC** (2026-10-07), crédito «ElHeraldo» y enlace a elheraldo.co: «De la Espriella fue enfático al señalar que en su Gobierno no se permitirán los bloqueos ni las vías de hecho». Literal; sigue «como forma de protesta».
- **Aspersión** (2026-09-08): las dos citas son literales («…impuesto por la Corte Constitucional» sigue con «de Colombia»). No se ve crédito externo en el texto. Confirmado.
- **Campesinos** (2026-10-07), crédito Caracol Radio y enlace a caracol.com.co: literal.
- **MOE y Cepeda** (2026-07-15), crédito Infobae y enlace a infobae.com. Confirmado.
- **Columna** del 2026-10-05, «Por: *Alexander Africano», categoría «Opinión»: literal.
  - Omisión del revisor: la firma lo presenta como «*Consejero Departamental de Paz – Putumayo».
  - Cláusula de los Términos de uso (`datePublished` 2010-03-01): literal.
- **Ecopetrol** (2026-09-02): literal. Las «otras tres piezas de Ecopetrol en agosto y septiembre» existen: 08-27, 09-10 y 09-14.
- **Búsquedas internas:** todos los slugs y fechas que cita el revisor existen.
  - Omite, en `?s=uribe`, «con-uribe-para-derrotar-a-abelardo-la-encrucijada-de-sandra-chindoy» (2026-07-20) y «alvaro-uribe-dice-que-en-la-frontera-con-ecuador…» (2026-04-16).
  - Omite, en `?s=De+la+Espriella`, cuatro piezas de septiembre sobre la aspersión y la zona de ubicación temporal (09-14, 09-25, 09-29 y 09-30).
  - No se leyeron, así que no se califican.
- **Titulares replicados** (el revisor no pudo comprobarlo). En las cuatro réplicas con enlace al original, el slug de MiPutumayo es **idéntico** al del original enlazado. Es un indicio de que el titular se reproduce, no de que se reescriba. No es prueba: no se abrieron los originales.

### La fuente «rota» del envío: falso positivo del armador

**La fuente no está rota.** `https://miputumayo.com.co/quienes-somos/` respondió 200 aquí:
- tres veces con curl (GET en ~0,3 s, 60 370 bytes; HEAD en ~1,3 s);
- cuatro veces con Node `fetch`, reproduciendo el armador: HEAD 200 en 1,3-2,1 s y GET 200 en ~0,2 s, servido por Cloudflare.

La propia auditoría del repositorio (`auditoria/estado.json`, `comprobadoEl` 2026-10-08) la tiene con `status` 200, `estado: "sano"`.

**Qué vio el script.** En `scripts/armarEnvio.mjs`, el texto `sin respuesta` solo aparece cuando el GET aborta por tiempo (`AbortError` tras `TIMEOUT_MS = 20_000`), después de un HEAD que tampoco dio un estado válido. **No hay reintento**: un solo tiempo agotado basta para declarar «NO RESUELVEN».
- Un 525 de Cloudflare habría salido en la cabecera como `` `525` ``, no como `sin respuesta`. Lo que vio el armador fue, por tanto, un tiempo agotado, coherente con un origen que va a ratos.
- **Es un falso positivo del script**: un fallo transitorio declarado como fuente rota.

**El diagnóstico del revisor acierta en lo sustancial** (intermitencia del servidor, no enlace muerto), pero falla en tres detalles:
- no fue «el centinela», sino el armador del envío;
- el 525 no es lo que registró el script;
- `--ssl-no-revoke` es una peculiaridad de curl con schannel en Windows. El `fetch` de Node no comprueba la revocación de certificados, así que no explica el fallo del script.
- En esta verificación no se reprodujo ningún 525 ni ningún tiempo agotado.

**Nota menor.** El envío se fechó «2026-10-09» porque el armador toma la fecha en UTC (`new Date().toISOString()`). Si se armó la noche del 2026-10-08 en Colombia, en UTC ya era día 9. Las cabeceras de las 00:51 GMT que cita el revisor van en el mismo sentido.

### ¿Está probada la identidad?

**(a) Director de MiPutumayo = titular de la matrícula 24541 = representante legal de Publimayo SAS en 2018-2020: acreditada por convergencia, con cargo cruzado.** Se publica como evidencia convergente, igual que en Boyacá Digital. La cadena:
1. «Quiénes somos» nombra a «Luis Carlos Chamorro Burbano» fundador y director, y enlaza su página personal, `www.chamorro.com.co`.
2. Esa página (sin fecha) lo presenta como «Periodista - Director MiPutumayo Noticias» y, en el mismo bloque, como «Desarrollo Web - Comunicaciones, Publicidad y Mercadeo Publimayo.com.co», con un correo de gerencia de Publimayo. La cita omite el teléfono y los correos: son datos de contacto de una persona natural.
3. En SECOP I, los cuatro contratos de Publimayo SAS de 2018-2020 llevan como representante legal a **«LUIS CARLOS CHAMORRO BURBANO»**, y su documento es **idéntico** al de la matrícula 24541 del Putumayo y al de la 827553 de Bogotá. Se comprobó por igualdad, sin escribirlo.
4. El sitio de Publimayo firma «© 2022 Publimayo SAS • MiPutumayo.com.co» y vende contenido en el medio.

Ningún documento del medio da el número de identificación de su director, así que la prueba no es documental en sentido estricto. Pero es exactamente el «cargo cruzado» cuya ausencia dejó sin probar el caso de El Pilón: la persona del registro ocupa el puesto que el propio director declara. **Lo que sigue sin constar:** quién posee las acciones de Publimayo SAS (el RUES abierto no lo publica) y quién posee el medio. Ni la ficha ni el medio documentan que «propiedad y dirección son la misma persona».

**(b) «Sandra Martínez», editora en la página de 2011 = Sandra Janneth Martínez Delgado, representante legal de Publimayo SAS: no probada. Homonimia no descartada.** El nombre es muy común y la página tiene quince años. No entra como hecho.
- Dato para la decisión del responsable editorial: con el documento de la representante legal (por igualdad, sin escribirlo), SECOP II devuelve **5 contratos de servicios profesionales suyos como persona natural, por $68.970.000**. Cuatro son con **Corpoamazonía** (2025-02-25, 2025-05-06, 2025-09-23 y 2026-01-13; tesorería y cartera). Uno es con la **Gobernación del Putumayo** (2026-07-24, $10.500.000; apoyo contable y financiero a la Secretaría de Desarrollo Agropecuario y Medio Ambiente).
- En los últimos 12 meses son 2, por $26.500.000.
- SECOP II escribe su nombre como «SANDRA JANNET MARTINEZ DELGADO». SECOP I: 0.
- No son contratos del medio ni de Publimayo.

### Motivo de cada rechazo

- **Obj. 1, la «homonimia» de Bogotá.** Es falsa: el número de identificación coincide. Afirmar que hay homonimia donde el registro muestra a la misma persona es el error inverso al de atribuir por nombre. Tampoco hace falta para nada: la matrícula de Bogotá es de 1997-1999, es decir, historia.
- **Obj. 1, «funciona hoy sin matrícula mercantil activa del director ni de una sociedad».** Es falsa en su segunda mitad: Publimayo SAS está activa, renovada en 2026, con el director como representante legal en 2018-2020, y es la sociedad que vende la publicidad del medio. Además, sugerir que el medio opera sin el registro que «respalde» su explotación comercial insinúa una irregularidad que nadie ha documentado.
- **Obj. 2, Tránsito como «anunciante visible».** La pieza está en «Otras Noticias», no en «Publicaciones». Nada indica que sea un aviso contratado.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente.** Todas las URL resuelven, las fechas coinciden y las citas literales aparecen en el HTML. Deformaciones y omisiones:
- **Homonimia de Bogotá:** falsa (ver arriba).
- **CIIU 6311 = «portales web»:** inexacto; los portales web son el 6312. Además, omite el 7310 (publicidad) de la misma matrícula.
- **Tránsito** entre los anunciantes de «Publicaciones»: deformado.
- **«No hay una sociedad que pueda venderse o fusionarse»:** el revisor buscó solo por «MiPutumayo» y no por «Publimayo», el nombre que él mismo encontró en todas las páginas. Es la omisión más importante de la respuesta.
- **SECOP de Publimayo SAS:** omitido (6 contratos con la Cámara de Comercio del Putumayo).
- **La fuente «rota»:** atribuida al centinela y a un 525; fue el armador, y fue un tiempo agotado.
- Menores: la cita del `robots.txt` normaliza «Allow :»; no menciona que el columnista es consejero departamental de paz; omite dos empresas de energía en «Publicaciones».
- **Errores de la propia ficha, para no repetirlos:**
  - «Una persona, ninguna sociedad»: hay una SAS activa ligada al director y al medio.
  - «No declara ni financiación ni sociedad»: el medio publica tarifa desde 2014 (modificada en 2024), y Publimayo declara que vende contenido patrocinado en él.
  - La declaración de nivel 4 se cita sin fecha; es de 2011.
  - «Su feed devolvió artículos de hace 51 horas»: caducado. La auditoría del 2026-10-08 da el feed sano, con 8,4 piezas/día.
  - En `shared/mediaOwnership.js`: **`ownerType: 'familiar'`** («Controlado por una familia») **no tiene ninguna fuente**. Nada en el expediente habla de una familia. Además, «Propiedad y dirección son la misma persona natural» no consta: «Quiénes somos» dice «fundado por» y «Director», no «propietario». La misma frase está en `shared/centinela.js` («Propiedad y dirección son la misma persona natural desde 2004») y, en otra forma, en el `biasRationale` de `shared/mediaRegistry.js` («Sin sociedad ni financiación declaradas»).

---

**Propuesta para la firma**

**(a) Valor: mantener 0,00, provisional de alta y NO firmable todavía.**
- **No se mueve**:
  - por la **regla 3**: no hay evidencia de nivel 1-3 que sitúe al medio. No hay nivel 2 (MiPutumayo no figura en `data/conducta.json`, y el envío fue sin cifras), y el nivel 1 identifica una sociedad comercial, no una línea;
  - por la **regla 2**: ante la duda, la banda mixta.
- **Lo que cambia es la razón escrita.** Ya no es «la mixta es lo que el propio medio declara ser». Pasa a ser: **«0,00 por las reglas 2 y 3: sin conducta medida. La propiedad del medio no está documentada; lo que consta es la sociedad que comercializa su publicidad y contenido patrocinado, Publimayo SAS, ligada al director y sin accionistas públicos. En 2026 replica a medios de signos distintos (El Tiempo, La Silla Vacía, El Heraldo, Caracol Radio, Infobae), publica avisos de prestadores de servicios públicos y material de Ecopetrol y de la fuerza pública, y no consta endoso. Nada de eso es nivel 1-3 ni lo mueve».**
- **No se firma** mientras no haya nivel 2 de 90 días que separe lo propio de lo replicado, y mientras no conste quién posee el medio y Publimayo SAS.

**(b) Correcciones de hecho, con su fuente**

En `fichas/miputumayo.md`:
1. **Título del nivel 1:** «Una persona, ninguna sociedad» → **«Un director-fundador, y una sociedad comercial ligada: Publimayo SAS. La propiedad del medio no está documentada»**.
2. **Fila «Razón social / NIT»:** «no constan» → **«El medio no declara sociedad editora. Consta Publimayo SAS ("PUBLIMAYO-COMUNICACIONES PUBLICIDAD Y MERCADEO SAS", NIT 901152998-5, Cámara de Comercio del Putumayo, matrícula 65530 del 07-02-2018, renovada el 07-05-2026, ACTIVA; CIIU 7310 publicidad y 6391 agencias de noticias; RUES, datos.gov.co `c82u-588k`, consultado el 2026-10-08). Ofrece "Banners (Publicidad) y Comunicados de prensa y artículos con Contenido Patrocinado en MiPutumayo.com.co y Portales Aliados" (publimayo.com.co, consultado el 2026-10-08)»**.
3. **Filas nuevas:**
   - **«Representante legal de Publimayo SAS: Sandra Janneth Martínez Delgado (RUES, actualizado el 07-05-2026). En 2018-2020, Luis Carlos Chamorro Burbano (SECOP I, cuatro contratos con la Cámara de Comercio del Putumayo)»**.
   - **«Matrícula mercantil personal del director: Cámara del Putumayo, n.º 24541, 2004-2021, CANCELADA el 29-04-2021 (RUES)»**.
   - **«Vínculo director-Publimayo: su página personal, enlazada desde "Quiénes somos", lo presenta como director de MiPutumayo y con la gerencia de Publimayo (www.chamorro.com.co, sin fecha, consultada el 2026-10-08). Evidencia convergente, no certificado»**.
4. **Fuente del nivel 1:** «su página "Quiénes somos"» → añadir **«(publicada el 07-02-2011, sin fecha de modificación; consultada el 2026-10-08)»**. Mantener «lo sigue dirigiendo hoy» solo con esa fecha a la vista.
5. **Nivel 4:** «No declara ni financiación ni sociedad» → **«No declara sociedad editora. Publica una tarifa de publicidad ("Paute Aquí", 2014, modificada el 12-01-2024) y una sección "Publicaciones" con avisos de prestadores de servicios públicos (Helios Energía, EMEVASI, Empresa de Energía del Putumayo, Empresa de Energía del Bajo Putumayo, Aguas Mocoa; septiembre de 2026). Sus Términos de uso (2010) separan la opinión firmada de "la posición editorial"»**.
6. **Nivel 2:** «Su feed devolvió artículos de hace 51 horas» → **«Feed sano (auditoría del 08-10-2026: 8,4 piezas/día). Sin conducta medida: no figura en `data/conducta.json`»**. Añadir que buena parte de lo nacional son réplicas acreditadas, publicadas con el usuario «director»: El Tiempo (19-08-2026), La Silla Vacía (24-09), El Heraldo y Caracol Radio (07-10), Infobae (15-07). La medición tiene que separarlas de lo propio.
7. **Nivel 5, nuevo, marcado «no mueve el número»:** las piezas verificadas de los días 15-07, 19-08, 08-09, 24-09, 05-10 y 07-10-2026, con sus citas, y la ausencia de endoso en lo revisado. La búsqueda no es exhaustiva: primera página de cada búsqueda interna.
8. **CONTRA:** añadir la tensión de (c)1.
9. **REFUTACIÓN:**
   - El punto 2 («Razón social y NIT») se da por respondido en parte y se reescribe así: **«El certificado de existencia de Publimayo SAS (matrícula 65530, Cámara del Putumayo) y quién es su accionista; y si hay un documento que diga quién posee el medio o su dominio»**.
   - El punto 1 se reescribe así: **«Quién paga las "Publicaciones" y qué piezas son contenido patrocinado»**.
   - El punto 3 añade **«separando lo propio de lo replicado»**.
10. **CONTRATACIÓN PÚBLICA**, línea nueva en el formato del protocolo:

> Contratación pública (SECOP I y II, consultado 2026-10-08). Del director como persona natural, consultado por su documento, que no se publica (dato personal, Ley 1581): 0 contratos en SECOP I y II a 2026-10-08. De Publimayo SAS (NIT 901152998), la sociedad que comercializa la publicidad del medio: 0 contratos en los últimos 12 meses (2025-10-08 → 2026-10-08); 6 por $6.520.500 en total desde 2018, todos en SECOP I y todos **contratados** con la Cámara de Comercio del Putumayo (hosting, dominios y web, 2018-2020; publicidad por banner «en distintos portales», 2024), y 0 en SECOP II. La Cámara de Comercio es una entidad privada con funciones públicas, no un gobierno. Las entidades públicas que publican avisos en el medio (Aguas Mocoa, EMEVASI) no tienen en SECOP contratos con el director ni con Publimayo.

En `shared/mediaOwnership.js`, entrada `miputumayo`:

11. **`ownerType: 'familiar'`**: no tiene fuente. Se propone **`null`**, a la espera del certificado de Publimayo SAS, como se hizo con otros medios que esperan su certificado. Si se prefiere no tocarlo, se declara la tensión en `notes`, como en Boyacá Digital. **Decisión del responsable editorial.**
12. **`holdings[0]`:** «Propiedad y dirección son la misma persona natural» → **«Lo fundó Luis Carlos Chamorro Burbano el 17 de marzo de 2004 en Mocoa, y figura como director en "Quiénes somos" (página de 2011). Quién posee el medio no consta.»** Añadir **`holdings[1]`** con Publimayo SAS (punto 2) y la representación legal (punto 3).
13. **`notes`:**
    - sustituir «No consta sociedad, ni NIT, ni fuente de financiación» por la línea de contratación del punto 10 y por la tensión de (c)1;
    - añadir la laguna: **«Quién es accionista de Publimayo SAS y quién posee el medio: no consta. Lo cierra el certificado de la Cámara de Comercio del Putumayo»**.
14. **`sources`:** añadir:
    - `https://miputumayo.com.co/paute-aqui/`;
    - `https://miputumayo.com.co/category/publicaciones/`;
    - `https://publimayo.com.co/`;
    - `https://www.chamorro.com.co/`;
    - la consulta del RUES por Publimayo (`https://www.datos.gov.co/resource/c82u-588k.json?$select=razon_social,sigla,nit,camara_comercio,matricula,organizacion_juridica,estado_matricula,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,fecha_cancelacion,cod_ciiu_act_econ_pri&nit=901152998`);
    - la de SECOP I por el NIT de Publimayo (`https://www.datos.gov.co/resource/f789-7hwg.json?$select=numero_de_constancia,nombre_entidad,nom_razon_social_contratista,fecha_de_firma_del_contrato,cuantia_contrato,valor_total_de_adiciones,detalle_del_objeto_a_contratar,estado_del_proceso&identificacion_del_contratista=901152998`).
    - **Ninguna URL lleva el documento del director.**

En `shared/centinela.js`, entrada `miputumayo`:

15. `vigila`: quitar «Propiedad y dirección son la misma persona natural desde 2004» y decir **«Que Luis Carlos Chamorro Burbano siga al frente; es director y fundador, y la propiedad no consta»**. Añadir una consulta **`'Publimayo'`** que vigile cambios en la sociedad que comercializa el medio.

En `shared/mediaRegistry.js`:

16. `biasRationale`: «Sin sociedad ni financiación declaradas» → **«Propiedad sin documentar; su publicidad y contenido patrocinado los comercializa Publimayo SAS, ligada al director»**, más la razón de (a).

En `scripts/armarEnvio.mjs` (no es un hecho de la ficha; **decisión del responsable editorial**):

17. Reintentar una vez, con espera, antes de declarar una fuente «NO RESUELVE» cuando el fallo es `sin respuesta`, y decir en la cabecera si el fallo fue tiempo agotado o código HTTP. Un tiempo agotado aislado no es un enlace muerto.

**(c) Tensiones a declarar en la ficha**
1. **Contenido patrocinado sin marca.** Publimayo SAS, ligada al director, vende «artículos con Contenido Patrocinado en MiPutumayo.com.co». En el medio, los avisos de prestadores de servicios públicos (septiembre de 2026) y la pieza corporativa de Ecopetrol del 2026-09-02 salen sin ninguna marca, con el usuario «director». **No consta que ninguna esté pagada.** Lo que consta es que el lector no puede distinguir lo pagado de lo que no lo es. Es desvelamiento, no acusación.
2. **Lagunas declaradas, no tensiones:**
   - quién posee el medio y quién es accionista de Publimayo SAS;
   - si la editora «Sandra Martínez» de 2011 es la representante legal actual de Publimayo (**homonimia no descartada**);
   - si hay hoy una editora o un defensor del lector;
   - quién paga las «Publicaciones».
   - Las cierra el certificado de la Cámara de Comercio del Putumayo y, en parte, una pregunta directa al medio.

**Lo que NO entra como hecho:**
- que los avisos de «Publicaciones» o las piezas de Ecopetrol estén pagados;
- que el director sea el dueño del medio;
- que la editora de 2011 y la representante legal de Publimayo sean la misma persona;
- que el medio opere de forma irregular por no tener matrícula personal activa;
- la «homonimia» de Bogotá;
- las oficinas de prensa de Rivera y Ochoa como vínculo político vigente, que es historia (regla del presente);
- **los contratos personales de la representante legal de Publimayo** con Corpoamazonía y la Gobernación del Putumayo. No son del medio ni de su sociedad, y su papel editorial no consta. **Decisión del responsable editorial.** Recomendación: dejarlos en el expediente interno, sin cédula, y llevarlos a la ficha solo si se documenta que tiene un papel editorial o societario en el medio más allá de la representación legal de Publimayo. El precedente de El Nuevo Día declaró el contrato de quien presidía la junta, que es un cargo con más peso.

**¿Aviso de quien dirige?** No procede. No consta candidatura ni cargo público vigente del director en lo consultado aquí: el sitio, el RUES, SECOP y Wikipedia. Sin buscador web, no se comprobó en prensa de terceros, y se declara como laguna.

---

### Nota posterior (2026-10-08, Claude Code)

**El envío no llevó la conducta medida.** Se armó sin regenerar `data/conducta.json`, que solo tenía los cinco medios de la tanda 3, así que el revisor no recibió cifras de nivel 2 y esta resolución no las usó. Medido después con `npm run conducta` (ventana 2026-08-31 → 2026-10-09, 38 días): 221 artículos, 28 en alguna historia, 29 historias, 34 % de agenda propia, 19 compartidas, compañía media 0,151; coincide con El Heraldo (6), Caracol Radio (6) y La Silla Vacía (4). Sigue en pie la advertencia de separar lo propio de lo replicado. Con 38 días no se llega a los 90 que pide el protocolo, así que **la propuesta para la firma no cambia**. Las cifras entran en el nivel 2 de la ficha con su advertencia.
