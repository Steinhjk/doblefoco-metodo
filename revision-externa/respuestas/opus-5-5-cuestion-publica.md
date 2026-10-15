# Respuesta — Claude Opus 5.5 sobre Cuestión Pública

| | |
|---|---|
| **Modelo** | Claude Opus 5.5 |
| **Versión exacta** | `claude-opus-5-5` |
| **Fecha de la consulta** | 2026-10-10 |
| **Quién la hizo** | Claude Code, a petición del responsable editorial (ciclo 2, fase 2, tanda 8; revisor de la misma casa que el autor de las fichas, ver DECISIONES.md 2026-10-07) |
| **¿Tuvo acceso a la red?** | sí |

> **Se pega LITERAL lo que devolvió el modelo, sin editar ni resumir.** Si se
> recorta, se pierde justo lo que pueda incomodar. Los comentarios nuestros van
> al final, en la sección de resolución, claramente separados.
>
> **Única edición:** se ha retirado una frase que transcribía la ubicación y las
> condiciones de seguridad de la directora del medio (dato personal). Se explica
> al principio de la resolución.

---

## RESPUESTA LITERAL

```
DECLARACIÓN PREVIA DE CONFLICTO
Soy Claude Opus 5.5 (id. claude-opus-5-5), de Anthropic: la misma casa que el modelo que escribió la ficha. Mi coincidencia con ella no sirve como aval. Por eso he buscado sobre todo en fuentes que la ficha no usa: el archivo completo de 12 meses del propio medio (su API pública de WordPress), sus piezas de opinión de la sección «La Tribuna», RUES y SECOP I y II. Revisión hecha el 2026-10-10.

MÉTODO Y DÓNDE BUSQUÉ
- robots.txt de cuestionpublica.com (2026-10-10): «User-agent: * / Disallow:», salvo /wp-admin/ y rutas de carrito. No excluye a ClaudeBot, Claude-Web ni anthropic-ai. robots.txt de sembramedia.org: solo excluye /wp-admin/. En datos.gov.co no hay exclusión para la API /resource/.
- HTML crudo descargado con curl -sL, UA de navegador y --ssl-no-revoke: https://cuestionpublica.com/nosotros/ y 23 piezas individuales.
- Barrido reproducible del archivo: https://cuestionpublica.com/wp-json/wp/v2/posts?after=2025-10-10T00:00:00&per_page=100&page=1..4&_fields=date,link,title,categories (y una segunda pasada con excerpt). Cabecera x-wp-total: 340, es decir, 340 entradas publicadas entre 2025-10-10 y 2026-10-10. Categorías en /wp-json/wp/v2/categories: la 192 es «La Tribuna» (opinión), la 87 «Cuestión Poder», la 88 «Cuestión Pública», la 1 «Video», la 36 «EscarbaBajo» y la 37 «EscarbaData».
- Conteo por blancos: regex sobre los 340 titulares, separando actores del gobierno saliente y su entorno (Petro, Pacto Histórico, Benedetti, Roa, Hollman Morris, Cepeda…) de actores de la derecha y del gobierno entrante (Uribe, De la Espriella/ADLE, Centro Democrático, Pastrana, Lafaurie, Paloma, Briceño, Ilva Myriam Hoyos, John Milton Rodríguez…). Corte en 2026-08-07. Los scripts (list.js, merge.js, cuenta.js) están en la carpeta t89. El conteo es aproximado: tiene falsos positivos que corrijo a mano más abajo.
- RUES (c82u-588k): $where=upper(razon_social) like '%ESCARBABAJO%' (además de ESCARABAJO S y CUESTION PUBLICA). $select limitado a camara_comercio, matricula, razon_social, nit, fechas, estado_matricula, organizacion_juridica, representante_legal y fecha_actualizacion.
- SECOP II (jbjy-vk9h, documento_proveedor) y SECOP I (f789-7hwg, identificacion_del_contratista): igualdad exacta con el NIT 901144502 y con los diez sufijos posibles de DV pegado (9011445020 a 9011445029). Control positivo con el NIT 899999063 (Universidad Nacional): 1544 registros en SECOP II y 848 en SECOP I, así que la consulta funciona.
- Buscador web: disponible. Hice 1 sola consulta («"Cuestión Pública" Diana Salinas directora 2026»). No aportó nada primario nuevo. Lo único citable fue un trino de @cuestion_p del 2026-04-02 que la llama «directora editorial», y no lo descargué.
- No toqué los dominios excluidos ni Wikipedia.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en 12 meses?
  No encontré venta, fusión ni escisión. La página Nosotros (descargada el 2026-10-10) dice: «Actualmente, la distribución de acciones de la compañía es así: Diana Salinas con el 66.37% y Claudia Báez con el 33,33%.» RUES (consulta del 2026-10-10): «EL ESCARBABAJO SAS», NIT 901144502, Cámara de Comercio de Bogotá, matrícula 2902958, fecha_matricula 20180111, fecha_renovacion 20260331, ultimo_ano_renovado 2026, estado «ACTIVA», representante_legal «DIANA MARIA SALINAS PLAZA», fecha_actualizacion «2026/09/15 14:16:41». Esa actualización de septiembre de 2026 no dice qué cambió, y RUES no publica la composición accionaria. Está en «Lo que no pude verificar».
  Hay además una señal de cambio organizativo que la ficha no recoge. El propio Informe 2025, en la misma página Nosotros, dice: «Aunque desde el inicio hicimos parte de una empresa llamada El Escarbabajo, al cerrar este primer ciclo vital de siete años decidimos quebrar el modelo establecido y apostar por formas diversas y flexibles de organización, capaces de capitalizar errores, reconocer fracasos y proponer liderazgos distintos.»
- ¿La persona que la ficha nombra como titular o directora sigue viva y en el cargo? (comprobado el 2026-10-10)
  Sí. Diana Salinas firma como «directora de Cuestión Pública» la columna «No todas las amenazas a la democracia son iguales» (2026-06-16) y la columna «El gobierno de ADLE será… un puto loop» (2026-07-14). RUES la mantiene como representante legal, con actualización del 2026-09-15.
- ¿Quién dirige hoy la redacción?
  Diana Salinas. En la pieza del 2026-06-16 escribe: «Soy Diana, […] directora de Cuestión Pública», «Como directora del medio de periodismo de investigación» y «le he dicho a la redacción». Nosotros dice de ella: «lleva a cabo una intensa labor entre la dirección del medio periodístico […]». [frase retirada: dato sobre la ubicación y las condiciones de seguridad de la directora; dato personal, ver el principio de la resolución]
- ¿Hay un registro mercantil o reporte más reciente que la fuente citada?
  Sí: RUES, con renovación del 2026-03-31 y actualización del 2026-09-15. Confirma la sociedad, su estado activo y la representante legal. No confirma los porcentajes. SECOP I y II: 0 contratos con el NIT, con o sin DV. Esto es coherente con la declaración del medio, «Cuestión Pública nunca ha contratado ni contratará con el Estado colombiano», en la página Nosotros, leída el 2026-10-10.

## OBJECIONES

OBJECIÓN 1 — La ficha omite la pieza que más pesa del año: la directora publicó, cinco días antes de la segunda vuelta, un encuadre asimétrico explícito entre los dos candidatos.
- QUÉ AFIRMA LA FICHA: no hay base para situar el número («ocho piezas en treinta días no lo dan»), y solo nombra como evidencia de selección cinco titulares de septiembre. No cita ningún editorial ni ninguna columna de la dirección.
- POR QUÉ ES INCORRECTO: la regla del polo fijo dice que «el encuadre asimétrico entre candidatos» sigue siendo «evidencia de primer orden». La directora, hablando como directora y en primera persona del plural de la redacción, escribió lo siguiente.
  Citas literales:
  «No se puede comparar a los dos candidatos de la segunda vuelta. No son lo mismo. Sin titubeo.»
  «Más que de la derecha, Abelardo es un candidato de una ultraderecha […]. Estamos, claramente, frente a un autoritario […].»
  «Mientras que, en toda la trayectoria del candidato Iván Cepeda no encontramos una sola decisión de su parte que no haya sido por la vía de la Constitución, las formas republicanas […].»
  «El asocio con la guerrilla es una mala prensa, hay que decirlo. Una imagen basada en noticias falsas construidas en buena parte por el expresidente Álvaro Uribe y su grupo.»
  «lo que intentamos argumentar aquí es simple: no hay equivalencia posible entre ambos proyectos políticos.»
  «Por eso Cuestión Pública ha puesto atención especial en el candidato Abelardo De la Espriella.»
  CONTRAPESOS, en la misma pieza, que deben constar:
  «No hinchamos por ningún presidente o candidato presidencial.»
  «nunca hemos entendido nuestro trabajo bajo la idea de militancia, salvo por el feminismo.»
  «No creemos que Cepeda sea el candidato perfecto, creemos que tiene un desafío enorme frente a los errores y las malas decisiones del gobierno de Gustavo Petro.»
  Y el pie de página: «*La Tribuna es el espacio de columnas de pensamiento de nuestros analistas y expertos en Cuestión Pública. Sus contenidos no comprometen al medio.»
  HECHO: no hay un endoso formal («votar por X»), y el texto niega «hinchar». INFERENCIA MÍA: aunque lleve el descargo de La Tribuna, es voz de la casa. Firma la directora, habla de «la redacción», escribe «para nosotras» y «Cuestión Pública ha puesto atención especial», y en la práctica es un encuadre asimétrico entre los dos candidatos de la segunda vuelta. Si el protocolo lo trata como endoso o como encuadre asimétrico de primer orden, eso decide si se aplica el tope de ±0,30. La ficha tiene que decidirlo por escrito, no omitirlo.
- FUENTE: https://cuestionpublica.com/no-todas-las-amenazas-a-la-democracia-son-iguales/ (publicada el 2026-06-16, meta article:published_time 2026-06-16T15:19:13+00:00; descargada el 2026-10-10).
- NIVEL: hecho editorial de los últimos 12 meses / declaración del propio medio (voz de la directora).

OBJECIÓN 2 — La ficha omite la declaración de valores de la casa, que está en su propia página Nosotros, la misma que cita como fuente.
- QUÉ AFIRMA LA FICHA: «el nivel 1 dice de quién es y de qué vive, no dónde está en el eje». Trata esa página solo como fuente de propiedad y financiación.
- POR QUÉ: esa misma página declara hoy posiciones de la casa:
  «durante nuestro primer septenio salimos de la caverna: nos proclamamos feministas.»
  «En esta casa apoyamos el aborto, los derechos reproductivos, denunciamos los abusos y acosos sexuales y laborales de poderosxs.»
  «Somos incómodas, feministas y soberanas de nuestros contenidos editoriales.»
  «Le gritamos un NO rotundo a la guerra en cualquier parte del mundo.»
  Es nivel 4: no basta por sí solo para mover el número. Pero es una posición declarada hoy, comprobable y que podría cambiar mañana. La ficha debería registrarla, y no dar a entender que el medio no declara nada sobre sí mismo más allá de sus cuentas. INFERENCIA: son posiciones de valores (derechos reproductivos, feminismo), no adscripción partidista. Su valor en el eje depende de cómo el protocolo codifique esos temas.
- FUENTE: https://cuestionpublica.com/nosotros/ (descargada el 2026-10-10; el banner de la página está fechado en uploads/2025/12).
- NIVEL: declaración del propio medio.

OBJECIÓN 3 — «Ninguno al gobierno saliente» (CONTRA, punto 2) es falso con el barrido de 12 meses, y la laguna de volumen («ocho piezas») viene del corpus, no del medio.
- QUÉ AFIRMA LA FICHA: «de estos cinco, cuatro apuntan al gobierno entrante y uno a Uribe. Ninguno al gobierno saliente». Y el nivel 2 se apoya en 8 artículos en 30 días.
- POR QUÉ:
  (a) Volumen. La API del medio da 340 entradas en 12 meses (x-wp-total: 340). Entre 2026-08-08 y 2026-09-07 hay 41, y entre 2026-08-31 y 2026-10-10 hay 42 (frente a las 30 de la medición del envío). El cuello de botella es la captura de DobleFoco, no la producción del medio. El barrido que la ficha da por imposible se puede hacer hoy.
  (b) Antes del 2026-08-07 el medio fiscalizó con regularidad al gobierno saliente y a su entorno. Lista corregida a mano (fecha | titular | URL relativa a cuestionpublica.com):
   1. 2025-11-13 | #EnVivo | Las casas del ministro Benedetti | /en-vivo-las-casas-del-ministro-benedetti/
   2. 2025-11-21 | La línea roja que cruzó el Gobierno Petro: contradicciones y preguntas que deja su decisión de bombardear a menores | /la-linea-roja-que-cruzo-el-gobierno-petro-contradicciones-y-preguntas-que-deja-su-decision-de-bombardear-a-menores/ (lead: «los atroces bombardeos que le costaron la vida a por lo menos 15 niños y niñas»)
   3. 2025-12-10 | Las empresas de Euclides Torres que financiaron la mansión de Benedetti | /las-empresas-de-euclides-torres-que-financiaron-la-mansion-de-benedetti/
   4. 2026-02-10 | Hilo | Ricardo Roa, presidente de Ecopetrol, en la mira de la Fiscalía | /hilo-ricardo-roa-presidente-de-ecopetrol-en-la-mira-de-la-fiscalia/
   5. 2026-02-12 | Pacto Histórico se 'raja' en rendición de cuentas […] | (listado en la API, categoría 1)
   6. 2026-02-17 | Familiares de la senadora Berenice Bedoya se habrían favorecido con contratos en el gobierno Petro: Sergio Mesa | (API)
   7-13. 2026-03-18 a 2026-04-23 | serie Hollman Morris / RTVC: siete piezas (p. ej. /al-mismo-tiempo-y-en-todas-partes-abogada-de-hollman-morris-es-quien-asesora-a-rtvc-para-hacer-demandas-a-quienes-critican-su-gestion-y-para-crear-politicas-de-genero/, /exclusivo-abogados-de-hollman-morris-no-tenian-poder-para-representarlo-afirma-el-tribunal-superior-de-bogota/)
   14. 2026-04-08 | #Primicia | Huertas: ¿el falso positivo de Petro? | /primicia-huertas-el-falso-positivo-de-petro/
   15. 2026-05-08 | Los seis regaños de la Corte al presidente Petro por fomentar la violencia machista contra mujeres periodistas | /los-seis-reganos-de-la-corte-al-presidente-petro-por-fomentar-la-violencia-machista-contra-mujeres-periodistas-1/
   16. 2026-05-20 | Hilo | ¡Casi que no! Presidente Petro se disculpó por llamar «muñecas de la mafia» a las mujeres periodistas de Colombia | /hilo-casi-que-no-presidente-petro-se-disculpo-[…]/
   17. 2026-05-27 | Quiénes rodean a Iván Cepeda y cómo han llegado al Gobierno | /quienes-rodean-a-ivan-cepeda-y-como-han-llegado-al-gobierno/
   18. 2026-07-30 | Consejo de Estado rechazó demanda que buscaba que Gral. reintegrado por Petro pagara ($) por un falso positivo | (API)
   19. 2026-07-31 | Petro aceleró el reparto de notarías en la fase final de su gobierno | /petro-acelero-el-reparto-de-notarias-en-la-fase-final-de-su-gobierno/ (lead: «Hoy nos aguzamos con el gobierno de Gustavo Petro, con la corrupción que se presenta en la izquierda»)
  También consta que su Informe 2025 presenta como logro «House of Nariño», una investigación sobre la corrupción en la UNGRD bajo el gobierno Petro.
  Conteo bruto por regex sobre titulares (con falsos positivos, p. ej. «Hollman Ibáñez» o el conjuez que anuló a Cepeda, que en realidad apuntan a la derecha):
  - antes del 07-08: 76 titulares con actores de la derecha, 27 con actores del gobierno saliente y su entorno (unos 21-23 tras depurar), 1 con ambos y 159 sin ninguno de esos actores;
  - después: 31 con la derecha o el gobierno entrante, 1-2 con la izquierda y 44 sin ninguno de esos actores.
  INFERENCIA: hay continuidad de fiscalización a los dos lados del cambio, que según el polo fijo es oficio. La desproporción previa (unas 3,3:1 hacia la derecha) se explica en buena parte por la cobertura judicial de los procesos de Álvaro y Santiago Uribe y por la campaña de De la Espriella. Eso también es fiscalización y no cuenta según la regla.
- FUENTE: API https://cuestionpublica.com/wp-json/wp/v2/posts?after=2025-10-10T00:00:00&per_page=100 (consulta del 2026-10-10) y las piezas citadas.
- NIVEL: conducta observable / hechos editoriales de los últimos 12 meses.

OBJECIÓN 4 — En las piezas con POSTURA (no de fiscalización) en voz de la casa sí hay asimetría a los dos lados del cambio. La ficha no la mide; la cuento aquí.
- QUÉ AFIRMA LA FICHA: no propone número y remite a un futuro conteo de 40 piezas en tres meses.
- POR QUÉ: aplico la regla de evidencia editorial histórica (2026-10-09). Criterio declarado: titular o lead con valoración política, firmado por la casa («Cuestión Pública» o la directora). Excluyo la fiscalización documental, las columnas de terceros y los análisis puestos en boca de un invitado.
  POSTURA CONTRA LA DERECHA / EL GOBIERNO ENTRANTE
   Antes del 07-08-2026:
   P1 2025-12-12 | «Verdades a medias y datos manipulados: el discurso de las 'bodegas' y candidatos de derecha para las elecciones» | /verdades-a-medias-y-datos-manipulados-el-discurso-de-las-bodegas-y-candidatos-de-derecha-para-las-elecciones/ (solo leí titular y extracto: es la de clasificación más débil)
   P2 2026-06-16 | Diana Salinas, «No todas las amenazas a la democracia son iguales» (ver objeción 1)
   P3 2026-06-22 | «Abelardo De la Espriella: el presidente electo que llega al poder lleno de 'banderas rojas' y con media Colombia en oposición» (lead: «tras una campaña marcada más por los símbolos y las polémicas que por las propuestas») | /abelardo-de-la-espriella-el-presidente-electo-que-llega-al-poder-lleno-de-banderas-rojas-y-con-media-colombia-en-oposicion/
   P4 2026-06-26 | «EN VIVO | Pride 2026: ¡En tu cara presidente electo!» (lead: «la caminata contra la ultraderecha») | /en-vivo-pride-2026-en-tu-cara-presidente-electo/
   P5 2026-07-14 | Diana Salinas, «El gobierno de ADLE será… un puto loop» («haber elegido a Abelardo De La Espriella (ADLE) en Colombia nos manda inmediatamente a los años cincuenta»; «el reencauche del Partido Conservador más radical») | /el-gobierno-de-adle-sera-un-puto-loop/
   Después del 07-08-2026:
   P6 2026-08-13 | «Abelardo no me cuida, me cuida mi pueblo» (lead: «Mientras el Presidente mandaba besos al aire desde la sede de la UNGRD […]») | /abelardo-no-me-cuida-me-cuida-mi-pueblo/
   P7 2026-08-13 | «Se vinieron los gringos a Colombia gracias a Abelardo de la Espriella» | /se-vinieron-los-gringos-a-colombia-gracias-a-abelardo-de-la-espriella/
   P8 2026-08-14 | «La mezquindad del gobierno de Abelardo con las ayudas internacionales» (lead: «Pareciera que la ideología se impone sobre el apoyo humanitario en este Gobierno») | /la-mezquindad-del-gobierno-de-abelardo-con-las-ayudas-internacionales/
   P9 2026-08-26 | «¿El ICE colombiano? Abelardo de la Espriella contra los inmigrantes» | /el-ice-colombiano-abelardo-de-la-espriella-contra-los-inmigrantes/
   P10 2026-09-07 | «Hilo | Con Ilva Miriam Hoyos, la educación quedó en manos de una de las personas más radicales del dogmatismo religioso en el país» («#DeMalEnPeor | La "batalla cultural" sigue y los derechos humanos van perdiendo terreno») | /hilo-con-ilva-miriam-hoyos-[…]/
   P11 2026-09-28 | «#28S ¡CON NUESTROS DERECHOS NO RETROCEDEMOS!» («recordamos por qué la lucha por el aborto legal, seguro y gratuito sigue más vigente que nunca») | /28s-con-nuestros-derechos-no-retrocedemos/
  POSTURA CONTRA LA IZQUIERDA / EL GOBIERNO SALIENTE, O FAVORABLE A LA DERECHA (contrapesos)
   C1 2025-10-10 | «María Corina Machado, ganadora del Premio Nobel de Paz: un triunfo de las papeletas sobre las balas» (favorable a una líder del «partido de centro-derecha Vente Venezuela», según la propia pieza) | /maria-corina-machado-ganadora-del-premio-nobel-de-paz-un-triunfo-de-las-papeletas-sobre-las-balas/
   C2 2025-11-21 | «La línea roja que cruzó el Gobierno Petro» («atroces bombardeos»). Es fiscalización con valoración: la cuento por prudencia.
   C3 2026-05-20 | «Hilo | ¡Casi que no! Presidente Petro se disculpó […]» (ironía contra Petro)
   C4 2026-07-31 | «Petro aceleró el reparto de notarías […]» («la corrupción que se presenta en la izquierda»)
   (Dentro de P2 hay además una crítica a «los errores y las malas decisiones del gobierno de Gustavo Petro». No la cuento aparte.)
  CUENTA: 11 piezas con postura contra la derecha (5 antes y 6 después del cambio) frente a 4 en sentido contrario. Razón 11:4, unas 2,75:1. Queda por debajo del umbral de 3:1 si se cuentan los contrapesos generosamente (C2 y C4 son más fiscalización que postura). Si se excluyen C2 y C4, la razón es 11:2 y supera el umbral. Se cumplen ≥10 piezas y ≥3 por lado del cambio.
  INFERENCIA: el resultado depende de cómo se clasifiquen dos piezas fronterizas. Lo que es robusto: después del 07-08-2026 no encontré ninguna pieza con postura favorable al gobierno entrante, ni ninguna con postura contra la izquierda (que ya no gobierna). Antes del 07-08, la postura de la casa contra la izquierda se limita al terreno feminista y de derechos (bombardeos de menores, «muñecas de la mafia», Hollman Morris), no al ideológico. Esto encaja con lo que la casa declara de sí misma («salvo por el feminismo»).
- FUENTE: las URL listadas, más la API, consultadas el 2026-10-10.
- NIVEL: hecho editorial de los últimos 12 meses (voz de la casa).

OBJECIÓN 5 — Menor: los porcentajes de propiedad que la ficha copia no suman 100 %, y la lista de financiadores 2025 del propio medio no coincide del todo con la que la ficha usa para equilibrarla.
- QUÉ AFIRMA LA FICHA: «Diana Salinas (66,37 %) y Claudia Báez (33,33 %)»; «Entre sus financiadores figuran Luminate, IFPIM, NED y Heinrich Böll».
- POR QUÉ: 66,37 + 33,33 = 99,70 %. Queda un 0,30 % sin titular declarado: o hay una errata en la fuente o hay un tercer accionista. La ficha lo copia sin anotarlo.
  En cuanto a financiadores, la página trae dos listas. La de «¿De dónde llegaron nuestros recursos?» coincide con la ficha: «Entre ellas se destacaron Luminate, The International Fund for Public Interest Media (IFPIM), National Endowment for Democracy (NED) y la Fundación Heinrich Böll.» Pero el bloque «Redes, alianzas y abrazos» del Informe 2025 enumera «Fundación Heinrich Böll, Luminate, Institute for War & Peace Reporting (IWPR), Organized Crime and Corruption Reporting Project (OCCRP), Report For The World (RFW), Reporteros Sin Fronteras (RSF)» y no menciona la NED. El argumento de la ficha de que los financiadores «no son de un solo lado» descansa en la NED. Conviene citar las dos listas y no solo una.
  La página también registra donantes anteriores: «Open Society Foundations y el Reino de los Países Bajos, que fueron financiadores clave hasta finales de 2023». Es historia, no cuenta.
- FUENTE: https://cuestionpublica.com/nosotros/ (descargada el 2026-10-10).
- NIVEL: propiedad / declaración del propio medio.

## LO QUE NO PUDE VERIFICAR
- Composición accionaria vigente en registro externo. RUES no publica accionistas. No pedí un certificado de existencia ni un extracto de la Cámara de Comercio (son de pago y no son descargables sin pasarela). El 66,37/33,33 solo consta en la página del medio.
- Qué cambió en la actualización del registro del 2026-09-15. El dataset solo da la fecha.
- Si el «quebrar el modelo establecido […] proponer liderazgos distintos» del Informe 2025 se tradujo en un cambio formal de gobierno corporativo o de dirección. Busqué en la página Nosotros y en el listado de 340 entradas: no hay una pieza que lo anuncie.
- La cifra de 18 personas en el equipo («La equipa cuenta con 18 personas») es autodeclarada. Sin fuente externa.
- No leí el cuerpo completo de P1 ni de las piezas de vídeo (P4, P9). Las clasifiqué por titular y lead.
- Fuentes externas de nivel 3 (RSF MOM, MOE, ColombiaCheck): no las consulté por economía de buscador. No encontré sentencias sobre el medio en los 12 meses. La pieza del 2025-10-10 «Álvaro Uribe nos tiene en la mira, pero no guardaremos silencio» menciona que Uribe «quiso indagar por nuestras fuentes de financiación». No verifiqué si hubo acción judicial.

## LO QUE FALTA
- La columna de la directora del 2026-06-16 (objeción 1) y la del 2026-07-14 (P5). Son la voz de la casa en el momento más polarizado del año.
- La declaración de valores de la página Nosotros (objeción 2).
- El barrido de 12 meses en el archivo del propio medio. Existe, se puede consultar por API y tiene 340 piezas. La ficha basa su laguna de nivel 2 en el corpus de DobleFoco (8 piezas) y no en el archivo del medio.
- RUES 2026 (NIT 901144502, activa, renovada el 2026-03-31, representante legal la directora) y la constancia de 0 contratos en SECOP I y II, como verificación externa de «nunca ha contratado con el Estado».
- La serie de fiscalización al gobierno Petro (objeción 3), que contradice el «ninguno al gobierno saliente».

## EVIDENCIA QUE NO MUEVE EL NÚMERO
- La declaración expresa de no hinchar: «No hinchamos por ningún presidente o candidato presidencial. Al contrario, tratamos de desnudar las redes sin importar el partido político ni el abolengo.» (2026-06-16, misma URL que la objeción 1). No hay un endoso formal de voto.
- Fiscalización del gobierno saliente durante todo el periodo previo al cambio (unas 20 piezas, objeción 3), incluida una investigación de bandera (UNGRD, «House of Nariño») presentada como logro en el Informe 2025.
- Pieza favorable a María Corina Machado (2025-10-10, C1).
- Investigación patrimonial al presidente en funciones, firmada «Por Cuestión Pública»: «Declaraciones de un cuarto oscuro» (2026-09-04/06), /declaraciones-de-un-cuarto-oscuro/. Es fiscalización del gobierno entrante, la misma conducta que aplicó al saliente: no cuenta como orientación.
- Financiación: 89,93 % de cooperación internacional en 2025, de unos $1.400 millones; 95,30 % en 2024 y 87 % en 2023 (página Nosotros). Confirma la ficha.
- 0 contratos en SECOP I y II con el NIT 901144502, con y sin DV (consulta del 2026-10-10). Constancia: SECOP II jbjy-vk9h documento_proveedor = 901144502 → 0; SECOP I f789-7hwg identificacion_del_contratista = 901144502 → 0; ídem con 9011445020 a 9011445029 → 0.
- La columna de una tercera, Teresita Goyeneche, «Susana me dio la razón» (2026-06-04, La Tribuna), es elogiosa con la exministra Susana Muhamad. Es columna de tercero y NO cuenta como voz de la casa. La registro para que no se cuente por error.
- Pertenencia a SIP (desde 2024) y a WAN-IFRA (finales de 2025), según la página Nosotros. Es una afiliación gremial sin valor en el eje.

## SIN OBJECIÓN
No aplica: presento 5 objeciones.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-10. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal (la única, por datos personales).** En «NIVEL 1», tercera pregunta, se retiró una frase: transcribía lo que la directora cuenta en su columna sobre **dónde está y en qué condiciones de seguridad**. Se sustituyó por una nota entre corchetes.
- Es un dato personal de una persona natural con riesgo propio, y nada de la clasificación depende de él.
- Esta resolución tampoco lo repite.
- **No hay más ediciones.** El revisor no copió cédulas, teléfonos ni direcciones, y no enlazó consultas de datos.gov.co, que describe solo por el nombre del dataset y el filtro. Su RUES nombra a la representante legal, que es su papel, y eso se deja.
- **Aviso:** la página Nosotros y las columnas de la directora publican su año y su lugar de nacimiento. Por la regla de datos personales **no pasan a la ficha**, y aquí no se transcriben.

**Cómo se verificó.**
- **robots.txt**, leído antes de descargar nada (2026-10-10):
  - `cuestionpublica.com`: el bloque general solo veta `/wp-admin/` y las rutas de WooCommerce; el de Yoast dice `User-agent: *` / `Disallow:`. **Literal, como dice el revisor.**
  - `datos.gov.co`: `Crawl-delay: 1`. Se usó solo `/resource`.
  - No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex. **No hubo buscador web.**
- **Sitio**, con `curl -s --ssl-no-revoke` y User-Agent de Chrome 126:
  - la API `wp-json/wp/v2/posts?after=2025-10-10T00:00:00&per_page=100&page=1&_fields=date,link,title,categories` y `wp/v2/categories`. Dio `x-wp-total: 340`, y la página 1 es **idéntica byte a byte** a la del revisor.
  - Al pedir el campo `excerpt`, el servidor respondió `303` hacia la portada. Minutos después **dejó de aceptar conexiones desde esta IP** (timeouts a partir de las 17:55, hora de Bogotá, y hasta el cierre de esta resolución).
  - Por eso las páginas 2-4 del listado, las entradillas y los cuerpos se leyeron en el **HTML crudo que descargó el revisor ese mismo día** (`t89/cuestion-dl`). Se leyeron como datos, sin ejecutar nada desde esa carpeta, y su página 1 coincide con la mía.
  - **Límite declarado:** las citas de abajo se cotejaron contra esas copias crudas, no contra una segunda descarga propia.
- **Registros** (datos.gov.co, 2026-10-10):
  - RUES `c82u-588k`: por `nit=901144502`, por `razon_social like '%ESCARBA%'` y por el nombre de la representante legal (para ver si dirige otra sociedad: no).
  - SECOP II `jbjy-vk9h` (`documento_proveedor`) y SECOP I `f789-7hwg` (`identificacion_del_contratista`): con `901144502`, `9011445022` (DV 2 pegado) y `901144502-2`, más por razón social `like '%ESCARBABAJO%'`.
  - Control positivo: el NIT 899999063 da 1.544 registros en SECOP II.
- **Repositorio:**
  - el envío, la ficha y sus entradas en `shared/mediaRegistry.js` y `shared/mediaOwnership.js` (en `shared/centinela.js` no hay entrada);
  - las menciones en otras fichas: `casa-macondo.md`, `las2orillas.md`, `voragine.md`, `revista-raya.md`, `colombia-informa.md` y `el-morichal.md`;
  - el protocolo, DECISIONES.md del 2026-10-07 al 2026-10-10, el commit `fa77249` y el modelo y barrido de El Informador.
- **El barrido**, reproducible, está en `revision-externa/barridos/cuestion-publica.md`.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

**El valor que se juzga.** La ficha dice «Valor actual −0,45», y con ella el envío. **El registro dice `bias: null`, «SIN MEDIR».**
- Lo decidió el responsable editorial el 2026-09-16 para el trío Vorágine-Cuestión Pública-RAYA y RTVC, y se aplicó el 2026-09-18 (commit `fa77249`: «El "sin medir" estaba decidido para cuatro medios —Voragine, Cuestion Publica, Revista RAYA y RTVC—»).
- El medio lleva además `noNoticioso: true`, desde el 2026-09-16: fuera del mapa.
- **La ficha se escribió el 2026-09-09 y no se actualizó.** Lo que se resuelve aquí es si hay evidencia para pasar de «sin medir» a un número.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | La columna de la directora del 16-06 es un encuadre asimétrico explícito entre candidatos, y la ficha la omite. ¿Endoso o encuadre? | sí | sí, literal | **Aceptada como omisión.** Todas sus citas y contrapesos son literales. **No es endoso explícito:** es encuadre asimétrico de primer orden (ver abajo). Cuenta en el barrido como I; no levanta el tope |
| 2 | Nosotros declara valores de la casa: feminismo, aborto, «NO rotundo a la guerra» | sí | sí, literal | **Aceptada.** Es nivel 4 y no mueve el número. Añadido: la misma página se presenta como «medio digital feminista e investigativo» |
| 3 | «Ninguno al gobierno saliente» es falso; 340 piezas al año, unas 20 que fiscalizan a Petro y 41-42 al mes | sí | sí | **Aceptada con matiz.** La frase es literal para los cinco titulares de septiembre, cuando Petro ya no gobernaba, pero como observación engaña: las 19 piezas de su lista existen, con esas fechas. Volumen: 41 piezas del 08-08 al 07-09, y 41 en la misma ventana de la ficha (09-08 → 08-09), **frente a las 8 que capturó el corpus**. Para el polo fijo, esto es oficio a los dos lados del cambio |
| 4 | Postura de la casa: 11 contra la derecha (5+6) frente a 4 contrapesos (2,75:1), u 11:2 sin dos dudosas | sí | sí, pieza a pieza | **Rechazada en la cuenta; aceptada como tensión.** Recontado: estricta, 5 (4+1) frente a 3; amplia, 10 (7+3) frente a 6. Proporción de 1,7:1 en las dos. **No cumple los mínimos.** Las dos dudosas cuentan como contrapeso, por la misma vara que el revisor aplica a sus piezas de después |
| 5 | 66,37 % + 33,33 % = 99,70 %; dos listas de financiadores, una sin la NED. RUES y SECOP | sí | sí | **Aceptada.** RUES literal, con un dato que el revisor no da: CIIU 7220, «investigación y desarrollo experimental en ciencias sociales y humanidades». 0 contratos con y sin DV, y también por razón social |

### Lo verificado, objeción por objeción

**Nivel 1 · RUES y SECOP.**
- **RUES**, `c82u-588k`, `nit=901144502` (2026-10-10), una fila, literal: «"camara_comercio":"BOGOTA"», «"matricula":"2902958"», «"razon_social":"EL ESCARBABAJO SAS"», «"nit":"901144502"», «"digito_verificacion":"2"», «"organizacion_juridica":"SOCIEDADES POR ACCIONES SIMPLIFICADAS SAS"», «"fecha_matricula":"20180111"», «"fecha_renovacion":"20260331"», «"ultimo_ano_renovado":"2026"», «"estado_matricula":"ACTIVA"», «"cod_ciiu_act_econ_pri":"7220"», «"representante_legal":"DIANA MARIA SALINAS PLAZA"», «"fecha_actualizacion":"2026/09/15 14:16:41.010000000"». **Exacto.**
  - Consulta sin datos personales: `https://www.datos.gov.co/resource/c82u-588k.json?nit=901144502&$select=camara_comercio,matricula,razon_social,nit,digito_verificacion,organizacion_juridica,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,estado_matricula,cod_ciiu_act_econ_pri,representante_legal,fecha_actualizacion`.
  - La representante legal no figura en ninguna otra sociedad del RUES.
  - «ESCARBABAJO» no tiene homónimos; «ESCARBA» da además ESCARBATO S.A.S. (Pereira), que no tiene relación con el medio.
- **SECOP, literal:** `[{"count_id_contrato":"0"}]` en SECOP II y `[{"count_numero_de_constancia":"0"}]` en SECOP I, con `901144502`, `9011445022` y `901144502-2`, y 0 por razón social.
  - Consultas: `https://www.datos.gov.co/resource/jbjy-vk9h.json?documento_proveedor=901144502&$select=count(id_contrato)` y `https://www.datos.gov.co/resource/f789-7hwg.json?identificacion_del_contratista=901144502&$select=count(numero_de_constancia)`.
- **Que no hubo cambio formal:** la frase «quebrar el modelo establecido» va en el Informe 2025, bajo el epígrafe «La redacción también creció». Habla de organización interna y liderazgo: «formas diversas y flexibles de organización». La sociedad sigue activa y renovada, y la representante legal es la misma.
- **Que la directora sigue en el cargo:**
  - firma «Por Diana Salinas» las columnas del 16-06 y el 14-07, y en la primera dice «directora de Cuestión Pública»;
  - la pieza del 10-10-2025 la llama «directora editorial de Cuestión P»;
  - el RUES la mantiene como representante legal.

**1 · La columna del 16-06-2026.** URL `https://cuestionpublica.com/no-todas-las-amenazas-a-la-democracia-son-iguales/`, `article:published_time` `2026-06-16T15:19:13+00:00`, categoría 192 (La Tribuna), «Por Diana Salinas».
- **Las once citas del revisor son literales:** «No se puede comparar a los dos candidatos de la segunda vuelta. No son lo mismo. Sin titubeo.», «Estamos, claramente, frente a un autoritario […]», «no hay equivalencia posible entre ambos proyectos políticos», «No hinchamos por ningún presidente o candidato presidencial», el pie «*La Tribuna es el espacio de columnas de pensamiento de nuestros analistas y expertos en Cuestión Pública. Sus contenidos no comprometen al medio.», etc.
- **Lo que no cita y pesa:**
  - «Fueron estos dos hitos los que marcaron la férrea idea de gritar si volvía a llegar un fascista al poder.»
  - «es inviable un candidato que promete de entrada irrespetarla [la Constitución]»
  - «De la Espriella eligió que su enriquecimiento viniera de la mano del capital de la mafia.»
- **¿Endoso explícito? No.** Así se compara con El Informador, el único endoso aceptado en el ciclo (DECISIONES 2026-10-10):
  - El Informador: editorial **sin firma**, la institución, con «con Abelardo habrá institucionalidad, democracia y libertad; con Cepeda habrá […] tiranía». Precedido de una **petición de voto** el 11-05: «deberán depositar su voto por Abelardo».
  - Cuestión Pública: una columna **firmada**, en un espacio de opinión con descargo, que **no pide el voto, no declara apoyo y lo niega** («No hinchamos…»; «No creemos que Cepeda sea el candidato perfecto»).
  - El protocolo trata por separado el «endoso editorial» y el «encuadre asimétrico entre candidatos». Los dos son evidencia de primer orden, pero solo el **endoso explícito** levanta el tope. Este texto es el caso más fuerte del segundo, no del primero.
  - Que la firme la directora y representante legal decide que es **voz de la casa**, porque el protocolo cuenta lo «firmado por […] su director». Por eso entra en el barrido pese al pie de La Tribuna. **No decide que sea endoso.**
  - Regla 2, ante la duda.
  - Y aunque se leyera como endoso, levantaría el tope, pero **no sustituye al barrido**, que no llega a los mínimos.

**2 · Nosotros.**
- **Literal:**
  - «durante nuestro primer septenio salimos de la caverna: nos proclamamos feministas»;
  - «En esta casa apoyamos el aborto, los derechos reproductivos, denunciamos los abusos y acosos sexuales y laborales de poderosxs»;
  - «Somos incómodas, feministas y soberanas de nuestros contenidos editoriales»;
  - «Le gritamos un NO rotundo a la guerra en cualquier parte del mundo».
- Añadido: «Es una de las creadoras de Cuestión Pública, medio digital feminista e investigativo».
- Es línea declarada por la casa: nivel 4, que no mueve el número por sí sola (regla 3). El protocolo la deja fuera del polo fijo: sigue siendo evidencia y se declara.
- Precedente que conviene tener a la vista: Volcánicas (−0,50) y CasaMacondo (−0,35) llevan valores puestos por declaración, y ninguno está firmado.

**3 · «Ninguno al gobierno saliente».**
- Las 19 piezas de su lista existen en la API con esas fechas y títulos. La serie de Hollman Morris son 7 piezas entre el 18-03 y el 23-04; contando Lina Castillo y la columna del 20-03, hay más.
- «House of Nariño» consta en el Informe 2025 («abordó de frente la corrupción en la Unidad Nacional para la Gestión del Riesgo de Desastres (UNGRD)»). El texto no dice «bajo el gobierno Petro»: eso lo añade el revisor, aunque sea un hecho conocido.
- Las cifras: 340 entradas (`x-wp-total`); 263 antes del 07-08 y 77 desde ese día. Del 08-08 al 07-09, 41; del 31-08 al 10-10, 42. **Exacto.**
- Los recuentos por regex (76 / 27 / 1 / 159) no se rehicieron: los sustituye el barrido manual.
- **Laguna nuestra, no del medio:** en la misma ventana de la ficha, el medio publicó 41 piezas y el corpus capturó 8. Más de la mitad del archivo es de la categoría Vídeo (157 de 340).

**4 · El barrido.** Completo en `barridos/cuestion-publica.md`. En corto:
- **Antes del cambio, cuentan 4 piezas:**
  - columna del 16-06;
  - «banderas rojas» del 22-06: «el nuevo referente de la ultraderecha nacional»;
  - Pride del 26-06: «la caminata contra la ultraderecha»;
  - columna del 14-07: «No hace falta decir fascistas, porque sería redundar».

  Hay 3 leves: el vídeo del 17-06 («¿hay peligros para el país si gana Abelardo?»), el preconteo del 22-06 y las «bodegas» del 12-12.
- **Después, cuenta 1 pieza:** Ilva Hoyos, 07-09. Hay 2 leves: «mezquindad», 14-08, y «batalla cultural de este gobierno», 02-09.
- **El resto de lo de después es fiscalización del Gobierno en ejercicio:**
  - «Abelardo no me cuida» es, en el cuerpo, una lista de aplicativos de ayuda;
  - en «Se vinieron los gringos», la crítica se atribuye a la senadora Pedraza;
  - «¿El ICE colombiano?» es una pregunta.

  Por la precisión del 2026-10-09, no suma.
- **«#28S»** es postura de valores sin destinatario: V, no suma.
- **Contrapesos:** 3 plenos (C1 línea roja, C2 «¡Casi que no!», C3 notarías) y 3 leves.
- **María Corina Machado** es internacional y queda fuera, como Kast en El Informador.
- **Resultado:** estricta, 5 frente a 3; amplia, 10 frente a 6. 1,7:1 en las dos. **No llega a 3:1.** En la estricta tampoco llega a 10 ni a 3 piezas después del cambio.

**5 · Propiedad y financiadores.**
- **Literal:** «Diana Salinas con el 66.37% y Claudia Báez con el 33,33%» (con punto en una cifra y coma en la otra). Suman 99,70 %, como dice el revisor.
- **Las dos listas, literales:**
  - la de «Entre ellas se destacaron Luminate, […] (IFPIM), National Endowment for Democracy (NED) y la Fundación Heinrich Böll»;
  - la de «Redes, alianzas y abrazos»: Heinrich Böll, Luminate, IWPR, OCCRP, RFW y RSF, sin la NED.
- También son literales «Open Society Foundations y el Reino de los Países Bajos […] hasta finales de 2023» y los 87 % / 95,30 % / 89,93 %.
- El encabezado de esa sección escribe «El Escarababajo SAS», con una errata del propio medio.

### Motivo de cada rechazo

- **Obj. 4, la cuenta.**
  - El revisor cuenta como postura cuatro piezas de después del cambio (P6, P7, P9 y P11) que fiscalizan al Gobierno en ejercicio, que atribuyen la crítica a una fuente o que no tienen destinatario político. Por la precisión del 2026-10-09, no suman.
  - Propone quitar C2 y C4 por ser «más fiscalización que postura», con un criterio que no aplica a P8 ni a P9.
  - Cuenta como contrapeso una pieza internacional (María Corina Machado).
  - Con una sola vara para los dos lados, no hay lectura que llegue a 3:1.
- **Obj. 3, «es falso».** Es literal para los cinco titulares que la ficha mira; lo engañoso es la generalización. Se acepta la corrección, no la calificación de falso.
- **Obj. 1, la alternativa del endoso.** No se rechaza: el revisor deja la decisión abierta. Aquí se decide en contra, por lo dicho arriba.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente ni cita inventada.** Las URL que cita existen en la API con esas fechas, y todas las citas cotejadas son literales. Lo que hay:
- un añadido de contexto: «House of Nariño» «bajo el gobierno Petro», que el Informe no dice;
- una cuenta inflada por criterios desiguales (obj. 4);
- **una frase sobre la situación personal de la directora**, retirada de la literal por datos personales. No es fuente falsa.

**Errores de la propia ficha, para no repetirlos:**
- **Cabecera «Valor actual −0,45»:** el registro lleva `bias: null` desde el 2026-09-18 (decisión del 16-09, commit `fa77249`). El CONTRA 3, «el −0,45 heredado sigue contando en la tasa de la izquierda», es falso desde esa fecha. El envío del ciclo 2 lo transmitió así al revisor.
  - **La decisión del «sin medir» no tiene entrada en DECISIONES.md:** solo está en el comentario del registro y en el commit.
  - Siguen citando el −0,45 `fichas/casa-macondo.md` (línea 63) y `fichas/voragine.md` (línea 13). El `biasRationale` de Las2Orillas (`shared/mediaRegistry.js:278`) se apoya en «la investigación militante (Vorágine, Cuestión Pública)».
- **Nivel 2 «8 artículos» y «con ocho piezas no se sostiene»:** el medio publicó 41 en esa ventana. La laguna es de nuestra captura, y la ficha no miró el archivo propio, que se puede barrer por API.
- **La REFUTACIÓN («si en tres meses acumula 40 o más piezas»)** ya estaba cumplida en el archivo del medio el día de la ficha.
- **«Ninguno al gobierno saliente»:** generaliza desde cinco titulares de septiembre.
- **No cita las columnas de la directora** (16-06 y 14-07) ni la línea declarada en Nosotros.
- **Sin la línea de contratación pública**, obligatoria desde el 2026-10-07. Y sin el RUES, que confirma la sociedad y la representante legal.
- **Copia los porcentajes que suman 99,70 %** sin anotarlo, y apoya «no son de un solo lado» en la NED, que falta en una de las dos listas del propio medio.
- **Lo que sí tenía bien:** que el nivel 1 no sitúa en el eje, que la constancia de selección no basta sin barrido y que el medio merece paciencia por publicar sus cuentas.

---

**Propuesta para la firma**

**Valor: se queda SIN MEDIR (`bias: null`), con `noNoticioso: true`.** No hay evidencia para pasar a un número:
- **El barrido de 12 meses no cumple los mínimos** de «Evidencia editorial histórica»: 1,7:1 en las dos lecturas. En la estricta, además, solo 5 piezas y 1 después del cambio. Por la segunda precisión del 2026-10-09, «un barrido que no llega a los mínimos no deshace nada»: se conserva el valor que había, y ese valor es «sin medir».
- **No hay endoso explícito.** Y aunque lo hubiera, levanta el tope, pero no sustituye al barrido.
- **No hay nivel 1 con posición conocida:** dos periodistas, una S.A.S. y financiación de cooperación de signo variado.
- **Tampoco 0,00 «con evidencia».** La voz propia no trata igual a los dos lados: rótulos ideológicos solo a la derecha. Eso es tensión declarada, no mixta.
- **Lo que cambia es el motivo.** Ya no es que «su volumen no da»; es que el barrido no alcanza los mínimos.

**Alternativa declarada:** −0,25, con tope de ±0,30 y sin endoso, solo si el responsable editorial acepta la cuenta del revisor sin sus dos dudosas (11:2). **No se recomienda:** exige contar la fiscalización con tono del Gobierno entrante como postura y la del saliente como oficio.

**Texto propuesto para `biasRationale`** (no se escribe en código):

> SIN MEDIR. Periodismo de investigación sobre poder político, corrupción y derechos de las mujeres; se declara «medio digital feminista e investigativo» y defiende el aborto legal (Nosotros, 2026). Barrido de sus 340 piezas de 12 meses (2025-10-10 → 2026-10-10): fiscaliza al gobierno de turno a los dos lados del 07-08 —Petro antes, De la Espriella después—, que es oficio. Su voz propia se inclina a la izquierda: rótulos ideológicos solo a la derecha («ultraderecha», «autoritario») y dos columnas de la directora que niegan toda equivalencia entre los candidatos de la segunda vuelta (16-06-2026) sin endosar a ninguno. Son 5 a 10 piezas con postura frente a 3 a 6 contrapesos, por debajo de la proporción de 3 a 1 que pide la regla: se declara como tensión y no fija número — ver fichas/cuestion-publica.md.

**`shared/mediaOwnership.js`, `cuestion-publica`** (no se escribe en código):
- **`ownerType: 'independiente'`** se mantiene: sociedad de dos periodistas que publica sus cuentas.
- **`verifiedAt: '2026-10-10'`** (hoy es `VERIFICADO`, 2026-07-29). El RUES confirma la sociedad, su estado y la representante legal; los porcentajes solo constan en el medio, y se dice.
- **`holdings`:**
  - la primera pasa a: «Lo publica El Escarbabajo SAS (NIT 901144502, matrícula 2902958 de la Cámara de Comercio de Bogotá, del 11-01-2018, ACTIVA, renovada el 31-03-2026; representante legal: Diana Salinas, RUES, actualizado el 15-09-2026). Según el propio medio, sus socias son las periodistas Diana Salinas (66,37 %) y Claudia Báez (33,33 %); la suma es 99,70 % y el RUES abierto no publica accionistas.»;
  - la de financiadores pasa a: «En 2025 se destacaron Luminate, el IFPIM, la National Endowment for Democracy y la Fundación Heinrich Böll; su lista de "redes y alianzas" del mismo informe nombra Heinrich Böll, Luminate, IWPR, OCCRP, Report for the World y Reporteros Sin Fronteras, sin la NED.»
- **`notes`:**
  - «Contratación pública (SECOP I y II, NIT 901144502, consultado 2026-10-10): 0 contratos en SECOP I y II a 2026-10-10 (también con el dígito de verificación pegado y por razón social). Coincide con lo que declara: "nunca ha contratado ni contratará con el Estado colombiano".»
  - «Línea declarada (nivel 4): feminista y a favor del aborto legal (Nosotros, 2026).»
- **`sources`:** añadir la consulta del RUES con `$select` y la de SECOP II con `$select=count(id_contrato)` citadas arriba.
- **`controlGroup` `el-escarbabajo`:** sin cambios. El `papel` de Diana Salinas puede añadir «directora y representante legal». No se añade ningún dato de su situación personal ni de su nacimiento.

**Textos a corregir** (los aplica quien el responsable editorial decida; aquí no se toca nada):

En `fichas/cuestion-publica.md`:
1. **Cabecera:**
   - «Valor actual | −0,45» → «**sin medir** (`bias: null`), decisión del responsable editorial del 2026-09-16, aplicada el 2026-09-18 (commit `fa77249`)»;
   - «Propuesta» → «Se queda sin medir: el barrido de 12 meses no alcanza los mínimos (ver `revision-externa/barridos/cuestion-publica.md`)».
2. **Nivel 1:**
   - añadir el RUES (NIT, matrícula, estado, renovación, representante legal, CIIU 7220);
   - anotar que los porcentajes suman 99,70 % y que el RUES abierto no da los socios;
   - citar las dos listas de financiadores.
3. **Sección nueva «CONTRATACIÓN PÚBLICA»**, con la línea de 0 contratos.
4. **Nivel 2:**
   - sustituir «CON OCHO PIEZAS…» por el volumen real (340 piezas al año; 41 en la ventana de 30 días, de las que el corpus capturó 8) y por el resumen del barrido;
   - las columnas del 16-06 y del 14-07, con sus contrapesos, incluido el pie de La Tribuna;
   - el veredicto: no es endoso explícito.
5. **Línea declarada (nivel 4):** las cuatro citas de Nosotros.
6. **CONTRA 2:** «Ninguno al gobierno saliente» → «Ninguno de estos cinco, todos de septiembre; en 12 meses, unas 20 piezas fiscalizaron al Gobierno Petro y su entorno mientras gobernaba».
7. **CONTRA 3:** retirar («el −0,45 heredado sigue contando»): desde el 18-09 no cuenta.
8. **REFUTACIÓN:** «Si en tres meses acumula 40 o más piezas» → «Si en el recuento de diciembre de 2026 aparecen rótulos o tomas de partido propias contra el Gobierno De la Espriella que lleven la proporción a 3:1 con al menos 3 piezas después del 07-08, el número se reabre con tope de ±0,30, salvo endoso explícito».
9. **REVISIÓN EXTERNA:** esta resolución, con modelo, versión y fecha.

En otras fichas:
- `fichas/casa-macondo.md:63` y `fichas/voragine.md:13`: el «−0,45» de Cuestión Pública → «sin medir desde el 2026-09-18».
- `shared/mediaRegistry.js:278` (Las2Orillas): la comparación «por debajo de la investigación militante (Vorágine, Cuestión Pública)» se apoya en valores que ya no existen. Que lo decida la tanda 9.

**Lo que NO entra como hecho:**
- nada sobre la ubicación ni sobre las condiciones de seguridad de la directora;
- su año y su lugar de nacimiento;
- la composición accionaria más allá de lo que declara el medio;
- que «quebrar el modelo» haya supuesto un cambio societario;
- el trino del 02-04-2026 que el revisor no descargó;
- que «House of Nariño» trate del Gobierno Petro, como cita del Informe.

**¿Aviso de quien dirige?** No procede: no consta candidatura ni cargo público de la directora.

**Decisiones para el responsable editorial:**
1. **Valor.** Recomendación: **sin medir**, con la razón reescrita y la tensión a la izquierda declarada. Alternativa: −0,25, que no se recomienda.
2. **El endoso.** Recomendación: la columna del 16-06 **no** es endoso explícito; cuenta en el barrido como encuadre asimétrico. Conviene escribir en el protocolo qué es «endoso explícito»: que la casa pida el voto o declare su apoyo a un candidato con nombre. El encuadre asimétrico sin petición ni apoyo declarado es evidencia de primer orden, cuenta en el barrido y no levanta el tope.
3. **El «sin medir» del 2026-09-16** no tiene entrada en DECISIONES.md. Recomendación: anotarlo con la tanda 8, junto con la cabecera desfasada de esta ficha y las de Vorágine y RAYA, si están igual.
4. **La captura del corpus:** 8 de 41 piezas en 30 días. Recomendación: revisar el feed (`/feed/`) y los filtros de ingesta para este medio, empezando por la categoría Vídeo, que es casi la mitad de lo que publica.
5. **Recuento en diciembre de 2026**, con 4 meses del Gobierno De la Espriella. Recomendación: sí, junto con el de Proclama del Pacífico.
