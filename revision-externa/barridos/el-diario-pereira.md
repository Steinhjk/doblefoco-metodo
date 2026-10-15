# Barrido editorial: El Diario (Pereira) / Diario del Otún

| | |
|---|---|
| **Medio** | El Diario (Pereira), que publica hoy con la cabecera *Diario del Otún* (`el-diario-pereira`) |
| **Valor vigente** | +0,20, provisional de alta, sin firmar. Dirección declarada: derecha, «coherente con +0,20» |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09) |
| **Ventana** | 2025-10-09 → 2026-10-09 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5 (`claude-opus-5-5`), a petición del responsable editorial, el 2026-10-09. Es de la misma casa que el autor de la ficha: su acuerdo no es aval |
| **Estado** | **DECIDIDO el 2026-10-09: +0,25** (antes +0,20), por el responsable editorial; firmado en bloque el 2026-10-10 (`DECISIONES.md`, «2026-10-09 · Reexamen de cinco fichas cerradas con la regla nueva»). Lo que más abajo dice «propuesta» o «pendiente» es el estado anterior a la decisión y se conserva como historia |
| **Decisión (2026-10-09)** | el responsable editorial: **de +0,20 a +0,25.** Desde el 07-08 se declara el 9 a 7; las 9 piezas posteriores son elogios al programa, no fiscalización (`DECISIONES.md`, «Reexamen de cinco fichas cerradas con la regla nueva»; ver la ficha) |

---

## 1. Método

- **robots.txt** (descargado el 2026-10-09): `User-agent: * / Disallow: /wp-admin/`. No excluye a ningún agente ni la API. El pie del sitio prohíbe reproducir el contenido «en inteligencia artificial o aprendizaje automático [...] sin autorización escrita». Por eso aquí solo se citan fragmentos breves como evidencia, y no se reproduce nada.
- **Fuente:** la API REST pública de WordPress del propio medio. Se usó `curl -sL` con el UA de un navegador.
  - **Consulta principal:** `https://www.eldiario.com.co/wp-json/wp/v2/posts?categories=77&after=2025-10-09T00:00:00&before=2026-10-10T00:00:00&per_page=100&page=1..4`.
    - La categoría 77 es «Editorial».
    - Devuelve **316 entradas** (cabecera `X-WP-Total: 316`): 263 antes del 07-08-2026 y 53 desde ese día.
    - **Es el archivo editorial completo de los 12 meses, sin muestreo.**
- **Voz de la casa.** Los editoriales salen sin firma y se suben desde cuentas técnicas: «Editor web», «M.E. - Editor Web», «Eds Say», «M.H. Editor Web» y «S.G - Editor Web». Hablan como la casa: «Este medio invita al Senador…» (10-11-2025) y «Desde estas líneas expresamos…» (12-08-2026).
  - Hay 3 entradas con doble categoría: dos con «Sin categoría» y una con «Opinión», la del 05-12-2025, «Un ranking esperanzador».
  - **Ninguna tiene posición en el eje.** Ninguna es contenido patrocinado (categoría 763).
- **Filtro.** Primero se buscaron en el texto completo de las 316 entradas los términos nacionales: Petro, De la Espriella/Abelardo, Cepeda, Fajardo, Paloma, Pacto Histórico, Paz Total, izquierda/derecha, constituyente, Uribe, Ecopetrol, «el presidente», «gobierno nacional», candidat-, elecci-, campaña y ministr-.
  - **132 entradas** tenían alguno.
  - Se leyeron una a una: los primeros 2.200 caracteres, y entera cuando hacía falta. Los editoriales miden unos 3.000 caracteres de media.
  - También se leyeron los títulos de las 184 restantes, para no perder ninguna pieza nacional sin palabra clave.
- **Duplicados.** El medio publicó tres editoriales dos veces, con otra URL. Cada uno cuenta una sola vez:
  - `un-episodio-que-afecta-al-pais` y `-2`;
  - `el-triste-papel-de-la-comision` y `-2`;
  - `el-cambio-de-tono-de-cepeda` y `senales-que-no-deben-ignorarse`, que tienen el mismo texto.
- **Qué se clasificó.** Solo las piezas con postura sobre el Gobierno nacional, sus políticas, su candidato o la candidatura rival, y sobre el presidente electo y el nuevo Gobierno.
  - **D, dirección derecha:**
    - critica al Gobierno Petro, a su modelo o a su candidato;
    - pide unir a la derecha contra «la opción de izquierda»;
    - celebra al presidente electo o al Gobierno De la Espriella, o su programa.
  - **C, contrapeso:**
    - critica o fiscaliza al presidente electo o al Gobierno De la Espriella;
    - elogia o reconoce a Petro, a su Gobierno o a la izquierda.
  - **M (mixta o institucional):** lleva postura, pero no se inclina hacia ningún lado. No cuenta.
  - **Fuera del recuento:**
    - los editoriales locales: Alcaldía, Gobernación, Gallo, terremoto sin destinatario nacional;
    - los de procedimiento electoral, las efemérides y los de política internacional (Maduro, 04-01-2026);
    - los históricos (Palacio de Justicia, 05-11-2025).
- **Límite declarado.** La clasificación de tono es juicio de un solo verificador. Las URL y las fechas están en la tabla para que cualquiera la rehaga. **No se clasificaron las columnas de opinión** (categoría 76) **ni las notas informativas**: no cuentan para la regla. Sobre los titulares de las noticias, ver el §5.

---

## 2. Tabla de piezas que cuentan (voz de la casa, sección Editorial)

Todas las URL son `https://www.eldiario.com.co/editorial/<slug>/`.

### 2.1 Antes del cambio: 2025-10-09 → 2026-08-06 (gobierna Petro)

| # | Fecha | Slug | Dir. | Clasificación (fragmento breve) |
|---|---|---|---|---|
| 1 | 2025-10-17 | `una-estrategia-con-lo-mismo` | D | Fiscaliza al Gobierno: el Bloque de Búsqueda presentado sin pie de fuerza nuevo |
| 2 | 2025-10-21 | `otra-vez-desfinanciado` | D | Presupuesto de Petro: subir impuestos en este momento «es más que una aventura, una irresponsabilidad» |
| 3 | 2025-10-22 | `los-efectos-de-la-imprudencia` | D | Diplomacia de Petro con EE. UU.: «la vanidad de un discurso ideológico» |
| 4 | 2025-10-25 | `rumbo-al-mismo-error` | D | Paz Total con el ELN: «fracasado proceso» |
| 5 | 2025-10-27 | `un-episodio-que-afecta-al-pais` (y `-2`) | D | Lista Clinton; política antidrogas «basada en la permisividad» |
| 6 | 2025-10-30 | `la-apatia-juvenil` | D | Leve: los jóvenes «no votaron por los candidatos de los partidos alternativos ni progresistas» |
| 7 | 2025-11-14 | `una-afrenta-al-orden-judicial` | D | El ministro Benedetti contra la Corte |
| 8 | 2025-11-18 | `unas-cifras-lejos-de-ser-halagadoras` | D | Fiscaliza la inversión nacional en Risaralda |
| 9 | 2025-12-08 | `sensatez-es-lo-que-se-pide` | D | Salario mínimo: el Presidente «se anticipó imprudentemente» |
| 10 | 2025-12-23 | `por-que-la-demora` | D | Antidrones; Paz Total que da «todas las gabelas» |
| 11 | 2025-12-28 | `una-emergencia-espuria` | D | Emergencia económica: «se adivina en el Gobierno mala intención» |
| 12 | 2025-12-30 | `el-dificil-momento-de-la-fuerza-publica` | D | Fuerza Pública; la Paz Total fortaleció a los armados |
| 13 | 2025-12-31 | `el-2025-un-ano-perdido` | D | «sus funestas reformas»; «Nada es rescatable al cierre del año» |
| 14 | 2026-01-03 | `un-2026-lleno-de-incertidumbre` | D | Constituyente «con propósitos oscuros» |
| 15 | 2026-01-04 | `el-triste-papel-de-la-comision` (y `-2`) | D | Salario mínimo: «la más ominosa burla» |
| 16 | 2026-01-15 | `un-subsidio-dificil-de-aplicar` | D | Leve: decreto del diésel de difícil aplicación |
| 17 | 2026-01-17 | `un-alza-inevitable` | D | «aumentar irresponsablemente el salario mínimo» |
| 18 | 2026-01-19 | `un-balance-dramatico` | D | Catatumbo: acciones del Gobierno «más pobres, más ineficaces y más erráticas» |
| 19 | 2026-01-22 | `los-efectos-de-una-improvisacion` | D | Decreto de la VIS: «intento desesperado» |
| 20 | 2026-01-24 | `la-fiesta-de-los-falsos-diplomas` | D | Diplomas en el entorno presidencial |
| 21 | 2026-01-30 | `la-ultima-encuesta-2` | D | **Candidaturas:** si la derecha y el centro-derecha no se unen, el país tendrá que «soportar un nuevo gobierno con el sello petrista» |
| 22 | 2026-01-31 | `hizo-bien-la-corte-constitucional` | D | Emergencia suspendida: «desdén por la separación de poderes» |
| 23 | 2026-02-05 | `el-desespero-del-presidente` | D | «la continuidad de su fracasado modelo de gobierno» |
| 24 | 2026-02-10 | `quien-se-esta-beneficiando` | D | Rebaja de la gasolina: «el populista anuncio» |
| 25 | 2026-02-12 | `aqui-se-burlan-de-la-ley` | D | El caso Guerrero, defendido por Petro |
| 26 | 2026-02-14 | `los-efectos-del-fallo` | D | Leve: la sospecha de un salario calculado «para capitalizar su efecto político» |
| 27 | 2026-02-18 | `una-oportunidad` | D | Leve: pide concertación «sin populismo» |
| 28 | 2026-02-21 | `todos-cayeron-en-la-trampa` | D | El Gobierno «hábil y maquiavélicamente tendió una trampa» |
| 29 | 2026-02-25 | `cerritos-no-merece-esa-obrita` | D | Fiscaliza al Invías y a la ministra de Transporte |
| 30 | 2026-03-03 | `cada-vez-peor` | D | Corrupción; dineros ilegales en la campaña del presidente |
| 31 | 2026-03-07 | `es-hora-de-votar-bien` | D | Leve: «el evidente fracaso de la Paz Total» |
| 32 | 2026-04-08 | `la-libertad-de-los-capos` | D | Libertad de cabecillas; «la manida justificación de la Paz Total» |
| 33 | 2026-04-15 | `el-pais-esta-patas-arriba` | D | Las cárceles y la «mesa de paz urbana» |
| 34 | 2026-04-24 | `un-desproposito-2` | D | Salario contra el Banco de la República: «maniobra de distracción» |
| 35 | 2026-04-30 | `un-mensaje-devastador` | D | Cajibío: «La indulgencia disfrazada de estrategia de "paz total"» |
| 36 | 2026-05-01 | `el-1o-de-mayo-es-de-los-trabajadores` | D | El Primero de Mayo usado «como lo intenta el presidente Petro» |
| 37 | 2026-05-14 | `una-peligrosa-concesion` | D | Clan del Golfo: «la peor afrenta a la justicia» |
| 38 | 2026-05-15 | `el-respeto-es-una-obligacion` | D | Petro contra el Consejo de Estado: «trasfondo autoritario» |
| 39 | 2026-05-23 | `urge-una-accion-inmediata` | D | Riesgo electoral: «desde el Gobierno se ve un esfuerzo por bajar el tono» |
| 40 | 2026-05-26 | `merece-el-repudio-general` | D | UNGRD: el «entramado criminal que desde el Gobierno se montó» |
| 41 | 2026-05-28 | `respeto-prudencia-y-vocacion-patriotica` | D | **Candidaturas:** «enfrentar con cohesión a la opción de izquierda» |
| 42 | 2026-05-29 | `los-mensajes-del-presidente` | D | Petro siembra dudas sobre el fraude sin pruebas |
| 43 | 2026-06-01 | `las-elecciones-de-ayer-5` | D | «quienes apoyan al presidente Petro y su fallido modelo de cambió» |
| 44 | 2026-06-03 | `la-ley-tambien-obliga-al-presidente` | D | Petro en la campaña de Cepeda: «decisión consciente de violar la ley» |
| 45 | 2026-06-04 | `lo-que-dejo-las-elecciones-2` | D | **Candidaturas:** el votante de centro, obligado «a girar hacia una derecha que le devuelva a ellos y al país las esperanzas» |
| 46 | 2026-06-06 | `el-presidente-en-campana` | D | «Hasta el último momento el presidente Petro irrespetó a los colombianos» |
| 47 | 2026-06-08 | `una-senal-que-no-espera-el-pais` | D | Carnetización: «la fallida paz total» |
| 48 | 2026-06-12 | `un-hecho-dificil-de-entender` | D | La suspensión de Petro como «victimización oficialista» |
| 49 | 2026-06-16 | `una-senal-de-esperanza` | D | Operación de EE. UU.; la Paz Total y la expansión criminal |
| 50 | 2026-06-22 | `de-la-espriella-presidente` | D | La victoria como rechazo «a la llamada Paz Total», a la corrupción, etc. |
| 51 | 2026-06-24 | `ya-paso-la-campana` | D | «la fracasada propuesta de cambio» frente a la «propuesta de recuperación» de De la Espriella. Le pide gobernar «sin revancha» |
| 52 | 2026-06-26 | `lo-que-va-de-ivan-a-gustavo` | D | Critica la reacción de Petro. **Contiene un contrapeso**: elogia que Cepeda aceptara la derrota |
| 53 | 2026-06-30 | `la-paz-negociada-con-la-criminalidad` | D | Acuerdos con el Clan del Golfo: «la entrega del Estado» |
| 54 | 2026-07-01 | `un-mensaje-claro-2` | D | Presidente electo con las Cortes: «señal positiva» |
| 55 | 2026-07-04 | `el-anunciado-ministro-de-hacienda` | D | Gabinete: «prudente optimismo» |
| 56 | 2026-07-06 | `el-cambio-de-tono-de-cepeda` (y `senales-que-no-deben-ignorarse`, 07-07) | D | Contra la «desobediencia civil» de Cepeda |
| 57 | 2026-07-08 | `un-escenario-preocupante` | D | Petro desconoce el resultado y suspende el empalme |
| 58 | 2026-07-14 | `un-final-lastimoso` | D | El Ministerio de la Igualdad, «por conveniencia política» |
| 59 | 2026-07-17 | `la-paz-total-no-va-mas` | D | El fin de la Paz Total: «resulta acertado» |
| 60 | 2026-07-30 | `el-doloroso-crespon-de-cierre` | D | Escándalos: «su fracaso ético y administrativo» |
| 61 | 2026-08-06 | `cuatro-anos-perdidos` | D | «la sucesión de hechos lamentables»; Ecopetrol «aniquilada» |
| 62 | 2026-07-23 | `una-pelea-que-no-debio-darse` | **C** | Presidente electo: «el Gobierno entrante se equivocó en el manejo» de la presidencia del Senado. Reparte la culpa con el CD |
| 63 | 2026-07-25 | `una-sede-alterna-innecesaria` | **C** | Barranquilla como sede alterna: «innecesario e inoportuno». Pide que no anuncie «cada idea que se le ocurre» |
| 64 | 2026-07-29 | `risaralda-tambien-cuenta` | **C** | Reclamo regional: Risaralda no está en el gabinete. Añade que el departamento «acompañó con decisión la campaña» |

### 2.2 Después del cambio: 2026-08-07 → 2026-10-09 (gobierna De la Espriella)

| # | Fecha | Slug | Dir. | Clasificación (fragmento breve) |
|---|---|---|---|---|
| 65 | 2026-08-07 | `un-nuevo-comienzo-para-colombia` | D | Leve: es del día de la posesión. Expectativa condicionada, «que prevalezcan la prudencia sobre la confrontación» |
| 66 | 2026-08-10 | `anuncios-que-auguran-futuro` | D | «confiar en que de verdad el país vive un nuevo amanecer» |
| 67 | 2026-08-26 | `la-nueva-politica-migratoria` | D | Respalda el endurecimiento. Con matiz: «no puede convertirse en sinónimo de delincuencia» |
| 68 | 2026-09-03 | `habra-autoridad-justicia-y-estado` | D | Fin de las mesas de diálogo. Contra el gobierno anterior: «Se perdieron cuatro años valiosos» |
| 69 | 2026-09-07 | `un-mensaje-claro-contra-el-crimen` | D | «Bendito Menor»: la orden presidencial «puede convertirse en resultados» |
| 70 | 2026-09-09 | `un-balance-muy-favorable` | D | «Con un equipo de gobierno bien escogido»; «Canceló la llamada Paz Total» |
| 71 | 2026-09-12 | `el-reto-es-el-control-de-la-ilegalidad` | D | Respalda el levantamiento de la restricción al porte de armas, con salvedades |
| 72 | 2026-09-18 | `autonomia-universitaria-no-impunidad` | D | Respalda un protocolo para la Fuerza Pública en las universidades, con matices |
| 73 | 2026-09-24 | `que-diferencia` | D | Elogia la respuesta del Presidente al paro armado, frente al gobernador. Reconoce que sus «expresiones fuertes» generaron cuestionamientos |
| 74 | 2026-08-25 | `no-basta-experiencia-empresarial` | **C** | Fiscaliza el nombramiento del gerente del Fondo Milagro |
| 75 | 2026-08-31 | `presidente-el-epicentro-fue-pereira` | **C** | «Aquí ya no se necesitan más anuncios, ni discursos, ni promesas» |
| 76 | 2026-09-08 | `una-visita-tardia` | **C** | El Fondo Milagro tarda un mes en ir a Pereira |
| 77 | 2026-09-16 | `un-silencio-que-preocupa` | **C** | «Preocupa el silencio del presidente De la Espriella frente a Pereira» |
| 78 | 2026-09-17 | `un-episodio-que-puede-afectar` | **C** | **Institucional, no regional:** el relevo del director del DANE «puede afectar la percepción de autonomía» |
| 79 | 2026-10-02 | `generalizar-crece-la-desconfianza` | **C** | La advertencia presidencial a los gobernantes regionales: «la generalización resulta injusta» |
| 80 | 2026-10-06 | `primero-reconstruir` | **C** | Visita del Plan Nacional de Desarrollo: «Pereira necesita respuestas concretas» |

**Con postura pero mixtas (M, no cuentan):**
- 12-08-2026 `un-balance-desolador`: reconoce la reacción del Presidente y del Alcalde ante el terremoto, y no hace más.
- 01-09-2026 `la-otra-tragedia`: el envío de 500 policías es «un mensaje de esperanza».
- 10-09-2026 `a-un-mes-de-la-tragedia`: elogia la presencia del Presidente y critica al Fondo Milagro a partes iguales.
- 09-10-2026 `un-ejercicio-valioso-pero`: «merece ser destacada», con reparos fiscales.
- 24-07-2026 `en-que-queda-pereira`: recibe «con esperanza» el plan del nuevo ministro de Defensa y reclama para Pereira.

**Nacionales, sin inclinación o fuera del objeto (no cuentan):**
- 11-10-2025 `la-policia-sabia` y 29-10-2025 `ojala-el-cambio-sirva`: dudan de la acusación de Petro, pero también de la Policía.
- 24-10-2025 `el-fallo-en-favor-de-uribe`: expone las dos lecturas.
- 09, 10 y 11-03-2026: los tres balances del 8 de marzo, que registran sin juicio la «muy importante» votación del Pacto Histórico.
- 16-03-2026 `los-vicepresidentes-escogidos`.
- Los de procedimiento electoral: 18-10-2025, 20-10-2025, 16-11-2025, 10-12-2025, 16-01-2026, 04-02-2026, 06-02-2026, 02-03-2026, 05-03-2026, 06-03-2026, 19-05-2026 y 20-06-2026.
- Las llamadas a votar sin nombrar candidato: 31-05, 19-06 y 21-06-2026.
- 11-05-2026 `german-vargas-lleras`: necrológica.
- 04-01-2026 `una-oportunidad-para-colombia`, sobre la captura de Maduro: tiene encuadre ideológico, pero es política exterior y no gobierno ni candidatura colombianos.
- 05-11-2025 `cuenta-anos-despues`, sobre el Palacio de Justicia: histórico.

---

## 3. Recuento

| | D (derecha) | C (contrapeso) | Total con postura |
|---|---|---|---|
| Antes del 07-08-2026 | **61** | **3** | 64 |
| Desde el 07-08-2026 | **9** | **7** | 16 |
| **Total** | **70** | **10** | **80** |

**Proporción global: 70 a 10, es decir 7 a 1.**

**La lectura del polo fijo**, que separa lo que es fiscalizar a quien manda de lo que no lo es:

| Trato al gobierno **en ejercicio** | Favorables | Críticos |
|---|---|---|
| Petro, mientras gobierna (52 piezas sobre su Gobierno) | **0** | **52** |
| De la Espriella, ya en el poder | **9** | **7** |

- **Con Petro**, la crítica no es solo de gestión. Es al **modelo**: «fallido modelo de cambió», «fracasado modelo de gobierno», «funestas reformas», la Paz Total en una docena de piezas.
- **Con De la Espriella**, el modelo se **celebra**: Paz Total cancelada, porte de armas, migración, universidades, «un nuevo amanecer». De las 7 críticas, **6 son reclamos de atención a Pereira tras el terremoto** (Fondo Milagro, silencio presidencial, la visita del Plan Nacional de Desarrollo) y **1 es institucional** (el DANE). **Ninguna critica una política de su programa.**
- **Sobre las candidaturas**, antes de las urnas, la casa se sitúa:
  - 30-01-2026: unir a la derecha para no «soportar un nuevo gobierno con el sello petrista»;
  - 28-05-2026: «enfrentar con cohesión a la opción de izquierda»;
  - 04-06-2026: «girar hacia una derecha que le devuelva [...] las esperanzas».
  - **No nombra candidato.** El 31-05, el 19-06 y el 21-06 pide votar sin decir por quién.
- **Después del cambio**, al gobierno saliente se le sigue tratando con dureza: «Se perdieron cuatro años valiosos» (03-09).

---

## 4. Contrapesos (lo que contradice la dirección, y cuánto pesa)

1. **La casa fiscaliza al Gobierno entrante, y con dureza:** 7 editoriales en 2 meses, más 3 al presidente electo entre el 23 y el 29-07. Titulares en segunda persona como «Presidente, el epicentro fue Pereira».
   - **Peso: medio.** Es real y en voz propia, pero localista. Lo que reclama es atención y recursos para Pereira, no un cambio de programa.
   - El único reparo de principio es el del DANE (17-09).
   - **Visto solo desde el 07-08, el lado favorable gana por 9 a 7, que no es 3 a 1.** Por eso la asimetría está en el **contenido** (se celebra el programa y se reclama la atención) y no en el recuento de ese lado.
2. **Reconocimientos a la izquierda.**
   - 26-06-2026: Cepeda «actuó dentro de los parámetros que exige una democracia madura».
   - 09-03-2026: la «muy importante e inesperada votación del Pacto Histórico», registrada sin juicio.
   - 02-09-2026: la cifra «alentadora» del desempleo de julio, todavía de la era Petro.
   - **Peso: bajo.** Son tres piezas sueltas frente a 52 críticas al Gobierno Petro.
3. **No hay endoso.** El diario no pide el voto por un candidato con nombre: 31-05, 19-06 y 21-06-2026.
   - **Peso: alto para la magnitud.** Mantiene el caso bajo el tope de ±0,30 de la regla.
   - Los editoriales del 28-05 y del 04-06 son lo más cercano a un endoso, pero no nombran a nadie.
4. **Matices dentro de las piezas favorables:**
   - la migración «no puede convertirse en sinónimo de delincuencia» (26-08);
   - el porte de armas «no significa convertir las calles en un territorio armado» (12-09);
   - las «expresiones fuertes» del Presidente «han generado cuestionamientos» (24-09);
   - «sin revancha, con mesura» (24-06).
   - **Peso: bajo.** No cambian el sentido de las piezas.
5. **El polo fijo, del lado de Petro.** Buena parte de las 52 críticas es fiscalización de quien manda, que por sí sola no cuenta.
   - Lo que convierte esa crítica en evidencia es lo que vino después: la celebración del programa entrante y el encuadre de las candidaturas.
   - **Peso:** obliga a no leer el 61 a 3 de antes del cambio como una medida de orientación por sí mismo.
6. **Conflictos de la casa ya declarados en la ficha.** El director apoyó en 2023 al alcalde Salazar; hay pauta municipal; hay pleito con Gallo.
   - **Son locales y no tocan el eje nacional.** No suman ni restan aquí.
   - Sí explican por qué la fiscalización del Gobierno entrante es localista.

---

## 5. Comprobación complementaria: titulares de noticias (no cuenta)

- **Búsqueda:** `posts?search=Petro` y `search=Espriella` en la misma ventana, 5 páginas de 100 por término.
- **Cobertura:** el orden es por fecha descendente, así que el recorte cubre sobre todo de abril a octubre de 2026. **No es un barrido completo.**
- **Resultado:** 842 entradas únicas, de ellas 595 noticias, 213 columnas y 34 editoriales. **276 titulares de noticias** nombran a Petro, De la Espriella o Cepeda.
- **Qué muestran:** son mayoritariamente atributivos («Petro dice…», «De la Espriella anuncia…»).
- **Calificativos en voz propia, a un lado:**
  - «Pereira y Risaralda le cumplieron al tigre De la Espriella» (22-06);
  - «El Eje Cafetero se tiñó de De la Espriella» (22-06);
  - «…arranque positivo para el nuevo Gobierno» (30-06);
  - «Economía colombiana crecerá a pesar de decisiones del Gobierno Petro» (28-05).
- **Al otro lado:**
  - «Iván Cepeda, una vida contra el olvido» (09-05);
  - «Logros sociales y sombras fiscales, el balance del gobierno Petro» (27-06);
  - «¿Qué tan viables son las propuestas de Abelardo de la Espriella?» (13-09);
  - «¿Una "Casa Blanca" en un batallón? La polémica sede…» (31-07).
- **Lectura:** el tono informativo es más plano que el editorial. Pero no lo contradice.

---

## 6. Veredicto por condición

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | **Sí** | Las 80 piezas son editoriales sin firma de la sección Editorial, que hablan como «este medio». No se cuenta ninguna columna, comunicado ni pieza pagada |
| 2. A los dos lados del cambio (07-08-2026), en 12 meses | **Sí** | 64 piezas antes y 16 después. Hay asimetría de contenido: con Petro se critica el modelo; con De la Espriella se celebra el programa y se fiscaliza la atención a Pereira. No es solo fiscalizar a quien manda |
| 3a. ≥10 piezas con postura | **Sí** | 80 |
| 3b. ≥3 a cada lado del cambio | **Sí** | En la dirección D: 61 antes y 9 después. Contrapesos: 3 antes y 7 después |
| 3c. Proporción ≥3:1 | **Sí, en el global** | 70:10 = 7:1. **Aviso:** solo desde el 07-08 es 9:7 |
| 4. Contrapesos escritos | **Sí** | §4, con peso asignado a cada uno |
| 5. Reproducible | **Sí** | La tabla del §2 tiene URL, fecha y clasificación. La consulta exacta está en el §1 |

**Las cinco condiciones se cumplen.** La regla permite mover el número, o sostenerlo ahora con evidencia, dentro del tope de ±0,30: no hay propiedad documentada con posición nacional (nivel 1) ni endoso explícito.

---

## 7. PROPUESTA (pendiente de la firma del responsable editorial)

**+0,25, derecha moderada.** Sube +0,05 desde el +0,20 vigente, y ahora como conducta medida y no como valor de banda regional.

**Por qué no bajar a 0,00.** El barrido no muestra la misma conducta con los dos gobiernos:
- con Petro: 0 piezas favorables y 52 críticas, la mayoría contra su modelo;
- con De la Espriella: 9 favorables a su programa, y críticas solo por la atención a Pereira y por el DANE.
- Antes de las urnas, la casa se situó contra «la opción de izquierda».

**Por qué no quedarse en +0,20 (El Pilón, El Heraldo):**
- La evidencia es más fuerte que una inclinación de encuadre. Son 80 piezas en voz propia, un año entero y los dos lados del cambio.
- Hay tres editoriales de campaña que toman partido por un bloque (30-01, 28-05 y 04-06).
- Se celebra explícitamente el programa entrante: «un nuevo amanecer», «un balance muy favorable».
- El +0,20 vigente salía del grupo, no de la conducta. Si el número se quedara igual, quedaría a la altura de medios con menos evidencia.

**Por qué no +0,30 (Archipiélago Press, propuesto):**
- Aquí la voz de la casa sí fiscaliza al Gobierno entrante: 7 editoriales, uno de ellos institucional (DANE), y 3 más al presidente electo. En Archipiélago no hay ninguna.
- Reconoce a Cepeda (26-06).
- No hay rótulos despectivos como «dictador».
- Desde el 07-08, el lado favorable no llega a 3 a 1 (9:7).

**Por qué +0,25, a la altura de Vive el Meta (propuesto).** Dirección clara y sostenida, magnitud moderada y contrapesos reales. La regla 2 y el principio de quedarse en lo más cercano a la mixta que la evidencia permite lo sitúan **por debajo** de Archipiélago y **un paso por encima** de los +0,20 sin barrido.

**Lectura alternativa, que se declara.** Si el responsable editorial pesa más los 7 contrapesos posteriores al cambio que el recuento global, **+0,20 sostenido ahora con evidencia** es defendible. La dirección no cambia; cambia solo la magnitud dentro de la misma banda. Lo que el barrido **no** sostiene es el 0,00.

**Lo que esta propuesta NO hace:**
- No hace firmable la ficha.
- No resuelve el accionariado: falta el certificado de la Cámara de Comercio.
- No toca las tensiones locales (pauta, Salazar, Gallo), que siguen declaradas como conflicto.

**Qué la refutaría:**
- que en los próximos meses los editoriales critiquen el programa del Gobierno De la Espriella (seguridad, Paz Total, migración, JEP) y no solo su atención a Pereira;
- o que aparezca un barrido de las columnas y notas con un sesgo opuesto que la casa haga suyo.

Si en cambio llega un endoso con nombre en la próxima elección, el tope de ±0,30 dejaría de aplicarse.

---

## 8. Avisos

- **Una sola lectura.** La clasificación es de un verificador de la misma casa que el autor de la ficha. Las piezas límite que otro podría leer como M se marcaron «leve»: #6, #16, #26, #27, #31 y #65. Aunque se pasaran todas a M, el recuento quedaría en 64 a 10, que sigue por encima de 3 a 1.
- **El 07-08-2026, en el lado de después.** Ese día se publicó «Un nuevo comienzo para Colombia». Si se pasa al lado de antes, el resultado no cambia.
- **El pie del sitio prohíbe el uso del contenido en IA.** Solo se citan fragmentos breves como evidencia. No se ha guardado ni se publica el texto completo en el repositorio.
- **Datos personales.** No se recogen cédulas, teléfonos ni direcciones de personas naturales. Los únicos nombres son de cargos públicos o de las piezas.
