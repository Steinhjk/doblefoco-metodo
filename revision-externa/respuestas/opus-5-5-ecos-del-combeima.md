# Respuesta — Claude Opus 5.5 sobre Ecos del Combeima

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
Soy Claude Opus 5.5 (id de modelo: claude-opus-5-5), de Anthropic: la misma casa que el modelo que escribió la ficha. Puede que comparta sus sesgos de compresión y sus puntos ciegos. Para compensarlo he dado prioridad a fuentes primarias que la ficha NO usa: el registro mercantil abierto (RUES), SECOP I y II, la parrilla y el tarifario de la propia emisora y sus notas fechadas. No he leído ningún archivo del repositorio, salvo el envío. Mi acuerdo no debe usarse como aval.

MÉTODO Y DÓNDE BUSQUÉ (2026-10-10, entre las 18:00 y las 18:30 UTC)
- robots.txt revisados antes de descargar: ecosdelcombeima.com (solo «User-agent: *», no excluye a ClaudeBot, Claude-Web ni anthropic-ai), bluradio.com (excluye a GPTBot y ChatGPT-user, no a los agentes de Anthropic) y es.wikipedia.org (sin exclusión para Anthropic; usé solo la ruta /wiki/).
- HTML crudo descargado con curl -sL y User-Agent de navegador en t7\combeima-dl: ecosdelcombeima.com en / , /nosotros, /al-aire (parrilla), /tarifas, /contacto, /ping-pong-politico y /tags/blu-radio, además de /rss.xml, dos notas sobre la muerte del titular, la nota del premio de periodismo y la nota sobre El Nuevo Día que cita la ficha. De bluradio.com, la portada: /emisoras y /frecuencias dan 404. De Wikipedia, /wiki/Ecos_del_Combeima.
- RUES abierto (datos.gov.co c82u-588k): razon_social like '%COMBEIMA%' (100 filas), representante_legal o razon_social like '%ARNULFO SANCHEZ%' o '%ECOS DEL%', y Cámara de Ibagué con CIIU 6010/6020/5911/6391 y matrícula activa. Así encontré la sociedad: NIT 809006687.
- SECOP II (jbjy-vk9h, documento_proveedor='809006687') y SECOP I (f789-7hwg, identificacion_del_contratista='809006687'), con igualdad exacta y sin dígito de verificación.
- Buscador web: lo usé 2 veces. Estuvo disponible. Solo lo usé para localizar URLs, y después leí las fuentes primarias en crudo.
- No toqué eltiempo.com, cambiocolombia.com, lasillavacia.com ni diariodelsur.com.co.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré venta, fusión ni escisión. La sociedad que factura como la emisora, INVERSIONES ECOS LIMITADA (NIT 809006687), sigue ACTIVA en la Cámara de Comercio de Ibagué y renovó la matrícula el 2026-05-26 (RUES, fecha_actualizacion 2026/05/26). El cambio material es anterior a la ventana pero la ficha no lo recoge: el titular murió el 14 de marzo de 2025 (ver objeción 1). La composición de socios tras la sucesión NO consta en el RUES abierto. No sé si hubo cesión de cuotas a herederos.

- La persona que la ficha nombra como titular o director, ¿sigue viva y en el cargo?
  NO. Arnulfo Sánchez López murió el 14 de marzo de 2025. Lo comprobé el 2026-10-10 en la propia emisora: https://www.ecosdelcombeima.com/ibague/nota-164793-luto-en-el-periodismo-tolimense-fallecio-arnulfo-sanchez (fechada «14 Mar 2025 - 7:15 COT»): «Este viernes 14 de marzo, el periodismo tolimense se viste de luto tras conocerse la muerte de Arnulfo Sánchez, el icónico maestro de la radio». La ficha, resuelta el 2026-08-18, lo da por propietario y director vigente 17 meses después de su muerte.

- ¿Quién dirige hoy la redacción?
  - Según el RUES, el representante legal de INVERSIONES ECOS LIMITADA es SANCHEZ BAQUERO JUAN PABLO (consultado el 2026-10-10).
  - La parrilla de la emisora (https://www.ecosdelcombeima.com/al-aire) pone como director de «Econoticias», de lunes a viernes de 05:00 a 13:00, a «Juan Pablo Sánchez». Esa parrilla dice «Actualizado 4 Oct 2024», así que es un dato de hace dos años.
  - No encontré un cargo de «director de la redacción web». Las notas van firmadas «por Ecos del Combeima».

- ¿Hay un registro mercantil más reciente que la fuente que la ficha cita?
  Sí. La ficha no cita ninguna fuente para la sociedad («Fuentes secundarias — no verificada en RUES»). El RUES abierto tiene un registro renovado el 2026-05-26 y muestra que la sociedad no es la que dice la ficha (ver objeción 2).

## OBJECIONES

OBJECIÓN 1 — El propietario y director vigente que nombra la ficha murió en marzo de 2025
- QUÉ AFIRMA LA FICHA: «Propietario y director | Arnulfo Sánchez López». También dice «Propietario y director son la misma persona», y su punto de refutación 3 se activa «Si Arnulfo Sánchez López aparece con cargo, contrato o candidatura pública».
- POR QUÉ ES INCORRECTO: murió el 14 de marzo de 2025. Es exactamente el tipo de error que el ciclo anterior encontró en cuatro fichas. La fuente que la ficha usa («Nosotros») está desactualizada: todavía dice «a la cabeza de Arnulfo Sánchez y Juan Pablo Sánchez Baquero». La ficha la leyó como si describiera el presente. El punto de refutación 3 sobra en su redacción actual, y la observación de gobernanza («quien decide la línea y quien pone el dinero» son la misma persona) hay que rehacerla con quien controle hoy la sociedad.
- FUENTES:
  · https://www.ecosdelcombeima.com/ibague/nota-164793-luto-en-el-periodismo-tolimense-fallecio-arnulfo-sanchez, del 14-03-2025. Cita: «Este viernes 14 de marzo, el periodismo tolimense se viste de luto tras conocerse la muerte de Arnulfo Sánchez». La misma nota: «tuvo dos hijos, Fernando y Juan Pablo, quienes continúan su legado en la radio a través de la emisora Ecos del Combeima y Ecos Interactiva».
  · https://www.ecosdelcombeima.com/tolima/nota-182531-nace-en-ibague-el-premio-arnulfo-sanchez-lopez-para-exaltar-el-periodismo, del 09-02-2026. Cita: «un reconocimiento que honra la memoria del fundador de Econoticias».
  · https://es.wikipedia.org/wiki/Ecos_del_Combeima, editada por última vez el 12-11-2025. Cita: «El 14 de marzo de 2025 fallece en Ibagué el periodista Arnulfo Sanchez López propietario de la emisora y director del informativo Econoticias». Es fuente terciaria y solo corrobora.
- NIVEL: propiedad.

OBJECIÓN 2 — La sociedad está mal identificada: no es «Inversiones Combeima», es INVERSIONES ECOS LIMITADA (NIT 809006687)
- QUÉ AFIRMA LA FICHA: «Sociedad | Inversiones Combeima | Fuentes secundarias — no verificada en RUES».
- POR QUÉ ES INCORRECTO: en el RUES abierto, las sociedades que se llaman «Inversiones Combeima» no son la emisora:
  · «INVERSIONES COMBEIMA LIMITADA», NIT 900162670: CANCELADA, último año renovado 2010.
  · «INVERSIONES COMBEIMA SAS EN LIQUIDACION», NIT 900746204: en liquidación, último año renovado 2015, CIIU 4771 (comercio de prendas de vestir), con un representante legal sin relación con la familia Sánchez.
  · «INVERSIONES COMBEIMA PLAZA S A»: Bogotá, CANCELADA.
  La sociedad que explota la emisora es INVERSIONES ECOS LIMITADA, de la Cámara de Ibagué, matriculada el 1999-09-27, ACTIVA, renovada el 2026-05-26, con CIIU principal 6010 (radiodifusión) y secundario 7310 (publicidad), inscrita como proponente en el RUP y con SANCHEZ BAQUERO JUAN PABLO como representante legal. El vínculo entre la sociedad y la emisora es un HECHO, no una inferencia: SECOP I lo dice literalmente en dos órdenes de la Cámara de Comercio del Sur y Oriente del Tolima, la OTB-234 (firmada el 2025-09-30) y la OTB-168 (firmada el 2025-06-09): «SERVICIO DE PUBLICIDAD RADIAL EN LA EMISORA (INVERSIONES ECOS LTDA. ES ECOS DEL COMBEIMA)». SECOP II registra el proveedor con NIT 809006687 bajo el nombre «ECOS DEL COMBEIMA».
  INFERENCIA, no hecho: el nombre «Inversiones Combeima S.A.S» de la ficha coincide con la ficha técnica de Wikipedia («Propietario: Inversiones Combeima S.A.S»). Lo más probable es que la ficha lo tomara de ahí.
  Lo que NO pude establecer: los socios de INVERSIONES ECOS LTDA y sus participaciones tras la sucesión. Para eso hace falta el certificado de existencia y representación (de pago) de la Cámara de Comercio de Ibagué.
- FUENTES (consultadas el 2026-10-10):
  · [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (fecha_renovacion 20260526)
  · [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (contratos OTB-234 y OTB-168)
- NIVEL: propiedad / registro externo.

OBJECIÓN 3 — Sí existía un primario sobre la afiliación a Blu, y la ficha no lo consultó; además, ese primario tiene fecha de 2024
- QUÉ AFIRMA LA FICHA: «Ni la página "Nosotros" de la emisora ni una lista oficial de afiliadas de Blu Radio lo dicen». Señala como primario pendiente «la parrilla de la emisora».
- POR QUÉ ES INCORRECTO: la parrilla está publicada en el sitio de la emisora y confirma la afiliación en fuente primaria. Esto refuerza el hecho de la afiliación, no lo tumba. https://www.ecosdelcombeima.com/al-aire (consultada el 2026-10-10) dice literalmente:
  · «Estás escuchando: Blu Radio … Descripción: Conexión Blu Radio».
  · De lunes a viernes: «01:00 pm a 02:00 pm Meridiano Blu — Blu Radio», «02:00 pm a 04:00 pm Blog Deportivo — Blu Radio», «04:00 pm a 07:00 pm Vox Pópuli — Blu Radio».
  · Sábados: «10:00 am a 12:00 pm Blu Radio».
  Sin embargo, la misma página dice «Actualizado 4 Oct 2024». Es un primario de hace 24 meses, no de hoy.
  El tarifario https://www.ecosdelcombeima.com/tarifas («Actualizado 13 de Septiembre de 2025») solo vende espacios propios: «Econoticias», «Golpes de Opinión», «Ecodeportes», «A toda máquina», «La Radioteka 790». Esos cuatro últimos programas no aparecen en la parrilla de 2024, lo que indica que la parrilla está desactualizada. No encontré un primario de 2026 que diga cuántas horas de Blu emite hoy. Wikipedia también lo afirma: «Desde el año 2013, está afiliado a la emisora Blu Radio». bluradio.com no publica una lista de afiliadas (/emisoras y /frecuencias dan 404 el 2026-10-10).
- NIVEL: declaración del propio medio.

OBJECIÓN 4 — El argumento dirimente («contaría dos veces al mismo grupo», «bajo Valorem») confunde afiliación de programación con propiedad, y lo que DobleFoco ingiere es el sitio web, que es producción local
- QUÉ AFIRMA LA FICHA: «Con Blu Radio ya en el catálogo en +0,25 y bajo Valorem, admitir esta emisora como voz propia del Tolima habría contado dos veces al mismo grupo», y que «comparte parrilla y quizá línea con una cadena nacional del grupo Santo Domingo».
- POR QUÉ ES DISCUTIBLE:
  · Propiedad (hecho, por las objeciones 1 y 2): la emisora es de una sociedad limitada local, administrada por la familia del fallecido titular. No encontré ningún vínculo societario con Valorem ni con Caracol. Afiliarse a una cadena es un contrato de emisión, no un control. Decir que el medio está «bajo» el grupo Santo Domingo no tiene respaldo.
  · Producción propia (hecho, con el límite de fecha de la objeción 3): según la parrilla, la franja informativa propia («Econoticias», 05:00–13:00, 8 horas) es mayor que la de Blu (13:00–19:00, 6 horas) en los días laborables.
  · Lo que entraría al corpus (hecho): el RSS (https://www.ecosdelcombeima.com/rss.xml, consultado el 2026-10-10, último pubDate «Sat, 10 Oct 2026 15:50:38 +0000») tiene 10 ítems. Ninguno contiene la cadena «blu». Todos son locales o comerciales: «Falsa patrullera y fotos hechas con IA: así estafaron a un adulto mayor en Ibagué», «‘Cultura SETP’, la estrategia que promueve el civismo…», «¡Este sábado en Aló Maestro…!». La sección propia de política (https://www.ecosdelcombeima.com/ping-pong-politico) es local y de autoría propia: entrevistas a precandidatos a la Alcaldía de Ibagué y a la Gobernación de 2027, de partidos distintos (Centro Democrático, Partido Conservador, una exgerente del IBAL). La página /tags/blu-radio no devolvió ninguna pieza listada en el HTML crudo.
  · INFERENCIA: el riesgo de «contar dos veces» solo existiría si el sitio republicara las piezas de Blu. Con lo que vi, no lo hace. Esto debilita la razón de fondo para negar el alta. La razón de fondo no se cae del todo, porque una parte de la antena sí es Blu.
  · Matiz (no medido): no puedo afirmar si la línea editorial imita la de Blu. El punto 2 de la refutación (90 días de corpus) sigue siendo la prueba correcta, y solo se puede hacer si se ingiere el feed.
- NIVEL: propiedad / declaración del propio medio / conducta observable (RSS, no medido).

OBJECIÓN 5 — Falta el hecho de gobernanza más material: la emisora depende en gran medida de la contratación de las administraciones que cubre
- QUÉ AFIRMA LA FICHA: nada. No hay sección de contratación pública, y la gobernanza solo se trata como «propietario = director».
- POR QUÉ IMPORTA: con el NIT 809006687, en igualdad exacta (SECOP II documento_proveedor, SECOP I identificacion_del_contratista, consultados el 2026-10-10):
  · Últimos 12 meses (firmados desde el 2025-10-10): 9 contratos por 736.000.000 COP.
    - SECOP II, 7 contratos por 731.000.000 COP:
      · CO1.PCCNTR.9076312 — Alcaldía de Ibagué — 2026-01-23 — 150.000.000 — contratación directa — «PRESTACIÓN DE SERVICIOS PARA CONTRIBUIR A LA DIFUSIÓN RADIAL MEDIANTE LA EMISIÓN DE CUÑAS; ENTREVISTAS; MENCIONES EN VIVO; ENTRE OTRAS; DE LAS ESTRATEGIAS Y GESTIONES ADELANTADAS POR LA ALCALDÍA MUNICIPAL DE IBAGUÉ».
      · CO1.PCCNTR.9766419 — Alcaldía de Ibagué — 2026-08-04 — 150.000.000 — contratación directa — «DIFUSIÓN RADIAL Y DIGITAL EN LOS DIFERENTES ESPACIOS INFORMATIVOS DE LA GESTIÓN PÚBLICA REALIZADA POR LA ALCALDÍA MUNICIPAL DE IBAGUÉ».
      · CO1.PCCNTR.9065920 — Gobernación del Tolima — 2026-01-24 — 275.000.000 — contratación directa — «SERVICIOS DE INTERCAMBIO INFORMATIVO DE LOS TEMAS INHERENTES AL FORTALECIMIENTO INSTITUCIONAL DE LA GOBERNACIÓN DEL TOLIMA; A TRAVÉS DE UN MEDIO DE COMUNICACIÓN RADIAL Y DIGITAL».
      · IBAL SA ESP Oficial: CO1.PCCNTR.9035717 (2026-01-22, 60.000.000) y CO1.PCCNTR.10028805 (2026-10-06, 30.000.000).
      · Cortolima: CO1.PCCNTR.9010502 (2026-01-20, 45.000.000) y CO1.PCCNTR.9801802 (2026-08-13, 21.000.000).
    - SECOP I, 2 contratos por 5.000.000 COP: OC-PB-2026-90, Cámara de Comercio de Ibagué, 2026-06-24, 4.000.000; y OTB-54, Cámara de Comercio del Sur y Oriente del Tolima, 2026-05-28, 1.000.000.
  · Total histórico: SECOP II, 55 contratos por 3.255.064.000 COP (2019–2026), con tendencia al alza: 2023, 511,9 M; 2024, 540,1 M; 2025, 775,7 M; 2026 hasta la fecha, 731 M. SECOP I, 35 contratos por 737.081.457 COP (2018–2026). Suma: unos 3.992 millones de COP.
  · Principales contratantes históricos en SECOP II: Alcaldía de Ibagué (1.198,5 M), Gobernación del Tolima (949 M), Cortolima (423,6 M), IBAL (341,3 M).
  · El objeto de dos contratos compra «entrevistas» y «menciones en vivo» y «espacios informativos de la gestión pública». Es decir, compra espacio dentro de la franja informativa, no solo cuñas. HECHO: así lo dice el texto del objeto. INFERENCIA: es un conflicto de interés estructural con la cobertura de la Alcaldía y la Gobernación, del mismo tipo que el que apareció con Diario La Libertad.
  · Corroboración adicional: la portada de la emisora (2026-10-10) enlaza un banner a https://tolima.gov.co/. Además, el 09-02-2026 la emisora publicó que la alcaldesa anunció, «durante una entrevista en Ecos del Combeima», un premio de periodismo con el nombre del fallecido propietario, «en articulación con la Gobernación del Tolima». Las dos entidades son sus mayores contratantes.
- FUENTES: [enlace retirado: puede mostrar documentos de identidad; ver la resolución] y [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (2026-10-10). Contratos citados como texto.
- NIVEL: registro externo / propiedad (gobernanza).
- CONSECUENCIA PARA LA DECISIÓN: este hecho, y no la afiliación a Blu, es el que con más solidez pide cautela ante un alta como «voz local independiente». Si se reconsidera el alta, debería ir con este conflicto declarado.

OBJECIÓN 6 — El único «hecho editorial de los últimos 12 meses» tiene casi tres años
- QUÉ AFIRMA LA FICHA: en «Nivel 5 — Hecho editorial de los últimos 12 meses» cita «Se acabó el impreso de EL NUEVO DÍA».
- POR QUÉ ES INCORRECTO: https://www.ecosdelcombeima.com/ibague/nota-235510-se-acabo-el-impreso-de-el-nuevo-dia está fechada «29 Dic 2023 - 15:23 COT» y relata el cierre del 22 de octubre de 2023. Queda fuera de la ventana de 12 meses y la regla del presente lo excluye. Hechos de producción local con fecha reciente sí los hay (los RSS del 08 al 10-10-2026 y Ping Pong Político, ver objeción 4).
- NIVEL: hecho editorial de los últimos 12 meses (mal fechado).

OBJECIÓN 7 — Incoherencias internas de la ficha
- QUÉ AFIRMA LA FICHA: a la vez, «Valor propuesto: NINGUNO» y, en ARGUMENTO, «+0,20». A la vez, «sustituye a El Nuevo Día» y «El Nuevo Día sí está en el catálogo». A la vez, «El Tolima se queda sin medio propio» y «el Tolima no queda mudo».
- POR QUÉ: son restos de la versión anterior a la resolución. Con estas contradicciones, el expediente no se puede auditar sobre qué se decidió.
- FUENTE: la propia ficha (envío del 2026-10-10).
- NIVEL: no aplica (coherencia documental).

## LO QUE NO PUDE VERIFICAR
- Los socios actuales de INVERSIONES ECOS LTDA y sus porcentajes, y si tras la sucesión hubo cambio de control. Busqué en el RUES abierto (c82u-588k) y ahí no constan socios. Hace falta el certificado de existencia y representación de la Cámara de Comercio de Ibagué.
- Si la afiliación a Blu Radio sigue vigente en octubre de 2026 y con cuántas horas. La parrilla primaria tiene fecha de 2024-10-04, y el tarifario de 2025-09-13 no menciona Blu. bluradio.com no publica una lista de afiliadas (404 en /emisoras y /frecuencias). La tarjeta «Estás escuchando: Blu Radio» de /al-aire es un widget de la página y no prueba qué sale al aire hoy.
- La sede «Cra. 8 n.º 57-29, Edificio Acqua WTC» coincide con /contacto (oficinas 1110-1111). Es la sede de la empresa, no una dirección particular.
- Qué fuentes secundarias «convergentes» usó la ficha el 2026-08-18: no las cita. No puedo comprobar de forma independiente la lista de afiliadas (La Caliente, Radio Magdalena, etc.), y no la busqué para ahorrar buscador.
- La asimetría a través del cambio de gobierno del 07-08-2026: no hice el barrido de 10 piezas con postura. Solo vi titulares de Ping Pong Político que no permiten contar posturas de la voz de la casa.

## LO QUE FALTA
- Una sección de contratación pública: 12 meses y total histórico (ver objeción 5).
- El RUES de INVERSIONES ECOS LTDA con su NIT, en lugar de una «Inversiones Combeima» sin fuente.
- La parrilla primaria (/al-aire) como fuente de la afiliación, con su fecha de actualización.
- El estado de la sucesión del titular fallecido y quién controla hoy la sociedad.
- Un hecho editorial realmente dentro de los 12 meses.
- Si se reconsidera el alta: ingerir el RSS, que funciona y no está declarado, para hacer la prueba de 90 días del punto 2 de la refutación.

## EVIDENCIA QUE NO MUEVE EL NÚMERO
- La afiliación a Blu queda confirmada por un primario (la parrilla propia), aunque esté fechado en 2024. Respalda el hecho que la ficha da por sentado, no lo refuta.
- La redacción local está activa: el RSS tiene piezas del 08 al 10-10-2026, y los audios de /al-aire muestran el «09/10/2026» con notas de Ibagué.
- Ping Pong Político da voz a varios partidos de cara a 2027 (Centro Democrático, conservadores, aspirantes empresariales, una exgerente del IBAL). En los titulares vistos no aparece un endoso editorial. No lo medí como asimetría.
- Columnistas de terceros (la portada lista a 10, entre ellos un exministro). Según el protocolo, las columnas de terceros no son voz de la casa.
- El tarifario vende «Envío de Whatsapp a la base Plus de seiscientos (600) empresarios, políticos y amigos de Ecos del Combeima» y «Publirreportaje multimedia». Es un modelo comercial, sin efecto directo sobre el eje.

## SIN OBJECIÓN
No aplica: hay 7 objeciones.

Balance (hecho e inferencia separados): la afiliación a Blu Radio es real según un primario de 2024, pero NO es propiedad del grupo Santo Domingo. El titular está muerto desde 2025, y la sociedad es otra (INVERSIONES ECOS LTDA). El argumento de «contar dos veces a Valorem» es débil por construcción. La recomendación de no dar el alta puede mantenerse, pero por otra razón mejor documentada: la fuerte dependencia de contratos de la Alcaldía de Ibagué y de la Gobernación del Tolima, que incluyen «entrevistas» y «menciones en vivo» en la franja informativa. Si se quiere un medio del Tolima, la vía es darlo de alta como afiliada local con propiedad familiar, con el conflicto contractual declarado y la prueba de 90 días sobre su RSS. Las dos opciones son defendibles. Lo que no es defendible es la motivación actual de la ficha.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-10. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal: ninguna.** El revisor no copió cédulas, teléfonos ni direcciones particulares de personas naturales. Se comprobó:
- el número de documento del representante legal que da el RUES no aparece en el texto (búsqueda literal del número, 0 apariciones);
- las cifras largas que contiene son el NIT de la sociedad, los NIT de dos sociedades homónimas, una fecha de renovación y los identificadores de contrato de SECOP;
- la dirección «Cra. 8 n.º 57-29, Edificio Acqua WTC» es la sede de la empresa, que el propio medio publica en `/contacto`; la regla no la cubre;
- no hay URL cuya página muestre la cédula de una persona natural: los enlaces de datos.gov.co que cita son consultas por NIT de una sociedad.

Esta resolución tampoco escribe ninguno de esos datos. De la nota necrológica del 14-03-2025 solo se usa el hecho de la muerte; se dejan fuera la edad, el cónyuge y demás datos de familia.

**Cómo se verificó.**
- **robots.txt**, leído antes de descargar nada (2026-10-10):
  - www.ecosdelcombeima.com: solo «User-agent: *», con exclusiones de Drupal (`/admin/`, `/search/`, `/user/…`, `/core/`). Nada sobre ClaudeBot, Claude-Web ni anthropic-ai. No se usó ninguna ruta excluida.
  - www.bluradio.com: «User-agent: *» con cuatro exclusiones técnicas; bloques propios para grapeshot, ChatGPT-user, GPTBot y bingbot. Nada para Anthropic.
  - es.wikipedia.org: sin exclusión para Anthropic; solo se usó `/wiki/`.
  - www.datos.gov.co: `Crawl-delay: 1`; se respetó con pausas entre consultas.
  - myradioenvivo.co (agregador, ver obj. 3): «User-agent: * … Allow: /».
  - No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com ni diariodelsur.com.co.
- **Sitio de la emisora**, descargado en crudo con `curl -sL --ssl-no-revoke` y User-Agent de navegador, en `t7\combeima-ver`: portada, `/nosotros`, `/al-aire`, `/tarifas`, `/contacto`, `/ping-pong-politico`, `/tags/blu-radio`, `/rss.xml`, las notas 164793 (muerte), 182531 (premio) y 235510 (El Nuevo Día), tres piezas de Ping Pong Político (194546, 194572 y 194611) y el audio 160384 (bienvenida de Blu, ver obj. 3). Todo 200. Texto extraído del HTML quitando etiquetas.
- **Blu Radio:** portada 200; `/emisoras` y `/frecuencias`, 404. Coincide con el revisor.
- **Wikipedia:** `/wiki/Ecos_del_Combeima`, revisión 170457690, «Esta página se editó por última vez el 12 nov 2025 a las 19:21».
- **Señal en vivo:** el reproductor de `/al-aire` apunta a un servidor Icecast. Su `status-json.xsl` responde (Icecast 2.4.4, arrancado el 2026-10-08), pero sin ninguna fuente montada a las 18:31 UTC: el `/stream` no devolvió audio ni metadatos. No se pudo saber qué sonaba.
- **Registros**, en datos.gov.co, todos con **igualdad exacta** y sin dígito de verificación:
  - RUES (`c82u-588k`): `nit='809006687'`; y `upper(razon_social) like '%COMBEIMA%' AND like '%INVERSIONES%'` para los homónimos.
  - SECOP II (`jbjy-vk9h`): `documento_proveedor='809006687'`, `$limit=5000`.
  - SECOP I (`f789-7hwg`): `identificacion_del_contratista='809006687'`, `$limit=5000`.
  - Duplicados: ningún `id_contrato` repetido en SECOP II ni `uid` repetido en SECOP I. En SECOP I, `valor_total_de_adiciones` es 0 en los 35. En SECOP II el conjunto no trae adiciones de valor; solo `dias_adicionados` (ver obj. 5).
- **Buscador web:** 1 consulta («"Ecos del Combeima" "Blu Radio" 2026»), solo para localizar URL. Lo útil que dio se leyó después en crudo.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | El propietario y director que la ficha da por vigente murió el 14-03-2025 | sí | sí | **Aceptada.** La nota de la propia emisora es fuente primaria y fechada. La ficha se resolvió el 2026-08-18, diecisiete meses después |
| 2 | La sociedad es INVERSIONES ECOS LIMITADA (NIT 809006687), no «Inversiones Combeima» | sí | sí | **Aceptada.** RUES y SECOP coinciden al dato. SECOP I lo dice literal en tres contratos, no dos |
| 3 | La afiliación a Blu consta en un primario (parrilla) de 2024; su vigencia hoy no está probada | sí | sí | **Aceptada, con un añadido.** Hay un primario más claro y más antiguo: un audio de la propia emisora del 18-08-2020 en que Blu le da «la bienvenida» como afiliada. La vigencia hoy sigue sin prueba: la señal no estaba en el aire al consultarla y el «Suena ahora» de un agregador repite la parrilla |
| 4 | La razón de «contar dos veces a Valorem» confunde afiliación con propiedad; lo que se ingeriría es producción local | sí | sí | **Aceptada en el fondo; parcial en la prueba.** Afiliación no es propiedad, y no hay vínculo societario con Valorem. Pero 10 ítems del RSS no bastan para llamar «local» al feed (dos son de Bogotá y Dosquebradas, sin autor), y las horas de antena salen de la parrilla de 2024 |
| 5 | La emisora depende de la contratación de las administraciones que cubre | sí | sí | **Aceptada; cifras exactas al peso.** Se añade que el contrato que compra «entrevistas; menciones en vivo» no es de 2026 solo: es el mismo objeto (PI03) en 2025, por 225 M. Va como **pauta informativa pagada**, tensión, igual que en Telecafé |
| 6 | La pieza sobre El Nuevo Día es del 29-12-2023 | sí | sí | **Aceptada** |
| 7 | Incoherencias internas de la ficha | sí | sí | **Aceptada, y ampliada:** el desfase alcanza también a `fichas/el-nuevo-dia.md`, a `fichas/LEEME.md`, a `MEDIOS_CANDIDATOS_DEPARTAMENTOS.md` y a un comentario de `shared/mediaRegistry.js` |

### Lo verificado, objeción por objeción

**1 · La muerte del titular.**
- **Nota 164793** (HTML crudo, 2026-10-10), fechada «14 Mar 2025 - 7:15 COT», literal: «Este viernes 14 de marzo, el periodismo tolimense se viste de luto tras conocerse la muerte de Arnulfo Sánchez, el icónico maestro de la radio». La misma nota dice que sus hijos «continúan su legado en la radio a través de la emisora Ecos del Combeima y Ecos Interactiva». Es un hecho sobre una persona fallecida, publicado por su propia emisora, y se puede citar.
- **Nota 182531**, «9 Feb 2026 - 8:10 COT», literal: «un reconocimiento que honra la memoria del fundador de Econoticias».
- **Wikipedia** (revisión 170457690, 12-11-2025), literal: «El 14 de marzo de 2025 fallece en Ibagué el periodista Arnulfo Sanchez López propietario de la emisora y director del informativo Econoticias». Terciaria; solo corrobora.
- **`/nosotros`**, hoy: «a la cabeza de Arnulfo Sánchez y Juan Pablo Sánchez Baquero». La página está desactualizada y la ficha la leyó como presente. Es el mismo error que la regla del presente nació para evitar.
- **Quién está hoy:**
  - el RUES da como representante legal de INVERSIONES ECOS LIMITADA a «SANCHEZ BAQUERO JUAN PABLO» (registro actualizado el 2026-05-26);
  - la parrilla de `/al-aire` (fechada 04-10-2024) pone a «Juan Pablo Sánchez» en la columna «Directores» de «Econoticias», de lunes a viernes de 05:00 a 13:00 y los sábados de 06:00 a 08:00.
  - **Que el representante legal y el director del informativo sean la misma persona es lo probable, no lo probado**: la parrilla no da el segundo apellido. **Socios:** no constan; el RUES abierto no los da. Que haya habido sucesión de cuotas no consta.

**2 · La sociedad.**
- **RUES**, `nit=809006687` (2026-10-10), una fila: «INVERSIONES ECOS LIMITADA», Cámara de IBAGUE, matrícula 119615, «ACTIVA», sociedad limitada, matriculada el 1999-09-27, renovada el 2026-05-26 (último año 2026), vigencia hasta 2039-07-29, CIIU principal 6010 y secundario 7310, inscrita como proponente (RUP), representante legal «SANCHEZ BAQUERO JUAN PABLO».
- **Homónimos**, todos sin relación documentada con la emisora:
  - «INVERSIONES COMBEIMA LIMITADA», NIT 900162670, Ibagué, CANCELADA, último año renovado 2010;
  - «INVERSIONES COMBEIMA SAS EN LIQUIDACION», NIT 900746204, Ibagué, estado «ACTIVA» pero en liquidación, último año renovado 2015, CIIU 4771, con un representante legal sin los apellidos de la familia;
  - «INVERSIONES COMBEIMA PLAZA S A», Bogotá, CANCELADA (último año 2014);
  - y una cuarta que el revisor no menciona, «INVERSIONES LA UNION DEL COMBEIMA LIMITADA. ILUC LTDA. EN LIQUIDACION», de 1982, sin renovación. Tampoco tiene relación.
- **El vínculo sociedad-emisora es un hecho:** SECOP I lo escribe literal en **tres** contratos de la Cámara de Comercio del Sur y Oriente del Tolima, no en dos: OTB-168 (2025-06-09) y OTB-234 (2025-09-30), «SERVICIO DE PUBLICIDAD RADIAL EN LA EMISORA (INVERSIONES ECOS LTDA. ES ECOS DEL COMBEIMA)», y OTB-54 (2026-05-28), «PAQUETE PUBLICITARIO EN LA EMISORA (INVERSIONES ECOS LTDA. ES ECOS DEL COMBEIMA)». En SECOP II, los 55 contratos del NIT van a nombre de «ECOS DEL COMBEIMA», y el campo de representante legal dice «EMISORA ECOS DEL COMBEIMA 790 AM» en todos.
- **El origen de «Inversiones Combeima»:** Wikipedia da «Propietario: Inversiones Combeima S.A.S» y «La emisora es propiedad de Inversiones Combeima, cuyo dueño es el empresario local Arnulfo Sánchez». Que la ficha lo tomara de ahí es inferencia del revisor, verosímil, y aquí tampoco entra como hecho.

**3 · La afiliación a Blu Radio.**
- **`/al-aire`** (2026-10-10), literal y completo en lo que importa:
  - «Estás escuchando: Blu Radio … Descripción: Conexión Blu Radio … Próximo programa: Blu Radio»;
  - de lunes a viernes: Econoticias de 05:00 a 13:00, «Meridiano Blu» de 13:00 a 14:00, «Blog Deportivo» de 14:00 a 16:00 y «Vox Pópuli» de 16:00 a 19:00, los tres con «Blu Radio» en la columna «Directores»;
  - sábados: Econoticias de 06:00 a 08:00, «Democracia en Acción» de 08:00 a 09:00, «Aló Maestro» de 09:00 a 10:00 y «Blu Radio» de 10:00 a 12:00;
  - «Actualizado 4 Oct 2024 - 20:03 COT».
  Exacto. La tarjeta «Estás escuchando: Blu Radio» se mostraba a las 13:30 COT de un sábado, una hora que la parrilla no cubre: es un dato de la página, no de la señal.
- **Primario que ni la ficha ni el revisor citan:** el audio 160384 de la propia emisora, fechado «18 Ago 2020 - 9:11 COT»: «Director del Servicio Informativo de Blu Radio, Ricardo Ospina, le da la bienvenida a Ecos del Combeima como emisora afiliada a la prestigiosa cadena del Grupo Valórem». Dos consecuencias:
  - la afiliación consta en primario desde 2020, y la frase de la ficha «Ni la página "Nosotros" de la emisora ni una lista oficial de afiliadas de Blu Radio lo dicen» era cierta de esas dos páginas pero no del sitio;
  - el «desde 2013» de Wikipedia y de la ficha **no casa** con una bienvenida en 2020. Puede ser una reafiliación o un error de Wikipedia; no se sabe. La fecha de inicio no entra como hecho.
- **`/tarifas`**, «Actualizado 13 de Septiembre de 2025»: vende «Econoticias», «Golpes de Opinión», «Ecodeportes», «A toda máquina» y «La Radioteka 790», más «Breaks Generales». Ninguna mención de Blu. Los cuatro últimos programas no están en la parrilla de 2024. Que la parrilla esté desfasada es la lectura más simple, pero no se sabe en qué horario van esos programas ni si ocupan franjas que en 2024 eran de Blu.
- **Hoy:**
  - la señal Icecast no tenía fuente montada al consultarla (ver «Cómo se verificó»): no se pudo oír ni leer qué sonaba;
  - el agregador myradioenvivo.co muestra «Suena ahora: Blu Radio - Blu Radio» y una «Programación» del día que copia la parrilla de la emisora (06:00 Econoticias … 10:00 Blu Radio). Es eco de la parrilla, no prueba de emisión;
  - bluradio.com no publica lista de afiliadas (404). Una búsqueda web no dio ningún documento de 2026.
  - **Conclusión:** la afiliación es un hecho con primarios de 2020 y 2024. **Que siga vigente hoy, y con cuántas horas, no consta.** Ninguna fuente dice que terminara.

**4 · Afiliación no es propiedad, y lo que se ingeriría.**
- **Propiedad:** sociedad limitada local, matriculada en Ibagué, representada por una persona cuyo nombre coincide con el de un hijo del fundador según la nota necrológica; la identidad y el parentesco no están probados. Ningún registro consultado la une a Valorem ni a Caracol. Que el medio esté «bajo» el grupo Santo Domingo no tiene respaldo; afiliarse es un contrato de emisión. **Aceptado.**
- **El RSS** (`/rss.xml`, 2026-10-10): 10 ítems; 0 apariciones de «blu». Cinco tienen el mismo `pubDate` («Sat, 10 Oct 2026 15:50:38 +0000») y `dc:creator` «Anónimo»; los otros cinco, del 08 y el 09-10, van firmados por un usuario del sitio y son de Ibagué. **Dos de los cinco anónimos no son locales**: uno de Bogotá (una moto recuperada) y otro de Dosquebradas (un rescate). Que el feed sea «todo local» es exagerado; que no reproduzca a Blu, con 10 ítems, es un indicio, no una medida.
- **«Cultura SETP»** (09-10-2026) trata una estrategia del sistema de transporte de Ibagué, ente municipal. No se abrió la pieza; no se califica.
- **Ping Pong Político:** tres piezas abiertas, del 6 al 8 de septiembre de 2026; dos van firmadas por una periodista del medio. Una pregunta en el titular si «la Administración está creciendo al mismo ritmo que la comuna» y dice que la Comuna 5 «sigue esperando respuestas en movilidad, transporte público, espacio público, iluminación, aseo y seguridad». Otra trata la posible alianza entre el senador Óscar Barreto y la alcaldesa a través de un concejal que pide medirla «por su impacto en la ciudadanía». **Es crítica municipal suave y atribuida**, y queda registrada como evidencia que no mueve el número. Tres piezas no son un barrido.
- **Horas de antena:** 8 h de Econoticias frente a 6 h de Blu, de lunes a viernes, según la parrilla **de 2024**. El revisor ya lo limita. El sábado sale 2 a 2.
- **Lo que queda de la razón original:** el miedo a «contar dos veces» afecta al **corpus** solo si el sitio republica a Blu, y con lo visto no lo hace. Pero la ficha también hablaba de la **etiqueta**: presentar como «voz propia del Tolima» una antena que emite seis horas diarias de Blu. Eso sigue siendo un dato que la vista departamental tendría que declarar. La razón no desaparece; deja de ser dirimente.

**5 · Contratación pública.**
- **SECOP II** (`documento_proveedor='809006687'`, 2026-10-10): **55 contratos, $3.255.064.000**, de 2019 a 2026, todos a nombre de «ECOS DEL COMBEIMA» y con tipo de documento NIT.
  - Por año: 2019, 6,32 M; 2020, 128 M; 2021, 259 M; 2022, 303 M; 2023, 511,9 M; 2024, 540,1 M; 2025, 775,7 M; 2026, 731 M.
  - Por entidad: Alcaldía de Ibagué, 1.198,5 M; Gobernación del Tolima («GOBIERNO DEPARTAMENTAL», NIT de entidad 800113672, departamento Tolima), 949 M; Cortolima, 423,6 M; IBAL, 341,3 M; Conservatorio del Tolima, 168 M; Fábrica de Licores del Tolima, 138,8 M; y seis menores (Espinal, Flandes, Líbano, Rama Judicial, Concejo de Ibagué, ACAC).
  - **Últimos 12 meses** (firmados del 2025-10-10 al 2026-10-10): **7 por $731.000.000**, exactos a los del revisor:

| Contrato | Entidad | Firma | Fin | Valor | Modalidad | Estado | Objeto (literal, abreviado) |
|---|---|---|---|---|---|---|---|
| CO1.PCCNTR.9010502 | Cortolima | 2026-01-20 | — | 45.000.000 | directa | Cerrado | «…PRODUCTOS DE COMUNICACIONES EXTERNAS…» |
| CO1.PCCNTR.9035717 | IBAL | 2026-01-22 | — | 60.000.000 | régimen especial | Modificado | «…PUBLICIDAD DE UNA EMISORA AM Y SUS REDES SOCIALES…» |
| **CO1.PCCNTR.9076312** | **Alcaldía de Ibagué** | 2026-01-23 | 2026-06-24 (+28 días) | **150.000.000** | directa | Modificado | «PI03 - … DIFUSIÓN RADIAL MEDIANTE LA EMISIÓN DE CUÑAS; ENTREVISTAS; MENCIONES EN VIVO; ENTRE OTRAS; DE LAS ESTRATEGIAS Y GESTIONES ADELANTADAS POR LA ALCALDÍA MUNICIPAL DE IBAGUÉ Y SUS DEPENDENCIAS.» |
| **CO1.PCCNTR.9065920** | **Gobernación del Tolima** | 2026-01-24 | 2026-12-23 | **275.000.000** | directa | En ejecución | «…SERVICIOS DE INTERCAMBIO INFORMATIVO DE LOS TEMAS INHERENTES AL FORTALECIMIENTO INSTITUCIONAL DE LA GOBERNACIÓN DEL TOLIMA; A TRAVÉS DE UN MEDIO DE COMUNICACIÓN RADIAL Y DIGITAL» |
| **CO1.PCCNTR.9766419** | **Alcaldía de Ibagué** | 2026-08-04 | 2026-12-31 | **150.000.000** | directa | Modificado | «PI09 - … DIFUSIÓN RADIAL Y DIGITAL EN LOS DIFERENTES ESPACIOS INFORMATIVOS DE LA GESTIÓN PÚBLICA REALIZADA POR LA ALCALDÍA MUNICIPAL DE IBAGUÉ Y SUS DEPENDENCIAS» |
| CO1.PCCNTR.9801802 | Cortolima | 2026-08-13 | — | 21.000.000 | directa | En ejecución | ídem 9010502 |
| CO1.PCCNTR.10028805 | IBAL | 2026-10-06 | — | 30.000.000 | régimen especial | Aprobado | «…PUBLICIDAD DE UNA EMISORA AM…» |

  - **La Alcaldía de Ibagué y la Gobernación del Tolima suman 575 M de los 731 M (79 %)**, los dos por contratación directa, y los dos contratos de 2026-08 y 2026-01 de esas entidades **están en vigor hoy**.
  - «Modificado» con `dias_adicionados` (28 en el PI03 de enero; 61 en el IBAL de enero). El conjunto no da adiciones de valor; no se consultó el de adiciones. Si las hubo, las cifras serían mayores, no menores.
- **SECOP I** (`identificacion_del_contratista='809006687'`): **35 contratos, $737.081.457**, de 2018 a 2026, con 0 en adiciones. En los 12 meses, **2 por $5.000.000**: OC-PB-2026-90 (Cámara de Comercio de Ibagué, 2026-06-24, 4 M, publicidad del Festival Folclórico) y OTB-54 (Cámara del Sur y Oriente del Tolima, 2026-05-28, 1 M). Exacto.
  - Un dato que el revisor no da: SECOP I tiene un contrato de 150 M con **Telecafé** (2022-01-06) cuyo detalle dice «CONTRATO INTERADMINISTRATIVO 1912 DEL 17 DE SEPTIEMBRE DE 2021. GOBERNACION DEL TOLIMA PAGO A TERCEROS». Es decir, pauta de la Gobernación pagada a la emisora a través del canal. Es historia (2022) y no entra en los 12 meses; se anota porque explica parte del total.
- **Totales:** 12 meses, **9 por $736.000.000**; histórico, **90 por $3.992.145.457** (SECOP II 3.255.064.000 + SECOP I 737.081.457). Coincide con los «~3.992 M» del revisor.
- **El objeto de los contratos con la Alcaldía, leído:**
  - **PI03** compra «CUÑAS; ENTREVISTAS; MENCIONES EN VIVO» de «las estrategias y gestiones adelantadas por la Alcaldía». Y **no es solo de 2026**: el mismo objeto PI03 está en el contrato de 2025-03-19, por **225.000.000**.
  - **PI09** compra difusión «EN LOS DIFERENTES ESPACIOS INFORMATIVOS DE LA GESTIÓN PÚBLICA».
  - La Gobernación compra «INTERCAMBIO INFORMATIVO» sobre su «FORTALECIMIENTO INSTITUCIONAL», cada año desde 2020 y en aumento (20 M en 2020, 275 M en 2026).
  - **Hecho:** el gobierno municipal y el departamental que el medio cubre le compran entrevistas, menciones en vivo y presencia en sus espacios informativos. Es **pauta informativa pagada**, el mismo caso que el contrato de «cubrimiento periodístico» de Telecafé con la Cámara de Comercio de Dosquebradas (DECISIONES 2026-10-10). Va como **tensión fuerte de independencia editorial**, no como posición en el eje.
  - **No es hecho:** qué entrevistas o menciones concretas fueron pagadas, ni que el contenido del sitio sea entregable del contrato. No se abrieron los expedientes ni se cruzó con piezas.
- **Corroboraciones del revisor:**
  - la portada enlaza dos veces a `https://tolima.gov.co/` (y una a coljuegos.gov.co). Exacto;
  - nota 182531 (09-02-2026), literal: «Durante una entrevista en Ecos del Combeima, la mandataria explicó que este premio da cumplimiento al Acuerdo Municipal aprobado en abril de 2025 […] y se realiza en articulación con la Gobernación del Tolima». Exacto.
- **Lo que se corrige:** el revisor lo compara con «Diario La Libertad». No se cotejó aquí, y el precedente más cercano, ya decidido, es Telecafé por la pauta informativa y **El Nuevo Día** (Ibagué), que ya está en el catálogo con contratos de la misma Alcaldía: 9 por 121,5 M en sus 12 meses (`fichas/el-nuevo-dia.md`). **Ecos del Combeima contrata unas seis veces más** con el mismo contratante principal.
- **«Contratado», no «cobrado».** `valor_pagado` da 150 M en el PI03 de enero y 35 M en el IBAL de enero, 0 en el resto. No se usa.

**6 · El hecho editorial.** Nota 235510, «29 Dic 2023 - 15:23 COT». Fuera de los 12 meses. **Aceptada.** En su lugar puede ir un hecho de producción propia fechado en la ventana: las piezas de Ping Pong Político de septiembre de 2026 (ver 4).

**7 · Incoherencias.** Todas las que el revisor cita están en la ficha. Se añaden:
- la cabecera trae «Firma: ☐ no procede» y «Departamento: Tolima — sustituye a El Nuevo Día», cuando El Nuevo Día entró en el catálogo el 2026-08-13;
- «Nivel 5 — Hecho editorial de los últimos 12 meses» para una pieza de 2023;
- la REFUTACIÓN 1 nombra como primario «el certificado de Cámara de Comercio de Ibagué de Inversiones Combeima», una sociedad que no es la emisora;
- fuera de la ficha, el desfase se repite:
  - `fichas/el-nuevo-dia.md`, «LO QUE ESTA ALTA NO RESUELVE»: «esa vía sigue abierta como alta condicionada», cuando desde el 2026-08-18 la ficha dice «no se da de alta»;
  - `shared/mediaRegistry.js`, comentario del bloque de altas regionales: «Ecos del Combeima— porque su alta está condicionada a resolver si es afiliada de Blu Radio»;
  - `MEDIOS_CANDIDATOS_DEPARTAMENTOS.md`, la tabla de fichas («**alta condicionada**: ¿es afiliada de Blu Radio?»), «Lo que queda» punto 1, «Trece candidatos NO entraron» y el punto 3 de la lista final;
  - `fichas/LEEME.md`, la fila de la ficha.

### Motivo de cada rechazo

No se rechaza entera ninguna objeción. Se corrigen o no entran como hecho estas partes:
- **Obj. 2, «en dos órdenes»:** son tres (OTB-54 lo dice también).
- **Obj. 3, «sí existía un primario» = la parrilla de 2024:** hay otro de 2020, más explícito, que además pone en duda el «desde 2013».
- **Obj. 4, el RSS «local» en todos sus ítems:** dos de diez son de Bogotá y Dosquebradas. Y 10 ítems no son conducta medida.
- **Obj. 4, la franja propia más larga que la de Blu:** vale para la parrilla de 2024 y de lunes a viernes. No es un dato de hoy.
- **Obj. 5, el paralelo con Diario La Libertad:** no se cotejó; los precedentes decididos son Telecafé y El Nuevo Día.
- **Obj. 5, que el 150 M que compra entrevistas sea un hecho de 2026:** es un objeto recurrente desde 2025 (225 M).
- **Representante legal = director del informativo:** probable, no probado (la parrilla no da el segundo apellido).

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente.** Todas las URL del sitio, de Wikipedia y de Blu respondieron como dice el revisor (200, salvo los dos 404 que él mismo declara). Las consultas de RUES y SECOP devuelven sus cifras al peso. Omisiones y matices:
- el audio de bienvenida de 2020, que es el primario más claro de la afiliación;
- el tercer contrato de SECOP I con la frase «INVERSIONES ECOS LTDA. ES ECOS DEL COMBEIMA»;
- el PI03 de 2025 (225 M) con el mismo objeto de entrevistas y menciones;
- el contrato de Telecafé como pagador de la Gobernación (2022);
- dos ítems no locales en un RSS que describe como local;
- la cuarta sociedad homónima de 1982.

**Errores de la propia ficha, para no repetirlos:**
- «Propietario y director: Arnulfo Sánchez López», como vigente: murió el 14-03-2025.
- «Sociedad: Inversiones Combeima»: es INVERSIONES ECOS LIMITADA, NIT 809006687. Las «Inversiones Combeima» del RUES están canceladas o en liquidación y no son la emisora.
- «Propietario y director son la misma persona»: ya no consta quién es el propietario; consta el representante legal.
- «Ni la página "Nosotros" de la emisora ni una lista oficial de afiliadas de Blu Radio lo dicen»: el propio sitio lo dice en 2020 (audio 160384) y en 2024 (`/al-aire`).
- «bajo Valorem», «una cadena nacional del grupo Santo Domingo» como si describiera al medio: Valorem es el dueño de Blu, no de la emisora.
- El hecho editorial de 2023 presentado como de los últimos 12 meses.
- «+0,20» en ARGUMENTO junto a «NINGUNO»; «sustituye a El Nuevo Día»; «El Tolima se queda sin medio propio» junto a «el Tolima no queda mudo».
- La REFUTACIÓN 3, sobre una persona fallecida.
- Falta la línea de contratación pública que exige el protocolo desde el 2026-10-07.

**Lo que la ficha sí tenía bien:**
- que es afiliada de Blu Radio (al menos en 2020 y 2024);
- el feed `/rss.xml`, que funciona y no está declarado;
- que «Nosotros» cuenta la historia de Súper de Colombia y no menciona a Blu;
- la prudencia de no dar el alta, aunque por una razón que no se sostiene como estaba escrita.

---

**Propuesta para la firma**

**Estado de la candidatura: sin alta (salida a), con la razón reescrita.** No se propone número. Ni se descarta (salida b), ni se da de alta con 0,00 (salida c).

**Por qué (a) y no las otras:**
- **(b) descartar** no procede: el medio está activo (RSS del 08 al 10-10-2026), con nivel 1 localizado (sociedad, NIT, representante legal) y producción propia visible. Diario de Cundinamarca se descartó por inactividad, y aquí no la hay.
- **(c) alta con 0,00** es defendible y sería coherente con El Nuevo Día, que está en el catálogo con socios sin documentar y contratos de la misma Alcaldía. Pero la diferencia de grado es grande: unas seis veces más contratado con el mismo contratante, y con objetos que compran **entrevistas, menciones en vivo y espacios informativos**, no solo cuñas. A eso se suma que el titular murió y no consta quién controla hoy la sociedad, y que la afiliación a Blu está sin fechar en 2026. Entrar en esas condiciones sería un 0,00 sobre tres incógnitas.
- **El coste de esperar es bajo:** el Tolima ya tiene voz en el catálogo, El Nuevo Día. La vista departamental no queda vacía.

**Razón nueva, en lugar de «es afiliada de Blu Radio, que ya está en el catálogo bajo Valorem»:**

> Sin alta. La afiliación a Blu Radio es real (primarios del propio medio de 2020 y 2024) pero es de programación, no de propiedad, y su vigencia hoy no está probada: deja de ser la razón. No se da de alta porque (1) su fundador y propietario murió el 14-03-2025 y no consta quién controla hoy INVERSIONES ECOS LIMITADA (NIT 809006687); (2) la Alcaldía de Ibagué y la Gobernación del Tolima, los dos gobiernos que más cubre, le contrataron 575 M de sus 736 M de los últimos 12 meses, con objetos que compran entrevistas, menciones en vivo y presencia en sus espacios informativos —pauta informativa pagada, tensión fuerte de independencia editorial—; y (3) el Tolima ya tiene voz en el catálogo con El Nuevo Día.

**Correcciones de hecho en `fichas/ecos-del-combeima.md`:**
1. **Cabecera:**
   - «Valor propuesto»: «**NINGUNO. Sin alta** — pauta informativa pagada por los gobiernos que cubre y control de la sociedad sin documentar tras la muerte de su fundador».
   - «Firma»: «☐ no procede: no hay número que firmar».
   - «Departamento»: «Tolima. El departamento tiene voz en el catálogo con El Nuevo Día (`fichas/el-nuevo-dia.md`)». Retirar «sustituye a El Nuevo Día».
   - Añadir «Revisión: ciclo 2, tanda 7, 2026-10-10».
2. **Nivel 1**, tabla:
   - **Sociedad:** INVERSIONES ECOS LIMITADA, NIT 809006687, sociedad limitada, matrícula 119615 de la Cámara de Comercio de Ibagué, activa, renovada el 2026-05-26, CIIU 6010 (radiodifusión) y 7310 (publicidad), inscrita en el RUP. Fuente: RUES abierto (`c82u-588k`), consultado el 2026-10-10. Vínculo con la emisora: SECOP I, contratos OTB-168, OTB-234 y OTB-54, «INVERSIONES ECOS LTDA. ES ECOS DEL COMBEIMA».
   - **Representante legal:** Juan Pablo Sánchez Baquero (RUES, 2026-05-26).
   - **Director de Econoticias:** «Juan Pablo Sánchez», según la parrilla de `/al-aire` (actualizada el 04-10-2024). Probablemente el mismo; no está probado.
   - **Fundador y propietario:** Arnulfo Sánchez López, **fallecido el 14-03-2025** ([nota de la emisora](https://www.ecosdelcombeima.com/ibague/nota-164793-luto-en-el-periodismo-tolimense-fallecio-arnulfo-sanchez)). La página «Nosotros» aún lo nombra al frente.
   - **Socios:** no constan; el RUES abierto no los da, y no consta cómo quedó la sucesión.
   - **Homónimas a no confundir:** Inversiones Combeima Limitada (NIT 900162670, cancelada) e Inversiones Combeima SAS en liquidación (NIT 900746204, sin renovar desde 2015). El nombre «Inversiones Combeima S.A.S» de Wikipedia no corresponde a la emisora.
   - **Sede:** se mantiene (es la de la empresa, publicada en `/contacto`).
   - Retirar «Propietario y director son la misma persona» y el párrafo de gobernanza que sigue; poner: «Tras la muerte del fundador, la sociedad la representa un miembro de su familia. Quién la controla no consta».
3. **Contratación pública**, sección nueva, con el formato del protocolo:

> Contratación pública (SECOP I y II, NIT 809006687, consultado 2026-10-10): 9 contratos por $736.000.000 **contratados** en los últimos 12 meses (SECOP II: 7 por $731.000.000; SECOP I: 2 por $5.000.000); 90 por $3.992.145.457 en total desde 2018 (SECOP II: 55 por $3.255.064.000, 2019-2026; SECOP I: 35 por $737.081.457, 2018-2026). Principales contratantes en SECOP II: Alcaldía de Ibagué ($1.198.500.000), Gobernación del Tolima ($949.000.000), Cortolima ($423.600.000) e IBAL ($341.264.000). **La Alcaldía de Ibagué y la Gobernación del Tolima son los gobiernos que el medio cubre**, y en los últimos 12 meses suman $575.000.000, por contratación directa. Los contratos de la Alcaldía compran «cuñas; entrevistas; menciones en vivo» (PI03, CO1.PCCNTR.9076312, $150.000.000, 2026-01-23; el mismo objeto en 2025, $225.000.000) y difusión «en los diferentes espacios informativos de la gestión pública» (PI09, CO1.PCCNTR.9766419, $150.000.000, 2026-08-04, en vigor hasta el 31-12-2026). La Gobernación compra «intercambio informativo» sobre su «fortalecimiento institucional» (CO1.PCCNTR.9065920, $275.000.000, 2026-01-24, hasta el 23-12-2026).

   Y debajo, como **tensión** (con el criterio de Telecafé, DECISIONES 2026-10-10): «Es pauta informativa pagada: los dos gobiernos que el medio cubre le compran entrevistas, menciones en vivo y presencia en sus espacios informativos. Qué piezas concretas fueron pagadas no consta. No mueve el eje».
4. **«LA PREGUNTA QUE BLOQUEABA EL ALTA»** se reescribe:
   - **Afiliación a Blu Radio: consta en primarios del propio medio**: el audio del 18-08-2020 en que Blu le da «la bienvenida […] como emisora afiliada» ([audio 160384](https://www.ecosdelcombeima.com/economia/audio-160384-director-del-servicio-informativo-de-blu-radio-ricardo-ospina-le-da-la)) y la parrilla de `/al-aire` (actualizada el 04-10-2024: Meridiano Blu, Blog Deportivo y Vox Pópuli de 13:00 a 19:00 entre semana; Blu de 10:00 a 12:00 los sábados). El tarifario del 13-09-2025 solo vende programas propios. **Vigencia hoy, sin prueba**; ninguna fuente dice que terminara. La fecha de inicio (2013 según Wikipedia, 2020 según la emisora) no se da por cierta.
   - **Es afiliación de programación, no de propiedad.** No hay vínculo societario con Valorem ni con Caracol. Retirar «bajo Valorem», «del grupo Santo Domingo» y «habría contado dos veces al mismo grupo».
   - **Lo que DobleFoco ingeriría es el sitio**, y su RSS no reproduce a Blu en los 10 ítems vistos el 2026-10-10. La prueba de 90 días (REFUTACIÓN 2) sigue siendo la que lo mediría.
   - Retirar la lista de afiliadas de otras ciudades: no tiene fuente citada y no hace falta.
5. **«El razonamiento original»:** se conserva como historia, con una nota fechada al principio: «Superado el 2026-10-10: la afiliación consta en primario, pero es de programación y no de propiedad».
6. **«Nivel 5»** pasa a llamarse «Hecho editorial», y la pieza del 29-12-2023 sale de la ventana. Si se quiere un hecho de los 12 meses: Ping Pong Político, septiembre de 2026, piezas propias sobre la Comuna 5 y sobre la posible alianza Barreto-Aranda, con crítica municipal atribuida.
7. **ARGUMENTO:** retirar «+0,20». Poner: «No se propone número: ver ESTADO».
8. **CONTRA:** sustituir por «El mejor caso a favor del alta: medio activo, de producción propia en el sitio y con nivel 1 localizado, en un departamento con un solo medio en el catálogo. El caso en contra es la pauta informativa pagada y el control sin documentar».
9. **REFUTACIÓN:**
   - el punto 1 se reescribe: «Para reabrir: el certificado de existencia y representación de INVERSIONES ECOS LIMITADA (Cámara de Comercio de Ibagué), con sus socios tras la sucesión»;
   - el punto 2 se mantiene (90 días de corpus);
   - el punto 3 se sustituye: «Si quien controle la sociedad aparece con cargo o candidatura pública, revisión extraordinaria»;
   - punto nuevo: «Que la pauta de los gobiernos que cubre deje de comprar entrevistas, menciones o espacios informativos, o que el medio la marque en antena y en el sitio».
10. **ESTADO:** la razón nueva de arriba. Retirar «El Tolima se queda sin medio propio, y es la conclusión correcta» y «Qué reabriría esto: un primario que desmienta la afiliación».

**Fuera de la ficha** (el medio no está en `mediaOwnership.js` ni en `centinela.js`, y no hace falta tocarlos):
11. `fichas/LEEME.md`, fila de `ecos-del-combeima.md`: «**Es afiliada de Blu Radio** […]» → «Sin alta: pauta informativa pagada por la Alcaldía de Ibagué y la Gobernación del Tolima, y control sin documentar tras la muerte de su fundador (ciclo 2, 2026-10-10). La afiliación a Blu es de programación, no de propiedad».
12. `fichas/el-nuevo-dia.md`, «LO QUE ESTA ALTA NO RESUELVE»: «esa vía sigue abierta como alta condicionada» → «quedó sin alta: primero por la afiliación a Blu (2026-08-18) y, desde el 2026-10-10, por la pauta informativa pagada y el control sin documentar».
13. `MEDIOS_CANDIDATOS_DEPARTAMENTOS.md`:
    - la fila de la tabla de fichas: «**alta condicionada**: ¿es afiliada de Blu Radio?» → «**sin alta**: pauta informativa pagada por los gobiernos que cubre + control sin documentar tras la muerte de su fundador · ciclo 2, 2026-10-10»;
    - «Lo que queda» punto 1 y el punto 3 de la lista final: marcarlos como resueltos, con la fecha y la razón nueva;
    - «Trece candidatos NO entraron», el párrafo «Uno, Ecos del Combeima…»: añadir la misma nota;
    - el párrafo «**Para el Tolima se propone Ecos del Combeima**» puede quedar como historia con una nota fechada.
14. `shared/mediaRegistry.js`: el comentario «uno —Ecos del Combeima— porque su alta está condicionada a resolver si es afiliada de Blu Radio» queda desfasado. Es solo un comentario; actualizarlo cuando se toque el archivo.

**¿Aviso de quien dirige?** No procede. El medio no está en el catálogo, y no consta cargo ni candidatura de su representante legal.

**Lo que NO entra como hecho:**
- que la afiliación a Blu siga vigente en octubre de 2026, y con cuántas horas;
- que empezara en 2013;
- quiénes son hoy los socios de INVERSIONES ECOS LIMITADA, y si la sucesión cambió el control;
- que el representante legal y el director de Econoticias sean la misma persona;
- qué entrevistas o menciones concretas fueron pagadas, o que el contenido del sitio sea entregable de un contrato;
- que la ficha tomara «Inversiones Combeima» de Wikipedia;
- que el RSS sea producción local en su totalidad.

**Decisiones para el responsable editorial:**
1. **Estado de la candidatura.** Recomendación: **(a) sin alta, con la razón reescrita** (pauta informativa pagada y control sin documentar, no Blu). La alternativa (c), alta con 0,00 provisional y el conflicto declarado, es coherente con El Nuevo Día, y sería la elección si se prefiere que la vista departamental tenga dos voces del Tolima. (b) descartar no se recomienda: el medio está activo y con nivel 1.
2. **Cómo se nombra el conflicto.** Recomendación: «**pauta informativa pagada** por la Alcaldía de Ibagué y la Gobernación del Tolima», como en Telecafé, y no «dependencia», que afirma algo de la economía del medio que SECOP no prueba (consta lo contratado, no su peso en los ingresos).
3. **La afiliación a Blu en la ficha.** Recomendación: dejarla como hecho con fecha (2020 y 2024) y vigencia sin probar; retirar todo lo que la presenta como propiedad de Valorem.
4. **Si se pide algo más.** Recomendación: **no** gastar ahora un certificado de Cámara de Comercio. Solo haría falta si se elige (c) o se reabre la candidatura. Si se reabre, ingerir el RSS 90 días antes de decidir.
5. **Coherencia con El Nuevo Día.** Sin recomendación de cambio: El Nuevo Día ya declara sus contratos con la Alcaldía. Pero si se elige (a) por la pauta, conviene escribir en DECISIONES dónde está la línea entre los 121,5 M de un medio dado de alta y los 736 M de uno que no entra: la diferencia que aquí se usa es de grado y de objeto (entrevistas y espacios informativos), no de tipo.
