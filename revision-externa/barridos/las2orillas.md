# Barrido editorial: Las2Orillas

| | |
|---|---|
| **Medio** | Las2Orillas (`las2orillas`), en el catálogo. Lo edita la Fundación Las Dos Orillas (NIT 900615503) |
| **Valor vigente** | **−0,35**, sin firmar (`reviewedAt: null`), puesto en el alta del 2026-08-24 «por comparación con CasaMacondo» (ver §8) |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus dos precisiones |
| **Ventana** | 2025-10-10 → 2026-10-10 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Resolución de origen** | `revision-externa/respuestas/opus-5-5-las2orillas.md` (el revisor contó 19 piezas con postura, aunque escribió 25: 7 a la izquierda y 12 a la derecha) |
| **Quién lo hizo** | Claude Opus 5.5 (`claude-opus-5-5`), verificador del ciclo 2, tanda 9, a petición del responsable editorial, el 2026-10-10. Es de la misma casa que el autor de la ficha y que el revisor, así que su acuerdo no es aval |
| **Estado** | **DECIDIDO el 2026-10-10: 0,00 con evidencia** (antes −0,35), por el responsable editorial; firmado en bloque el mismo día (`DECISIONES.md`, «2026-10-10 · Tandas 8 y 9 del ciclo 2: el barrido manda sobre los números sin evidencia»). Lo que más abajo dice «propuesta», «recomendada» o «pendiente» es el estado anterior a la decisión y se conserva como historia |
| **Resultado** | **No cumple los mínimos en ninguna dirección.** 23 piezas con postura en la voz de la casa: 9 a la izquierda, todas antes del 07-08 (1 plena y 8 leves), y 14 a la derecha (5 antes y 9 después, todas leves). La proporción es de 1,6 a 1 **hacia la derecha**, que es el signo contrario al del valor vigente. Lo que el barrido sí muestra es una conducta que se repite con los dos gobiernos: fiscaliza a quien manda y, a la vez, publica piezas amables con sus medidas (5 con Petro y 9 con De la Espriella) |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas, la clase y
> el fragmento están aquí para eso, y el apéndice lista las 469 piezas del
> universo. **La clasificación de cada pieza es juicio de un solo lector**, de
> la misma casa que el autor de la ficha y que el revisor.

---

## 1. Método

- **robots.txt** de `www.las2orillas.co`, leído el 2026-10-10 antes de descargar nada: `User-agent: *` con `Disallow: /wp-admin/` y `Allow: /wp-admin/admin-ajax.php`, más tres sitemaps. No nombra a ClaudeBot, Claude-Web ni anthropic-ai. La API `/wp-json/` y las piezas no están vetadas.
- **Descarga:** `curl -sL --ssl-no-revoke` con User-Agent de navegador (Chrome 126), con una pausa de 3 a 4 segundos entre peticiones. El servidor devolvió 522 cuatro veces. Tres piezas se recuperaron al reintentar. Una no se pudo leer (§7).
- **Voz de la casa (condición 1).** En la API de WordPress, la casa publica con tres cuentas: el autor 457 (`/author/l2oadm/`) y el autor 2 (`/author/2orillas/`), los dos con `<meta name="author" content="Las Dos Orillas"/>`, y el autor 456 (`/author/l2oia/`, «Las2orillas.»), con 3 piezas en el universo. El resto son periodistas de plantilla con firma (Elisa Pastrana, Adriana Arcila, Daniel Murcia, Andrés Felipe Páez, Jorge González, Juan Manuel Ospina, Mauricio Cárdenas…) o columnistas, y **no se cuentan**. La directora no tiene piezas firmadas en la ventana: la búsqueda por su nombre devuelve una sola pieza, firmada por la cuenta 456. No hay categoría editorial: `/wp-json/wp/v2/categories?search=editorial` devuelve `[]`, y la etiqueta «editorial» (id 185884, 10 piezas) agrupa reseñas.
- **Universo, sin muestreo dentro de cada parte:**
  1. **Todas las piezas de la casa en la categoría Poder (id 142)** en 12 meses: 257 de las 693 de Poder (230 del autor 457, 26 del 2 y 1 del 456). Consulta: `/wp-json/wp/v2/posts?categories=142&after=2025-10-10T00:00:00&per_page=100&page=1..7&_fields=id,date,author,link,title,categories`.
  2. **Todas las piezas de la casa de cualquier otra categoría cuyo título nombra a un actor nacional del eje**, a los dos lados del cambio: 212. Se sacaron de las búsquedas `search=Petro` (2.001 resultados), `Espriella` (961), `Cepeda` (654) y `Paloma` (277), todas desde el 2025-10-10, paginadas enteras. De esas 2.556 piezas únicas, 665 son de la casa, y de ellas se quedan las que no están en Poder y llevan en el título Petro, Espriella, Abelardo, Tigre, Cepeda, Paloma, gobierno o presidente.
  
  **Total: 469 piezas, 402 antes del 07-08 y 67 después** (434 del autor 457, 32 del 2 y 3 del 456). El revisor añadió las piezas de fuera de Poder **solo después del cambio** («Espriella» en el título desde el 07-08). Eso infla el lado derecho posterior. Aquí la segunda parte se tomó igual a los dos lados.
- **Lectura.**
  - Las 324 piezas cuyo título toca la política nacional se leyeron por la entrada (unas 90 palabras) y por las frases evaluativas del cuerpo. Las demás 145 son de empresas, crónica, internacional o farándula sin actor del eje, y no se leyeron más allá del título («NP» en el apéndice).
  - **Las 19 piezas que contó el revisor y las 23 que suman aquí se leyeron enteras**, con el cuerpo extraído del HTML (del bloque `addtoany_content_top` al bloque `post-share`). También se leyeron enteras las piezas límite.
  - Cada fragmento entre comillas de este archivo se comprobó por programa contra el texto de su página.
- **Clases.**
  - **I, izquierda** (cuenta): elogio o perfil laudatorio de un actor de izquierda que no gobierna; elogio de una medida del Gobierno Petro mientras gobierna; rótulo descalificador contra un actor de derecha.
  - **D, derecha** (cuenta): lo simétrico. Elogio de un actor de derecha que no gobierna; elogio de una medida del Gobierno De la Espriella; rótulo o burla contra un actor de izquierda.
  - **Leve** (cuenta, pero se marca): la postura está en el título o en un adjetivo, o la pieza la matiza.
  - **F, solo fiscaliza a quien manda** (no cuenta, se declara). Precisión del responsable editorial del 2026-10-09: no suma para el mínimo por lado.
  - **I (inv.), investiga a una candidatura** (no cuenta, se declara): pesquisa con fuentes sobre una campaña o un candidato que no gobierna. Hay seis, de los dos lados.
  - **M, mixta** (no cuenta): elogio y reparo de peso parecido en la misma pieza.
  - **No es voz de la casa** (no cuenta, se declara):
    - **COM:** comunicado o informe oficial reescrito, con la nota «* Con información de…».
    - **CAMP:** texto de campaña («* Con información suministrada por la Campaña de…»).
    - **FIRM:** pieza que lleva otra firma en el cuerpo («Texto escrito por: …»).
    - **REIMP:** reimpresión de otro medio.
    - **OP:** categoría Opinión, con el aviso de que «no compromete el pensamiento ni la opinión de Las2Orillas».
  - **INT:** internacional (Venezuela, Irán, Haití…). **Fuera**, igual que en los barridos de El Informador y El Diario (Pereira).
  - **X:** sin postura en el eje (farándula, sucesos, cultura).
  - **N:** descriptiva, atribuida o informativa.

---

## 2. Piezas que cuentan

### 2.1 Antes del cambio: 2025-10-10 → 2026-08-06 (gobierna Petro)

| # | Fecha | Título (enlace) | Clase | Revisor | Fragmento o motivo |
|---|---|---|---|---|---|
| 1 | 2025-10-27 | [La batalla más grande que ha ganado Iván Cepeda no fue la de este domingo sino cuando derroto el cáncer](https://www.las2orillas.co/la-batalla-mas-grande-que-ha-ganado-ivan-cepeda-no-fue-la-de-este-domingo-sino-cuando-derroto-el-cancer/) | I (plena) | FI1 | Cepeda y el cáncer: «se convirtió en símbolo de resistencia institucional»; «la historia de un hombre que resistió donde otros se habrían rendido» |
| 2 | 2025-10-28 | [Dos mujeres, los pilares en la vida de Iván Cepeda](https://www.las2orillas.co/dos-mujeres-los-pilares-en-la-vida-de-ivan-cepeda/) | I (leve) | FI2 | Dos mujeres de Cepeda: perfil cálido («los bastiones de su firmeza») |
| 3 | 2025-11-05 | ["Petro necesita tener un motivo para que alguien me mate. Ya mataron a Miguel Uribe"](https://www.las2orillas.co/petro-necesita-tener-un-motivo-para-que-alguien-me-mate-ya-mataron-a-miguel-uribe/) | D (leve) | — | entrevista a Vicky Dávila: entradilla elogiosa («Sin miedo publicó denuncias») |
| 4 | 2025-11-16 | [La frenada de Petro a Temu y Shein que ayudará a los confeccionistas colombianos](https://www.las2orillas.co/la-frenada-de-petro-a-temu-y-shein-que-ayudara-a-los-confeccionistas-colombianos/) | I (leve) | FI3 | Temu y Shein: título y entrada a favor de la medida del gobierno de turno; el cuerpo recoge el reparo del sector hilandero |
| 5 | 2025-12-31 | [Petro puso a Colombia en el top 5 de los países de la región con mayor salario mínimo](https://www.las2orillas.co/petro-puso-a-colombia-en-el-top-5-de-los-paises-de-la-region-con-mayor-salario-minimo/) | I (leve) | — | «Petro puso a Colombia en el top 5 de los países de la región con mayor salario mínimo»: encuadre celebratorio de medida del gobierno de turno |
| 6 | 2026-01-10 | [Petro ordena levantar los peajes en el Eje Cafetero y poner fin a la concesión Autopistas del Café](https://www.las2orillas.co/petro-ordena-levantar-los-peajes-en-el-eje-cafetero-y-poner-fin-a-la-concesion-autopistas-del-cafe/) | I (leve) | — | peajes Eje Cafetero: «noticia largamente esperada», «un respiro económico» |
| 7 | 2026-01-10 | [Dos mujeres le dan la fuerza a Iván Cepeda, el sucesor de Petro que no la tiene fácil con Abelardo de la Espriella](https://www.las2orillas.co/dos-mujeres-le-dan-la-fuerza-a-ivan-cepeda-el-sucesor-de-petro-que-no-la-tiene-facil-con-abelardo-de-la-espriella/) | I (leve) | FI4 | Dos mujeres de Cepeda (2): reescritura del perfil del 28-10, cálido |
| 8 | 2026-01-25 | [La senadora y candidata del CD Paloma Valencia logró lo que Petro no pudo: tumbar al director de la Unidad de Víctimas](https://www.las2orillas.co/la-senadora-y-candidata-del-cd-paloma-valencia-logro-lo-que-petro-no-pudo-tumbar-al-director-de-la-unidad-de-victimas/) | D (leve) | — | «Paloma Valencia logró lo que Petro no pudo» |
| 9 | 2026-01-28 | [Álvaro Uribe, el único sobreviviente como político activo de los 15 fundadores de su partido Centro  Democrático](https://www.las2orillas.co/alvaro-uribe-el-unico-sobreviviente-como-politico-activo-de-los-15-fundadores-de-su-partido-centro-democratico/) | D (leve) | — | Uribe: «Un dirigente político innato, con una vocación de poder que le da la fuerza parar no bajar la guardia ni en los momentos de mayor adversidad» (sic) |
| 10 | 2026-01-30 | [La joven monteriana, esposa de Abelardo de la Espriella, a quien la vida le dio un vuelco total](https://www.las2orillas.co/la-joven-monteriana-esposa-de-abelardo-de-la-espriella-a-quien-la-vida-le-dio-un-vuelco-total/) | D (leve) | FD2 | esposa de De la Espriella: perfil cálido («firme y silenciosa»; «con sensatez aconseja») |
| 11 | 2026-03-20 | [Las cuentas de las elecciones no le cuadran a Petro y le pidió a la fiscal Luz Adriana Camargo que intervenga](https://www.las2orillas.co/las-cuentas-de-las-elecciones-no-le-cuadran-a-petro-y-le-pidio-a-la-fiscal-luz-adriana-camargo-que-intervenga/) | I (leve) | — | «Las cuentas de las elecciones no le cuadran a Petro»: análisis propio que respalda la duda del presidente frente a la Registraduría («esa cifra no responde la pregunta que realmente importa») |
| 12 | 2026-04-08 | [Quién es Sandra Muñoz, la dama de hierro del MinTrabajo que le puso 'tatequieto' a Caracol y RTVC por casos de acoso](https://www.las2orillas.co/quien-es-sandra-munoz-la-dama-de-hierro-del-mintrabajo-que-le-puso-tatequieto-a-caracol-y-rtvc-por-casos-de-acoso/) | I (leve) | — | viceministra «la dama de hierro del MinTrabajo» (perfil elogioso de funcionaria del gobierno de turno) |
| 13 | 2026-06-21 | [“Somos la mitad de Colombia” y no vamos a dejar enterrar nuestras conquistas sociales y de derechos”: Cepeda](https://www.las2orillas.co/somos-la-mitad-de-colombia-y-no-vamos-a-dejar-enterrar-nuestras-conquistas-sociales-y-de-derechos-cepeda/) | I (leve) | — | Cepeda tras la derrota: «con la serenidad de un ganador vocero de 12.7 millones» |
| 14 | 2026-06-22 | [Así se construyó la estrategia del tigre, una marca más allá del propio Abelardo de la Espriella](https://www.las2orillas.co/asi-se-construyo-la-estrategia-del-tigre-una-marca-mas-alla-del-propio-abelardo-de-la-espriella/) | D (leve) | — | estrategia del tigre: «un movimiento que toco el espíritu nacional» (sic) |


**Desglose de las 14 piezas anteriores al cambio:**
- **9 hacia la izquierda.** Cuatro elogian al candidato Cepeda: dos perfiles familiares casi idénticos, la pieza del cáncer (la única plena) y su discurso de derrota. Las otras cinco tratan bien medidas del gobierno de turno: Temu y Shein, el salario mínimo, los peajes, una viceministra y la duda del presidente sobre el preconteo.
- **5 hacia la derecha.** Todas tratan bien a figuras de derecha que no gobiernan: Vicky Dávila, Paloma Valencia, Uribe, la esposa de De la Espriella y la estrategia de su campaña.

### 2.2 Después del cambio: 2026-08-07 → 2026-10-10 (gobierna De la Espriella)

| # | Fecha | Título (enlace) | Clase | Revisor | Fragmento o motivo |
|---|---|---|---|---|---|
| 1 | 2026-08-14 | [El embajador de Suecia y otros cuatro quisieron atornillarse al cargo y El Tigre los declaro insubsistentes](https://www.las2orillas.co/el-embajador-de-suecia-y-otros-cuatro-quisieron-atornillarse-al-cargo-y-el-tigre-los-declaro-insubsistentes/) | D (leve) | — | embajadores que «quisieron atornillarse» y «El Tigre los declaro insubsistentes» (sic) |
| 2 | 2026-08-29 | [Jalón de orejas del presidente a Nueva EPS logra que un niño de siete años reciba la atención esperada durante un año](https://www.las2orillas.co/jalon-de-orejas-del-presidente-a-nueva-eps-logra-que-un-nino-de-siete-anos-reciba-la-atencion-esperada-durante-un-ano/) | D (leve) | — | «Jalón de orejas del presidente a Nueva EPS logra que un niño de siete años reciba la atención esperada durante un año» |
| 3 | 2026-08-31 | [La senadora petrista que se enoja y arma show porque a Gustavo Petro le dicen expresidente](https://www.las2orillas.co/la-senadora-petrista-que-se-enoja-y-arma-show-porque-a-gustavo-petro-le-dicen-expresidente/) | D (leve) | — | «La senadora petrista que se enoja y arma show» (burla a la oposición de izquierda) |
| 4 | 2026-09-12 | [De la Espriella buscó que el reemplazo de Juliana Guerrero en la U del Cesar fuera el polo opuesto](https://www.las2orillas.co/de-la-espriella-busco-que-el-reemplazo-de-juliana-guerrero-en-la-u-del-cesar-fuera-el-polo-opuesto/) | D (leve) | — | reemplazo de Juliana Guerrero «el polo opuesto» |
| 5 | 2026-09-12 | [Las 2 fundaciones a las que Abelardo de la Espriella les va entregar su primer salario, 52 millones](https://www.las2orillas.co/las-2-fundaciones-a-las-que-abelardo-de-la-espriella-les-va-entregar-su-primer-salario-52-millones/) | D (leve) | FD7 | salario donado: contraste con Gustavo Bolívar («se cuestionó el destino de las donaciones») |
| 6 | 2026-09-19 | [La mano dura de De la Espriella con 120 presos para hacerle la guerra a la extorsión en Buenaventura](https://www.las2orillas.co/la-mano-dura-de-de-la-espriella-con-120-presos-para-hacerle-la-guerra-a-la-extorsion-en-buenaventura/) | D (leve) | FD9 | «La mano dura de De la Espriella»: reproduce el trino presidencial sin contraste |
| 7 | 2026-09-21 | [Adiós a los delincuentes de cuello blanco en cárceles de privilegio: 12 políticos ya fueron trasladados](https://www.las2orillas.co/adios-a-los-delincuentes-de-cuello-blanco-en-carceles-de-privilegio-12-politicos-ya-fueron-trasladados/) | D (leve) | FD10 | «Adiós a los delincuentes de cuello blanco en cárceles de privilegio»; matiza («impuestas por el gobierno, no por jueces») |
| 8 | 2026-10-01 | [La Casa Gómez, influyente y respaldo de Abelardo De la Espriella, pone ahora alcalde ad hoc para Cali](https://www.las2orillas.co/la-casa-gomez-influyente-y-respaldo-de-abelardo-de-la-espriella-pone-ahora-alcalde-ad-hoc-para-cali/) | D (leve) | — | alcalde ad hoc: «La oposición podría quejarse de nepotismo, pero desde el punto de vista jurídico su designación cumple» |
| 9 | 2026-10-10 | [La promesa cumplida de De la Espriella reabriendo embajada en Jerusalén a donde llega una Gilinski](https://www.las2orillas.co/la-promesa-cumplida-de-de-la-espriella-reabriendo-embajada-en-jerusalen-a-donde-llega-una-gilinski/) | D (leve) | FD12 | «La promesa cumplida»: título evaluativo; cuerpo descriptivo con el contexto internacional en contra |


**Las 9 tratan bien al gobierno de turno**, y todas son leves: la postura está en el título o en un adjetivo. En la misma ventana hay **7 piezas que lo fiscalizan** (§4). **Hacia la izquierda no hay ninguna** en la voz de la casa después del 07-08. Las críticas al Gobierno De la Espriella en clave de izquierda que publica el sitio van firmadas por terceros (Nota Ciudadana, Opinión) y no cuentan.

### 2.3 Piezas que el revisor contó y aquí no cuentan

Las 19 se leyeron enteras.

| Revisor | Pieza | Aquí | Por qué |
|---|---|---|---|
| FD1 | [Machado, Nobel](https://www.las2orillas.co/la-valiente-lucha-contra-el-regimen-chavista-que-le-dio-a-maria-corina-machado-el-nobel-de-paz/) (2025-10-10) | INT | Internacional (Venezuela). Fuera, como en los barridos anteriores |
| FI5 | [Estratega de Paloma](https://www.las2orillas.co/quien-es-el-estratega-de-paloma-valencia-senalado-de-ser-un-experto-desinformando-en-redes/) (2026-05-23) | I (inv.) | Pesquisa con fuente (Reporteros de Investigación) sobre una campaña que no gobierna. Su simétrica, sobre la UNP y la campaña de Cepeda (22-04), tampoco cuenta |
| FI6 | [Logros de MinSalud](https://www.las2orillas.co/mas-de-11-billones-invertidos-desde-2022-entre-las-cifras-que-dejo-la-gestion-del-gobierno-petro-en-la-salud-colombiana/) (2026-06-04) | COM | Cierra con «* Con información del Ministerio de Salud y Protección Social». Es un comunicado reescrito |
| FI7 | [El camino de Cepeda](https://www.las2orillas.co/el-camino-de-ivan-cepeda-a-una-presidencia-que-se-le-escapo-por-250-mil-votos/) (2026-06-22) | N | Crónica de campaña. El único elogio es un adjetivo («aguerrido senador»), y la misma pieza lo llama «candidato del continuismo» |
| FD3 | [«El antipolítico que… ganó»](https://www.las2orillas.co/abelardo-de-la-espriella-el-antipolitico-que-se-conecto-con-el-pais-y-gano/) (2026-05-31) | M | El elogio («fenómeno electoral») va con el reparo: «cuestionado por muchos de los casos que ha defendido», «su gran aliado es la emocionalidad más que las ideas» |
| FD4 | [«Ha despertado confianza internacional»](https://www.las2orillas.co/el-triunfo-de-abelardo-de-la-espriella-y-jose-manuel-restrepo-en-primera-vuelta-han-despertado-confianza-internacional/) (2026-06-16) | CAMP | Cierra con «* Con información suministrada por la Campaña de Abelardo de la Espriella». **Es texto de campaña con la firma de la casa** (§5) |
| FD5 | [El camino de Abelardo](https://www.las2orillas.co/el-camino-de-abelardo-de-la-espriella-para-lograr-la-presidencia-de-colombia-en-6-meses/) (2026-06-21) | M | «sibaritismo», «obsesión», «cuestionados clientes» junto a «defensor de victimas» (sic) y «ola ganadora» |
| FD6 | [Primera banda que se entrega](https://www.las2orillas.co/la-primera-banda-criminal-que-se-entregara-ante-el-ultimatum-de-de-la-espriella-la-cual-tiene-azotada-a-barranquilla/) (2026-07-08) | N | Crónica policial. El revisor la clasificó solo por el título, que es el único encuadre; el cuerpo no celebra |
| FD8 | [«La frágil oposición»](https://www.las2orillas.co/el-pacto-liderado-por-cepeda-mais-por-la-investigada-peralta-y-en-marcha-por-cristo-son-la-fragil-oposicion/) (2026-09-13) | N | Análisis de bancadas. «La investigada Peralta» es un dato. Cierra con un reparo al gobierno: «sin que se sepa aún el costo de este apoyo» |
| FD11 | [Drones de EE. UU.](https://www.las2orillas.co/el-respaldo-de-ee-uu-a-de-la-espriella-ya-empieza-a-sentirse-con-poderosos-drones-militares-para-rastrear-narcos/) (2026-10-07) | N | Descriptiva. Solo el título encuadra |

**Coinciden con el revisor** 9 de sus 19: FI1 a FI4 (aquí FI1 es plena y las otras tres son leves), FD2, FD7, FD9, FD10 y FD12 (todas leves). **Las 14 restantes que cuentan aquí no las contó**: 9 son de fuera de Poder o de antes del cambio, que él no barrió con el mismo criterio. Su suma también falla. Escribe «25 piezas con postura», pero su lista tiene 19 (7 + 6 + 6). Y dice «13 de 25» clasificadas solo por el título, cuando las marcadas «[título]» son 10.

---

## 3. Recuento

| | Izquierda (plena + leve) | Derecha (plena + leve) | F, solo fiscaliza a quien manda (no suma) |
|---|---|---|---|
| Antes del 07-08-2026 (300 días) | **9** (1 + 8) | **5** (0 + 5) | 53 (al Gobierno Petro) |
| Desde el 07-08-2026 (65 días) | **0** | **9** (0 + 9) | 7 (al Gobierno De la Espriella) |
| **Total** | **9** | **14** | 60 |

**Desglose por destinatario:**

| | Hacia la izquierda | Hacia la derecha |
|---|---|---|
| Candidatos y figuras que no gobiernan | 4 (Cepeda) | 5 (Vicky Dávila, Paloma Valencia, Uribe, la esposa de De la Espriella, la campaña del Tigre) |
| Medidas del gobierno de turno | 5 (Gobierno Petro, mientras gobierna) | 9 (Gobierno De la Espriella, desde el 07-08) |

**Mínimos de la regla:**
- **≥10 piezas con postura:** 23. Se cumple.
- **≥3 a cada lado del 07-08 en la misma dirección:**
  - Hacia la derecha: 5 antes y 9 después. Se cumple.
  - Hacia la izquierda: 9 antes y **0 después**. No se cumple.
- **≥3:1 en la misma dirección:** 14 a 9, es decir, **1,6 a 1 hacia la derecha**. No se cumple en ninguna dirección.

**No hay nivel 2 por la regla del 2026-10-09 en ningún sentido.** La única asimetría que aparece, débil, va **en sentido contrario al valor vigente**.

---

## 4. Lo que contradice cada dirección, y cuánto pesa

- **Contra una lectura a la izquierda (la del −0,35):**
  - En 12 meses hay **una sola pieza plena** a la izquierda: el perfil de Cepeda del 27-10-2025 («se convirtió en símbolo de resistencia institucional»).
  - Después del 07-08 no hay ninguna.
  - Antes del cambio, la casa fiscalizó al Gobierno Petro en 53 piezas: Lista Clinton, UNGRD, Roa y Ecopetrol, Juliana Guerrero, Alcocer, Gripen, La Rebaja, la constituyente…
  - Y llegó a criticar la misma medida que había celebrado: los aranceles a los hilos, presentados el 16-11-2025 como la medida «que ayudará a los confeccionistas colombianos», y el cierre de Fabricato del 29-01-2026.
- **Contra una lectura a la derecha:**
  - Las 14 son leves.
  - Las 9 posteriores caen en los dos primeros meses de un gobierno nuevo, sin un solo rótulo contra la izquierda en voz de la casa salvo la burla a una senadora (31-08).
  - Mientras tanto, la casa fiscaliza al Gobierno De la Espriella en 7 piezas: ministros endeudados, el círculo del presidente en la junta de Ecopetrol, Ordóñez, los abogados de su bufete en embajadas, el voto en la ONU, el director de la UNP («zurdos de mierda») y dos abogadas «sin experiencia en el sector público».
  - Antes del cambio también trató bien a Cepeda: 4 piezas, una plena.
- **Cuánto pesa la diferencia de ritmo.** Las piezas amables con el gobierno de turno pasan de 5 en 300 días (con Petro) a 9 en 65 días (con De la Espriella). La fiscalización baja de 53 en 300 días a 7 en 65. Es un indicio de **deferencia mayor al gobierno entrante en su luna de miel**. Con 65 días y piezas todas leves, no es un hecho de línea. **Se declara y se recuenta** (§10).

---

## 5. Comprobaciones y avisos de lectura

- **La firma de la casa no garantiza que la pieza sea voz de la casa.** Bajo las cuentas 457 y 2 se publican:
  - comunicados reescritos («* Con información del Ministerio de Salud…», «…de la Alcaldía de Cali»);
  - texto de campaña («* Con información suministrada por la Campaña de Abelardo de la Espriella», 16-06-2026);
  - texto de un gremio («*Con información suministrada por Asocaña», 11-05-2026);
  - y, **sin nota ninguna**, al menos 22 entregables pagados por la Registraduría: 15 del contrato de 500 M y los 7 del de 200 M (ver la resolución, objeción 2).

  Ninguno de esos entregables entra en este universo, porque sus títulos no nombran a ningún actor del eje y no están en Poder. Lo que no se puede descartar es que haya **otras piezas pagadas sin nota** dentro del universo. Este barrido excluye las que llevan nota, y no puede excluir las que no la llevan.
- **Piezas firmadas por terceros con la cuenta de la casa:**
  - «Texto escrito por: María García» (04-06-2026);
  - «Texto escrito por: Diego Arias» (07-07-2026);
  - una Nota Ciudadana firmada por un ciudadano (14-07-2026).

  No cuentan.
- **Una reimpresión:** «Los 12 Apóstoles» (05-06-2026) reproduce un artículo de Revista Raya de 2024.
- **Duplicado:** los dos perfiles de las mujeres de Cepeda (28-10-2025 y 10-01-2026) son el mismo texto reescrito. Cuentan como dos piezas porque se publicaron dos veces; sin el duplicado, el recuento sería 8 a 14.
- **Fuentes de Pares sin declarar el vínculo.** Dos piezas de la casa sobre candidatos cuestionados (07-03 y 08-03-2026) se basan en datos de la Fundación Paz y Reconciliación, que dirige León Valencia, fundador y asociado del medio. No lo dicen. Ver la objeción 4 en la resolución.

---

## 6. Excluidas con motivo (no son voz de la casa, son internacionales, investigan una candidatura o son mixtas)

| # | Fecha | Título (enlace) | Clase | Revisor | Fragmento o motivo |
|---|---|---|---|---|---|
| 1 | 2025-10-10 | [La valiente lucha contra el régimen chavista que le dio a María Corina Machado el Nobel de Paz](https://www.las2orillas.co/la-valiente-lucha-contra-el-regimen-chavista-que-le-dio-a-maria-corina-machado-el-nobel-de-paz/) | INT | FD1 | Machado Nobel: celebratoria, pero internacional (Venezuela); fuera, como en los barridos de El Informador y El Diario |
| 2 | 2025-11-08 | [El caso que despertó la pasión de Natalia París por Abelardo De La Espriella](https://www.las2orillas.co/el-caso-que-desperto-la-pasion-de-natalia-paris-por-abelardo-de-la-espriella/) | I | — | Natalia París / denuncia chuzadas De la Espriella (investiga candidato) |
| 3 | 2025-12-11 | [Así se escapó María Corina Machado de Venezuela y llegó a Oslo a recibir el Nobel de la Paz](https://www.las2orillas.co/asi-se-escapo-maria-corina-machado-de-venezuela-y-llego-a-oslo-a-recibir-el-nobel-de-la-paz/) | INT | — | Machado Oslo |
| 4 | 2025-12-29 | [Apoyo de la Cámara de Comercio de Villavicencio a Abelardo de la Espriella terminó en multa de la Supersociedades](https://www.las2orillas.co/apoyo-de-la-camara-de-comercio-de-villavicencio-a-abelardo-de-la-espriella-termino-en-multa-de-la-supersociedades/) | I | — | multa Cámara Comercio Villavicencio por apoyo a Abelardo |
| 5 | 2026-01-03 | [En otra operación militar, el gobierno de EE. UU. derrocó y detuvo al dictador Manuel Antonio Noriega hace 37 años](https://www.las2orillas.co/en-otra-operacion-militar-el-gobierno-de-ee-uu-derroco-y-detuvo-al-dictador-manuel-antonio-noriega-hace-37-anos/) | INT | — | Noriega |
| 6 | 2026-01-08 | [Dos Republicanos gringos empiezan a jugar en el caso Venezuela con  Maduro y Petro](https://www.las2orillas.co/dos-republicanos-gringos-empiezan-a-jugar-en-el-caso-venezuela-con-maduro-y-petro/) | INT | — | Republicanos Maduro |
| 7 | 2026-01-11 | [El negociazo de Abelardo de la Espriella con un edificio de apartamentos en Bogotá del que salió la plata de la campaña](https://www.las2orillas.co/el-negociazo-de-abelardo-de-la-espriella-con-un-edificio-de-apartamentos-en-bogota-del-que-salio-la-plata-de-la-campana/) | I | — | negociazo Abelardo edificio, financia campaña |
| 8 | 2026-01-15 | [¿Quién es el lobista de Delcy Rodríguez en Washington que busca romper el hielo con el gobierno Trump?](https://www.las2orillas.co/quien-es-el-lobista-de-delcy-rodriguez-en-washington-que-busca-romper-el-hielo-con-el-gobierno-trump/) | INT | — | lobista de Delcy |
| 9 | 2026-02-05 | [¿Qué ha pasado con los dirigentes más cercanos a María Corina Machado que fueron encarcelados en el Helicoide?](https://www.las2orillas.co/que-ha-pasado-con-los-dirigentes-mas-cercanos-a-maria-corina-machado-que-fueron-encarcelados-en-el-helicoide/) | INT | — | Helicoide |
| 10 | 2026-02-07 | [Cómo tres famosos españoles, un expresidente, el líder de un partido y un juez le sacaron millones al régimen de Maduro](https://www.las2orillas.co/como-tres-famosos-espanoles-un-expresidente-el-lider-de-un-partido-y-un-juez-le-sacaron-millones-al-regimen-de-maduro/) | INT | — | españoles y Maduro |
| 11 | 2026-02-11 | [El negociazo que montó Abelardo de la Espriella con su campaña: relojes costosos y esculturas de millones](https://www.las2orillas.co/el-negociazo-que-monto-abelardo-de-la-espriella-con-su-campana-relojes-costosos-y-esculturas-de-millones/) | I | — | relojes de la campaña de De la Espriella (tono irónico leve) |
| 12 | 2026-02-20 | [Con pedida de perdón pública los hermanos Rodríguez dejarán libres cientos de presos políticos en Venezuela](https://www.las2orillas.co/con-pedida-de-perdon-publica-los-hermanos-rodriguez-dejaran-libres-cientos-de-presos-politicos-en-venezuela/) | INT | — | presos políticos Venezuela |
| 13 | 2026-03-20 | [Con la descabezada de Padrino y la salida de 7 ministros nombrados por Maduro, Delcy toma las riendas de Venezuela](https://www.las2orillas.co/con-la-descabezada-de-padrino-y-la-salida-de-7-ministros-nombrados-por-maduro-delcy-toma-las-riendas-de-venezuela/) | INT | — | Delcy |
| 14 | 2026-04-22 | [El hijo de Augusto Rodríguez director de la UNP que sacude la campaña de Cepeda por supuestos apoyos desde el Gobierno](https://www.las2orillas.co/el-hijo-de-augusto-rodriguez-director-de-la-unp-que-sacude-la-campana-de-cepeda-por-supuestos-apoyos-desde-el-gobierno/) | I | — | UNP y campaña de Cepeda (investiga candidato de izquierda) |
| 15 | 2026-05-23 | [Quién es el estratega de Paloma Valencia señalado de ser un experto desinformando en redes](https://www.las2orillas.co/quien-es-el-estratega-de-paloma-valencia-senalado-de-ser-un-experto-desinformando-en-redes/) | I | FI5 | estratega de Paloma: investiga a la campaña de la derecha (desinformación en Honduras, con fuente); simétrico al de la UNP y la campaña de Cepeda |
| 16 | 2026-05-31 | [Abelardo de la Espriella, el antipolítico que se conectó con el país y ganó](https://www.las2orillas.co/abelardo-de-la-espriella-el-antipolitico-que-se-conecto-con-el-pais-y-gano/) | M | FD3 | «el antipolítico que se conectó con el país y ganó»: elogio («fenómeno electoral») y reparo («cuestionado por muchos de los casos», «su gran aliado es la emocionalidad más que las ideas») |
| 17 | 2026-06-04 | [Más de $11 billones invertidos desde 2022 entre las cifras que dejó la gestión del gobierno Petro en la salud colombiana](https://www.las2orillas.co/mas-de-11-billones-invertidos-desde-2022-entre-las-cifras-que-dejo-la-gestion-del-gobierno-petro-en-la-salud-colombiana/) | COM | FI6 | logros de MinSalud: «* Con información del Ministerio de Salud y Protección Social» |
| 18 | 2026-06-04 | [La cuestionada senadora que impulsa a Iván Cepeda en La Guajira](https://www.las2orillas.co/la-cuestionada-senadora-que-impulsa-a-ivan-cepeda-en-la-guajira/) | FIRM | — | «Texto escrito por: María García»: firmada por otra persona; no es voz de la casa |
| 19 | 2026-06-05 | [Quiénes eran “Los 12 Apóstoles”, el grupo paramilitar por el que condenaron a Santiago Uribe](https://www.las2orillas.co/quienes-eran-los-los-12-apostoles-el-grupo-paramilitar-por-el-que-condenaron-a-santiago-uribe/) | REIMP | — | Los 12 Apóstoles: reimpresión de un artículo de Revista Raya de 2024; no cuenta |
| 20 | 2026-06-16 | [El triunfo de Abelardo De La Espriella y José Manuel Restrepo en primera vuelta ha despertado confianza internacional](https://www.las2orillas.co/el-triunfo-de-abelardo-de-la-espriella-y-jose-manuel-restrepo-en-primera-vuelta-han-despertado-confianza-internacional/) | CAMP | FD4 | «ha despertado confianza internacional»: cierra con «* Con información suministrada por la Campaña de Abelardo de la Espriella»; texto de campaña bajo la firma de la casa |
| 21 | 2026-06-21 | [El camino de Abelardo De la Espriella para lograr la presidencia de Colombia en 6 meses](https://www.las2orillas.co/el-camino-de-abelardo-de-la-espriella-para-lograr-la-presidencia-de-colombia-en-6-meses/) | M | FD5 | el camino de Abelardo: «sibaritismo», «obsesión», «cuestionados clientes», y también «defensor de víctimas», «ola ganadora» |
| 22 | 2026-07-07 | [Los aciertos que tuvo la malograda 'Paz Total' de Gustavo Petro](https://www.las2orillas.co/los-aciertos-que-tuvo-la-malograda-paz-total-de-gustavo-petro/) | FIRM | — | «Texto escrito por: Diego Arias» (aciertos de la Paz Total) |
| 23 | 2026-07-14 | [El plan de seguridad de Abelardo de la Espriella despierta a los peores fantasmas de la violencia en Colombia](https://www.las2orillas.co/el-plan-de-seguridad-de-abelardo-de-la-espriella-despierta-a-los-peores-fantasmas-de-la-violencia-en-colombia/) | FIRM | — | Nota Ciudadana firmada por un ciudadano, contra el plan de seguridad (no es voz de la casa) |
| 24 | 2026-07-18 | [Los primeros símbolos del poder revelan cómo gobernará Abelardo de la Espriella](https://www.las2orillas.co/los-primeros-simbolos-del-poder-revelan-como-gobernara-abelardo-de-la-espriella/) | OP | — | categoría Opinión con aviso de que no compromete a Las2Orillas (no es voz de la casa) |
| 25 | 2026-07-24 | [Más de 21 mil víctimas recibieron indemnizaciones judiciales por más de 806 mil millones durante el gobierno Petro](https://www.las2orillas.co/mas-de-21-mil-victimas-recibieron-indemnizaciones-por-mas-de-806-mil-millones-durante-el-gobierno-petro/) | COM | — | balance de la Unidad para las Víctimas (comunicado reescrito) |
| 26 | 2026-08-06 | [Los millonarios hallazgos que destapó la Contraloría en contratos de Defensa y que tienen un $1 billón en el limbo](https://www.las2orillas.co/los-millonarios-hallazgos-que-destapo-la-contraloria-en-contratos-de-defensa-y-que-tienen-un-1-billon-en-el-limbo/) | COM | — | hallazgos de la Contraloría en Defensa (reescritura de informe) |
| 27 | 2026-08-09 | [Las irregularidades por más de $233 mil millones que dejó la lupa de la Contraloría sobre el sector Trabajo](https://www.las2orillas.co/las-irregularidades-por-mas-de-233-mil-millones-que-dejo-la-lupa-de-la-contraloria-sobre-el-sector-trabajo/) | COM | — | Contraloría, sector Trabajo (reescritura) |
| 28 | 2026-08-10 | [Los casi $57 mil millones en irregularidades que encontró la Contraloría al revisar las cuentas ambientales de Colombia](https://www.las2orillas.co/los-casi-57-mil-millones-en-irregularidades-que-encontro-la-contraloria-al-revisar-las-cuentas-ambientales-de-colombia/) | COM | — | Contraloría, ambiente (reescritura) |
| 29 | 2026-09-21 | [Qué les espera a los 17 mercenarios colombianos acusados del crimen del presidente Moïse que se llevaron para EE.UU.](https://www.las2orillas.co/que-les-espera-a-los-17-mercenarios-colombianos-acusados-del-crimen-del-presidente-moise-que-se-llevaron-para-ee-uu/) | INT | — | mercenarios Moïse |


---

## 7. Solo fiscaliza a quien manda (F): se declara y no suma

53 antes del cambio (Gobierno Petro) y 7 después (Gobierno De la Espriella).

| # | Fecha | Título (enlace) | Clase | Revisor | Fragmento o motivo |
|---|---|---|---|---|---|
| 1 | 2025-10-26 | [Estocolmo, la última aparición de Verónica Alcocer como Primera dama, el país que convirtió en su destino preferido](https://www.las2orillas.co/estocolmo-la-ultima-aparicion-de-veronica-alcocer-como-primera-dama-el-pais-que-convirtio-en-su-destino-preferido/) | F | — | Alcocer viajes (fiscaliza) |
| 2 | 2025-10-27 | [Con recortes a la Rama Judicial el Gobierno sigue siendo juez único de la reforma agraria](https://www.las2orillas.co/con-recortes-a-la-rama-judicial-el-gobierno-sigue-siendo-juez-unico-de-la-reforma-agraria/) | F | — | recortes a la Rama Judicial |
| 3 | 2025-10-30 | [Los dueños de las concesiones se fueron contra el Estado y el presidente de la ANI carga con demandas 10.5 billones](https://www.las2orillas.co/el-presidente-de-la-ani-javier-torres-enfrenta-demandas-de-los-duenos-de-las-concesiones-por-10-5-billones/) | F | — | ANI demandas |
| 4 | 2025-11-04 | [La compañera de alias Calarcá quien está negociando con el gobierno Petro es la reina de la extorsión en Caquetá](https://www.las2orillas.co/la-companera-de-alias-calarca-quien-esta-negociando-con-el-gobierno-petro-es-la-reina-de-la-extorsion-en-caqueta/) | F | — | Calarcá negociación |
| 5 | 2025-11-05 | [La USO se le para a Petro y a minminas  para que Ecopetrol no frene el fracking en EEUU](https://www.las2orillas.co/la-uso-se-le-para-a-petro-y-a-minminas-para-que-ecopetrol-no-frene-el-fracking-en-eeuu/) | F | — | USO vs Petro |
| 6 | 2025-11-09 | [El lío de nunca acabar, la Fundación de Educación Superior San José anula el título de Juliana Guerrero](https://www.las2orillas.co/el-lio-de-nunca-acabar-la-fundacion-de-educacion-superior-san-jose-anula-el-titulo-de-juliana-guerrero/) | F | — | Juliana Guerrero |
| 7 | 2025-11-10 | [El retrato de la embajadora de Colombia en Alemania pagado por el Estado, que colgó en su despacho en Berlín](https://www.las2orillas.co/el-retrato-de-la-embajadora-de-colombia-en-alemania-pagado-por-el-estado-que-colgo-en-su-despacho-en-berlin/) | F | — | retrato embajadora |
| 8 | 2025-11-11 | [Esta es la valiosa casa en el corazón de Londres donde Laura Sarabia vivirá como embajadora de Colombia](https://www.las2orillas.co/esta-es-la-valiosa-casa-en-el-corazon-de-londres-donde-laura-sarabia-vivira-como-embajadora-de-colombia/) | F | — | Sarabia casa Londres |
| 9 | 2025-11-13 | [La maratón de contratos por $ 2.1 billones que firmó el gobierno Petro en 7 días para evitar la Ley de Garantías.](https://www.las2orillas.co/la-maraton-de-contratos-por-2-1-billones-que-firmo-el-gobierno-petro-en-7-dias-para-evitar-la-ley-de-garantias/) | F | — | maratón contratos |
| 10 | 2025-11-14 | [El misterio detrás del asesinato del creador de la cripto Daily Cop y dueño del avión en el que Petro hizo campaña](https://www.las2orillas.co/el-misterio-detras-del-asesinato-del-creador-de-la-cripto-daily-cop-y-dueno-del-avion-en-el-que-petro-hizo-campana/) | F | — | Daily Cop avión campaña Petro |
| 11 | 2025-11-18 | [En qué gasta Gustavo Petro los más de $600 millones que se gana al año como Presidente](https://www.las2orillas.co/en-que-gasta-gustavo-petro-los-mas-de-600-millones-que-se-gana-al-ano-como-presidente/) | F | — | gastos personales de Petro |
| 12 | 2025-11-21 | [El proyecto secreto del gobierno de convertir la inteligencia financiera en instrumento de lucha política](https://www.las2orillas.co/el-proyecto-secreto-del-gobierno-de-convertir-la-inteligencia-financiera-en-instrumento-de-lucha-politica/) | F | — | UIAF proyecto secreto |
| 13 | 2025-11-22 | [La Fiscalía sueca entra a jugar en el caso de 18 aviones Gripen por los que pagó el gobierno Petro $ 16. 5 billones](https://www.las2orillas.co/la-fiscalia-sueca-entra-a-jugar-en-el-caso-de-18-aviones-gripen-por-los-que-pago-el-gobierno-petro-16-5-billones/) | F | — | Gripen Fiscalía sueca |
| 14 | 2025-11-24 | [Dos pesados generales que Petro vinculó al gobierno eran infiltrados de Calarcá y sus disidencias](https://www.las2orillas.co/dos-pesados-generales-que-petro-vinculo-al-gobierno-eran-infiltrados-de-calarca-y-sus-disidencias/) | F | — | generales infiltrados |
| 15 | 2025-11-25 | [Los 2 experimentados fiscales escogidos por la Fiscal Camargo para investigar la infiltración de Calarca en el gobierno](https://www.las2orillas.co/los-2-experimentados-fiscales-escogidos-por-la-fiscal-camargo-para-investigar-la-infiltracion-de-calarca-en-el-gobierno/) | F | — | fiscales Calarcá |
| 16 | 2025-11-25 | [El empresario catalán que acompaña a Verónica Alcocer en Europa, es cercano al gobierno de Petro](https://www.las2orillas.co/el-es-el-empresario-catalan-que-acompana-a-veronica-alcocer-en-europa-es-cercano-al-gobierno-de-petro/) | F | — | Grau |
| 17 | 2025-11-26 | [¿Por qué dos de los ex ministros más cercanos a Petro están a las puertas de la cárcel?](https://www.las2orillas.co/por-que-dos-de-los-ex-ministros-mas-cercanos-a-petro-estan-a-las-puertas-de-la-carcel/) | F | — | exministros cárcel |
| 18 | 2025-11-27 | [Ricardo Roa el gran paganini con la drástica sanción del CNE por violación de topes de la campaña de Petro](https://www.las2orillas.co/ricardo-roa-el-gran-paganini-con-la-drastica-sancion-del-cne-por-violacion-de-topes-de-la-campana-de-petro/) | F | — | Roa topes campaña |
| 19 | 2025-11-28 | [Las alternativas del Valle para no quedarse sin el tren de cercanías para responder a la cachetada del gobierno Petro](https://www.las2orillas.co/las-alternativas-del-valle-para-no-quedarse-sin-el-tren-de-cercanias-para-responder-a-la-cachetada-del-gobierno-petro/) | F | — | tren Valle, «cachetada del gobierno Petro» |
| 20 | 2025-12-04 | [La poderosa familia sueca dueña del periódico Expressen que le sigue los pasos a Verónica Alcocer en Estocolmo](https://www.las2orillas.co/la-poderosa-familia-sueca-duena-del-periodico-expressen-que-le-sigue-los-pasos-a-veronica-alcocer-en-estocolmo/) | F | — | Expressen / Alcocer |
| 21 | 2025-12-10 | [Las fiestas de los Petro en España con Manuel Grau que lo volvió íntimo de Verónica Alcocer y contratista del Estado](https://www.las2orillas.co/las-fiestas-de-los-petro-en-espana-con-manuel-grau-que-lo-volvieron-la-sombra-de-veronica-alcocer-en-europa/) | F | — | fiestas Petro España / Grau |
| 22 | 2025-12-18 | [Quien es la magistrada que mando a la cárcel a dos de los ministros más cercanos de Petro](https://www.las2orillas.co/quien-es-la-magistrada-que-mando-a-la-carcel-a-dos-de-los-ministros-mas-cercanos-de-petro/) | F | — | magistrada UNGRD |
| 23 | 2025-12-19 | [La revancha del español dueño de la EPS Sanitas contra Petro: lo puso a rectificar](https://www.las2orillas.co/la-revancha-del-espanol-dueno-de-la-eps-sanitas-contra-petro-lo-puso-a-rectificar/) | F | — | Sanitas obliga a Petro a rectificar |
| 24 | 2025-12-26 | [Los influyentes directivos de Colfuturo que no convencieron a Petro de las bondades de un modelo que funcionó 25 años](https://www.las2orillas.co/los-influyentes-directivos-de-colfuturo-que-no-convencieron-a-petro-de-las-bondades-de-un-modelo-que-funciono-25-anos/) | F | — | Colfuturo |
| 25 | 2025-12-26 | [Donde le compró Colpensiones la gran camioneta de $ 404 millones al presidente de la entidad Jaime Dussan](https://www.las2orillas.co/donde-le-compro-colpensiones-la-gran-camioneta-de-404-millones-al-presidente-de-la-entidad-jaime-dussan/) | F | — | Dussán camioneta |
| 26 | 2026-01-13 | [El fiasco de la intervención de Drogas La Rebaja por parte del gobierno Petro queterminó de quebrarlas](https://www.las2orillas.co/el-fiasco-de-la-intervencion-de-drogas-la-rebaja-por-parte-del-gobierno-petro-quetermino-de-quebrarlas/) | F | — | fiasco La Rebaja |
| 27 | 2026-01-21 | [El imperio educativo de Francisco Pareja, el dueño de U. San José que le vendió el título a Juliana Guerrero](https://www.las2orillas.co/el-imperio-educativo-de-francisco-pareja-el-dueno-de-u-san-jose-que-le-vendio-el-titulo-a-juliana-guerrero/) | F | — | Pareja / Juliana Guerrero |
| 28 | 2026-01-22 | [La revancha de Petro contra Daniel Noboa podría terminar pagándola los ecuatorianos con apagones, como ocurrió antes](https://www.las2orillas.co/la-revancha-de-petro-contra-daniel-noboa-podria-terminar-pagandola-los-ecuatorianos-con-apagones-como-ocurrio-antes/) | F | — | revancha de Petro contra Noboa |
| 29 | 2026-01-27 | [La ruta de Nhora Mondragón que la llevó al Dapre de la mano de Juliana Guerrero y Armando Benedetti](https://www.las2orillas.co/la-ruta-de-nhora-mondragon-que-la-llevo-al-dapre-de-la-mano-de-juliana-guerrero-y-con-armando-benedetti-como-padrino/) | F | — | Nhora Mondragón |
| 30 | 2026-01-29 | [Fabricato no aguantó la competencia con los hilos y fibras extranjeras a los que Petro les quitó el arancel](https://www.las2orillas.co/fabricato-no-aguanto-la-competencia-con-los-hilos-y-fibras-extranjeras-a-los-que-petro-les-quito-el-arancel/) | F | — | Fabricato: la medida de aranceles que celebró el 16-11 la critica ahora |
| 31 | 2026-02-20 | [El recorte de $600 mil millones al Canal del Dique con el que Petro expone al país a gigante demanda](https://www.las2orillas.co/el-recorte-de-600-mil-millones-al-canal-del-dique-con-el-que-petro-expone-al-pais-a-gigante-demanda/) | F | — | Canal del Dique |
| 32 | 2026-02-23 | [Quién es el mexicano a quien Petro le compra el glifosato que tanto criticó en el que se ha gastado $3 mil millones](https://www.las2orillas.co/quien-es-el-mexicano-a-quien-petro-le-compra-el-glifosato-que-tanto-critico-en-el-que-se-ha-gastado-3-mil-millones/) | F | — | glifosato |
| 33 | 2026-02-26 | [Apoyado por un obediente gabinete, Petro le dio un empujón a la Asamblea Constituyente](https://www.las2orillas.co/apoyado-por-un-obediente-gabinete-petro-le-dio-un-empujon-a-la-asamblea-constituyente/) | F | — | «obediente gabinete», constituyente |
| 34 | 2026-02-27 | [Al banquillo la junta directiva de ISA que nombró de manera irregular a Jorge Carrillo presidente de la compañía ](https://www.las2orillas.co/al-banquillo-la-junta-directiva-de-isa-que-nombro-de-manera-irregular-a-jorge-carrillo-presidente-de-la-compania/) | F | — | ISA |
| 35 | 2026-03-05 | [Los escándalos de Cuba Gooding Jr., la estrella de la película sobre el almirante Padilla que financió el gobierno Petro](https://www.las2orillas.co/los-escandalos-de-cuba-gooding-jr-la-estrella-de-la-pelicula-sobre-el-almirante-padilla-que-financio-el-gobierno-petro/) | F | — | película Padilla financiada por el gobierno |
| 36 | 2026-03-19 | [El desplome de Ecopetrol y la disparada del Grupo Éxito de los Callejas y Nutresa de Gilinski en ganancias](https://www.las2orillas.co/el-desplome-de-ecopetrol-y-la-disparada-del-grupo-exito-de-los-callejas-y-nutresa-de-gilinski-en-ganancias/) | F | — | Ecopetrol debacle, Roa |
| 37 | 2026-03-25 | [El mismo abogado que defendió a Eduardo Montealegre de Álvaro Uribe Vélez ahora esta con el presidente de Ecopetrol](https://www.las2orillas.co/el-mismo-abogado-que-defendio-a-eduardo-montealegre-de-alvaro-uribe-velez-ahora-esta-con-el-presidente-de-ecopetrol/) | F | — | abogado de Roa |
| 38 | 2026-03-26 | [Los 12 helicópteros que EE.UU. le regaló a Colombia y que Petro no calificó de chatarras por haberlos recibido él](https://www.las2orillas.co/los-12-helicopteros-que-ee-uu-le-regalo-a-colombia-y-que-petro-no-califico-de-chatarras-por-haberlos-recibido-el/) | F | — | helicópteros, «Petro no calificó de chatarras por haberlos recibido él» |
| 39 | 2026-04-07 | [En contravía de Petro, sus alfiles en la junta de Ecopetrol apoyaron el retiro de Roa hasta las elecciones](https://www.las2orillas.co/en-contravia-de-petro-sus-alfiles-en-la-junta-de-ecopetrol-apoyaron-el-retiro-de-roa-hasta-las-elecciones/) | F | — | Roa / junta Ecopetrol |
| 40 | 2026-04-08 | [El contratista que tiene que dejar con agua el colegio-universidad del Catatumbo que Petro inauguró sin servicios](https://www.las2orillas.co/el-contratista-que-tiene-que-dejar-con-agua-el-colegio-universidad-del-catatumbo-que-petro-inauguro-sin-servicios/) | F | — | colegio del Catatumbo inaugurado sin servicios |
| 41 | 2026-04-21 | [Cómo el Mindefensa Pedro Sánchez terminó con 2 viceministras inexpertas que llegaron a pagar favores políticos](https://www.las2orillas.co/como-el-mindefensa-pedro-sanchez-termino-con-2-viceministras-inexpertas-que-llegaron-a-pagar-favores-politicos/) | F | — | viceministras de Defensa |
| 42 | 2026-04-27 | [Duelo de titanes entre 3 pesados abogados involucrados en el negocio del apartamento 901 del expresidente de Ecopetrol](https://www.las2orillas.co/duelo-de-titanes-entre-3-pesados-abogados-involucrados-en-el-negocio-del-apartamento-901-del-expresidente-de-ecopetrol/) | F | — | apartamento de Roa |
| 43 | 2026-04-27 | [Con parrandón de cumpleaños en Valledupar Juliana Guerrero quiso bailarse las graves acusaciones de Angie Rodríguez](https://www.las2orillas.co/con-parrandon-de-cumpleanos-en-valledupar-juliana-guerrero-quiso-bailarse-las-graves-acusaciones-de-angie-rodriguez/) | F | — | Juliana Guerrero |
| 44 | 2026-04-29 | [La alta funcionaria que Petro mantiene atornillada en el cargo llevó a dos de los suyos a rendir cuentas en el Congreso](https://www.las2orillas.co/la-alta-funcionaria-que-petro-mantiene-atornillada-en-el-cargo-llevo-a-dos-de-los-suyos-a-rendir-cuentas-en-el-congreso/) | F | — | funcionaria «atornillada» |
| 45 | 2026-05-01 | [Gran favor de Petro a otra amiga de Verónica Alcocer: le entregó la Notaria 35](https://www.las2orillas.co/gran-favor-de-petro-a-otra-amiga-de-veronica-alcocer-le-entrego-la-notaria-35/) | F | — | Notaría 35 |
| 46 | 2026-05-03 | [Petro le mete el acelerador a la Constituyente y empieza a pedir donaciones desde su cuenta X](https://www.las2orillas.co/petro-le-mete-el-acelerador-a-la-constituyente-y-empieza-a-pedir-donaciones-desde-su-cuenta-x/) | F | — | constituyente, «obsesiona a Gustavo Petro» |
| 47 | 2026-05-07 | [Así fue como Katherine Miranda se le atravesó a Petro y su plan de mandar millones de afiliados a la Nueva EPS](https://www.las2orillas.co/asi-fue-como-katherine-miranda-se-le-atraveso-a-petro-y-su-plan-de-mandar-millones-de-afiliados-a-la-nueva-eps/) | F | — | Katherine Miranda y Nueva EPS |
| 48 | 2026-05-11 | [Los millonarios contratos detrás de la familia del tesorero de la Constituyente de Petro](https://www.las2orillas.co/los-millonarios-contratos-detras-de-la-familia-del-tesorero-de-la-constituyente-de-petro/) | F | — | tesorero de la Constituyente (con El Colombiano) |
| 49 | 2026-05-14 | [La caída de Juan Gonzalo Castaño, el directivo que el Gobierno sacó de Ecopetrol por oponerse a Roa](https://www.las2orillas.co/la-caida-de-juan-gonzalo-castano-el-directivo-que-el-gobierno-saco-de-ecopetrol-por-oponerse-a-roa/) | F | — | Castaño fuera de Ecopetrol |
| 50 | 2026-07-01 | [Puntillazo de Petro a la negociación con el Clan del golfo: firmó la extradición de Chiquito Malo](https://www.las2orillas.co/puntillazo-de-petro-a-la-negociacion-con-el-clan-del-golfo-firmo-la-extradicion-de-chiquito-malo/) | F | — | Chiquito Malo: «necesitó un año y diez meses para admitir» |
| 51 | 2026-07-21 | [¿Por qué se disparó la minería ilegal en el Gobierno de Gustavo Petro?](https://www.las2orillas.co/por-que-se-disparo-la-mineria-ilegal-en-el-gobierno-de-gustavo-petro/) | F | — | minería ilegal en el gobierno Petro (antes del cambio) |
| 52 | 2026-08-03 | [Petro le cumplió a Lula Da Silva y aceleró la compra de dos Embraer KC – 390 Milennium por 366 millones de dólares](https://www.las2orillas.co/petro-le-cumplio-a-lula-da-silva-y-acelero-la-compra-de-dos-embraer-kc-390-milennium-366-millones-de-dolares/) | F | — | Embraer: «Petro no respetó el proceso interno» |
| 53 | 2026-08-04 | [Portazo de De la Espriella al canal público RTVC que controla Petro para que no trasmita la posesión presidencial](https://www.las2orillas.co/portazo-de-de-la-espriella-al-canal-publico-rtvc-que-controla-petro-para-que-no-trasmita-la-posesion-presidencial/) | F | — | RTVC «al servicio del gobierno como un espacio de propaganda política» (04-08, aún gobierna Petro) |
| 54 | 2026-08-17 | [Dos abogadas del bufete De La Espriella Lawyers sin experiencia en el sector público saltan al alto gobierno](https://www.las2orillas.co/dos-abogadas-del-bufete-de-la-espriella-lawyers-sin-experiencia-en-el-sector-publico-saltan-al-alto-gobierno/) | F | — | «Dos abogadas del bufete De La Espriella Lawyers sin experiencia en el sector público saltan al alto gobierno» |
| 55 | 2026-08-26 | [A excepción de minHacienda y el canciller, todos los ministros de De la Espriella llegan endeudados](https://www.las2orillas.co/a-excepcion-de-minhacienda-y-el-canciller-todos-los-ministros-de-de-la-espriella-llegan-endeudados/) | F | — | ministros endeudados |
| 56 | 2026-09-02 | [Estos son los escogidos que el presidente De la Espriella quiere sentar en la junta directiva de Ecopetrol](https://www.las2orillas.co/estos-son-los-escogidos-que-el-presidente-de-la-espriella-quiere-sentar-en-la-junta-directiva-de-ecopetrol/) | F | — | junta de Ecopetrol: círculo del presidente |
| 57 | 2026-09-06 | [El regreso de Alejandro Ordoñez a la vida pública de Colombia con más poder que nunca en la era del Tigre](https://www.las2orillas.co/el-regreso-de-alejandro-ordonez-a-la-vida-publica-de-colombia-con-mas-poder-que-nunca-en-la-era-del-tigre/) | F | — | regreso de Ordóñez |
| 58 | 2026-09-17 | [A la embajada clave para el tema de derechos humanos llega otro de los abogados de De La Espriella Lawyers](https://www.las2orillas.co/a-la-embajada-clave-para-el-tema-de-derechos-humanos-llega-otro-de-los-abogados-de-de-la-espriella-lawyers/) | F | — | otro abogado del bufete del presidente a una embajada |
| 59 | 2026-09-21 | [El debut del embajador de De la Espriella en la ONU con un voto minoritario alineado con Trump contra Palestina](https://www.las2orillas.co/el-debut-del-embajador-de-de-la-espriella-en-la-onucon-un-voto-minoritario-alineado-con-trump-contra-palestina/) | F | — | voto en la ONU alineado con Trump |
| 60 | 2026-09-23 | [El nuevo director de UNP empezó la barrida de esquemas de seguridad del Pacto empezando por parientes y amigos de Petro](https://www.las2orillas.co/el-nuevo-director-de-unp-empezo-la-barrida-de-esquemas-de-seguridad-del-pacto-empezando-por-parientes-y-amigos-de-petro/) | F | — | nuevo director de la UNP, «zurdos de mierda» |


**Límites declarados.**
- Las 145 piezas «NP» (empresas, crónica, internacional, sucesos) se descartaron por el título y no se leyeron. Una pieza amable con un empresario no es postura en el eje, pero en esas 145 podría haber alguna con postura escondida.
- Las piezas «N» se leyeron por la entrada y por las frases evaluativas, no enteras.
- Una pieza no se pudo leer: el servidor devolvió 522 tres veces. Es «Así fue la llegada a Cali de presidentes e invitados especiales a la posesión de Abelardo De la Espriella» (07-08-2026). Su título es descriptivo.
- No se barrieron las piezas firmadas por la plantilla. La regla las deja fuera, pero en este medio son la mayor parte de la reportería política.
- Una sola persona clasificó todo.

---

## 8. Cómo se llegó al −0,35, y con qué evidencia

- **Origen.** El valor entra en el commit `3296b22` del 2026-08-24, «Las2Orillas entra al catalogo: no estaba mudo, lo callaba nuestra tilde», con `bias: -0.35` y `reviewedAt: null`. El `biasRationale` de `shared/mediaRegistry.js` dice, literal: «su seleccion y encuadre son sostenidamente progresistas. Valor propuesto por comparacion con CasaMacondo (-0,35) y por debajo de la investigacion militante (Voragine, Cuestion Publica). SIN FIRMAR.» **No cita ninguna pieza, ningún registro ni ninguna medición.**
- **No hay decisión en `DECISIONES.md`** que fije o apruebe ese valor. La única entrada con «−0,35» (2026-08-08) es la de RTVC, que es otro medio.
- **La propia ficha lo reconoce** (2026-09-08): la comparación con CasaMacondo «no es evidencia de nivel 1-3: es una colocación relativa dentro de nuestra propia escala». Su nivel 2 dice que el medio «se aparta, no hacia dónde».
- **El punto de comparación ya no está en el mapa.** CasaMacondo salió del mapa el 2026-09-16 como medio «no noticioso». El comentario de `shared/mediaRegistry.js` dice que esos números «eran colocaciones relativas que el expediente de Vorágine demostró insostenibles». El valor de CasaMacondo, a su vez, se apoya en una declaración de su compromiso editorial que Las2Orillas no hace.
- **Antes del alta, el criterio era el contrario.** El 2026-07-30, Las2Orillas quedó fuera del catálogo porque «no tiene una línea editorial propia que clasificar» (`LOG_IMPLEMENTACIONES.md`, `CONTEXTO_ALGORITMO_SESGO.md`). El alta del 08-24 corrigió el motivo técnico (el 403), no ese juicio.

**Conclusión:** el −0,35 es un valor por defecto con dirección, sin evidencia de nivel 1 a 3. Este barrido es la primera evidencia de dirección que se mide, y contradice el signo.

---

## 9. Veredicto por condición

| Condición | ¿Se cumple? | Nota |
|---|---|---|
| 1. Voz de la casa | Sí, con reservas | Cuentas 457, 2 y 456. Se excluyen 11 piezas por nota o firma ajena (§6). **No se pueden excluir las pagadas sin nota** (§5) |
| 2. A los dos lados del cambio | Solo hacia la derecha | Izquierda: 9 antes y 0 después. Derecha: 5 antes y 9 después |
| 3. Sostenida (≥10; ≥3 por lado; ≥3:1) | **No** | 23 piezas; 14 a 9 = 1,6:1 |
| 4. Contrapesos escritos | Sí | §4 |
| 5. Reproducible | Sí | Tablas del §2 al §7 y apéndice con las 469 piezas |

**El barrido no mueve el número por asimetría en ninguna dirección.** Lo que sí hace, y es lo que hay que decidir:
- **No sostiene el signo del valor vigente.** No hay asimetría hacia la izquierda en 12 meses de voz de la casa: 1 pieza plena y 0 desde el cambio.
- **Muestra la misma conducta con los dos gobiernos:**
  - fiscaliza a quien manda: 53 piezas con Petro y 7 con De la Espriella;
  - publica, además, piezas amables con sus medidas: 5 y 9;
  - y trata con calidez a candidatos de los dos lados: 4 de izquierda y 5 de derecha.

  El protocolo prevé este caso: «Un barrido que muestra la misma conducta con los dos gobiernos sostiene el 0,00 como evidencia, y ya no como valor por defecto».
- **Choca con la otra precisión del protocolo:** «Un barrido que no llega a los mínimos no deshace nada. La ficha conserva el valor que tenía.» Leída al pie de la letra, el −0,35 se quedaría.

---

## 10. PROPUESTA (pendiente de la decisión del responsable editorial)

**Recomendación: 0,00, sin firmar, «con evidencia» y no por defecto.**
- **Por qué 0,00 y no −0,35:**
  - El −0,35 no tuvo nunca evidencia de nivel 1 a 3 (§8).
  - El único barrido sistemático de su voz de la casa no encuentra asimetría hacia la izquierda y sí la misma conducta con los dos gobiernos.
  - La regla 2 pide, ante la duda, la banda más cercana a la mixta: «El error de clasificar de más es más caro que el de clasificar de menos: acusa».
  - La precisión «un barrido que no llega no deshace nada» se escribió para no deshacer valores «puestos por otras razones». Aquí no hay ninguna razón escrita que deshacer, y el mismo §1 da al 0,00 con evidencia una vía propia.
- **Por qué no un valor positivo:** la inclinación hacia el gobierno entrante (9 piezas leves en 65 días) no llega a los mínimos, se confunde con la luna de miel de un gobierno nuevo y no tiene ni una pieza plena.
- **Alternativa literal: −0,35.** Es la lectura estricta de «no deshace nada». Si el responsable editorial la elige, la ficha tiene que decir que el único barrido medido **contradice el signo**, y que el número se sostiene solo por la regla 3. Es la situación que la regla 2 existe para evitar.
- **Precisión de protocolo que conviene, en cualquier caso:** «Un valor sin evidencia de nivel 1 a 3 que un barrido sistemático contradice en el signo pasa a 0,00, aunque el barrido no llegue a los mínimos de asimetría.» Así este caso no depende de cómo se lean dos frases que chocan.
- **Recuento:** a los 90 días del cambio (05-11-2026), con el mismo universo y el mismo método. Si las piezas amables con el gobierno de turno siguen al ritmo de los primeros 65 días, y la fiscalización no se recupera, el signo se reexamina hacia la derecha. Ese recuento tiene que excluir los entregables pagados que se identifiquen.

---

## Apéndice: el universo completo (469 piezas)

Clases: FI y FIl (izquierda, plena y leve), FDl (derecha, leve), F, I (investiga una candidatura), M, COM, CAMP, FIRM, REIMP, OP, INT, X, N y NP (descartada por el título). La de clase «?» no se pudo leer. Para ver qué clase y qué nota lleva cada pieza, mírese la fila con el mismo id en las tablas de arriba. Las «N», «X» y «NP» no llevan nota.

| Id | Fecha | Clase | URL |
|---|---|---|---|
| 973832 | 2025-10-10 | INT | https://www.las2orillas.co/la-valiente-lucha-contra-el-regimen-chavista-que-le-dio-a-maria-corina-machado-el-nobel-de-paz/ |
| 974022 | 2025-10-11 | NP | https://www.las2orillas.co/el-boom-de-los-rones-venezolanos-en-el-mundo-que-le-esta-llevando-millones-de-dolares-a-venezuela/ |
| 974129 | 2025-10-12 | N | https://www.las2orillas.co/espaldarazo-de-la-defensora-del-pueblo-a-la-negociacion-de-petro-con-bandas-criminales-y-la-delincuencia-comun/ |
| 974679 | 2025-10-16 | NP | https://www.las2orillas.co/el-pleito-que-un-pequeno-empresario-de-bucaramanga-le-gano-a-la-marca-victorias-secret-y-sus-poderosos-abogados/ |
| 974862 | 2025-10-16 | N | https://www.las2orillas.co/el-dia-que-abelardo-desprecio-el-ajiaco-tipico-bogotano-y-lo-tildo-de-comida-para-presos/ |
| 974980 | 2025-10-18 | NP | https://www.las2orillas.co/por-incumplimiento-del-contratista-otra-vez-se-pospone-la-entrega-de-la-biblioteca-espana-una-obra-que-lleva-20-anos/ |
| 974957 | 2025-10-19 | NP | https://www.las2orillas.co/el-ingeniero-venezolano-que-se-invento-la-formula-para-hacer-de-la-arepa-una-industria-millonaria/ |
| 973889 | 2025-10-20 | NP | https://www.las2orillas.co/como-una-avanzada-de-350-pequenos-empresarios-venezolanos-se-ha-ido-abriendo-camino-en-cucuta/ |
| 975662 | 2025-10-21 | N | https://www.las2orillas.co/la-historia-de-jaime-granados-el-penalista-que-defendio-a-alvaro-uribe-hasta-lograr-su-absolucion/ |
| 975915 | 2025-10-22 | N | https://www.las2orillas.co/en-el-rifi-rafe-entre-petro-y-su-ministra-de-vivienda-alrededor-de-los-aviones-de-combate-suecos-se-omitio-un-dato-clave/ |
| 975948 | 2025-10-23 | N | https://www.las2orillas.co/con-una-firma-gringa-lobista-y-8-funcionarios-de-carrera-el-embajador-garcia-pena-enfrenta-la-crisis-con-trump/ |
| 976234 | 2025-10-24 | N | https://www.las2orillas.co/montealegre-se-va-del-gobierno-advirtiendole-a-petro-sobre-traiciones-en-la-casa-de-narino/ |
| 976372 | 2025-10-25 | N | https://www.las2orillas.co/el-abogado-gringo-antiuribista-que-defendera-a-petro-tras-su-inclusion-en-la-lista-clinton/ |
| 976460 | 2025-10-26 | F | https://www.las2orillas.co/estocolmo-la-ultima-aparicion-de-veronica-alcocer-como-primera-dama-el-pais-que-convirtio-en-su-destino-preferido/ |
| 976507 | 2025-10-26 | N | https://www.las2orillas.co/cepeda-duplico-a-carolina-corcho-con-2-millones-de-votos-cuando-hace-4-anos-fueron-de-mas-5-millones/ |
| 976613 | 2025-10-27 | FI | https://www.las2orillas.co/la-batalla-mas-grande-que-ha-ganado-ivan-cepeda-no-fue-la-de-este-domingo-sino-cuando-derroto-el-cancer/ |
| 976519 | 2025-10-27 | F | https://www.las2orillas.co/con-recortes-a-la-rama-judicial-el-gobierno-sigue-siendo-juez-unico-de-la-reforma-agraria/ |
| 976638 | 2025-10-27 | N | https://www.las2orillas.co/por-ahora-no-hay-tutela-que-valga-al-presidente-petro-para-escapar-a-los-efectos-de-la-lista-clinton/ |
| 976498 | 2025-10-27 | NP | https://www.las2orillas.co/como-un-colombiano-podria-convertirse-en-el-rey-de-los-supermercados-en-argentina-2/ |
| 976699 | 2025-10-28 | FIl | https://www.las2orillas.co/dos-mujeres-los-pilares-en-la-vida-de-ivan-cepeda/ |
| 976861 | 2025-10-28 | X | https://www.las2orillas.co/el-presidente-del-concurso-nacional-de-belleza-raymundo-angulo-se-impuso-y-la-senorita-antioquia-debio-hacerse-a-un-lado/ |
| 977011 | 2025-10-29 | N | https://www.las2orillas.co/entre-petrodolares-y-principes-arabes-la-primera-escala-de-petro-en-oriente-medio/ |
| 977234 | 2025-10-30 | NP | https://www.las2orillas.co/el-brutal-asesinato-de-mercedes-chaparro-la-empleada-mas-querida-de-victor-carranza/ |
| 977137 | 2025-10-30 | F | https://www.las2orillas.co/el-presidente-de-la-ani-javier-torres-enfrenta-demandas-de-los-duenos-de-las-concesiones-por-10-5-billones/ |
| 977396 | 2025-10-31 | X | https://www.las2orillas.co/los-2-hermanos-de-la-espriella-duenos-de-cachivaches-que-dan-la-pelea-a-la-invasion-de-disfraces-chinos/ |
| 977412 | 2025-10-31 | N | https://www.las2orillas.co/en-mas-de-1-millon-de-dolares-le-costara-a-benedetti-el-abogado-que-intentara-sacarlo-de-la-lista-clinton/ |
| 977492 | 2025-11-01 | N | https://www.las2orillas.co/con-gustavo-petro-su-hijo-nicolas-su-esposa-veronica-y-benedetti-son-171-los-colombianos-que-estan-en-la-lista-clinton/ |
| 977558 | 2025-11-02 | NP | https://www.las2orillas.co/como-la-marca-cacao-hunters-puso-a-los-japoneses-a-comer-chocolates-bajados-de-la-sierra-arauca-y-tumaco/ |
| 977423 | 2025-11-02 | NP | https://www.las2orillas.co/la-multa-de-mas-de-ocho-mil-millones-contra-la-dimayor-y-clubes-por-tener-listas-de-futbolistas/ |
| 977464 | 2025-11-02 | NP | https://www.las2orillas.co/la-minera-canadiense-aris-mining-logro-sentar-en-su-junta-directiva-a-una-prestigiosa-lider-ambientalista/ |
| 977695 | 2025-11-04 | F | https://www.las2orillas.co/la-companera-de-alias-calarca-quien-esta-negociando-con-el-gobierno-petro-es-la-reina-de-la-extorsion-en-caqueta/ |
| 977769 | 2025-11-04 | N | https://www.las2orillas.co/la-version-de-petro-de-la-toma-del-palacio-de-justicia-que-califica-como-una-genialidad-del-comandante-luis-otero/ |
| 977258 | 2025-11-04 | NP | https://www.las2orillas.co/los-poderosos-chinos-a-los-que-los-ortega-y-su-hijo-les-entregaron-500-mil-hectareas-de-nicaragua-para-buscar-metales/ |
| 977829 | 2025-11-04 | N | https://www.las2orillas.co/el-exgeneral-zapateiro-cerro-filas-alrededor-de-abelardo-de-la-espriella/ |
| 978032 | 2025-11-05 | N | https://www.las2orillas.co/el-contra-ataque-de-petro-a-uno-de-los-congresistas-en-la-comision-de-acusaciones-le-resulto-sera-investigado/ |
| 978063 | 2025-11-05 | FDl | https://www.las2orillas.co/petro-necesita-tener-un-motivo-para-que-alguien-me-mate-ya-mataron-a-miguel-uribe/ |
| 977921 | 2025-11-05 | F | https://www.las2orillas.co/la-uso-se-le-para-a-petro-y-a-minminas-para-que-ecopetrol-no-frene-el-fracking-en-eeuu/ |
| 978366 | 2025-11-07 | N | https://www.las2orillas.co/duro-con-el-m-19-el-presidente-de-la-corte-constitucional-dijo-que-este-no-puede-romantizado-por-el-horror-del-palacio/ |
| 978450 | 2025-11-07 | N | https://www.las2orillas.co/la-rabia-de-marbelle-contra-petro-y-la-izquierda-que-desfoga-con-su-twitter-y-ahora-apoyando-a-abelardo-de-la-espriella/ |
| 978527 | 2025-11-08 | I | https://www.las2orillas.co/el-caso-que-desperto-la-pasion-de-natalia-paris-por-abelardo-de-la-espriella/ |
| 978610 | 2025-11-09 | F | https://www.las2orillas.co/el-lio-de-nunca-acabar-la-fundacion-de-educacion-superior-san-jose-anula-el-titulo-de-juliana-guerrero/ |
| 978486 | 2025-11-09 | NP | https://www.las2orillas.co/la-gigante-petrolera-brasilera-con-la-que-lula-se-hace-sentir-en-colombia/ |
| 978629 | 2025-11-10 | NP | https://www.las2orillas.co/los-5-mil-millones-que-vale-cuidar-los-valiosos-animales-incautados-a-los-narcos-en-poder-de-la-sae/ |
| 978743 | 2025-11-10 | NP | https://www.las2orillas.co/el-gringo-del-partido-de-trump-dueno-de-la-empresa-que-le-incumplio-al-ejercito-con-el-arreglo-de-los-helicopteros-rusos/ |
| 978819 | 2025-11-10 | F | https://www.las2orillas.co/el-retrato-de-la-embajadora-de-colombia-en-alemania-pagado-por-el-estado-que-colgo-en-su-despacho-en-berlin/ |
| 978737 | 2025-11-11 | N | https://www.las2orillas.co/el-senador-paisa-que-llevo-a-pipe-cordoba-a-pelear-la-candidatura-presidencial-conservadora-y-enredo-a-efrain-cepeda/ |
| 979056 | 2025-11-11 | F | https://www.las2orillas.co/esta-es-la-valiosa-casa-en-el-corazon-de-londres-donde-laura-sarabia-vivira-como-embajadora-de-colombia/ |
| 979081 | 2025-11-12 | NP | https://www.las2orillas.co/la-empresa-calena-que-fabrico-los-carruajes-electricos-de-cartagena-que-reemplazan-los-coches-de-caballos/ |
| 979118 | 2025-11-12 | N | https://www.las2orillas.co/como-logro-abelardo-de-la-espriella-jalonar-a-4-lideres-cristianos-a-su-campana-presidencial/ |
| 979372 | 2025-11-13 | F | https://www.las2orillas.co/la-maraton-de-contratos-por-2-1-billones-que-firmo-el-gobierno-petro-en-7-dias-para-evitar-la-ley-de-garantias/ |
| 979478 | 2025-11-13 | N | https://www.las2orillas.co/el-magistrado-que-se-enfrento-a-uribe-desde-la-corte-es-el-nuevo-ministro-de-justicia-de-petro/ |
| 979600 | 2025-11-14 | F | https://www.las2orillas.co/el-misterio-detras-del-asesinato-del-creador-de-la-cripto-daily-cop-y-dueno-del-avion-en-el-que-petro-hizo-campana/ |
| 979624 | 2025-11-16 | NP | https://www.las2orillas.co/los-negocios-con-los-que-gilinski-y-otros-empresarios-colombianos-mueven-millones-en-en-chile/ |
| 979730 | 2025-11-16 | FIl | https://www.las2orillas.co/la-frenada-de-petro-a-temu-y-shein-que-ayudara-a-los-confeccionistas-colombianos/ |
| 979974 | 2025-11-17 | NP | https://www.las2orillas.co/fernando-carrillo-y-su-proyeccion-en-sector-privado-tras-una-rica-experiencia-de-vida-publica/ |
| 979772 | 2025-11-17 | NP | https://www.las2orillas.co/el-contrato-de-106-mil-millones-en-cartagena-que-el-alcalde-dumek-turbay-le-entrego-a-un-constructor-sancionado/ |
| 980014 | 2025-11-18 | NP | https://www.las2orillas.co/los-polemicos-bombardeos-contra-ivan-mordisco-que-han-dado-de-baja-19-de-sus-cabecillas/ |
| 980065 | 2025-11-18 | F | https://www.las2orillas.co/en-que-gasta-gustavo-petro-los-mas-de-600-millones-que-se-gana-al-ano-como-presidente/ |
| 980175 | 2025-11-19 | N | https://www.las2orillas.co/a-los-114-procesos-que-tiene-petro-en-la-comision-de-acusaciones-se-le-sumo-la-prohibicion-de-exportar-carbon-a-israel/ |
| 980182 | 2025-11-19 | N | https://www.las2orillas.co/los-cuatro-corredores-ferreos-que-tiene-listos-para-licitar-el-gobierno-petro/ |
| 980247 | 2025-11-19 | N | https://www.las2orillas.co/adios-a-los-kfir-en-colombia-los-aviones-de-guerra-que-compraron-barco-y-uribe-y-reemplazo-petro-por-los-gripen/ |
| 980243 | 2025-11-19 | NP | https://www.las2orillas.co/la-reinvencion-del-famoso-hotel-cosmos-100-de-bogota-como-ancianato-de-lujo/ |
| 980335 | 2025-11-20 | N | https://www.las2orillas.co/luis-gilberto-murillo-un-exministro-de-petro-y-santos-que-le-apuesta-al-centro-para-ir-por-la-presidencia/ |
| 980516 | 2025-11-21 | F | https://www.las2orillas.co/el-proyecto-secreto-del-gobierno-de-convertir-la-inteligencia-financiera-en-instrumento-de-lucha-politica/ |
| 980622 | 2025-11-22 | F | https://www.las2orillas.co/la-fiscalia-sueca-entra-a-jugar-en-el-caso-de-18-aviones-gripen-por-los-que-pago-el-gobierno-petro-16-5-billones/ |
| 980613 | 2025-11-23 | NP | https://www.las2orillas.co/mondomo-el-pueblo-del-cauca-que-vive-entre-el-almidon-y-la-guerra/ |
| 980829 | 2025-11-23 | N | https://www.las2orillas.co/carlos-caicedo-le-gano-el-pulso-a-petro-en-el-magdalena-y-puso-gobernadora-margarita-guerra/ |
| 980911 | 2025-11-24 | F | https://www.las2orillas.co/dos-pesados-generales-que-petro-vinculo-al-gobierno-eran-infiltrados-de-calarca-y-sus-disidencias/ |
| 980550 | 2025-11-25 | NP | https://www.las2orillas.co/el-negocio-hotelero-de-german-efromovich-que-hace-15-anos-empezo-con-un-hotel-pequeno-en-cartagena-y-no-ha-parado-de-crecer/ |
| 981092 | 2025-11-25 | F | https://www.las2orillas.co/los-2-experimentados-fiscales-escogidos-por-la-fiscal-camargo-para-investigar-la-infiltracion-de-calarca-en-el-gobierno/ |
| 981226 | 2025-11-25 | F | https://www.las2orillas.co/el-es-el-empresario-catalan-que-acompana-a-veronica-alcocer-en-europa-es-cercano-al-gobierno-de-petro/ |
| 981238 | 2025-11-25 | N | https://www.las2orillas.co/el-cura-clave-en-la-creacion-del-grupo-de-los-doce-apostoles-por-el-que-condenaron-a-28-anos-a-santiago-uribe/ |
| 981403 | 2025-11-26 | F | https://www.las2orillas.co/por-que-dos-de-los-ex-ministros-mas-cercanos-a-petro-estan-a-las-puertas-de-la-carcel/ |
| 981492 | 2025-11-27 | F | https://www.las2orillas.co/ricardo-roa-el-gran-paganini-con-la-drastica-sancion-del-cne-por-violacion-de-topes-de-la-campana-de-petro/ |
| 981614 | 2025-11-27 | NP | https://www.las2orillas.co/los-barranquilleros-que-compraron-pepa-ganga-un-negocio-que-los-convirtio-en-los-zares-de-los-juguetes-importados/ |
| 981624 | 2025-11-28 | NP | https://www.las2orillas.co/este-es-el-barrio-mas-poblado-de-bogota-que-se-levanto-en-una-finca-agricola-y-ganadera/ |
| 981486 | 2025-11-28 | F | https://www.las2orillas.co/las-alternativas-del-valle-para-no-quedarse-sin-el-tren-de-cercanias-para-responder-a-la-cachetada-del-gobierno-petro/ |
| 981937 | 2025-11-30 | NP | https://www.las2orillas.co/la-pelea-entre-los-santo-domingo-y-guillermo-franco-el-periodista-que-junto-a-luis-fernando-santos-puso-a-andar-pulzo/ |
| 981951 | 2025-11-30 | NP | https://www.las2orillas.co/los-guatemaltecos-productores-de-fertilizantes-pisan-duro-y-superan-en-ventas-la-venezolana-monomeros/ |
| 981962 | 2025-11-30 | NP | https://www.las2orillas.co/el-poder-intocable-de-victor-carranza-un-hombre-que-ni-la-justicia-ni-la-guerra-lograron-derribar/ |
| 982204 | 2025-12-02 | NP | https://www.las2orillas.co/los-portugueses-se-quedaron-con-dos-megacontratos-en-cartagena-llevan-decadas-con-negocios-en-colombia/ |
| 982287 | 2025-12-02 | NP | https://www.las2orillas.co/la-historia-detras-de-la-foto-que-mostro-en-la-morgue-de-medellin-el-final-de-pablo-escobar/ |
| 982390 | 2025-12-03 | NP | https://www.las2orillas.co/colmedica-las-clinicas-del-country-y-la-colina-quedaron-en-manos-brasileras/ |
| 982732 | 2025-12-04 | F | https://www.las2orillas.co/la-poderosa-familia-sueca-duena-del-periodico-expressen-que-le-sigue-los-pasos-a-veronica-alcocer-en-estocolmo/ |
| 982770 | 2025-12-05 | NP | https://www.las2orillas.co/el-es-el-millonario-dueno-del-ferrari-amarillo-accidentado-en-la-calera-tiene-8-mas-en-su-garaje/ |
| 927829 | 2025-12-06 | NP | https://www.las2orillas.co/la-margarita-del-ocho-el-restaurante-de-fabio-ochoa-que-termino-en-manos-del-hijo-de-diomedes-diaz/ |
| 982844 | 2025-12-07 | NP | https://www.las2orillas.co/la-historia-de-foto-japon-la-iconica-tienda-fotografica-que-hoy-lucha-por-sobrevivir/ |
| 981315 | 2025-12-10 | F | https://www.las2orillas.co/las-fiestas-de-los-petro-en-espana-con-manuel-grau-que-lo-volvieron-la-sombra-de-veronica-alcocer-en-europa/ |
| 982059 | 2025-12-10 | NP | https://www.las2orillas.co/el-legado-de-jose-alejandro-cortes-testigo-del-salto-del-grupo-bolivar-a-la-cima-en-tarjetas-de-credito-a-sus-94-anos/ |
| 983461 | 2025-12-11 | INT | https://www.las2orillas.co/asi-se-escapo-maria-corina-machado-de-venezuela-y-llego-a-oslo-a-recibir-el-nobel-de-la-paz/ |
| 983635 | 2025-12-14 | X | https://www.las2orillas.co/las-poderosas-sociedades-que-los-ardila-y-echavarria-de-corona-tienen-con-chilenos-que-hoy-eligen-su-presidente/ |
| 984128 | 2025-12-17 | N | https://www.las2orillas.co/las-2-encuestadores-chilenas-que-convirtieron-a-paloma-valencia-en-la-candidata-presidencial-del-centro-democratico/ |
| 984195 | 2025-12-17 | N | https://www.las2orillas.co/comision-de-acusaciones-archiva-17-casos-contra-petro-pero-mantiene-mas-de-100-procesos-en-pausa/ |
| 984271 | 2025-12-18 | NP | https://www.las2orillas.co/quien-fabrica-las-polisombras-que-tienen-invadida-bogota-tapando-la-multitud-de-obras/ |
| 984442 | 2025-12-18 | F | https://www.las2orillas.co/quien-es-la-magistrada-que-mando-a-la-carcel-a-dos-de-los-ministros-mas-cercanos-de-petro/ |
| 984612 | 2025-12-19 | F | https://www.las2orillas.co/la-revancha-del-espanol-dueno-de-la-eps-sanitas-contra-petro-lo-puso-a-rectificar/ |
| 984658 | 2025-12-20 | N | https://www.las2orillas.co/antes-de-que-el-campo-sirius-empiece-a-producir-gas-ecopetrol-petrobras-tienen-vendido-mas-de-la-mitad/ |
| 984476 | 2025-12-21 | NP | https://www.las2orillas.co/los-hermanos-paisas-que-triunfaron-en-ee-uu-a-punta-de-bocadillo-supercocos-y-puro-mecato-colombiano/ |
| 984749 | 2025-12-22 | N | https://www.las2orillas.co/jose-antonio-ocampo-rompe-el-silencio-asi-ve-la-economia-colombiana-a-9-meses-del-adios-petro/ |
| 984879 | 2025-12-23 | NP | https://www.las2orillas.co/el-chino-que-se-invento-tiktok-perdio-su-control-en-eeuu-ante-oracle-y-los-arabes-aliados-de-los-gilinski/ |
| 984995 | 2025-12-23 | NP | https://www.las2orillas.co/la-famosa-mina-de-sal-de-zipaquira-se-quedo-sin-quien-la-explote-y-ahora-es-el-turismo-el-que-manda-alli/ |
| 985108 | 2025-12-24 | NP | https://www.las2orillas.co/le-llego-la-hora-a-emilio-tapia-de-responder-por-su-corrupcion-la-fiscalia-lo-golpeo-donde-mas-le-duele-la-plata/ |
| 985244 | 2025-12-26 | F | https://www.las2orillas.co/los-influyentes-directivos-de-colfuturo-que-no-convencieron-a-petro-de-las-bondades-de-un-modelo-que-funciono-25-anos/ |
| 985116 | 2025-12-26 | F | https://www.las2orillas.co/donde-le-compro-colpensiones-la-gran-camioneta-de-404-millones-al-presidente-de-la-entidad-jaime-dussan/ |
| 985081 | 2025-12-28 | NP | https://www.las2orillas.co/curarse-sin-medicamentos-quimicos-el-camino-de-la-homeopatia-que-boiron-y-heel-han-abierto-en-colombia/ |
| 985341 | 2025-12-29 | I | https://www.las2orillas.co/apoyo-de-la-camara-de-comercio-de-villavicencio-a-abelardo-de-la-espriella-termino-en-multa-de-la-supersociedades/ |
| 985498 | 2025-12-29 | NP | https://www.las2orillas.co/mano-dura-de-la-super-con-el-dueno-del-bus-y-el-diagnosticentro-que-le-dio-via-libre-donde-murieron-los-17-bachilleres/ |
| 985752 | 2025-12-30 | NP | https://www.las2orillas.co/una-pequena-empresa-de-alimentos-en-cota-cundinamarca-le-gano-al-poderoso-grupo-de-los-ardila-lulle/ |
| 985777 | 2025-12-31 | NP | https://www.las2orillas.co/de-las-10-gigantes-mineras-del-mundo-solo-dos-estan-en-colombia/ |
| 985947 | 2025-12-31 | X | https://www.las2orillas.co/los-herederos-del-ex-presidente-sebastian-pinera-salieron-de-terpel-controlada-por-otros-chilenos/ |
| 985935 | 2025-12-31 | NP | https://www.las2orillas.co/gilinsky-se-defiende-y-logra-que-no-le-toquen-sus-hamburguesas-el-corral/ |
| 985987 | 2025-12-31 | FIl | https://www.las2orillas.co/petro-puso-a-colombia-en-el-top-5-de-los-paises-de-la-region-con-mayor-salario-minimo/ |
| 985896 | 2025-12-31 | NP | https://www.las2orillas.co/entre-multinacional-inglesa-y-una-francesa-se-reparten-los-licores-importados-que-se-consumen-en-colombia/ |
| 986097 | 2026-01-02 | NP | https://www.las2orillas.co/una-empresa-gringa-le-llevara-energia-solar-a-los-arhuacos-de-la-sierra-nevada/ |
| 985895 | 2026-01-02 | N | https://www.las2orillas.co/quien-es-el-pastor-de-cucuta-que-sera-clave-para-el-nuevo-embajador-de-colombia-en-el-brasil/ |
| 986212 | 2026-01-03 | INT | https://www.las2orillas.co/en-otra-operacion-militar-el-gobierno-de-ee-uu-derroco-y-detuvo-al-dictador-manuel-antonio-noriega-hace-37-anos/ |
| 222154 | 2026-01-03 | NP | https://www.las2orillas.co/ella-es-la-mujer-que-maduro-no-se-atrevia-a-desobedecer-y-ahora-lo-acompanara-a-pagar-carcel-en-ee-uu/ |
| 986310 | 2026-01-04 | NP | https://www.las2orillas.co/una-dura-y-radical-pero-con-cintura-politica-toma-las-riendas-de-venezuela/ |
| 986186 | 2026-01-04 | N | https://www.las2orillas.co/el-estado-colombiano-se-queda-sin-su-parte-de-movistar-y-petro-espera-recoger-856-mil-millones-con-la-venta-del-32-5/ |
| 986375 | 2026-01-05 | NP | https://www.las2orillas.co/la-rica-familia-duena-de-farmatodo-que-no-se-dejo-sacar-de-venezuela-y-esta-vendiendo-mas-que-nunca/ |
| 986407 | 2026-01-05 | NP | https://www.las2orillas.co/la-enriquecida-que-logro-jaime-gilinski-con-la-compra-de-nutresa-multiplico-su-fortuna/ |
| 986418 | 2026-01-05 | NP | https://www.las2orillas.co/un-curtido-juez-conocido-como-el-sheriff-de-wall-street-decidira-la-suerte-de-maduro-a-quien-le-tienen-lista-la-carcel/ |
| 986497 | 2026-01-06 | NP | https://www.las2orillas.co/la-fatal-herencia-de-natasha-avendano-a-santa-marta-el-contrato-de-basuras-de-atesa-que-ha-resultado-una-calamidad/ |
| 986545 | 2026-01-06 | NP | https://www.las2orillas.co/la-cooperativa-de-productores-de-leche-del-caribe-un-sueno-que-empieza-a-marchitarse/ |
| 986575 | 2026-01-06 | NP | https://www.las2orillas.co/la-multinacional-minera-glencore-despidio-el-ano-con-la-venta-de-otra-de-sus-propiedades-en-colombia-puerto-nuevo/ |
| 986657 | 2026-01-07 | NP | https://www.las2orillas.co/el-coronel-cubano-que-protegia-a-maduro-y-cayo-en-operativo-de-trump-habia-cuidado-al-papa-francisco-en-su-visita-a-cuba/ |
| 986769 | 2026-01-08 | X | https://www.las2orillas.co/donde-se-consigue-la-chaqueta-de-aviador-que-petro-lucio-en-la-plaza-de-bolivar-y-cuanto-cuesta/ |
| 986796 | 2026-01-08 | INT | https://www.las2orillas.co/dos-republicanos-gringos-empiezan-a-jugar-en-el-caso-venezuela-con-maduro-y-petro/ |
| 986803 | 2026-01-09 | N | https://www.las2orillas.co/en-medio-de-la-disputa-con-el-gobierno-canal-uno-lleva-su-testimonio-contra-caracol-y-rcn/ |
| 986816 | 2026-01-09 | NP | https://www.las2orillas.co/los-contratistas-que-aun-no-concluyen-el-hospital-mental-de-antioquia-tienen-en-su-historial-mas-de-un-proyecto-enredado/ |
| 986861 | 2026-01-10 | NP | https://www.las2orillas.co/la-ultima-tragedia-de-caroline-la-hija-del-asesinado-john-f-kennedy-despedir-a-su-hija-y-tantos-del-clan-kennedy/ |
| 987008 | 2026-01-10 | FIl | https://www.las2orillas.co/petro-ordena-levantar-los-peajes-en-el-eje-cafetero-y-poner-fin-a-la-concesion-autopistas-del-cafe/ |
| 987033 | 2026-01-10 | FIl | https://www.las2orillas.co/dos-mujeres-le-dan-la-fuerza-a-ivan-cepeda-el-sucesor-de-petro-que-no-la-tiene-facil-con-abelardo-de-la-espriella/ |
| 987069 | 2026-01-11 | I | https://www.las2orillas.co/el-negociazo-de-abelardo-de-la-espriella-con-un-edificio-de-apartamentos-en-bogota-del-que-salio-la-plata-de-la-campana/ |
| 987089 | 2026-01-11 | NP | https://www.las2orillas.co/cuatro-empresarios-tecnologicos-venezolanos-que-lograron-crecer-en-medio-del-regimen-de-maduro-y-sus-barreras/ |
| 986901 | 2026-01-12 | N | https://www.las2orillas.co/que-va-a-hacer-petro-con-los-13-6-millones-de-informales-de-colombia/ |
| 986974 | 2026-01-12 | NP | https://www.las2orillas.co/el-multimillonario-de-la-florida-amigo-de-trump-que-vigilara-la-operacion-de-las-petroleras-que-vuelven-a-venezuela/ |
| 987178 | 2026-01-13 | N | https://www.las2orillas.co/petro-y-galan-no-se-ponen-de-acuerdo-ni-para-decidir-sobre-un-multicampus-universitario-para-el-enorme-sector-de-suba/ |
| 987283 | 2026-01-13 | F | https://www.las2orillas.co/el-fiasco-de-la-intervencion-de-drogas-la-rebaja-por-parte-del-gobierno-petro-quetermino-de-quebrarlas/ |
| 986824 | 2026-01-13 | NP | https://www.las2orillas.co/como-sierracol-la-mas-grande-petrolera-colombiana-se-levanto-para-seguir-dando-la-pelea/ |
| 987313 | 2026-01-14 | NP | https://www.las2orillas.co/estos-son-los-venezolanos-que-se-hicieron-millonarios-con-chavez-a-quienes-suiza-les-congelo-sus-cuentas/ |
| 987453 | 2026-01-15 | NP | https://www.las2orillas.co/tres-familias-millonarias-de-venezuela-que-sobrevivieron-al-chavismo-y-se-preparan-para-la-transicion/ |
| 987474 | 2026-01-15 | N | https://www.las2orillas.co/rector-de-la-u-de-la-rioja-afin-al-gobierno-petro-dara-becas-icetex-para-maestrias-virtuales/ |
| 987550 | 2026-01-15 | INT | https://www.las2orillas.co/quien-es-el-lobista-de-delcy-rodriguez-en-washington-que-busca-romper-el-hielo-con-el-gobierno-trump/ |
| 987744 | 2026-01-16 | N | https://www.las2orillas.co/la-historia-del-amarillo-un-aguardiente-que-popularizo-yeison-jimenez-y-al-que-petro-quiere-subirle-el-precio/ |
| 987795 | 2026-01-18 | NP | https://www.las2orillas.co/una-mujer-que-perdio-a-sus-hermanas-por-orden-del-regimen-irani-se-la-juega-ahora-enfrentando-al-ayatola-ali-jamenei/ |
| 987909 | 2026-01-18 | N | https://www.las2orillas.co/mario-montoya-el-militar-emblematico-en-antioquia-bajo-la-sombra-de-los-falsos-positivos/ |
| 987774 | 2026-01-18 | NP | https://www.las2orillas.co/la-nueva-vida-de-ruben-minski-tras-perder-procaps-la-gran-farmacetica-que-fundo-y-manejo-45-anos/ |
| 987864 | 2026-01-19 | N | https://www.las2orillas.co/la-historia-de-la-concesion-autopista-del-cafe-que-petro-quiere-quitarle-a-sus-duenos-para-eliminar-peajes/ |
| 988107 | 2026-01-20 | NP | https://www.las2orillas.co/dos-familias-extranjeras-controlan-el-70-del-negocio-de-gasolina-en-colombia-a-la-que-tendran-que-bajarle-300-al-galon/ |
| 988134 | 2026-01-20 | N | https://www.las2orillas.co/la-prima-de-casi-17-millones-que-petro-le-quito-a-los-congresistas-la-habia-otorgado-por-decreto-juan-manuel-santos/ |
| 988235 | 2026-01-21 | F | https://www.las2orillas.co/el-imperio-educativo-de-francisco-pareja-el-dueno-de-u-san-jose-que-le-vendio-el-titulo-a-juliana-guerrero/ |
| 988303 | 2026-01-21 | NP | https://www.las2orillas.co/la-bonanza-petrolera-de-una-pequena-isla-del-caribe-a-la-que-le-estan-sacando-jugo-tres-constructoras-colombianas/ |
| 988416 | 2026-01-22 | F | https://www.las2orillas.co/la-revancha-de-petro-contra-daniel-noboa-podria-terminar-pagandola-los-ecuatorianos-con-apagones-como-ocurrio-antes/ |
| 988420 | 2026-01-23 | N | https://www.las2orillas.co/cuales-son-las-empresas-vallecaucanas-golpeadas-por-el-arancel-que-impuso-el-presidente-ecuatoriano/ |
| 988194 | 2026-01-24 | NP | https://www.las2orillas.co/diez-start-ups-colombianas-buscan-abrirse-camino-en-chile-cuales-fueron-las-escogidas/ |
| 988599 | 2026-01-24 | N | https://www.las2orillas.co/los-colombianos-se-inclinan-mas-hacia-la-tendencia-de-derecha-aunque-aparezca-ivan-cepeda-liderando-las-encuestas/ |
| 988734 | 2026-01-25 | FDl | https://www.las2orillas.co/la-senadora-y-candidata-del-cd-paloma-valencia-logro-lo-que-petro-no-pudo-tumbar-al-director-de-la-unidad-de-victimas/ |
| 988789 | 2026-01-26 | N | https://www.las2orillas.co/cual-fue-el-empresario-que-apoyo-el-bloque-de-los-4-de-petro-en-la-junta-de-la-camara-de-comercio-de-bogota/ |
| 988957 | 2026-01-27 | F | https://www.las2orillas.co/la-ruta-de-nhora-mondragon-que-la-llevo-al-dapre-de-la-mano-de-juliana-guerrero-y-con-armando-benedetti-como-padrino/ |
| 989049 | 2026-01-27 | N | https://www.las2orillas.co/garrotazo-del-presidente-ecuatoriano-a-ecopetrol-costo-del-transporte-del-petroleo-hacia-el-puerto-de-esmeraldas/ |
| 989075 | 2026-01-28 | FDl | https://www.las2orillas.co/alvaro-uribe-el-unico-sobreviviente-como-politico-activo-de-los-15-fundadores-de-su-partido-centro-democratico/ |
| 989187 | 2026-01-28 | NP | https://www.las2orillas.co/dos-empresas-colombianas-que-nadie-imaginaba-lograron-entrar-a-vender-sus-productos-en-china/ |
| 989235 | 2026-01-28 | NP | https://www.las2orillas.co/los-mega-planes-de-almacenes-flamingo-que-le-pegaron-un-susto-a-sus-duenos-pero-pudieron-retomar-el-vuelo/ |
| 989263 | 2026-01-29 | NP | https://www.las2orillas.co/el-centro-de-la-musica-vallenata-que-enfrento-si-clan-genecco-y-la-familia-araujo-que-tras-5-anos-sigue-sin-estrenarse/ |
| 989370 | 2026-01-29 | N | https://www.las2orillas.co/la-pelea-que-unio-a-catolicos-y-cristianos-contra-el-presidente-petro-sobre-la-vida-sexual-de-jesus/ |
| 989347 | 2026-01-29 | F | https://www.las2orillas.co/fabricato-no-aguanto-la-competencia-con-los-hilos-y-fibras-extranjeras-a-los-que-petro-les-quito-el-arancel/ |
| 989473 | 2026-01-30 | FDl | https://www.las2orillas.co/la-joven-monteriana-esposa-de-abelardo-de-la-espriella-a-quien-la-vida-le-dio-un-vuelco-total/ |
| 989677 | 2026-01-31 | N | https://www.las2orillas.co/quienes-acompanaran-a-petro-a-su-reunion-con-trump-en-washington-donde-no-puede-estar-mas-de-5-dias/ |
| 989606 | 2026-02-01 | NP | https://www.las2orillas.co/dos-militares-y-la-alcaldia-de-la-jagua-de-ibirico-se-amangualaron-para-cobrar-la-comida-de-soldados-inexistentes/ |
| 989859 | 2026-02-02 | N | https://www.las2orillas.co/el-costoso-equipo-de-asesores-internacionales-con-el-que-roy-barreras-busca-derrotar-a-ivan-cepeda-en-la-consulta/ |
| 989559 | 2026-02-02 | NP | https://www.las2orillas.co/que-hay-detras-de-los-derrumbes-los-cierres-y-el-caos-en-la-via-al-llano-hay-solucion/ |
| 989948 | 2026-02-03 | N | https://www.las2orillas.co/la-carta-con-la-que-petro-espera-convencer-a-trump-de-que-en-colombia-si-se-persigue-a-los-narcos/ |
| 990098 | 2026-02-04 | N | https://www.las2orillas.co/cronica-del-encuentro-entre-trump-y-petro-quien-por-primera-vez-en-casi-4-anos-llego-antes-de-la-hora-a-una-cita/ |
| 990089 | 2026-02-04 | NP | https://www.las2orillas.co/el-famoso-fruver-que-ocupo-el-vacio-que-dejo-surtifruver-al-que-le-cayo-la-super-por-quedarse-con-las-vueltas/ |
| 990182 | 2026-02-04 | N | https://www.las2orillas.co/la-casona-mas-de-100-anos-de-la-embajada-de-colombia-en-washington-donde-petro-afino-su-cara-a-cara-con-trump/ |
| 990229 | 2026-02-05 | INT | https://www.las2orillas.co/que-ha-pasado-con-los-dirigentes-mas-cercanos-a-maria-corina-machado-que-fueron-encarcelados-en-el-helicoide/ |
| 990504 | 2026-02-07 | INT | https://www.las2orillas.co/como-tres-famosos-espanoles-un-expresidente-el-lider-de-un-partido-y-un-juez-le-sacaron-millones-al-regimen-de-maduro/ |
| 990516 | 2026-02-07 | N | https://www.las2orillas.co/con-cepeda-y-de-la-espriella-al-frente-15-candidatos-se-pelearan-la-presidencia-de-colombia-el-proximo-31-de-mayo/ |
| 990355 | 2026-02-08 | X | https://www.las2orillas.co/el-artesano-y-la-disenadora-tras-el-jaguar-y-el-vestido-que-petro-llevo-a-ee-uu-como-regalos-a-donald-y-melania-trump/ |
| 990526 | 2026-02-08 | NP | https://www.las2orillas.co/el-chileno-de-alejandro-weinstein-que-destrono-a-los-minski-de-procaps-esta-en-lios-con-otra-de-sus-empresas/ |
| 990608 | 2026-02-10 | NP | https://www.las2orillas.co/la-pelea-que-lleva-10-anos-en-colombia-por-los-millonarios-derechos-de-la-obra-de-la-pintora-frida-khalo/ |
| 990753 | 2026-02-10 | N | https://www.las2orillas.co/juan-acevedo-polemico-presidente-de-urra-lleva-mas-de-30-anos-en-la-empresa-que-lo-pensiono/ |
| 990799 | 2026-02-10 | NP | https://www.las2orillas.co/el-fracaso-de-4-vias-claves-que-poderosos-concesionarios-privados-no-lograron-construir/ |
| 990810 | 2026-02-11 | N | https://www.las2orillas.co/petro-reforzo-la-junta-ecopetrol-con-2-ambientalistas-para-asegurar-el-fin-del-contrato-de-fracking-con-la-oxy-en-eeuu/ |
| 990832 | 2026-02-11 | NP | https://www.las2orillas.co/asi-funciona-el-negocio-de-las-vallas-publicitarias-quienes-mandan-en-bogota/ |
| 990853 | 2026-02-11 | X | https://www.las2orillas.co/petro-responde-al-video-en-gorgona-y-asi-defiende-su-vida-privada-ante-los-rumores-de-que-tiene-nueva-novia/ |
| 990848 | 2026-02-11 | I | https://www.las2orillas.co/el-negociazo-que-monto-abelardo-de-la-espriella-con-su-campana-relojes-costosos-y-esculturas-de-millones/ |
| 990956 | 2026-02-12 | N | https://www.las2orillas.co/gloria-gaitan-con-88-anos-y-los-otros-veteranos-que-junto-a-uribe-y-robledo-buscan-curul-en-el-senado/ |
| 991073 | 2026-02-12 | NP | https://www.las2orillas.co/por-que-los-arabes-que-se-quedaron-con-coscuez-la-rica-mina-de-esmeraldas-de-carranza-tiraron-la-toalla-y-se-van/ |
| 991211 | 2026-02-13 | N | https://www.las2orillas.co/silvana-guerrero-la-comandante-del-frente-mas-duro-del-eln-que-le-huye-a-los-bombardeos-de-petro-en-el-catatumbo/ |
| 990978 | 2026-02-14 | NP | https://www.las2orillas.co/dictador-un-ron-con-un-siglo-de-tradicion-que-el-cartagenero-hernan-parra-revivio-con-calidad-y-precio-hace-20-anos/ |
| 991195 | 2026-02-15 | NP | https://www.las2orillas.co/como-los-canadienses-se-quedaron-con-el-oro-de-santurban-y-sacaron-del-camino-a-los-arabes-que-le-apostaron-primero/ |
| 991569 | 2026-02-16 | NP | https://www.las2orillas.co/nuevo-reves-para-epm-y-sus-poderosos-abogados-en-el-caso-de-hidroituango-tiene-que-pagar-multa-por-781-mil-millones/ |
| 991699 | 2026-02-17 | N | https://www.las2orillas.co/aparecio-el-hijo-de-petro-asilado-en-canada-al-que-le-pico-la-politica/ |
| 991876 | 2026-02-18 | NP | https://www.las2orillas.co/el-fracaso-del-abogado-ivan-cancino-no-pudo-evitar-que-la-interpol-se-fuera-con-toda-contra-carlos-ramon-gonzalez/ |
| 991891 | 2026-02-18 | N | https://www.las2orillas.co/un-pastor-gringo-con-vinculos-religiosos-en-los-laches-de-bogota-le-habla-a-trump-al-oido/ |
| 992135 | 2026-02-20 | NP | https://www.las2orillas.co/una-sociedad-calena-con-franceses-se-quedaron-con-el-contrato-para-operar-el-trasmicable-de-ciudad-bolivar/ |
| 992216 | 2026-02-20 | INT | https://www.las2orillas.co/con-pedida-de-perdon-publica-los-hermanos-rodriguez-dejaran-libres-cientos-de-presos-politicos-en-venezuela/ |
| 991937 | 2026-02-20 | F | https://www.las2orillas.co/el-recorte-de-600-mil-millones-al-canal-del-dique-con-el-que-petro-expone-al-pais-a-gigante-demanda/ |
| 992455 | 2026-02-23 | NP | https://www.las2orillas.co/montesacro-el-consorcio-en-el-que-pesa-una-poderosa-familia-paisa-manejara-los-cementerios-de-bogota/ |
| 992635 | 2026-02-23 | F | https://www.las2orillas.co/quien-es-el-mexicano-a-quien-petro-le-compra-el-glifosato-que-tanto-critico-en-el-que-se-ha-gastado-3-mil-millones/ |
| 992764 | 2026-02-24 | NP | https://www.las2orillas.co/despues-de-13-anos-kiko-gomez-perdio-su-mansion-en-barrancas-el-pueblo-donde-lucho-diaz-aprendio-a-patear-el-balon/ |
| 992821 | 2026-02-25 | NP | https://www.las2orillas.co/rotorr-como-logro-un-grupo-de-profesores-de-la-u-nacional-poner-el-conocimiento-y-la-academia-al-servicio-de-la-sociedad/ |
| 992846 | 2026-02-26 | N | https://www.las2orillas.co/dura-pelea-entre-cepeda-y-roy-barreras-por-los-dirigentes-sindicales-colombianos/ |
| 992940 | 2026-02-26 | F | https://www.las2orillas.co/apoyado-por-un-obediente-gabinete-petro-le-dio-un-empujon-a-la-asamblea-constituyente/ |
| 992985 | 2026-02-26 | NP | https://www.las2orillas.co/los-2-millonarios-que-fueron-duenos-de-bancolombia-antes-de-que-fuera-controlado-por-el-grupo-empresarial-antioqueno/ |
| 993124 | 2026-02-27 | F | https://www.las2orillas.co/al-banquillo-la-junta-directiva-de-isa-que-nombro-de-manera-irregular-a-jorge-carrillo-presidente-de-la-compania/ |
| 993305 | 2026-03-02 | N | https://www.las2orillas.co/el-poder-de-petro-se-impuso-en-urra-y-la-junta-manejada-por-el-gobierno-autorizo-recursos-para-las-familias-afectadas/ |
| 993442 | 2026-03-02 | NP | https://www.las2orillas.co/como-fue-la-operacion-que-llevo-a-asesinar-de-un-golpe-al-ayatola-supremo-y-a-10-hombres-de-su-poderosa-cupula/ |
| 993531 | 2026-03-02 | NP | https://www.las2orillas.co/la-megacarcel-de-alta-seguridad-inspirada-la-de-bukele-que-se-construye-en-medellin-con-la-que-fico-saca-pecho/ |
| 993582 | 2026-03-03 | N | https://www.las2orillas.co/la-millonada-que-petro-les-dara-a-los-taxistas-para-cambiar-su-viejo-amarillito-a-gasolina-por-uno-electrico/ |
| 993554 | 2026-03-03 | N | https://www.las2orillas.co/quienes-son-los-asesores-que-le-hablan-al-oido-a-ivan-cepeda-el-candidato-presidencial-que-lidera-las-encuestas/ |
| 993612 | 2026-03-03 | NP | https://www.las2orillas.co/la-empresa-espanola-que-se-encargara-de-consolidar-y-dar-legalidad-a-los-resultados-electorales-del-proximo-8-de-marzo/ |
| 993767 | 2026-03-04 | N | https://www.las2orillas.co/que-es-lo-que-segun-abelardo-de-la-espriella-no-tiene-arreglo-en-juan-daniel-oviedo-un-nuevo-ataque-del-abogado/ |
| 993766 | 2026-03-04 | NP | https://www.las2orillas.co/la-nueva-subasta-en-bogota-donde-encontrara-obras-desde-100-mil-hasta-cuadros-de-botero-que-arrancan-en-70-millones/ |
| 993877 | 2026-03-04 | N | https://www.las2orillas.co/las-4-peleas-virales-que-ha-casado-abelardo-de-la-espriella-con-otros-politicos-en-colombia/ |
| 993975 | 2026-03-05 | F | https://www.las2orillas.co/los-escandalos-de-cuba-gooding-jr-la-estrella-de-la-pelicula-sobre-el-almirante-padilla-que-financio-el-gobierno-petro/ |
| 994034 | 2026-03-05 | NP | https://www.las2orillas.co/aida-merlano-y-julio-gerlein-un-oculto-romance-que-termino-en-tribunales-juicios-y-carcel/ |
| 994058 | 2026-03-05 | N | https://www.las2orillas.co/gustavo-petro-y-otros-cuatro-presidentes-latinoamericanos-no-fueron-invitados-por-trump-a-una-cumbre-en-miami/ |
| 994069 | 2026-03-06 | NP | https://www.las2orillas.co/las-mas-de-1000-quejas-que-tienen-a-los-venezolanos-de-farmatodo-bajo-investigacion/ |
| 994048 | 2026-03-06 | NP | https://www.las2orillas.co/los-sudafricanos-de-anglogold-ashanti-perdieron-su-millonaria-inversion-en-la-mina-de-oro-la-colosa-en-el-tolima/ |
| 993048 | 2026-03-07 | N | https://www.las2orillas.co/los-30-candidatos-mas-cuestionados-que-aspiran-al-senado/ |
| 993402 | 2026-03-08 | N | https://www.las2orillas.co/desde-las-regiones-20-candidatos-cuestionados-de-seis-partidos-politicos-aspiran-a-llegar-a-la-camara-de-representantes/ |
| 983961 | 2026-03-08 | N | https://www.las2orillas.co/el-es-tomas-rodriguez-el-esposo-de-paloma-valencia-la-nueva-candidata-presidencial-del-centro-democratico/ |
| 985629 | 2026-03-08 | N | https://www.las2orillas.co/de-un-duelo-en-su-ninez-claudia-lopez-saco-la-fuerza-para-dar-las-batallas-politicas-que-no-siempre-gana/ |
| 994352 | 2026-03-08 | N | https://www.las2orillas.co/el-outsider-juan-daniel-oviedo-el-palo-en-la-gran-consulta-por-colombia-en-la-que-se-impuso-paloma-valencia/ |
| 994364 | 2026-03-08 | N | https://www.las2orillas.co/estos-son-los-9-candidatos-que-junto-a-cepeda-y-de-la-espriella-estaran-en-la-pelea-por-la-presidencia-de-colombia/ |
| 994375 | 2026-03-09 | N | https://www.las2orillas.co/uribe-polo-polo-angelica-lozano-y-robledo-entre-los-grandes-quemados-que-dejo-la-eleccion-al-congreso/ |
| 994343 | 2026-03-09 | N | https://www.las2orillas.co/los-senadores-del-centro-democratico-escogidos-para-el-periodo-2026-2030/ |
| 994402 | 2026-03-09 | N | https://www.las2orillas.co/dos-candidatos-sin-maquinaria-jp-hernandez-y-enrique-gomez-apoyado-por-abelardo-estan-en-los-10-senadores-mas-votados/ |
| 994442 | 2026-03-09 | N | https://www.las2orillas.co/los-representantes-a-la-camara-de-uribe-de-la-espriella-y-alejandro-char-se-alzaron-con-la-mayor-cantidad-de-votos/ |
| 994484 | 2026-03-09 | NP | https://www.las2orillas.co/los-2-amigos-de-trump-que-hicieron-monona-con-el-petroleo-en-venezuela-ahora-quieren-repetir-en-cuba/ |
| 994517 | 2026-03-09 | N | https://www.las2orillas.co/ella-es-aida-quilcue-la-indigena-que-acompanara-a-ivan-cepeda-como-su-vicepresidenta/ |
| 994602 | 2026-03-10 | N | https://www.las2orillas.co/quien-es-el-negro-de-tumaco-que-logro-quitarle-la-curul-afro-en-la-camara-al-polemico-polo-polo/ |
| 994629 | 2026-03-10 | N | https://www.las2orillas.co/una-cristiana-del-poderoso-g12-de-los-esposos-castellanos-le-puso-los-votos-al-partido-de-abelardo-en-bogota/ |
| 994613 | 2026-03-10 | N | https://www.las2orillas.co/veronica-alcocer-se-volvio-a-montar-en-el-avion-presidencial-y-estuvo-con-el-presidente-en-la-votacion-del-8-de-marzo/ |
| 994910 | 2026-03-12 | NP | https://www.las2orillas.co/la-caida-de-los-manzur-la-poderosa-familia-conservadora-de-cordoba-que-termino-muy-mal/ |
| 995082 | 2026-03-13 | X | https://www.las2orillas.co/el-neurocirujano-que-intento-salvar-a-miguel-uribe-ya-tendra-donde-rezarle-a-san-charbel-el-santo-al-que-le-tiene-fe/ |
| 992749 | 2026-03-15 | NP | https://www.las2orillas.co/empresarios-venezolanos-duenos-de-fortunas-tradicionales-como-los-cisneros-estan-de-regreso-a-invertir-en-su-pais/ |
| 995048 | 2026-03-16 | NP | https://www.las2orillas.co/por-que-la-crisis-en-medio-oriente-puede-golpear-el-gas-y-la-energia-en-colombia/ |
| 995318 | 2026-03-16 | N | https://www.las2orillas.co/el-gerente-de-corferias-que-petro-intento-tumbar-arranca-con-la-gran-remodelacion-del-recinto-ferial/ |
| 995415 | 2026-03-17 | NP | https://www.las2orillas.co/la-odisea-de-construir-un-puerto-en-el-golfo-de-uraba-que-lidero-el-vallecaucano-oscar-isaza-empezo-a-dar-frutos/ |
| 995667 | 2026-03-19 | F | https://www.las2orillas.co/el-desplome-de-ecopetrol-y-la-disparada-del-grupo-exito-de-los-callejas-y-nutresa-de-gilinski-en-ganancias/ |
| 995736 | 2026-03-20 | INT | https://www.las2orillas.co/con-la-descabezada-de-padrino-y-la-salida-de-7-ministros-nombrados-por-maduro-delcy-toma-las-riendas-de-venezuela/ |
| 995460 | 2026-03-20 | N | https://www.las2orillas.co/eutoquio-timote-el-tolimense-que-hace-un-siglo-se-convirtio-en-el-primer-indigena-en-ser-candidato-a-la-presidencia/ |
| 995877 | 2026-03-20 | FIl | https://www.las2orillas.co/las-cuentas-de-las-elecciones-no-le-cuadran-a-petro-y-le-pidio-a-la-fiscal-luz-adriana-camargo-que-intervenga/ |
| 995377 | 2026-03-20 | N | https://www.las2orillas.co/las-7-eps-que-tienen-sus-cuentas-en-rojo-y-estan-en-la-mira-de-presidente-para-liquidarlas/ |
| 995945 | 2026-03-21 | N | https://www.las2orillas.co/la-captura-de-el-viejo-en-los-llanos-quien-confeso-la-verdad-del-crimen-de-miguel-uribe-turbay/ |
| 993695 | 2026-03-22 | NP | https://www.las2orillas.co/el-punto-clave-del-mar-arabigo-por-donde-pasan-miles-de-barriles-de-peroleo-y-gas-para-el-mundo-que-iran-bloqueo/ |
| 996059 | 2026-03-23 | N | https://www.las2orillas.co/avion-hercules-que-cayo-en-putumayo-llevaba-mas-de-40-anos-volando-y-llego-en-el-gobierno-duque/ |
| 995769 | 2026-03-23 | NP | https://www.las2orillas.co/el-mas-rico-de-filipinas-que-ya-tiene-puerto-en-buenaventura-le-aposto-ahora-a-un-gran-negocio-petrolero-en-colombia/ |
| 996156 | 2026-03-24 | N | https://www.las2orillas.co/seis-gobernadores-y-dos-poderosos-alcaldes-llevaron-a-sus-parientes-y-socios-politicos-al-congreso/ |
| 996185 | 2026-03-25 | F | https://www.las2orillas.co/el-mismo-abogado-que-defendio-a-eduardo-montealegre-de-alvaro-uribe-velez-ahora-esta-con-el-presidente-de-ecopetrol/ |
| 996194 | 2026-03-25 | X | https://www.las2orillas.co/el-tio-matematico-del-ivan-cepeda-un-discreto-profesor-que-acaba-ganarse-el-premio-al-mejor-del-pais/ |
| 996276 | 2026-03-25 | N | https://www.las2orillas.co/obligado-por-la-justicia-alex-florez-la-ficha-de-daniel-quintero-le-dice-adios-al-senado/ |
| 996330 | 2026-03-26 | N | https://www.las2orillas.co/quien-es-martin-revelo-el-duro-presidente-de-la-uso-que-confronto-a-petro-e-insiste-en-la-salida-de-roa/ |
| 996379 | 2026-03-26 | F | https://www.las2orillas.co/los-12-helicopteros-que-ee-uu-le-regalo-a-colombia-y-que-petro-no-califico-de-chatarras-por-haberlos-recibido-el/ |
| 996500 | 2026-03-27 | NP | https://www.las2orillas.co/la-cuantiosa-fortuna-que-mauduro-esconde-y-que-no-quiere-usar-para-pagar-su-defensa/ |
| 996645 | 2026-03-29 | N | https://www.las2orillas.co/quienes-son-los-asesores-y-coequiperos-que-acompanaran-a-paloma-valencia-en-su-camino-a-la-presidencia/ |
| 996660 | 2026-03-30 | NP | https://www.las2orillas.co/megacolegio-de-taganga-elefante-blanco-con-casi-10-mil-millones-perdidos-enfrenta-alcalde-y-gobernadora-del-magdalena/ |
| 996831 | 2026-03-30 | X | https://www.las2orillas.co/dos-colombianos-lideran-el-ranking-de-streamers-en-latinoamerica-en-el-que-tambien-esta-la-presidenta-de-mexico/ |
| 996895 | 2026-03-30 | N | https://www.las2orillas.co/quienes-son-los-5-funcionarios-publicos-escogidos-por-petro-que-tienen-los-mejores-sueldos/ |
| 996900 | 2026-03-31 | NP | https://www.las2orillas.co/un-viejo-conocido-en-la-contratacion-en-el-caribe-se-quedo-con-la-construccion-del-malecon-en-magangue/ |
| 996982 | 2026-03-31 | NP | https://www.las2orillas.co/los-30-congresistas-que-la-corte-suprema-senala-de-intercambiar-su-voto-por-contratos-en-invias/ |
| 996996 | 2026-03-31 | NP | https://www.las2orillas.co/el-duro-informe-de-la-onu-sobre-la-ninez-en-colombia-que-pone-en-jaque-al-pais/ |
| 997024 | 2026-04-01 | N | https://www.las2orillas.co/el-amigo-y-asesor-de-la-espriella-carlos-suarez-de-estrategia-y-poder-gano-por-punta-y-punta-el-pasado-8-de-marzo/ |
| 997102 | 2026-04-01 | N | https://www.las2orillas.co/petro-escogio-aviones-brasileros-para-reemplazar-los-viejos-hercules-como-el-de-la-tragedia-del-putumayo/ |
| 997106 | 2026-04-01 | N | https://www.las2orillas.co/cepeda-paloma-de-la-espriella-y-fajardo-refrescan-sus-mensajes-con-nuevos-videos-a-la-caza-de-votos/ |
| 997320 | 2026-04-02 | N | https://www.las2orillas.co/la-pintura-que-paloma-valencia-tiene-en-su-casa-en-la-que-alvaro-uribe-aparece-como-jesucristo/ |
| 997358 | 2026-04-05 | N | https://www.las2orillas.co/olga-lucia-acosta-el-palo-en-la-rueda-para-las-pretensiones-del-gobierno-con-la-junta-del-banco-de-la-republica/ |
| 997200 | 2026-04-05 | N | https://www.las2orillas.co/la-madrina-politica-de-juan-daniel-oviedo-que-lo-conecto-con-el-centro-democratico-y-el-poder-politico/ |
| 997577 | 2026-04-06 | NP | https://www.las2orillas.co/la-pelea-por-el-control-de-velotax-la-empresa-que-lleva-70-anos-mandando-en-el-tolima/ |
| 997711 | 2026-04-07 | N | https://www.las2orillas.co/liberales-reunidos-en-el-apartamento-de-gaviria-tienen-algo-claro-para-las-presidenciales-cualquiera-menos-cepeda/ |
| 997724 | 2026-04-07 | F | https://www.las2orillas.co/en-contravia-de-petro-sus-alfiles-en-la-junta-de-ecopetrol-apoyaron-el-retiro-de-roa-hasta-las-elecciones/ |
| 997718 | 2026-04-08 | F | https://www.las2orillas.co/el-contratista-que-tiene-que-dejar-con-agua-el-colegio-universidad-del-catatumbo-que-petro-inauguro-sin-servicios/ |
| 997835 | 2026-04-08 | N | https://www.las2orillas.co/julian-caicedo-el-caleno-en-el-que-ricardo-roa-se-refugia-en-los-momentos-mas-dificiles/ |
| 997808 | 2026-04-08 | FIl | https://www.las2orillas.co/quien-es-sandra-munoz-la-dama-de-hierro-del-mintrabajo-que-le-puso-tatequieto-a-caracol-y-rtvc-por-casos-de-acoso/ |
| 997869 | 2026-04-08 | NP | https://www.las2orillas.co/al-menos-10-multinacionales-se-le-acomodaron-al-regimen-y-siguen-haciendo-fortuna-en-cuba-pese-al-bloqueo-y-la-crisis/ |
| 997932 | 2026-04-09 | N | https://www.las2orillas.co/colombia-veinte-anos-de-gobiernos-calificados-como-malos-en-la-administracion-publica-segun-el-banco-mundial/ |
| 997968 | 2026-04-09 | N | https://www.las2orillas.co/el-imperio-de-droguerias-creado-por-los-rodriguez-orejuela-que-ahora-petro-usara-para-que-las-eps-entreguen-medicamentos/ |
| 998020 | 2026-04-10 | NP | https://www.las2orillas.co/quienes-son-los-duenos-de-las-encuestadoras-que-pesan-en-la-decision-final-de-por-quien-votar-en-colombia/ |
| 998200 | 2026-04-11 | NP | https://www.las2orillas.co/alvaro-leyva-da-la-cara-frente-al-caso-de-los-pasaportes-y-enfrenta-nuevamente-al-presidente/ |
| 998089 | 2026-04-12 | NP | https://www.las2orillas.co/el-despegue-del-puerto-de-tumaco-despues-de-decadas-de-postracion/ |
| 997941 | 2026-04-13 | NP | https://www.las2orillas.co/un-restaurante-en-panama-es-el-lugar-de-encuentro-de-ricos-colombianos-que-han-salido-del-pais-por-las-medidas-de-petro/ |
| 998378 | 2026-04-13 | N | https://www.las2orillas.co/la-pelea-entre-paloma-valencia-y-abelardo-de-la-espriella-por-el-voto-caribe-esta-caliente-la-candidata-anoto-un-round/ |
| 998410 | 2026-04-14 | NP | https://www.las2orillas.co/los-empresarios-caldenses-duros-de-los-detergentes-que-lograon-venderle-sus-productos-a-dos-competidores-exito-y-d1/ |
| 998503 | 2026-04-14 | N | https://www.las2orillas.co/la-toma-de-carlos-amaya-del-partido-verde-que-aplasto-a-las-minorias-para-irse-con-ivan-cepeda/ |
| 998593 | 2026-04-15 | N | https://www.las2orillas.co/petro-escogio-a-4-ex-alumnos-de-su-universidad-para-la-corte-permanente-de-arbitraje-internacional/ |
| 998650 | 2026-04-16 | N | https://www.las2orillas.co/el-presidente-encargado-de-ecopetrol-se-distancia-de-roa-y-de-petro-y-no-frenara-proyectos-claves/ |
| 998683 | 2026-04-16 | N | https://www.las2orillas.co/petro-lula-y-claudia-sheinbaum-en-la-cumbre-de-los-progresistas-en-espana-y-ausentes-de-la-convocada-por-trump/ |
| 998729 | 2026-04-16 | N | https://www.las2orillas.co/un-abogado-barranquillero-logro-la-libertad-de-la-exesposa-de-nicolas-petro-quien-destapo-sus-delitos/ |
| 998755 | 2026-04-17 | N | https://www.las2orillas.co/en-medio-de-la-campana-presidencial-con-de-la-espriella-en-la-carrera-su-bufete-escoge-un-nuevo-director/ |
| 999173 | 2026-04-20 | NP | https://www.las2orillas.co/un-hospital-publico-del-valle-logro-unas-millonarias-utilidades-similares-a-las-prepagadas-de-colmedica-y-colsanitas-ips/ |
| 999185 | 2026-04-20 | N | https://www.las2orillas.co/la-voltereta-de-mauricio-pava-que-paso-de-ser-el-abogado-de-benedetti-petro-y-sarabia-a-la-campana-de-fajardo/ |
| 999378 | 2026-04-21 | N | https://www.las2orillas.co/el-congresista-conservador-que-vio-en-ivan-cepeda-su-tabla-de-salvacion-y-ahora-quedo-en-el-limbo/ |
| 999377 | 2026-04-21 | F | https://www.las2orillas.co/como-el-mindefensa-pedro-sanchez-termino-con-2-viceministras-inexpertas-que-llegaron-a-pagar-favores-politicos/ |
| 999402 | 2026-04-22 | N | https://www.las2orillas.co/bukele-y-claudia-sheinbaum-polos-opuestos-y-con-la-mejor-imagen-petro-lejos-del-top/ |
| 999412 | 2026-04-22 | I | https://www.las2orillas.co/el-hijo-de-augusto-rodriguez-director-de-la-unp-que-sacude-la-campana-de-cepeda-por-supuestos-apoyos-desde-el-gobierno/ |
| 999477 | 2026-04-22 | NP | https://www.las2orillas.co/una-empresa-extranjera-de-muchos-anos-en-colombia-es-la-que-mejor-le-paga-a-los-miembros-de-su-junta-directiva/ |
| 999540 | 2026-04-22 | N | https://www.las2orillas.co/ninos-y-ninas-pusieron-sobre-la-mesa-el-gasto-publico-y-la-educacion-en-conversacion-con-candidatos-a-la-presidencia/ |
| 1000001 | 2026-04-27 | F | https://www.las2orillas.co/duelo-de-titanes-entre-3-pesados-abogados-involucrados-en-el-negocio-del-apartamento-901-del-expresidente-de-ecopetrol/ |
| 1000061 | 2026-04-27 | F | https://www.las2orillas.co/con-parrandon-de-cumpleanos-en-valledupar-juliana-guerrero-quiso-bailarse-las-graves-acusaciones-de-angie-rodriguez/ |
| 1000285 | 2026-04-29 | F | https://www.las2orillas.co/la-alta-funcionaria-que-petro-mantiene-atornillada-en-el-cargo-llevo-a-dos-de-los-suyos-a-rendir-cuentas-en-el-congreso/ |
| 1000316 | 2026-04-29 | N | https://www.las2orillas.co/el-expresidente-gaviria-no-logro-unificar-a-los-liberales-alrededor-de-paloma-valencia-estos-dijeron-no/ |
| 1000461 | 2026-05-01 | F | https://www.las2orillas.co/gran-favor-de-petro-a-otra-amiga-de-veronica-alcocer-le-entrego-la-notaria-35/ |
| 1000445 | 2026-05-02 | N | https://www.las2orillas.co/el-reelecto-senador-de-cambio-radical-didier-lobo-y-aliado-de-paloma-que-tendra-que-rendir-cuentas-ante-la-justicia/ |
| 1000542 | 2026-05-03 | F | https://www.las2orillas.co/petro-le-mete-el-acelerador-a-la-constituyente-y-empieza-a-pedir-donaciones-desde-su-cuenta-x/ |
| 1000457 | 2026-05-03 | N | https://www.las2orillas.co/el-lado-costeno-de-ivan-cepeda-por-su-abuela-aurita-chadid-que-lo-hace-familia-de-los-guerra-los-name-y-otros/ |
| 1000850 | 2026-05-05 | NP | https://www.las2orillas.co/entre-el-poder-y-el-abandono-la-mansion-de-kiko-gomez-que-el-estado-intenta-rescatar/ |
| 1000981 | 2026-05-06 | N | https://www.las2orillas.co/senadores-conservadores-jugarian-a-dos-bandas-en-los-apoyos-a-de-la-espriella-y-a-paloma/ |
| 1001091 | 2026-05-07 | F | https://www.las2orillas.co/asi-fue-como-katherine-miranda-se-le-atraveso-a-petro-y-su-plan-de-mandar-millones-de-afiliados-a-la-nueva-eps/ |
| 1001323 | 2026-05-08 | X | https://www.las2orillas.co/el-cancer-que-apago-la-vida-de-german-vargas-lleras/ |
| 1001201 | 2026-05-11 | N | https://www.las2orillas.co/el-pacto-entre-asocana-los-ingenios-azucareros-indigenas-y-gobierno-que-empieza-a-transformar-el-norte-del-cauca/ |
| 1001333 | 2026-05-11 | F | https://www.las2orillas.co/los-millonarios-contratos-detras-de-la-familia-del-tesorero-de-la-constituyente-de-petro/ |
| 1001892 | 2026-05-14 | F | https://www.las2orillas.co/la-caida-de-juan-gonzalo-castano-el-directivo-que-el-gobierno-saco-de-ecopetrol-por-oponerse-a-roa/ |
| 1001973 | 2026-05-14 | N | https://www.las2orillas.co/los-contrastes-de-la-campana-de-abelardo-de-la-espriella-en-medellin-con-lleno-total-y-denuncias-de-intimidacion/ |
| 1001991 | 2026-05-15 | NP | https://www.las2orillas.co/la-inesperada-derrota-de-la-gigante-studio-f-frente-a-una-firma-calena-de-creditos-y-finanzas/ |
| 1002031 | 2026-05-15 | NP | https://www.las2orillas.co/el-plan-de-la-alcaldia-de-cali-que-incluye-10-obras-con-las-que-buscan-cambiarle-la-cara-a-la-ciudad/ |
| 1002566 | 2026-05-21 | NP | https://www.las2orillas.co/dos-costosos-abogados-expertos-en-negociar-con-la-justicia-gringa-defienden-a-alex-saab/ |
| 1002582 | 2026-05-21 | N | https://www.las2orillas.co/la-cifra-de-observadores-internacionales-que-estaran-en-las-elecciones-presidenciales-ya-supero-la-de-2022/ |
| 1002086 | 2026-05-22 | NP | https://www.las2orillas.co/desenmascaran-red-delictiva-para-no-pagar-deudas-y-estafar-a-acreedores-el-cartel-de-la-insolvencia/ |
| 1002845 | 2026-05-23 | NP | https://www.las2orillas.co/la-historica-cifra-de-testigos-electorales-en-el-exterior-que-fueron-acreditados-para-las-presidenciales-del-31-de-mayo/ |
| 1002866 | 2026-05-23 | I | https://www.las2orillas.co/quien-es-el-estratega-de-paloma-valencia-senalado-de-ser-un-experto-desinformando-en-redes/ |
| 1002979 | 2026-05-25 | X | https://www.las2orillas.co/la-pelea-de-poder-en-el-prestigioso-liceo-frances-de-bogota-que-tiene-en-riesgo-el-apoyo-del-gobierno-macron/ |
| 1003119 | 2026-05-26 | N | https://www.las2orillas.co/la-olvidada-conversacion-entre-ivan-cepeda-y-de-la-espriella-entre-risas-elogios-y-guinos-a-timochenko/ |
| 1003011 | 2026-05-26 | N | https://www.las2orillas.co/el-cartagenero-detras-de-la-subasta-de-la-central-termica-que-irrito-a-petro/ |
| 1003215 | 2026-05-27 | NP | https://www.las2orillas.co/como-un-abogado-y-empresario-se-convirtio-en-uno-de-los-fenomenos-politicos-mas-visibles-de-la-campana-presidencial-2026/ |
| 1003280 | 2026-05-28 | NP | https://www.las2orillas.co/luis-carlos-sarmiento-con-promigas-entro-a-las-grandes-ligas-de-la-energia-solar-en-colombia/ |
| 1003679 | 2026-05-31 | N | https://www.las2orillas.co/abelardo-de-la-espriella-sorprende-y-supera-a-ivan-cepeda-el-candidato-del-gobierno-y-el-favorito-de-las-encuestas/ |
| 1003683 | 2026-05-31 | M | https://www.las2orillas.co/abelardo-de-la-espriella-el-antipolitico-que-se-conecto-con-el-pais-y-gano/ |
| 1003691 | 2026-05-31 | N | https://www.las2orillas.co/como-logro-ivan-cepeda-dar-el-salto-de-una-curul-en-el-senado-a-estar-peleando-por-la-casa-de-narino/ |
| 1003699 | 2026-06-01 | N | https://www.las2orillas.co/el-fracaso-de-las-encuestas-todas-dieron-a-cepeda-ganador-y-no-vieron-el-desplome-de-paloma/ |
| 1003736 | 2026-06-01 | N | https://www.las2orillas.co/cepeda-triunfo-en-europa-pero-de-la-espriella-se-impuso-en-eeuu-fueron-569-000-los-colombianos-votantes-en-el-exterior/ |
| 1003789 | 2026-06-01 | N | https://www.las2orillas.co/bogota-le-dio-la-victoria-a-cepeda-pero-no-consiguio-los-2-millones-de-votos-que-se-habian-propuesto/ |
| 1003784 | 2026-06-02 | N | https://www.las2orillas.co/cuantos-millones-pueden-recibir-los-4-candidatos-mas-votados-para-cubrir-los-gastos-de-sus-campanas/ |
| 1004042 | 2026-06-04 | N | https://www.las2orillas.co/la-popular-alcaldesa-de-ibague-que-enfrento-a-petro-esta-enredada-con-la-justicia/ |
| 1004106 | 2026-06-04 | COM | https://www.las2orillas.co/mas-de-11-billones-invertidos-desde-2022-entre-las-cifras-que-dejo-la-gestion-del-gobierno-petro-en-la-salud-colombiana/ |
| 1004148 | 2026-06-04 | FIRM | https://www.las2orillas.co/la-cuestionada-senadora-que-impulsa-a-ivan-cepeda-en-la-guajira/ |
| 1004219 | 2026-06-05 | REIMP | https://www.las2orillas.co/quienes-eran-los-los-12-apostoles-el-grupo-paramilitar-por-el-que-condenaron-a-santiago-uribe/ |
| 1004258 | 2026-06-05 | N | https://www.las2orillas.co/quienes-son-las-army-y-las-kpopers-que-son-tendencia-en-redes-y-ahora-respaldan-a-ivan-cepeda/ |
| 1004465 | 2026-06-08 | N | https://www.las2orillas.co/petro-le-dijo-adios-al-esquema-de-seguridad-de-uribe-que-costaba-casi-1-500-millones-anuales/ |
| 1004582 | 2026-06-09 | NP | https://www.las2orillas.co/la-exreina-gabriela-tafur-consiguio-que-el-dueno-de-nubank-le-apostara-a-sus-micro-dramas/ |
| 1004590 | 2026-06-09 | NP | https://www.las2orillas.co/la-otra-empresa-de-los-hermanos-bautista-de-thomas-greg-que-se-ocupa-de-la-identificacion-de-los-votantes/ |
| 1004757 | 2026-06-10 | N | https://www.las2orillas.co/las-fechas-claves-del-cne-para-la-postulacion-de-testigos-y-observadores-electorales-para-las-elecciones-del-21-de-junio/ |
| 1004791 | 2026-06-13 | N | https://www.las2orillas.co/un-chileno-junto-a-abelardo-y-un-antiguo-asesor-de-petro-que-esta-con-cepeda-lideran-la-batalla-digital/ |
| 1005176 | 2026-06-15 | NP | https://www.las2orillas.co/premiados-los-cafeteros-del-huila-con-un-gran-centro-en-gigante-que-prepara-la-fruta-para-su-venta-y-exportacion/ |
| 1005042 | 2026-06-15 | N | https://www.las2orillas.co/el-amigo-del-tino-asprilla-que-estuvo-detras-del-video-de-las-estrellas-colombianas-apoyando-a-de-la-espriella/ |
| 1005257 | 2026-06-16 | N | https://www.las2orillas.co/el-ultimo-cartucho-de-ivan-cepeda-para-empujar-su-estrategia-digital-que-no-ha-logrado-despegar/ |
| 1005359 | 2026-06-16 | CAMP | https://www.las2orillas.co/el-triunfo-de-abelardo-de-la-espriella-y-jose-manuel-restrepo-en-primera-vuelta-han-despertado-confianza-internacional/ |
| 1005711 | 2026-06-19 | N | https://www.las2orillas.co/por-que-veronica-alcocer-termino-viviendo-en-suecia-lo-mas-lejos-posible-de-petro-y-en-medio-de-escandalos/ |
| 1005901 | 2026-06-21 | N | https://www.las2orillas.co/de-la-espriella-gana-la-presidencia-de-colombia-un-outsider-llega-a-la-casa-de-narino-por-un-estrecho-margen-de-votos/ |
| 1005863 | 2026-06-21 | M | https://www.las2orillas.co/el-camino-de-abelardo-de-la-espriella-para-lograr-la-presidencia-de-colombia-en-6-meses/ |
| 1005916 | 2026-06-21 | FIl | https://www.las2orillas.co/somos-la-mitad-de-colombia-y-no-vamos-a-dejar-enterrar-nuestras-conquistas-sociales-y-de-derechos-cepeda/ |
| 1005900 | 2026-06-22 | FDl | https://www.las2orillas.co/asi-se-construyo-la-estrategia-del-tigre-una-marca-mas-alla-del-propio-abelardo-de-la-espriella/ |
| 1005850 | 2026-06-22 | N | https://www.las2orillas.co/el-camino-de-ivan-cepeda-a-una-presidencia-que-se-le-escapo-por-250-mil-votos/ |
| 1005946 | 2026-06-22 | N | https://www.las2orillas.co/ivan-cepeda-supero-a-petro-y-se-convierte-en-el-candidato-mas-votado-de-la-izquierda-en-colombia/ |
| 1005986 | 2026-06-22 | N | https://www.las2orillas.co/misael-pastrana-turbay-y-samper-lograron-la-presidencia-con-una-diferencia-menor-a-la-de-abelardo-y-cepeda/ |
| 1004891 | 2026-06-22 | NP | https://www.las2orillas.co/panama-el-nuevo-escenario-de-negocios-de-luis-carlos-sarmiento-angulo-a-donde-traslado-del-52-de-corficolombiana/ |
| 1006292 | 2026-06-25 | N | https://www.las2orillas.co/el-parque-solar-en-neiva-que-estrena-la-primera-licencia-ambiental-expres-un-empeno-de-la-ministra-irene-velez/ |
| 1006585 | 2026-06-26 | N | https://www.las2orillas.co/rosa-aguilar-aragon-la-wayuu-que-recibio-al-presidente-electo-en-su-primera-visita-a-riohacha/ |
| 1006617 | 2026-06-26 | N | https://www.las2orillas.co/una-vieja-amistad-con-de-la-espriella-y-una-apuesta-dura-por-el-tigre-tienen-a-rodrigo-lara-en-el-gabinete-ministerial/ |
| 997800 | 2026-06-29 | NP | https://www.las2orillas.co/industrias-la-victoria-de-la-tradicion-molinera-al-liderazgo-en-el-sector-de-aseo-y-cuidado-personal/ |
| 1006771 | 2026-06-29 | N | https://www.las2orillas.co/de-la-espriella-le-suelta-el-empalme-al-vicepresidente-restrepo-mientras-visita-cuatro-emblematicos-santuarios/ |
| 1006895 | 2026-06-30 | NP | https://www.las2orillas.co/cuando-los-holandeses-de-makro-aterrizaron-en-colombia-hace-30-anos-a-hacerle-competencia-a-los-paisas-de-alkosto/ |
| 1007052 | 2026-07-01 | F | https://www.las2orillas.co/puntillazo-de-petro-a-la-negociacion-con-el-clan-del-golfo-firmo-la-extradicion-de-chiquito-malo/ |
| 1007385 | 2026-07-05 | N | https://www.las2orillas.co/la-cuota-liberal-del-gobierno-petro-busca-un-nuevo-espacio-en-el-congreso/ |
| 1007415 | 2026-07-05 | N | https://www.las2orillas.co/de-la-espriella-anuncia-la-creacion-de-un-bloque-de-defensa-para-la-seguridad-urbana-desde-su-primer-dia-de-gobierno/ |
| 1007558 | 2026-07-07 | X | https://www.las2orillas.co/petronio-agroexpo-la-feria-de-cali-entre-los-mas-de-40-eventos-que-tendra-la-ciudad-en-el-segundo-semestre-de-2026/ |
| 1007584 | 2026-07-07 | FIRM | https://www.las2orillas.co/los-aciertos-que-tuvo-la-malograda-paz-total-de-gustavo-petro/ |
| 1007638 | 2026-07-08 | N | https://www.las2orillas.co/la-primera-banda-criminal-que-se-entregara-ante-el-ultimatum-de-de-la-espriella-la-cual-tiene-azotada-a-barranquilla/ |
| 1007858 | 2026-07-09 | N | https://www.las2orillas.co/el-abogado-que-volvio-el-alegato-de-petro-contra-la-eleccion-de-de-la-espriella-a-una-demanda-de-nulidad/ |
| 1007803 | 2026-07-09 | N | https://www.las2orillas.co/comfamiliar-atlantico-la-ultima-de-las-10-cajas-de-compensacion-intervenidas-por-el-gobierno/ |
| 1007881 | 2026-07-09 | N | https://www.las2orillas.co/lagos-de-caujaral-el-exclusivo-club-y-conjunto-residencial-en-barranquilla-desde-donde-despachara-de-la-espriella/ |
| 1007887 | 2026-07-10 | N | https://www.las2orillas.co/de-la-espriella-despachara-desde-barranquilla-como-lo-hizo-rafael-nunez-el-otro-presidente-caribe/ |
| 1008290 | 2026-07-14 | FIRM | https://www.las2orillas.co/el-plan-de-seguridad-de-abelardo-de-la-espriella-despierta-a-los-peores-fantasmas-de-la-violencia-en-colombia/ |
| 1008332 | 2026-07-15 | N | https://www.las2orillas.co/con-2-duros-escuderos-jose-manuel-restrepo-le-dio-la-cara-al-banco-mundial-y-el-fondo-monetario-en-washington/ |
| 1008416 | 2026-07-15 | N | https://www.las2orillas.co/un-trio-de-congresistas-cubanoamericanos-el-gran-apoyo-del-tigre-en-washington/ |
| 1008657 | 2026-07-18 | OP | https://www.las2orillas.co/los-primeros-simbolos-del-poder-revelan-como-gobernara-abelardo-de-la-espriella/ |
| 1008752 | 2026-07-20 | N | https://www.las2orillas.co/el-equipo-economico-del-ex-presidente-duque-aterrizo-en-el-gobierno-del-tigre-y-el-mininterior-escogio-viceministro/ |
| 1008776 | 2026-07-20 | N | https://www.las2orillas.co/la-casa-en-una-urbanizacion-campestre-en-chia-que-gustavo-petro-puso-en-venta-antes-de-dejar-el-poder/ |
| 1008681 | 2026-07-21 | N | https://www.las2orillas.co/son-solo-6-los-embajadores-de-petro-que-han-renunciado-que-esperan-los-demas/ |
| 1008953 | 2026-07-21 | F | https://www.las2orillas.co/por-que-se-disparo-la-mineria-ilegal-en-el-gobierno-de-gustavo-petro/ |
| 1009081 | 2026-07-23 | N | https://www.las2orillas.co/un-congresista-gobiernista-y-otro-de-oposicion-junto-a-15-mas-integran-la-comision-que-juzgara-a-de-la-espriella/ |
| 1009221 | 2026-07-24 | N | https://www.las2orillas.co/los-9-congresistas-que-se-le-habrian-volteado-al-tigre-y-eligieron-presidente-del-senado-al-candidato-de-uribe-y-petro/ |
| 1009290 | 2026-07-24 | COM | https://www.las2orillas.co/mas-de-21-mil-victimas-recibieron-indemnizaciones-por-mas-de-806-mil-millones-durante-el-gobierno-petro/ |
| 1009355 | 2026-07-24 | N | https://www.las2orillas.co/con-remezon-en-la-junta-de-ecopetrol-se-prepara-la-llegada-del-candidato-de-de-la-espriella-para-la-presidencia/ |
| 1009300 | 2026-07-26 | NP | https://www.las2orillas.co/la-millonaria-inversion-de-los-gilinski-en-el-sector-petrolero-coloco-a-dos-de-los-herederos-en-la-junta-de-geopark/ |
| 1009457 | 2026-07-26 | N | https://www.las2orillas.co/el-rumbon-de-abelardo-de-la-espriella-en-las-fiestas-del-mar-en-santa-marta-en-las-que-hizo-gran-promesa/ |
| 1009541 | 2026-07-27 | N | https://www.las2orillas.co/el-dia-que-abelardo-de-la-espriella-dejo-de-ser-ateo-para-convertirse-en-un-ferviente-catolico/ |
| 1009614 | 2026-07-27 | N | https://www.las2orillas.co/que-le-espera-a-colombia-con-abelardo-de-la-espriella-a-partir-del-7-de-agosto/ |
| 1009660 | 2026-07-28 | N | https://www.las2orillas.co/con-bendicion-de-uribe-gabriel-gilinski-y-la-apuesta-al-tigre-pusieron-a-sandra-suarez-directora-de-prosperidad-social/ |
| 1009664 | 2026-07-28 | NP | https://www.las2orillas.co/gilinski-va-con-todo-por-el-mercado-de-50-millones-de-venezolanos-y-detras-de-el-otros-empresarios-prendieron-motores/ |
| 1009807 | 2026-07-29 | NP | https://www.las2orillas.co/el-exfiscal-que-defendio-al-exgobernador-carlos-caicedo-no-logro-salvarlo-de-la-carcel-y-una-multa-de-4-500-millones/ |
| 1009854 | 2026-07-30 | N | https://www.las2orillas.co/dos-poderosas-funcionarias-cercanisimas-a-petro-contrataron-abogados-de-la-cuerda-de-abelardo-de-la-espriella/ |
| 1009898 | 2026-07-30 | NP | https://www.las2orillas.co/con-golpe-a-los-duenos-de-la-sociedad-portuaria-de-buenaventura-cielo-rusinque-alista-su-salida-de-la-superindustria/ |
| 1010029 | 2026-07-31 | NP | https://www.las2orillas.co/asi-se-esta-alistando-el-batallon-paraiso-en-barranquilla-para-ser-la-sede-presidencial-desde-este-7-de-agosto/ |
| 1010313 | 2026-08-03 | F | https://www.las2orillas.co/petro-le-cumplio-a-lula-da-silva-y-acelero-la-compra-de-dos-embraer-kc-390-milennium-366-millones-de-dolares/ |
| 1010387 | 2026-08-04 | N | https://www.las2orillas.co/asi-repartio-petro-10-billones-para-costear-matriculas-gratis-en-las-universidades-la-unad-se-llevo-la-tajada-mayor/ |
| 1010409 | 2026-08-04 | F | https://www.las2orillas.co/portazo-de-de-la-espriella-al-canal-publico-rtvc-que-controla-petro-para-que-no-trasmita-la-posesion-presidencial/ |
| 1010476 | 2026-08-05 | NP | https://www.las2orillas.co/por-que-la-brecha-digital-sigue-sin-desaparecer-pese-a-los-billones-que-colombia-ha-invertido-en-internet/ |
| 1010570 | 2026-08-06 | COM | https://www.las2orillas.co/los-millonarios-hallazgos-que-destapo-la-contraloria-en-contratos-de-defensa-y-que-tienen-un-1-billon-en-el-limbo/ |
| 1010777 | 2026-08-07 | ? | https://www.las2orillas.co/asi-fue-la-llegada-a-cali-de-presidentes-e-invitados-especiales-a-la-posesion-de-abelardo-de-la-espriella/ |
| 1010790 | 2026-08-07 | N | https://www.las2orillas.co/el-colegio-de-sacerdotes-que-hace-32-anos-saco-bachiller-a-abelardo-de-la-espriella/ |
| 1010794 | 2026-08-07 | N | https://www.las2orillas.co/los-funcionarios-que-petro-escogio-para-el-adios-a-la-casa-de-narino-donde-se-colo-el-hijo-de-veronica/ |
| 1010852 | 2026-08-08 | N | https://www.las2orillas.co/de-la-escuela-de-carabineros-a-ibague-la-decision-de-de-la-espriella-que-cambio-la-prision-de-epa-colombia/ |
| 1010858 | 2026-08-09 | NP | https://www.las2orillas.co/como-avianca-se-quedo-con-tampa-la-transportadora-de-carga-fundada-hace-50-anos-en-medellin/ |
| 1010655 | 2026-08-09 | COM | https://www.las2orillas.co/las-irregularidades-por-mas-de-233-mil-millones-que-dejo-la-lupa-de-la-contraloria-sobre-el-sector-trabajo/ |
| 1011028 | 2026-08-10 | COM | https://www.las2orillas.co/los-casi-57-mil-millones-en-irregularidades-que-encontro-la-contraloria-al-revisar-las-cuentas-ambientales-de-colombia/ |
| 1011513 | 2026-08-13 | N | https://www.las2orillas.co/de-la-espriella-le-entrega-una-responsabilidad-mayor-a-un-cercano-de-ivan-duque-que-trabajo-en-su-bufete/ |
| 1011616 | 2026-08-13 | N | https://www.las2orillas.co/eva-ferrer-destapa-la-banda-de-los-3-empoderados-por-veronica-alcocer-que-mandaban-en-la-casa-de-narino/ |
| 1011696 | 2026-08-14 | X | https://www.las2orillas.co/el-petronio-no-sono-en-cali-pero-los-ganadores-de-2024-se-unieron-a-juanpis-para-convertir-la-tragedia-en-solidaridad/ |
| 1011755 | 2026-08-14 | FDl | https://www.las2orillas.co/el-embajador-de-suecia-y-otros-cuatro-quisieron-atornillarse-al-cargo-y-el-tigre-los-declaro-insubsistentes/ |
| 1010718 | 2026-08-16 | NP | https://www.las2orillas.co/la-familia-paisa-que-resiste-a-venderle-a-multinacionales-y-sigue-jugando-duro-en-el-negocio-de-las-salsas-en-colombia/ |
| 1011838 | 2026-08-17 | N | https://www.las2orillas.co/los-once-senadores-que-no-quieren-que-petro-no-salga-bien-del-pais/ |
| 1011835 | 2026-08-17 | F | https://www.las2orillas.co/dos-abogadas-del-bufete-de-la-espriella-lawyers-sin-experiencia-en-el-sector-publico-saltan-al-alto-gobierno/ |
| 1011694 | 2026-08-18 | N | https://www.las2orillas.co/una-barranquillera-que-suma-la-cercania-de-su-papa-el-petrolero-federico-restrepo-con-el-presidente-sera-vicecanciller/ |
| 1012565 | 2026-08-22 | X | https://www.las2orillas.co/la-abogada-exesposa-de-abelardo-de-la-espriella-al-que-su-exmarido-le-tiro-un-buen-salvavidas/ |
| 1012572 | 2026-08-22 | N | https://www.las2orillas.co/aterrizada-de-jets-privados-en-barranquilla-para-cita-de-los-grandes-cacaos-con-el-presidente-de-la-espriella/ |
| 1012654 | 2026-08-24 | N | https://www.las2orillas.co/por-que-colombia-podria-pagar-mas-por-la-energia-en-los-proximos-anos-la-alerta-de-la-contraloria/ |
| 1012671 | 2026-08-24 | N | https://www.las2orillas.co/salen-los-tres-delegados-de-petro-de-la-camara-de-comercio-de-bogota-y-se-le-despeja-el-camino-a-maria-paula-correa/ |
| 1010474 | 2026-08-26 | NP | https://www.las2orillas.co/yuno-empresa-digital-creada-por-dos-ex-rappi-que-compite-con-los-gigantes-mundiales-de-pagos/ |
| 1012881 | 2026-08-26 | F | https://www.las2orillas.co/a-excepcion-de-minhacienda-y-el-canciller-todos-los-ministros-de-de-la-espriella-llegan-endeudados/ |
| 1013009 | 2026-08-27 | N | https://www.las2orillas.co/a-quienes-puso-petro-a-manejar-las-lujosas-oficinas-de-procolombia-en-el-exterior-que-el-tigre-va-a-acabar/ |
| 1012840 | 2026-08-28 | N | https://www.las2orillas.co/el-entusiasmo-del-presidente-de-la-espriella-con-la-orinoquia-que-minagricultura-tiene-que-volver-realidad/ |
| 1013192 | 2026-08-29 | N | https://www.las2orillas.co/la-formula-del-presidente-de-vanti-para-asegurar-que-no-habra-escasez-de-gas/ |
| 1013377 | 2026-08-29 | FDl | https://www.las2orillas.co/jalon-de-orejas-del-presidente-a-nueva-eps-logra-que-un-nino-de-siete-anos-reciba-la-atencion-esperada-durante-un-ano/ |
| 1013493 | 2026-08-31 | FDl | https://www.las2orillas.co/la-senadora-petrista-que-se-enoja-y-arma-show-porque-a-gustavo-petro-le-dicen-expresidente/ |
| 1013466 | 2026-09-02 | F | https://www.las2orillas.co/estos-son-los-escogidos-que-el-presidente-de-la-espriella-quiere-sentar-en-la-junta-directiva-de-ecopetrol/ |
| 1013826 | 2026-09-02 | N | https://www.las2orillas.co/asi-queda-el-nuevo-consejo-nacional-electoral-que-tendra-a-su-cargo-la-democracia-colombiana-hasta-2030/ |
| 1014174 | 2026-09-06 | F | https://www.las2orillas.co/el-regreso-de-alejandro-ordonez-a-la-vida-publica-de-colombia-con-mas-poder-que-nunca-en-la-era-del-tigre/ |
| 1014443 | 2026-09-07 | NP | https://www.las2orillas.co/con-14-anuncios-y-un-billon-de-pesos-cerro-la-cumbre-en-choco-del-presidente-y-los-empresarios-mas-ricos-del-pais/ |
| 1014606 | 2026-09-08 | NP | https://www.las2orillas.co/el-plan-del-millonario-indio-que-queria-los-80-hipopotamos-de-escobar-con-los-animales-silvestres-de-venezuela/ |
| 1014652 | 2026-09-09 | X | https://www.las2orillas.co/por-que-fallecio-juliana-avila-la-nuera-del-vicepresidente-jose-manuel-restrepo/ |
| 1014667 | 2026-09-09 | NP | https://www.las2orillas.co/el-paseo-por-barranquilla-de-la-esposa-de-marco-rubio-mientras-el-y-el-presidente-hacian-acuerdos-de-cooperacion/ |
| 1014854 | 2026-09-10 | N | https://www.las2orillas.co/de-la-espriella-entierra-de-un-plumazo-cualquier-dialogo-con-el-clan-de-chiquito-malo-y-el-eln-de-antonio-garcia/ |
| 1015144 | 2026-09-12 | FDl | https://www.las2orillas.co/de-la-espriella-busco-que-el-reemplazo-de-juliana-guerrero-en-la-u-del-cesar-fuera-el-polo-opuesto/ |
| 1015008 | 2026-09-12 | NP | https://www.las2orillas.co/una-empresa-digital-de-aseo-de-hogares-y-oficinas-le-ha-ido-ganando-terreno-a-la-tradicional-casa-limpia/ |
| 1015156 | 2026-09-12 | FDl | https://www.las2orillas.co/las-2-fundaciones-a-las-que-abelardo-de-la-espriella-les-va-entregar-su-primer-salario-52-millones/ |
| 1015175 | 2026-09-13 | N | https://www.las2orillas.co/el-pacto-liderado-por-cepeda-mais-por-la-investigada-peralta-y-en-marcha-por-cristo-son-la-fragil-oposicion/ |
| 1015228 | 2026-09-14 | N | https://www.las2orillas.co/una-maestra-convertida-en-guerrillera-y-comandante-del-frente-de-guerra-nororiental-esta-en-la-mira-de-de-la-espriella/ |
| 1015328 | 2026-09-14 | X | https://www.las2orillas.co/el-terremoto-no-pudo-con-el-petronio-alvarez-y-asi-puede-vivirlo-en-bogota-luego-de-ser-suspendio-en-cali/ |
| 1015535 | 2026-09-16 | N | https://www.las2orillas.co/los-santandereanos-de-marval-los-primeros-escogidos-por-de-la-espriella-para-metersele-al-tema-de-las-megacarceles/ |
| 1015600 | 2026-09-16 | NP | https://www.las2orillas.co/la-empresa-tierrasua-con-la-que-el-gobernador-carlos-amaya-y-un-alfil-politico-manejan-contratos-en-boyaca/ |
| 1015726 | 2026-09-17 | F | https://www.las2orillas.co/a-la-embajada-clave-para-el-tema-de-derechos-humanos-llega-otro-de-los-abogados-de-de-la-espriella-lawyers/ |
| 1015794 | 2026-09-18 | NP | https://www.las2orillas.co/los-aprietos-del-gerente-de-la-eps-sos-en-cali-y-sus-oscuras-deudas-que-pueden-afectar-la-entidad/ |
| 1015968 | 2026-09-19 | FDl | https://www.las2orillas.co/la-mano-dura-de-de-la-espriella-con-120-presos-para-hacerle-la-guerra-a-la-extorsion-en-buenaventura/ |
| 1016010 | 2026-09-21 | N | https://www.las2orillas.co/una-conocedora-de-la-crisis-de-canacol-sera-contrapeso-tecnico-en-la-junta-de-ecopetrol-junto-al-circulo-de-la-espriella/ |
| 1016018 | 2026-09-21 | FDl | https://www.las2orillas.co/adios-a-los-delincuentes-de-cuello-blanco-en-carceles-de-privilegio-12-politicos-ya-fueron-trasladados/ |
| 1016065 | 2026-09-21 | N | https://www.las2orillas.co/la-puja-por-la-rectoria-de-unipamplona-terminaria-aliando-a-de-la-espriella-con-su-enemigo-politico-juan-fernando-cristo/ |
| 1016070 | 2026-09-21 | INT | https://www.las2orillas.co/que-les-espera-a-los-17-mercenarios-colombianos-acusados-del-crimen-del-presidente-moise-que-se-llevaron-para-ee-uu/ |
| 1016098 | 2026-09-21 | F | https://www.las2orillas.co/el-debut-del-embajador-de-de-la-espriella-en-la-onucon-un-voto-minoritario-alineado-con-trump-contra-palestina/ |
| 1016317 | 2026-09-23 | X | https://www.las2orillas.co/este-es-el-potente-radio-telefono-militar-del-que-no-se-desprende-abelardo-de-la-espriella/ |
| 1016312 | 2026-09-23 | F | https://www.las2orillas.co/el-nuevo-director-de-unp-empezo-la-barrida-de-esquemas-de-seguridad-del-pacto-empezando-por-parientes-y-amigos-de-petro/ |
| 1016621 | 2026-09-27 | N | https://www.las2orillas.co/el-senador-mas-cercano-al-presidente-de-la-espriella-encontro-socio-para-la-cruzada-contra-la-jep-en-el-congreso/ |
| 1016717 | 2026-09-28 | N | https://www.las2orillas.co/el-embajador-de-iran-que-asumio-cuando-petro-era-presidente-tendra-que-empacar-maletas-a-la-carrera/ |
| 1016785 | 2026-09-28 | N | https://www.las2orillas.co/las-cifras-que-tienen-enfrentados-al-gobierno-con-asoganorte-por-las-reses-muertas-en-atlantico-durante-el-nino/ |
| 1017213 | 2026-09-30 | N | https://www.las2orillas.co/de-esta-lista-de-los-23-senalados-por-el-tigre-en-campana-ya-dos-se-quedaron-sin-visa-quienes-siguen/ |
| 1017280 | 2026-10-01 | FDl | https://www.las2orillas.co/la-casa-gomez-influyente-y-respaldo-de-abelardo-de-la-espriella-pone-ahora-alcalde-ad-hoc-para-cali/ |
| 1017545 | 2026-10-03 | X | https://www.las2orillas.co/la-pequena-empresa-del-sur-de-bogota-que-espera-acunar-la-moneda-oficial-de-de-la-espriella-ya-lo-hizo-con-duque-y-petro/ |
| 1017555 | 2026-10-03 | N | https://www.las2orillas.co/por-fin-gustavo-petro-tiene-casa-propia/ |
| 1017536 | 2026-10-04 | NP | https://www.las2orillas.co/brasil-decide-si-se-queda-con-lula-o-vuelve-a-la-presidencia-un-bolsonaro/ |
| 1017464 | 2026-10-05 | N | https://www.las2orillas.co/los-3-aliados-del-presidente-de-la-espriella-que-llegan-a-cargos-diplomaticos-en-el-exterior/ |
| 1017748 | 2026-10-05 | N | https://www.las2orillas.co/con-tutela-de-por-medio-con-la-que-petro-le-gano-a-davibank-el-round-para-que-le-dejaran-tener-casa-propia/ |
| 1017838 | 2026-10-06 | N | https://www.las2orillas.co/el-remezon-en-ecopetrol-con-el-que-el-nuevo-presidente-joaquin-gutierrez-arma-su-equipo-de-vicepresidentes/ |
| 1017977 | 2026-10-07 | N | https://www.las2orillas.co/el-respaldo-de-ee-uu-a-de-la-espriella-ya-empieza-a-sentirse-con-poderosos-drones-militares-para-rastrear-narcos/ |
| 1018044 | 2026-10-07 | N | https://www.las2orillas.co/la-nueva-auditoria-al-fondo-ganadero-que-revive-la-historia-de-fedegan-con-el-gobierno-santos/ |
| 1018335 | 2026-10-09 | N | https://www.las2orillas.co/juan-carlos-gossain-el-exliberal-que-se-unio-a-la-de-la-espriella-y-llega-como-embajador-a-francia/ |
| 1018189 | 2026-10-10 | FDl | https://www.las2orillas.co/la-promesa-cumplida-de-de-la-espriella-reabriendo-embajada-en-jerusalen-a-donde-llega-una-gilinski/ |
