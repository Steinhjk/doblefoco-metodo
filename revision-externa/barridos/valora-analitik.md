# Barrido editorial: Valora Analitik

| | |
|---|---|
| **Medio** | Valora Analitik (`valora-analitik`), medio digital de economía y mercados, valoraanalitik.com. Lo edita Valora Inversiones S.A.S. Tiene ficha técnica: `fichas/valora-analitik.md` |
| **Valor vigente** | **+0,10**, orientación mixta, `reviewedAt: '2026-10-10'` (firma en bloque). La ficha lo sitúa dentro de la banda mixta por dos indicios: el encuadre «Empresarios celebran», estable con los dos gobiernos, y dos pares de piezas asimétricos a través del cambio de gobierno (tensión 1). Ninguno de los dos es un barrido: son ejemplos. **Se apoya en los niveles 4 y 5** (la descripción del género, «la orientación del capital», y hechos editoriales sueltos); la conducta medida del nivel 2 (compañía media +0,152) no puede mover el número |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con la regla del polo fijo y la precisión del 2026-10-10 |
| **Ventana** | 2025-10-12 → 2026-10-12 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-12. Es de la misma casa que quien escribió la ficha y otros barridos del catálogo: su acuerdo con ellos no es aval |
| **Estado** | **FIRMADO el 2026-10-12: 0,00 con evidencia** (antes +0,10), como se propuso; se descarta la alternativa de conservar +0,10. Aplicado en el registro, la ficha y el texto público el 2026-10-12 (`DECISIONES.md`, «Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Resultado** | **No cumple los mínimos.** La voz de la casa de Valora (titulares y entradillas sin atribuir; el medio no publica editorial) casi no toma postura en el eje: **1 pieza D (leve), 0 I y 1 M** en las 103 piezas de la ventana que se leyeron. Lo que sí hace, y mucho, es **fiscalizar en voz propia al gobierno de turno**: **27 piezas contra el Gobierno Petro** en 43 semanas y **3 contra el de De la Espriella** en 9 semanas (más 1 sobre su presidente de Ecopetrol cuando aún era electo). Rama de la precisión: **la segunda, misma conducta con los dos gobiernos → 0,00 con evidencia**. Alternativa: conservar +0,10 |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas, los
> títulos literales y el método están aquí para eso. **La clasificación de
> cada pieza es el juicio de un solo lector.** El §6 dice dónde la lectura
> es más discutible y qué cambiaría el resultado.

---

## 1. Método

- **robots.txt** de `www.valoraanalitik.com`, descargado el 2026-10-12 antes de cualquier otra petición (HTTP 200). Lo literal que importa:
  - Bloques `Disallow: /` solo para agentes de copia con nombre propio (`UbiCrawler`, `DOC`, `Zao`, `HTTrack`, `WebZIP`, `wget`, `libwww`, `larbin` y otros). **No nombra a `ClaudeBot`, `Claude-Web` ni `anthropic-ai`.**
  - Bloque `User-agent: *`: `Disallow: /embed/`, `/m/`, `/cdn-cgi/*`, `/wp-admin/`, `/cgi-bin`, `/*/attachment/`, `/tag/*/feed/`, `/tag/*`, `/author/valora/*`, `/featured/*`, `/21761426377/*`, `/dashboard/`, `/nota-recomendada/` y `/plataforma/imagenes/boletines/images/*`.
  - Declara `Sitemap: https://www.valoraanalitik.com/sitemap.xml` y el de Google News.
  - **No excluye nada de lo usado**: sitemaps, páginas de categoría y piezas. No se tocó `/tag/` ni `/author/`.
- **User-Agent honesto en todas las peticiones:** `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. Nunca el de un navegador. Cliente `curl -s --ssl-no-revoke`, una petición tras otra, **2 s de pausa** después de cada una. Una sola descarga a la vez en el dominio.
- **Incidente que se declara.** Una petición a la API de WordPress (`/wp-json/wp/v2/categories?...`), que el robots.txt no veta, devolvió **403** del cortafuegos del sitio («Your request looks suspiciously similar to automated requests»). No se reintentó ni se buscó otra vía: se pasó a los sitemaps, que el sitio publica para esto.
- **Otro error, declarado.** Antes de usar los sitemaps se recorrieron las categorías `/gobierno-petro/` y `/noticias-politicas/gobierno-de-la-espriella/` (124 páginas). Su rejilla solo cambia de 4 en 4 piezas por página y no da fechas; se abandonó. Esas páginas no se usaron para clasificar.
- **Peticiones al dominio:** robots.txt (1), índice de sitemaps (1), sitemap de categorías (1), sitemaps de entradas 82 a 97 (16), páginas de categoría (124, una con error), API (1, 403), piezas (105, contando una de prueba). **Unas 250.**
- **No se tocaron** eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex. Ni buscadores ni Internet Archive. Valora tiene muro para su plataforma premium; las piezas leídas las sirve abiertas. Descargas en una carpeta temporal fuera del repositorio; no se ejecutó nada desde ella.

### Cómo se armó el universo

1. Los sitemaps `post-sitemap84.xml` a `post-sitemap97.xml` cubren la ventana (el 84 empieza a finales de septiembre de 2025): **13.853 URL únicas**, todas las secciones.
2. **Filtro por la URL** (el *slug* repite el titular):
   - piezas que nombran al Gobierno, al presidente o a las candidaturas: `petro` (sin `petróleo`), `espriella`, `abelardo`, `gobierno`, `presiden`, `cepeda`, `candidat`: **2.190 URL**;
   - piezas de política económica sin esos nombres: `hacienda`, `tributari`, `emergencia-economica`, `patrimonio`, `regla-fiscal`, `deficit`, `presupuesto`, `salario-minimo`, `reforma-laboral`, `reforma-pensional`, `reforma-a-la-salud`, `celebran`, `fondo-milagro`, `libro-de-la-verdad`, `empalme`, `consulta-popular`, `constituyente`, `carf`, `fiscal`: **683 URL** más.
3. **Se leyeron los 2.873 slugs.** La gran mayoría son informativos (nombramientos, encuestas, mercados, relevo de anuncios oficiales) o atribuyen la valoración a una fuente en el propio titular.
4. Se descargaron del sitio vivo las **104 piezas** (103 en la ventana; la otra, del 2025-10-10, quedó fuera) cuyo titular podía llevar una valoración en voz propia, más las citadas por la ficha. De cada una: fecha (`datePublished` del JSON-LD), autor, titular (`og:title`), entradilla (`meta description`) y los primeros párrafos.

### Quién es «voz de la casa» en Valora

- **No hay editorial.** La sección de opinión, «En Perspectiva», la escriben «presidentes de empresas y gremios, analistas económicos especializados, académicos» (lo dice la sección). Son terceros y no cuentan.
- **Cuentan los titulares y entradillas sin atribuir**, como en los barridos de NTN24 y Noticias RCN, y como pide el encargo para la prensa económica: lo que dicen de la política económica del Gobierno nacional sin ponerlo en boca de una fuente. Las piezas van firmadas por periodistas de la redacción o por «Valora Analitik»; dos de las citadas las firma el director de contenidos.
- **No cuentan:** lo atribuido en el titular o la entradilla («según expertos», «advierte ANIF», «Banco de Bogotá advierte», «dice…»), los avisos de ley y el contenido de alianza (ver la ficha), y la sección «En Perspectiva».

### Clases

La lógica de los barridos de NTN24, KienyKe y Las2Orillas:

- **D**, dirección derecha (cuenta): en voz propia, elogio, celebración o disculpa del candidato o el Gobierno De la Espriella, o rótulo descalificador contra Petro, su Gobierno o la izquierda que va más allá de fiscalizar un acto. **D (leve)**: lo mismo con menos carga.
- **I**, dirección izquierda (cuenta): lo simétrico. **No apareció ninguna.**
- **M**, mixta: postura repartida en la misma pieza. No suma.
- **F**, fiscaliza a quien gobierna, aunque el tono sea duro. Se declara y **no suma** (polo fijo; precisión del 2026-10-09). **F (saliente)**: examina al gobierno que ya se fue. **F (electo)**: examina al presidente electo antes de posesionarse.
- **X**, sin postura en voz propia: informativa, o con la valoración atribuida a una fuente.

---

## 2. Cobertura y huecos

| Universo | En la ventana | Leído | Cuenta |
|---|---:|---|---|
| URL de los sitemaps | 13.853 | Filtradas por slug | — |
| Slugs de Gobierno, candidaturas y política económica | 2.873 | Todos, el slug | Universo del barrido |
| Piezas descargadas | 103 (más 1 fuera de la ventana) | Titular, entradilla y primeros párrafos | Las 103 se clasifican |
| «En Perspectiva» (opinión de terceros) | sin contar | 0 | No |

**Huecos que se declaran:**

- **El filtro es por URL y la lectura del universo, por slug.** El slug pierde comillas, tildes y signos: una valoración atribuida puede parecer propia y al revés. Por eso todo lo que parecía tener postura se descargó y se leyó. Lo que no se descargó se clasificó X por el slug.
- **Del cuerpo se leyeron los primeros párrafos**, no la pieza entera. Una pieza X por titular puede tener postura más abajo.
- **El conteo de F no es exhaustivo.** Se descargaron las piezas con valoración posible; el número de fiscalizaciones reales a cada gobierno puede ser mayor que el de las tablas. Lo que sí se leyó entero es el universo de slugs.
- **No se barrieron** los vídeos, los boletines ni la plataforma de pago.

---

## 3. Las piezas

Todas en `https://www.valoraanalitik.com/<slug>/`. Título literal según `og:title`.

### 3.1 Antes del cambio: 2025-10-12 → 2026-08-06 (gobierna Petro)

**En voz propia, fiscalizan al Gobierno Petro (F, 27; no suman):**

| # | Fecha | Título literal (enlace) | Clase | Nota |
|---|---|---|---|---|
| 1 | 2025-10-18 | [Trenes prometidos por Petro siguen sin avanzar en estudios iniciales: ¿en qué van los megaproyectos?](https://www.valoraanalitik.com/trenes-prometidos-petro-siguen-sin-avanzar/) | F | |
| 2 | 2025-10-23 | [La historia detrás del regaño de Petro al viceministro de aguas en Consejo de Ministros: ¿por qué el presidente está equivocado?](https://www.valoraanalitik.com/la-historia-detras-del-regano-de-petro-al-viceministro-de-aguas-en-consejo-de-ministros-por-que-el-presidente-esta-equivocado/) | F | |
| 3 | 2025-10-26 | [El programa bandera de Petro para vías terciarias apenas lleva 10 % de avance en tres años: ¿qué hay detrás?](https://www.valoraanalitik.com/el-programa-bandera-de-petro-para-vias-terciarias-apenas-lleva-10-de-avance-en-tres-anos-que-hay-detras/) | F | |
| 4 | 2025-10-28 | [Así estaría inflando el gobierno Petro las cifras de energías renovables](https://www.valoraanalitik.com/asi-estaria-inflando-gobierno-petro-cifras-de-energias-renovables/) | F | «Un análisis de varias fuentes hecho por Valora Analitik» |
| 5 | 2025-11-23 | [Gasto del gobierno Petro está disparado y ya preocupa por impacto en la inflación](https://www.valoraanalitik.com/gasto-del-gobierno-petro-esta-disparado-y-ya-preocupa-por-impacto-en-la-inflacion/) | F | |
| 6 | 2025-12-09 | [Gobierno Petro se gastó todo el espacio fiscal que le generó estrategia de manejo de deuda](https://www.valoraanalitik.com/gobierno-petro-se-gasto-todo-el-espacio-fiscal-que-le-genero-estrategia-de-manejo-de-deuda/) | F | Firma «Valora Analitik»; el dato es de ANIF |
| 7 | 2025-12-14 | [Balance Fiscal del gobierno Petro: Déficit histórico, deuda disparada y la sombra de una crisis en 2026](https://www.valoraanalitik.com/balance-fiscal-del-gobierno-petro-deficit-historico-deuda-disparada-y-la-sombra-de-una-crisis-en-2026/) | F | |
| 8 | 2025-12-14 | [La encrucijada para la infraestructura en Colombia: tres años de incertidumbre con Petro](https://www.valoraanalitik.com/infraestructura-en-colombia-completa-tres-anos-incertidumbre-con-petro/) | F | «ataques sistemáticos al modelo de APP» |
| 9 | 2026-01-02 | [Gobierno reconoce golpe a inflación por fuerte alza del salario; quiere control de precios, una medida que ha fracasado](https://www.valoraanalitik.com/gobierno-reconoce-golpe-a-inflacion-por-fuerte-alza-del-salario-quiere-control-de-precios-una-medida-que-ha-fracasado/) | F | |
| 10 | 2026-01-13 | [Cambios de Petro a precios de viviendas VIS frenarán acceso de colombianos a casa propia](https://www.valoraanalitik.com/cambios-petro-a-precios-vis-frenaran-acceso-colombianos-casa-propia/) | F | La entradilla atribuye el «diagnóstico incompleto»; el titular afirma |
| 11 | 2026-01-14 | [Petro pidió ventas masivas de deuda tras confundir tasas del mercado](https://www.valoraanalitik.com/petro-pidio-ventas-masivas-de-deuda-tras-confudir-tasas-mercado/) | F | |
| 12 | 2026-01-18 | [Petro se va contra negocio de gas del Grupo Aval y desconoce déficit de gas que ha elevado las importaciones](https://www.valoraanalitik.com/petro-se-va-contra-negocio-de-gas-del-grupo-aval-y-desconoce-deficit-de-gas-que-ha-elevado-las-importaciones/) | F | |
| 13 | 2026-01-23 | [El riesgoso decreto de Petro que pone en jaque el futuro de la energía en Colombia](https://www.valoraanalitik.com/riesgoso-decreto-de-petro-pone-en-jaque-futuro-energia-colombia/) | F | Firma «Valora Analitik» |
| 14 | 2026-01-31 | [Tres años en rojo: gobierno Petro vuelve a incumplir la meta de recaudo tributario](https://www.valoraanalitik.com/tres-anos-en-rojo-gobierno-petro-vuelve-a-incumplir-la-meta-de-recaudo-tributario/) | F | |
| 15 | 2026-02-17 | [Las imprecisiones de Petro sobre el incremento del mínimo, la inflación y las tasas](https://www.valoraanalitik.com/las-imprecisiones-de-petro-sobre-el-incremento-del-minimo-la-inflacion-y-las-tasas/) | F | Firma «Valora Analitik» |
| 16 | 2026-02-25 | [Petro se salta la Ley de Garantías con decretazo de emergencia económica](https://www.valoraanalitik.com/petro-se-salta-la-ley-de-garantias-con-decretazo-de-emergencia-economica/) | F | |
| 17 | 2026-03-12 | [Imputados, capturados y prófugos: el mapa judicial del petrismo a meses del final del gobierno](https://www.valoraanalitik.com/imputados-capturados-y-profugos-el-mapa-judicial-del-petrismo-a-meses-del-final-del-gobierno/) | F | |
| 18 | 2026-03-28 | [Primicia \| Aeropuerto de Ayapel prometido por Petro nunca arrancó: solo hubo piloto para hidroaviones](https://www.valoraanalitik.com/primicia-aeropuerto-de-ayapel-prometido-por-petro-nunca-arranco-solo-hubo-piloto-para-hidroaviones/) | F | |
| 19 | 2026-04-02 | [Las peleas de Petro contra el BanRep y otras instituciones: Gobierno 'patea' la mesa cuando no gana](https://www.valoraanalitik.com/las-peleas-de-petro-contra-el-banrep-y-otras-instituciones-gobierno-patea-la-mesa-cuando-no-gana/) | F | La más dura: «cuando no le dan la razón, el problema deja de ser del Gobierno y pasa a ser de las propias instituciones». Fiscaliza conductas concretas; no la cuento como rótulo (§6) |
| 20 | 2026-04-30 | [Gobierno Petro ahoga al CARF: Se quedará sin presupuesto en octubre](https://www.valoraanalitik.com/gobierno-petro-ahoga-al-carf-se-quedara-sin-presupuesto-en-octubre/) | F | |
| 21 | 2026-05-08 | [Gobierno destaca reducción de la deuda pública externa y le llueven críticas](https://www.valoraanalitik.com/gobierno-destaca-reduccion-de-la-deuda-publica-externa-y-le-llueven-criticas/) | F | |
| 22 | 2026-05-28 | [En dos meses quedarán listos estudios para acueducto de Urabá antioqueño: Petro lo prometió pero no cumplió](https://www.valoraanalitik.com/en-dos-meses-quedaran-listos-estudios-para-acueducto-de-uraba-antioqueno-petro-lo-prometio-pero-no-cumplio/) | F | |
| 23 | 2026-05-31 | [Petro no acepta los resultados del preconteo y denuncia, sin pruebas, cambios en el censo](https://www.valoraanalitik.com/petro-no-acepta-los-resultados-preconteo-denuncia-sin-pruebas-cambios-censo/) | F | |
| 24 | 2026-06-24 | [Colombia perdió la mitad de sus reservas de gas en los últimos siete años: mayor desplome se dio en el Gobierno Petro](https://www.valoraanalitik.com/colombia-perdio-la-mitad-de-sus-reservas-de-gas-en-los-ultimos-siete-anos-mayor-desplome-se-dio-en-el-gobierno-petro/) | F | |
| 25 | 2026-07-21 | [Gobierno Petro castigaría a personas naturales en nueva reforma tributaria; insiste en IVA a más productos](https://www.valoraanalitik.com/gobierno-petro-castigaria-a-personas-naturales-en-nueva-reforma-tributaria-insiste-en-iva-a-mas-productos/) | F | |
| 26 | 2026-08-03 | [El otro hueco billonario sin rigor técnico que le deja el Gobierno Petro a De la Espriella y futuros gobiernos](https://www.valoraanalitik.com/el-otro-hueco-billonario-sin-rigor-tecnico-que-le-deja-el-gobierno-petro-a-de-la-espriella-y-futuros-gobiernos/) | F | Firma el director de contenidos; el análisis es de Corficolombiana |
| 27 | 2026-08-06 | [Gobierno Petro aprobó nuevo e importante subsidio a horas de acabar mandato, a pesar de alto déficit](https://www.valoraanalitik.com/gobierno-petro-aprobo-nuevo-subsidio-a-horas-de-acabar-mandato-pese-a-deficit-fiscal/) | F | |

**Con postura en el eje (suma):**

| # | Fecha | Título literal (enlace) | Clase | Nota |
|---|---|---|---|---|
| 28 | 2026-07-02 | [Se acaban los aumentos desproporcionados del salario mínimo: Gobierno De la Espriella revela cómo lo definirá](https://www.valoraanalitik.com/se-acaban-los-aumentos-desproporcionados-del-salario-minimo-gobierno-de-la-espriella-revela-como-lo-definira/) | **D (leve)** | Hace suyo, en el titular, el anuncio del gobierno electo y califica de «desproporcionados» los aumentos del saliente. La entradilla lo atribuye al Gobierno |

**Fiscalizan al presidente electo:**

| # | Fecha | Título literal (enlace) | Clase | Nota |
|---|---|---|---|---|
| 29 | 2026-07-25 | [¿Quién es Joaquín Gutiérrez? El estratega de confianza de De la Espriella que sería presidente de Ecopetrol](https://www.valoraanalitik.com/quien-es-joaquin-gutierrez-el-estratega-de-confianza-de-de-la-espriella-que-seria-presidente-de-ecopetrol/) | F (electo) | Entradilla: «no tiene experiencia en cargos directivos del sector hidrocarburos» |

**Atribuidas o informativas, con el tema del Gobierno (X; se listan las que la ficha o un lector podrían leer como postura):**

| Fecha | Título literal (enlace) | Por qué X |
|---|---|---|
| 2026-01-09 | [Decreto de Petro para desindexar precios de viviendas VIS del salario mínimo sería un “error”: empresario del sector](https://www.valoraanalitik.com/decreto-petro-desindexar-precios-viviendas-error/) | Atribuida |
| 2026-01-30 | [Empresarios celebran decisión de suspender emergencia económica](https://www.valoraanalitik.com/emergencia-economica-empresarios-celebran-suspension/) | Habla la ANDI (patrón de la ficha) |
| 2026-02-07 | [Estrategia de deuda del gobierno Petro solo "compra tiempo"; persisten desbalances estructurales](https://www.valoraanalitik.com/estrategia-de-deuda-del-gobierno-petro-solo-compra-tiempo-persisten-desbalances-estructurales/) | Algebra Labs |
| 2026-02-10 | [Petro busca revivir la emergencia económica por lluvias, pero no tendría sustento económico](https://www.valoraanalitik.com/petro-busca-revivir-la-emergencia-economica-no-tendria-sustento-economico/) | «según analistas» |
| 2026-02-13 | [El error del gobierno Petro que llevó a suspender el salario mínimo 2026, según el Consejo de Estado](https://www.valoraanalitik.com/el-error-del-gobierno-petro-que-llevo-a-suspender-el-salario-minimo-2026/) | Consejo de Estado |
| 2026-02-28 | [Nuevo impuesto al patrimonio para empresas reduce su músculo financiero y envía señales de incertidumbre](https://www.valoraanalitik.com/nuevo-impuesto-al-patrimonio-para-empresas-reduce-su-musculo-financiero-y-envia-senales-de-incertidumbre/) | Consultores (par de la ficha) |
| 2026-04-09 | [Ahora \| Gobierno Petro expide decreto que reconfigura inversiones de fondos de pensiones en el extranjero](https://www.valoraanalitik.com/gobierno-petro-expide-decreto-que-reconfigura-inversiones-de-fondos-de-pensiones-en-el-extranjero/) | Informativa (par de la ficha) |
| 2026-04-15 | [Los pecados del Gobierno Petro que llevaron al Banco de la República a subir tasas de Interés](https://www.valoraanalitik.com/los-pecados-del-gobierno-petro-que-llevaron-al-banco-de-la-republica-a-subir-tasas-de-interes/) | Explica al gerente del BanRep. Titular duro; podría leerse F |
| 2026-05-14 | [Gobierno proyecta ahorro histórico de US$15.000 millones en intereses y reducción masiva de su deuda pública](https://www.valoraanalitik.com/gobierno-proyecta-ahorro-historico-de-us15-000-millones-en-intereses-y-reduccion-masiva-de-su-deuda-publica/) | Relevo del Gobierno Petro, con «ambiciosa estrategia técnica» en el primer párrafo. Contrapeso (§6) |
| 2026-05-20 | [Estudio advierte que gobierno Petro sigue lejos de cumplir varias de sus principales promesas](https://www.valoraanalitik.com/gobierno-petro-sigue-sin-cumplir-sus-principales-promesas/) | Politécnico Grancolombiano |
| 2026-06-01 | [AtlasIntel, la única encuestadora que acertó en el 'boom' de Abelardo; las demás se rajaron](https://www.valoraanalitik.com/atlasintel-la-unica-encuestadora-que-acerto-en-el-boom-de-abelardo-las-demas-se-rajaron/) | Balance de encuestadoras |
| 2026-06-22 | ["Efecto De la Espriella" tumba el dólar a mínimos de seis años; deuda pública se valoriza](https://www.valoraanalitik.com/efecto-de-la-espriella-tumba-el-dolar-a-minimos-historicos-deuda-publica-se-valoriza/) | Mercados; la expresión va entre comillas |
| 2026-06-22 | [La “bomba fiscal” que enfrentará De la Espriella cuando llegue a la Presidencia a pesar del optimismo del Gobierno Petro](https://www.valoraanalitik.com/la-bomba-fiscal-que-enfrentara-de-la-espriella-cuando-llegue-a-la-presidencia-a-pesar-del-optimismo-del-gobierno-petro/) | ANIF |
| 2026-06-24 | [J.P. Morgan prevé fuerte impulso económico con el gobierno de De la Espriella: TES, petróleo y seguridad, las claves](https://www.valoraanalitik.com/j-p-morgan-preve-fuerte-impulso-economico-con-el-gobierno-de-de-la-espriella-tes-petroleo-y-seguridad-las-claves/) | J.P. Morgan |
| 2026-06-25 | [De la Espriella heredará de Petro una "bomba de tiempo" financiera: Banco de Bogotá advierte por canjes de deuda](https://www.valoraanalitik.com/de-la-espriella-heredara-de-petro-una-bomba-de-tiempo-financiera-banco-de-bogota-advierte-por-canjes-de-deuda/) | Banco de Bogotá |
| 2026-06-26 | [Gobierno Petro casi agota cupo de deuda y deja a De la Espriella un faltante de $30 billones para 2026](https://www.valoraanalitik.com/gobierno-petro-casi-agota-cupo-de-deuda-y-deja-a-de-la-espriella-un-faltante-de-30-billones-para-2026/) | Banco de Bogotá |
| 2026-07-02 | [¿Los US$60 millones del BID que anunció De la Espriella para el empalme con Petro aumentan la deuda de Colombia?](https://www.valoraanalitik.com/60-millones-de-dolares-del-bid-para-empalme-de-la-espriella-endeudan-a-colombia/) | Verifica una crítica de la oposición |
| 2026-07-06 | [Gobierno De la Espriella entregó detalles del ambicioso plan para la salud y las EPS en Colombia](https://www.valoraanalitik.com/gobierno-de-la-espriella-entrego-detalles-del-ambicioso-plan-para-la-salud-y-las-eps-en-colombia/) | Relevo; «ambicioso» también se dijo del plan de deuda de Petro (05-14) |
| 2026-07-12 | [Decisiones políticas del gobierno Petro y desorden en las cuentas dispararon la crisis fiscal, según expertos](https://www.valoraanalitik.com/decisiones-politicas-del-gobierno-petro-y-desorden-en-las-cuentas-dispararon-la-crisis-fiscal-segun-expertos/) | «según expertos» |
| 2026-07-14 | [Cuentas ‘alegres' del Gobierno Petro chocan con la realidad económica del país: Observatorio Fiscal](https://www.valoraanalitik.com/cuentas-alegres-del-gobierno-petro-chocan-con-la-realidad-economica-del-pais-observatorio-fiscal/) | Observatorio Fiscal |
| 2026-07-14 | ["No más falsa paz": De la Espriella anuncia el desmonte de la institucionalidad de la Paz Total y arremete contra la JEP](https://www.valoraanalitik.com/no-mas-falsa-paz-de-la-espriella-anuncia-el-desmonte-de-la-institucionalidad-de-la-paz-total-y-arremete-contra-la-jep/) | La frase es del presidente electo, entre comillas |
| 2026-07-25 | [El sello "made in USA" que De la Espriella imprime a su gobierno antes de posesionarse](https://www.valoraanalitik.com/el-sello-made-in-usa-que-de-la-espriella-imprime-a-su-gobierno-antes-de-posesionarse/) | Análisis descriptivo |
| 2026-07-26 | [Nuevo gobierno anuncia "comité de sabios" encabezado por empresario Arturo Calle y lanza Ruta Milagro para emprendedores](https://www.valoraanalitik.com/nuevo-gobierno-anuncia-comite-de-sabios-encabezado-por-empresario-arturo-calle-y-lanza-ruta-milagro-para-emprendedores/) | Relevo |

### 3.2 Después del cambio: 2026-08-07 → 2026-10-12 (gobierna De la Espriella)

**En voz propia, fiscalizan al Gobierno De la Espriella (F, 3; no suman):**

| # | Fecha | Título literal (enlace) | Clase | Nota |
|---|---|---|---|---|
| 30 | 2026-09-11 | [Gobierno De la Espriella sufre revés: Juzgado suspendió aspersión para combatir cultivos ilícitos](https://www.valoraanalitik.com/gobierno-de-la-espriella-sufre-reves-juzgado-suspendio-aspersion-para-combatir-cultivos-ilicitos/) | F (leve) | «tuvo un nuevo revés» |
| 31 | 2026-09-17 | [Relevante \| Carlos Suárez, estratega de Abelardo de La Espriella, es nuevo presidente de Junta Directiva de Ecopetrol](https://www.valoraanalitik.com/relevante-carlos-suarez-estratega-de-abelardo-de-la-espriella-es-nuevo-presidente-de-junta-directiva-de-ecopetrol/) | F (leve) | Señala en el titular el vínculo de campaña |
| 32 | 2026-09-20 | [Tasas de los TES rozan el 12,7 % y el riesgo país escala ante la incertidumbre fiscal del Gobierno De la Espriella](https://www.valoraanalitik.com/tasas-de-los-tes-rozan-el-127-y-el-riesgo-pais-escala-ante-la-incertidumbre-fiscal-del-gobierno-de-la-espriella/) | F | |

**Con postura en el eje:**

| # | Fecha | Título literal (enlace) | Clase | Nota |
|---|---|---|---|---|
| 33 | 2026-08-30 | [Presupuesto de Colombia 2027 desfinanciado: El reto de "poner la casa en orden" al límite de la Regla Fiscal](https://www.valoraanalitik.com/presupuesto-de-colombia-2027-desfinanciado-el-reto-de-poner-la-casa-en-orden-al-limite-de-la-regla-fiscal/) | M | Entradilla: «le apuntó a desmantelar los cálculos de la administración anterior, pero dejó un sabor agridulce en los mercados» |

**Examinan al gobierno saliente:**

| Fecha | Título literal (enlace) | Clase | Nota |
|---|---|---|---|
| 2026-08-29 | [Proyecto de presupuesto para 2027 de Petro demostró que recortar en funcionamiento era posible](https://www.valoraanalitik.com/proyecto-de-presupuesto-para-2027-de-petro-demostro-que-recortar-en-funcionamiento-era-posible/) | F (saliente) | Con el Observatorio Fiscal: el gobierno anterior desmintió su propia tesis de la inflexibilidad. Leída rápido parece un elogio a Petro; no lo es |

**Atribuidas o informativas (X):**

| Fecha | Título literal (enlace) | Por qué X |
|---|---|---|
| 2026-08-07 | [Uribe arribó a Cali para la posesión de De la Espriella: un gesto de unidad tras la incertidumbre](https://www.valoraanalitik.com/uribe-arribo-a-cali-para-la-posesion-de-de-la-espriella-un-gesto-de-unidad-tras-la-incertidumbre/) | Crónica |
| 2026-08-11 | [Empresarios celebran anuncio del gobierno De la Espriella de eliminar impuesto al patrimonio en Colombia](https://www.valoraanalitik.com/empresarios-celebran-anuncio-del-gobierno-de-la-espriella-de-eliminar-impuesto-al-patrimonio-en-colombia/) | Habla la ANDI (patrón de la ficha) |
| 2026-08-14 | [The Economist y De la Espriella: critica la respuesta al terremoto en Colombia](https://www.valoraanalitik.com/the-economist-le-toma-el-primer-pulso-al-gobierno-de-la-espriella-por-cuenta-del-terremoto/) | The Economist |
| 2026-08-19 | [De la Espriella revela en “Libro de la Verdad” nueve patrones que habrían facilitado la corrupción en gobierno Petro](https://www.valoraanalitik.com/de-la-espriella-revela-en-libro-de-la-verdad-nueve-patrones-que-habrian-facilitado-la-corrupcion-en-gobierno-petro/) | Atribuida al Gobierno, en condicional |
| 2026-08-20 | [Libro de la Verdad revela cómo recibe el Gobierno De la Espriella la DIAN: hay millonarios contratos que siguen sin operar](https://www.valoraanalitik.com/libro-de-la-verdad-revela-como-recibe-la-dian-el-gobierno-de-la-espriella/) | Atribuida al informe del Gobierno |
| 2026-08-21 | [Colombia Mayor quedaría desfinanciado hasta diciembre: Libro de la Verdad revela que cobertura iba hasta julio](https://www.valoraanalitik.com/colombia-mayor-quedaria-desfinanciado-hasta-diciembre-libro-de-la-verdad-revela-que-cobertura-iba-hasta-julio/) | Atribuida |
| 2026-08-21 | [Pasaportes en Colombia podrían tener demoras: el problema que recibe De la Espriella del Gobierno Petro](https://www.valoraanalitik.com/pasaportes-en-colombia-tendrian-demoras-por-problema-que-dejo-petro-a-de-la-espriella/) | Explica un proceso judicial |
| 2026-08-21 | [Gobierno De la Espriella tumbó importante circular del gobierno Petro que impactaba a empleadas domésticas](https://www.valoraanalitik.com/gobierno-de-la-espriella-tumbo-importante-circular-gobierno-petro-que-impactaba-empleadas-domesticas/) | Relevo |
| 2026-08-22 | [Caja en mínimos, déficit fiscal alto y entidades de Hacienda en rojo: Hallazgos del gobierno De la Espriella](https://www.valoraanalitik.com/caja-en-minimos-deficit-fiscal-alto-y-entidades-de-hacienda-en-rojo-hallazgos-del-gobierno-de-la-espriella/) | Atribuida al informe del Gobierno |
| 2026-09-07 | [De la Espriella y empresarios lanzan ambicioso “Plan Marshall” para el Chocó: $1 billón en vías, malecón y canal interoceánico](https://www.valoraanalitik.com/de-la-espriella-y-empresarios-lanzan-ambicioso-plan-marshall-para-el-choco-1-billon-en-vias-malecon-y-canal-interoceanico/) | Relevo; el nombre es del presidente |
| 2026-09-09 | [Los ministros mejor y peor calificados del Gobierno De la Espriella en redes: así quedó el ranking](https://www.valoraanalitik.com/los-ministros-mejor-y-peor-calificados-del-gobierno-de-la-espriella-en-redes-asi-quedo-el-ranking/) | Medición de redes |
| 2026-09-09 | [Ministro de Vivienda enfrenta primera moción de censura del gobierno de Abelardo de la Espriella](https://www.valoraanalitik.com/ministro-de-vivienda-enfrenta-primera-mocion-de-censura-del-gobierno-de-abelardo-de-la-espriella/) | Informativa |
| 2026-09-15 | [Gobierno De la Espriella anuncia radical recorte al 4x1.000: así será el cambio](https://www.valoraanalitik.com/gobierno-de-la-espriella-anuncia-radical-recorte-al-4x1-000-asi-sera-el-cambio/) | Relevo |
| 2026-09-25 | [Joaquín Gutiérrez, nuevo presidente Ecopetrol, va por 'renacer' de la empresa](https://www.valoraanalitik.com/joaquin-gutierrez-nuevo-presidente-ecopetrol-va-por-renacer-de-la-empresa/) | La palabra va entre comillas: es del directivo |
| 2026-10-07 | [Gobierno expide decreto que elimina el límite del 30 % a las inversiones de los fondos de pensiones en el exterior](https://www.valoraanalitik.com/gobierno-expide-decreto-que-elimina-el-limite-del-30-a-las-inversiones-de-los-fondos-de-pensiones-en-el-exterior/) | Relevo sin contraste (par de la ficha) |
| 2026-10-08 | [Gobierno De la Espriella descarta subir “con fuerza” el salario mínimo de 2027: Apunta a decisión técnica](https://www.valoraanalitik.com/gobierno-de-la-espriella-descarta-subir-con-fuerza-el-salario-minimo-de-2027-estas-son-las-causas/) | «aumento desproporcionado» va en boca de «empresarios y analistas» |

---

## 4. Números

| | D | I | M | F (a quien gobierna) | F (saliente o electo) | Piezas leídas |
|---|---:|---:|---:|---:|---:|---:|
| Antes del 07-08-2026 | 1 (leve) | 0 | 0 | 27 | 1 (electo) | 76 |
| Desde el 07-08-2026 | 0 | 0 | 1 | 3 | 1 (saliente) | 27 |
| **Total** | **1** | **0** | **1** | **30** | **2** | **103** |

(Las 103 incluyen las X que no se listan una por una: relevos de anuncios, encuestas y mercados.)

**Antes y después:**

- **Antes (valor vigente):** +0,10, apoyado en ejemplos (el patrón «Empresarios celebran» y dos pares) y en la descripción del género.
- **Después (lo que mide el barrido):** postura en voz propia casi nula (1 D leve, 0 I, 1 M); fiscalización en voz propia a los dos gobiernos: 27 a Petro y 3 a De la Espriella.

**La prueba del polo fijo.** La dureza con Petro no da dirección: las 27 piezas lo fiscalizan a él, que gobernaba. Lo que hay que mirar es si el trato cambia con el gobierno nuevo:

- **Con Petro:** 27 fiscalizaciones en voz propia en 43 semanas (unas 0,6 por semana), varias con titular duro («patea la mesa», «se salta la Ley de Garantías», «tras confundir tasas»). Un relevo favorable con adjetivo propio («ambiciosa estrategia técnica», 14-05).
- **Con De la Espriella:** 3 fiscalizaciones en voz propia en 9 semanas (unas 0,3 por semana), más suaves («sufre revés», el estratega en la junta de Ecopetrol, la «incertidumbre fiscal»). Ningún elogio en voz propia; los adjetivos favorables («ambicioso Plan Marshall») tienen su espejo con Petro.

**Si el gobierno cambiara de signo y el medio mantuviera esta conducta, la clasificación no cambiaría**: fiscaliza a quien manda y no celebra a ninguno. La diferencia de ritmo y de tono existe (§6), pero va en piezas que, una a una, son fiscalización o relevo, y la regla no las cuenta.

---

## 5. Veredicto por condición y rama de la precisión

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | Sí | Titulares y entradillas sin atribuir. No hay editorial; la opinión es de terceros |
| 2. A los dos lados del cambio | No | 1 pieza con dirección, antes del cambio |
| 3. Sostenida (≥10; ≥3 por lado; ≥3:1) | **No** | 1 pieza D (leve), 0 I |
| 4. Contrapesos escritos | Sí | §6 |
| 5. Reproducible | Sí | Tablas del §3 |

**Rama: la segunda, «misma conducta con los dos gobiernos» → 0,00 con evidencia.** El valor vigente se apoya en los niveles 4 y 5, así que el barrido manda. No llega a los mínimos, y documenta la misma conducta: al menos 3 piezas de fiscalización a cada lado del cambio (27 y 3) y postura por debajo de 3:1 en el único sentido en que puede leerse con una sola pieza (1 a 0 no es una dirección).

- No es la primera rama: no hay 10 piezas con postura.
- No es la tercera («dirección clara sin mínimos»): una pieza leve no es dirección clara.
- No es la cuarta: hay piezas suficientes a los dos lados para juzgar la conducta.

---

## 6. Contrapesos, y lo que el barrido no decide

- **El tono cambia, aunque la regla no lo cuente.** Con Petro, los titulares fiscalizadores son muchos y duros, y varios son análisis de la redacción («Así estaría inflando…», «Las imprecisiones de Petro…», «Las peleas de Petro…»). Con De la Espriella, la redacción releva sus anuncios en serie («Gobierno De la Espriella anuncia…», «… confirma…», «… alista…»: más de 150 slugs en 9 semanas) y fiscaliza poco y suave. **Peso medio**, y es la razón de la alternativa. Dos lecturas, sin que el barrido decida: luna de miel de un gobierno recién posesionado, con el terremoto del 10 de agosto en medio; o un medio del capital que encuentra al nuevo gobierno más cerca de su audiencia. Lo segundo encaja con la tensión 1 de la ficha.
- **El par de los fondos de pensiones (tensión 1 de la ficha) se confirma, pero es un par.** El decreto de Petro (09-04) se contó con «El rechazo de los expertos a la medida»; el de De la Espriella que lo revierte (07-10), solo con la voz del Gobierno. Las dos piezas son X en voz propia; la asimetría está en la elección de fuentes, que este barrido no mide.
- **El patrón «Empresarios celebran» es atribuido.** Las dos piezas de la ventana (30-01 con Petro y 11-08 con De la Espriella) son voz de la ANDI. Es estable con los dos gobiernos: no da dirección.
- **Una pieza amable con Petro.** El 14-05 la redacción describe la operación de deuda de Hacienda como «ambiciosa estrategia técnica» y titula con el «ahorro histórico» que proyecta el Gobierno. Peso bajo.
- **La pieza D es leve y discutible.** «Se acaban los aumentos desproporcionados…» (02-07) adopta el anuncio del gobierno electo; la entradilla lo atribuye. Si se lee X, el barrido no tiene ninguna pieza con dirección; si se suma «Los pecados del Gobierno Petro…» como rótulo, sería F igual, porque fiscaliza a quien gobernaba.
- **Lo que mueve el número es el conflicto de interés, no la postura.** La ficha lo dice: la plataforma de pago, los avisos de ley con forma de noticia y el etiquetado comercial desigual. Nada de eso es el eje izquierda-derecha y este barrido no lo toca.

---

## 7. PROPUESTA (pendiente de firma)

- **Valor: 0,00 con evidencia**, orientación mixta. Rama 2 de la precisión del 2026-10-10. Es un juicio declarado, razonado contra los vecinos:
  - **Las2Orillas, 0,00 con evidencia:** fiscalizó a Petro 53 veces y a De la Espriella 7, con piezas amables a los dos lados. Valora tiene el mismo perfil, con menos piezas amables y ninguna dirección.
  - **Noticias RCN, +0,15:** cumplió los mínimos con 22 a 4 en titulares. Valora no se acerca: 1 a 0.
  - **Portafolio (+0,10) y La República (+0,15)**, los otros diarios económicos, siguen sin barrido (Portafolio no puede leerse por IA; ver su barrido). Si se quiere que los tres diarios del capital estén en el mismo sitio de la banda mixta, conviene decidirlos juntos (tensión 2 de la ficha).
- **Alternativa: conservar +0,10.** Es defendible si se da peso al cambio de tono del §6 y al par de los fondos de pensiones: los dos van en la dirección del +0,10 y la ficha ya lo razonaba así. En contra: ni uno ni otro son piezas con postura en voz propia, y la precisión del 2026-10-10 pide que el barrido mande sobre un valor apoyado en ejemplos.
- **No se toca el registro, la propiedad ni el texto público.** La ficha técnica ya existe y no se modifica: si se firma, habría que actualizar su ARGUMENTO y su tensión 2.
- **Revisión:** recontar en enero de 2027, con cinco meses de gobierno detrás, la fiscalización en voz propia de De la Espriella (hoy, 3 piezas) y medir la elección de fuentes en pares de decretos de los dos gobiernos, que es donde la ficha ve la asimetría.
