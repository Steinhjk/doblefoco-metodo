# Boyacá Digital — ficha de orientación

| | |
|---|---|
| **Medio** | Boyacá Digital · `boyaca-digital` · boyacadigital.com |
| **Valor vigente** | **0,00** · valor **por ausencia de evidencia de orientación** (regla 3 del §5) — **ficha incompleta**. No es una orientación observada<br>**Banda (registro):** Orientación mixta |
| **Firma** | ☑ **FIRMADA el 2026-10-10 — el responsable editorial** (firma en bloque tras el ciclo 2; ver DECISIONES.md. Lo que más abajo dice «sin firmar», «no se firma» o «provisional» es el estado anterior a esta firma y se conserva como historia) |
| **Alta** | 2026-08-09 (candidatura, del barrido nacional) · **corregida el 2026-10-07** con las correcciones de hecho del ciclo 2 (ver TENSIONES) |
| **Última revisión** | — |
| **Departamento / ámbito** | Boyacá |
| **Fuentes de propiedad** | `shared/mediaOwnership.js` (`boyaca-digital`): 11 fuentes; comprobada el 2026-10-07 |
| **Recogida** | `https://www.boyacadigital.com/rss.xml` · vía `direct` |
| **Protocolo** | `PROTOCOLO_JUICIO_EDITORIAL.md` |

## Estado

> **Su redacción no es humana.** El propio medio declara ser «un medio operado
> por una redacción de agentes de inteligencia artificial bajo supervisión
> editorial», y se presenta como «el primer periódico autónomo con agentes de
> inteligencia artificial de Colombia».

### ENTRA, POR DECISIÓN DEL RESPONSABLE EDITORIAL (2026-08-09)

Esta ficha se escribió recomendando NO darlo de alta. **El responsable editorial decidió admitirlo:
«es el primero».** Se admite con marca visible y con la propiedad rastreada, que
era la condición implícita de esa decisión.

Los tres reparos que motivaban la recomendación contraria siguen en pie y se
dejan escritos, porque admitirlo no los resuelve:

**1. Su orientación no es una propiedad de la casa sino de su configuración**,
que puede cambiar en una tarde sin que nada externo lo registre. Un número
nuestro sobre eso caducaría sin aviso. **Y aquí está el giro que apuntó el responsable editorial:
eso lo hace MÁS medible, no menos.** En una redacción humana el sesgo se reparte
entre personas y días; en una configurada es una propiedad del sistema, y su
salida es sistemática. Con corpus suficiente, la deriva de este medio debería
poder calcularse más directamente que la de uno humano, y una alteración de su
configuración debería verse como un SALTO y no como ruido. Es trabajo del motor
de sesgo y queda anotado en `shared/mediaRegistry.js`, junto al campo.

**2. El recuento de pluralidad.** Todo el sitio se apoya en «cuántos medios
distintos cubren este hecho». Una redacción que reescribe lo que ya publicaron
otros suma sin aportar una voz. **Por eso la marca no es decorativa**: sin ella,
este medio infla en silencio la cifra que da sentido a la portada.
**Constatado el 2026-10-07, ya no es solo hipótesis:** su sección
[/opinion](https://www.boyacadigital.com/opinion) está hecha, en las piezas
listadas, de reescrituras atribuidas de columnas de La Silla Vacía, Boyacá 7 Días
y La República, firmadas «Redacción Boyacá Digital · IA». Ejemplo literal, de la
pieza del 2026-09-27: «El columnista Juan Pablo Ossa publicó en La Silla Vacía un
análisis…». Un recuento que sume esas piezas cuenta dos veces la misma voz.

**3. Nadie firma.** Su política editorial dice que un Editor en Jefe responde
legalmente, pero no publica su nombre. El protocolo pide que haya alguien a
quien preguntarle por qué; aquí hay un cargo, no una persona. **Matiz del
2026-10-07:** el medio sí nombra a su gerente, Carlos O. Rosas A., y el contacto
del Editor en Jefe es `[correo omitido]`. Que el Editor en Jefe sea
Rosas es una sospecha, y no se afirma.

## Evidencia

### Nivel 4 — Lo que declara de sí mismo, y es lo decisivo

En su propia portada: **«Boyacá Digital es un medio operado por una redacción de
agentes de inteligencia artificial bajo supervisión editorial»**. Se anuncia
como el primer periódico autónomo con agentes de IA del país. Dice citar fuente
en todo su contenido y acogerse al derecho de rectificación del artículo 20 de
la Constitución.

Cubre Boyacá con secciones municipales de Tunja, Duitama, Sogamoso,
Chiquinquirá, Paipa y Villa de Leyva.

Fuente: [boyacadigital.com](https://www.boyacadigital.com/).

### Nivel 1 — Quién lo posee

Se rastreó y hay algo, aunque incompleto: **Holding Consultants** lo opera y lo
edita. **Corregido el 2026-10-07:** esta ficha decía que no había razón social,
NIT ni una persona con nombre que respondiera, y los tres constaban en una
página que ella misma citaba.

- **Razón social declarada:** «Holding Consultants S.A.S.», **NIT
  900.143.612-6**. Lo dicen el pie y el JSON-LD de
  [holdingconsultants.org/nosotros/](https://www.holdingconsultants.org/nosotros/)
  («2006–2026 © Holding Consultants® · NIT 900.143.612-6 · Bogotá, Colombia»;
  `"legalName":"Holding Consultants S.A.S."`, `"taxID":"900143612-6"`). La
  forma jurídica está en tensión: ver TENSIONES, 1.
- **Representante legal en SECOP II: Carlos Octavio Rosas Acevedo**, en los 58
  registros del NIT ([datos.gov.co, `jbjy-vk9h`](https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=id_contrato,nombre_entidad,proveedor_adjudicado,fecha_de_firma,valor_del_contrato,modalidad_de_contratacion,objeto_del_contrato,estado_contrato&$where=documento_proveedor%20like%20%27%25900143612%25%27)),
  con domicilio en la Carrera 47 # 127 D 03, la dirección de la consultora. Es
  un registro público, no una autodeclaración.
- **La consultora lo presenta como «CEO y Fundador»** (/nosotros/), **y el
  medio, como su gerente:** «Carlos O. Rosas A. es gerente de Boyacá Digital y
  columnista de opinión» ([boyacadigital.com/equipo](https://www.boyacadigital.com/equipo)).
- **Accionariado: no consta.** Ser representante legal, CEO y fundador no prueba
  que sea el accionista. Eso solo lo dice el certificado de Cámara de Comercio.

El detalle está en el apartado «La propiedad, rastreada», más abajo.

**Edad del medio.** Wikidata
([Q140398679](https://www.wikidata.org/wiki/Special:EntityData/Q140398679.json),
enlazado desde el `sameAs` del JSON-LD del propio medio) le da fecha de creación
2025, con precisión de año. Es un indicio editable por cualquiera, no un
registro: si es cierto, toda la vida del medio cae dentro de los últimos doce
meses.

### Nivel 2 — Conducta medida: 37 días, sin peso todavía

**Corregido el 2026-10-07:** esta ficha decía «NO EXISTE. No está ingerido», y
la medición ya estaba en el expediente
(`revision-externa/envios/ciclo-2-2026-10-07/boyaca-digital.md`, medición del
2026-10-07, ventana 31-08 → 07-10):

- 1178 artículos, 328 en alguna historia y 338 historias;
- agenda propia del 20 %, 269 historias compartidas y compañía media de 0,141;
- coincide sobre todo con El Colombiano (76), El Tiempo (43) y La Silla Vacía (39).

**No sostiene el número.** Son 37 días, la compañía media está saturada y mide
con quién coincide, no qué dice. **Publica mucho y muy rápido**, que es lo
esperable de una redacción automatizada y no es mérito.

### SUS TRECE PERIODISTAS TIENEN NOMBRE Y APELLIDO, Y NO EXISTEN

Mariana Restrepo en judicial, Andrés Cárdenas en política, Carolina Pinilla en
Boyacá hiperlocal, Diego Saavedra en deportes, Valeria Torres en economía, Don
Hernán Bautista en agro… trece agentes con nombres humanos y sección asignada.

**El medio lo declara en su página de equipo, y eso cuenta a su favor.** Pero la
firma es donde el lector se encuentra al autor, y ahí parecen personas. Su feed
RSS **no trae etiqueta de autor**, así que esa firma no nos llega y no podemos
reproducirla ni corregirla: otra razón para que la marca esté en el medio.

Declara además etiquetar las imágenes generadas y no simular personas reales.
**Conviene comprobar qué proporción de sus fotos es generada antes de mostrarlas
como «la foto del medio»**: la regla del proyecto es imagen real del medio o
ninguna, y una ilustración de IA no es ninguna de las dos.

## Argumento

**0,00 por ausencia de evidencia de orientación, no por orientación observada**
(cabecera: regla 3 del §5, ficha incompleta). La tensión 6 lo dice sin rodeos:
«El 0,00 es un valor por defecto, no una medición».

- **Nivel 1.** Consta quién lo opera y lo edita —Holding Consultants, NIT
  900.143.612-6, por evidencia convergente— y su representante legal en
  SECOP; no consta el accionariado. Y aunque constara, el dueño no determina la
  orientación (regla 1 del §5).
- **Nivel 2.** 37 días de corpus: 1178 artículos, agenda propia del 20 % y
  compañía media de 0,141. Mide con quién coincide, no qué dice, y la compañía
  media no mueve un número.
- **Voz de la casa.** No hay qué barrer con la regla «Evidencia editorial
  histórica»: su sección /opinion está hecha de reescrituras atribuidas de
  columnas de La Silla Vacía, Boyacá 7 Días y La República, y las columnas de
  terceros no cuentan. La ficha no documenta editoriales propios.
- **Nivel 4.** Lo que declara de sí mismo —una redacción de agentes de IA «bajo
  supervisión editorial»— dice cómo produce, no dónde está en el eje.

Sin nivel 1-3 que lo sitúe, la regla 3 deja el número donde está.

## El mejor caso en contra

- **Hacia «sin medir» (el más fuerte).** Si el 0,00 es «un valor por defecto,
  no una medición» (tensión 6), y la línea del medio es «una propiedad de su
  configuración, que puede cambiar en una tarde sin que nada externo lo
  registre» (Estado, reparo 1), un número publicado sobre él puede caducar sin
  aviso. El lector ve un 0,00 al lado de medios que sí se leyeron, y aquí no hay
  ni una pieza contada.
- **Hacia una dirección, por quien le paga a la dueña.** La consultora que lo
  opera contrató con entidades nacionales que el medio cubre: 12 contratos por
  COP 70 386 247 desde el 2025-10-07 (entre ellos CNE, Policía, Ministerio de
  Transporte, Fondo del Congreso y Politécnico JIC), tres de ellos posteriores
  al 07-08-2026. Si su
  cobertura resultara sistemáticamente favorable a ellas, «ya no será un
  conflicto potencial sino conducta medida». No se ha medido, y una relación con
  contratantes no tiene signo por sí sola.
- **Hacia una dirección, por la selección de su opinión.** Qué columnas ajenas
  elige reescribir puede tener sesgo. La ficha no lo documenta: no cita ninguna
  pieza con postura, a ningún lado del 07-08-2026.

**Contrapeso:** el reparo 1 corre también al revés. Una salida configurada es
sistemática, y debería medirse con menos ruido que una humana (REFUTACIÓN, 4).
Pero eso es una promesa de medición, no una medición.

## Qué cambiaría el número

### REFUTACIÓN — qué reabriría el expediente

1. **El certificado de Cámara de Comercio de Holding Consultants**, que llevaría
   el vínculo de «evidencia convergente» a identidad jurídica probada, y
   cerraría la forma jurídica y el accionariado (TENSIONES, 1 y 3). Hoy se apoya
   en la declaración del medio, en que Rosas aparece a los dos lados, en el
   teléfono compartido, en la publicidad de la casa y en /terminos.
2. **Que el medio publique quién es el Editor en Jefe y su sociedad editora**,
   que es el mínimo del protocolo para cualquiera.
3. **Que se documente qué parte es generada y qué parte es reportería humana.**
   «Bajo supervisión editorial» no dice si alguien va al sitio de los hechos.
4. **A los 90 días con más de 60 historias suyas**, y aquí es donde esta ficha
   se separa de las demás: si la hipótesis del responsable editorial es correcta, su orientación
   se podrá calcular con menos ruido que la de cualquier medio humano del
   catálogo. **Este medio es el primer caso de prueba de esa idea.**
   **Esa medición debe mirar también el trato a las entidades que contratan con
   su dueña**, hoy nacionales (CNE, Policía, MinTransporte, Fondo del Congreso,
   Politécnico JIC).

## Tensiones declaradas

### LO QUE ESTE CASO OBLIGA A MIRAR

Boyacá Digital se anuncia como **el primero** de Colombia. Si es cierto, habrá
más, y llegarán antes a los departamentos vacíos que los medios humanos —
montar un portal automatizado para Vaupés cuesta mucho menos que sostener una
redacción allí.

**El mapa departamental podría llenarse de departamentos «cubiertos» que en
realidad no tienen a nadie reporteando.** Merece una comprobación explícita en
el alta de cualquier candidato futuro, y por eso queda escrito aquí y no solo
en una conversación.

### TENSIONES — lo que la revisión del ciclo 2 deja abierto (2026-10-07)

El responsable editorial aprobó el 2026-10-07 las correcciones de hecho de arriba. **El 0,00 no
cambia y no se firma: falta el certificado del RUES.** Estas tensiones se
escriben antes de la firma para que nadie la lea como cierre.

1. **La forma jurídica no cuadra entre fuentes públicas.** Su sitio dice
   «Holding Consultants S.A.S.». SECOP integrado registra el mismo NIT a nombre
   de «FUNDACION HOLDING CONSULTANTS DE COLOMBIA» en 3 contratos (Soacha 2007,
   Nobsa 2016 y Positiva 2017). Y su
   [página de empleabilidad](https://www.holdingconsultants.org/servicios/proyectos-de-empleabilidad-e-inclusion-social/)
   dice que «actúa como Agencia Privada No Lucrativa de Gestión y Colocación de
   Empleo», autorizada por la Resolución 0472 del 19-12-2025. Una fundación y una
   S.A.S. no se poseen igual. Una lectura posible, sin confirmar: nació como
   fundación y se transformó. **La cierra el certificado de Cámara de Comercio.**
2. **`ownerType: 'conglomerado'` no tiene respaldo.** Nada de lo leído muestra
   un grupo con intereses mayoritarios en otros sectores: lo que consta es una
   consultora con su NIT y su representante legal, de forma jurídica dudosa. La
   resolución no propone otro tipo con fuente, así que **se deja como está y se
   declara aquí**. Que el responsable editorial decida, con el certificado delante, si se queda o
   pasa a un tipo que no presuponga forma societaria.
3. **Persona natural frente a dueño.** Rosas es representante legal (SECOP), CEO
   y fundador (sitio de la consultora) y gerente del medio. **Que sea el
   accionista no consta.**
4. **El Editor en Jefe sigue sin nombre**, con el correo `gerente@`. Que sea
   Rosas es una sospecha. Hoy no consta candidatura ni cargo público de Rosas,
   así que la regla de quien dirige no se dispara.
5. **El conflicto de interés existe, pero con otra contraparte** que la que
   suponía la ficha: entidades nacionales, no Boyacá. La comprobación de nivel 2
   apunta a ellas.
6. **El 0,00 es un valor por defecto, no una medición.** Ni la ficha ni la
   revisión tienen evidencia de orientación de nivel 1 a 3: el nivel 1 dice quién
   es el dueño, y el dueño no determina la orientación (regla 1 del §5); el nivel
   2 tiene 37 días y mide compañía, no contenido. Por la regla 3 del §5 el número
   no se mueve y la ficha queda **incompleta**. El medio tiene, según Wikidata, un
   año de vida.

Fuente de las seis: `revision-externa/respuestas/opus-5-5-boyaca-digital.md`,
RESOLUCIÓN, «Propuesta para la firma» (b) y (c). El revisor es de la misma casa
que el autor de esta ficha y que quien escribió la resolución: el acuerdo entre
los tres no es aval.

## Propiedad y lo que no consta

### LA PROPIEDAD, RASTREADA

| Dato | Valor |
|---|---|
| Opera y edita | **Holding Consultants** (lo dice su política editorial) |
| Responsable legal | «Editor en Jefe», **sin nombre publicado**. Contacto publicado: `[correo omitido]` (/sobre-nosotros, /politica-editorial). Que sea Rosas no consta |
| Humanos con nombre | **Carlos O. Rosas A.**, gerente del medio y columnista; representante legal de la consultora en SECOP. **Juan Pablo Sáenz**, columnista: «Periodista · Ex Funcionario UTL · Estratega en comunicación política · Cofundador de WHITE · Columnista de Boyacá Digital» (literal de /equipo) |
| Razón social / NIT | **Holding Consultants S.A.S.** (según su sitio) · **NIT 900.143.612-6** · forma jurídica en tensión (ver TENSIONES, 1) |
| Sede declarada | El medio: Carrera 11 #12-64, Sogamoso (su JSON-LD). La consultora: Carrera 47 No. 127D-03, Bogotá |

Lo de Sáenz entra como dato descriptivo, atribuido al medio, y nada más: la
regla de quien dirige excluye la militancia pasada y pide un cargo **vigente** de
quien dirige, y él es columnista invitado.

#### El vínculo, y cómo se comprobó

Con ese nombre existe en Bogotá **Holding Consultants**, consultora de sistemas
de gestión —ISO 9001, seguridad y salud en el trabajo—, con cobertura declarada
en Cundinamarca y Boyacá y clientes en el sector privado **y en el público**.

> **Fuente caída (2026-10-06), sustituida por la captura (2026-10-07).** La
> página «Nuestra organización» de la consultora da 404 desde la auditoría del
> 2026-10-01: el sitio se rehízo. Su
> [captura de archive.org del 2023-03-24](https://web.archive.org/web/20230324172804/https://www.holdingconsultants.org/nuestra-organizacion/),
> la última con HTTP 200, dice literal: «En el transcurso de nuestra permanencia
> en el mercado de **quince (15) años** sostenemos relaciones comerciales con
> numerosas empresas tanto del sector **Privado como Público** en varias ciudades
> del País». **La frase de los clientes públicos queda confirmada. Los «veinte
> años» que esta ficha le atribuía, no:** la captura dice quince. Los veinte
> constan hoy en el JSON-LD del sitio nuevo («20 años de experiencia en
> Colombia»).
>
> Por la regla del presente, la captura de 2023 solo prueba que la frase
> existió. **La prueba vigente de clientes públicos es SECOP**, y es mejor: ver
> el conflicto de interés, más abajo.
>
> El resto sigue publicado en [«Nosotros»](https://www.holdingconsultants.org/nosotros/)
> —licencia SST n.º 3070, ISO 9001:2015— y en
> [«Cobertura»](https://www.holdingconsultants.org/cobertura/) —Cundinamarca,
> Boyacá y el resto del país—. **La fundación es inconsistente en la propia
> fuente:** /nosotros/ da el «26 de marzo de 2007»; el JSON-LD,
> `"foundingDate":"2006"`, y el pie, «2006–2026».

Que sea la misma organización dejó de ser una coincidencia de nombre:

| Indicio | Qué muestra |
|---|---|
| Declaración del propio medio | Su política editorial y su política de privacidad dicen que lo «opera y edita» Holding Consultants |
| **La misma persona a los dos lados** | Rosas es «CEO y Fundador» de la consultora (/nosotros/), su representante legal en SECOP y «gerente de Boyacá Digital» (/equipo) |
| **El mismo teléfono** | El JSON-LD `NewsMediaOrganization` del medio y el de la consultora declaran el mismo número de teléfono de contacto (comprobado el 2026-10-07; no se reproduce: es un móvil, y el protocolo no copia teléfonos de personas naturales) |
| **Publicidad de la casa** | El medio enlaza a holdingconsultants.org y holdingsoft.org con `utm_source=boyacadigital&utm_medium=house`: 19 enlaces en la portada, 4 en /opinion, 4 en /escenario-politico y 1 en cada página legal y en /equipo |
| **Sus términos de uso** | [/terminos](https://www.boyacadigital.com/terminos): «…y el diseño del sitio son propiedad de Holding Consultants o se usan con licencia» |
| Servidores de nombres | `boyacadigital.com`, `holdingconsultants.org` y también `holdingsoft.org` usan el par de Cloudflare `dylan`/`fatima`. **Es indicio, no huella:** no hay fuente de que un par sea exclusivo de una cuenta |
| Geografía | La consultora declara cobertura en Boyacá; el medio es de Boyacá |

**Corregido el 2026-10-07:** esta ficha hacía descansar el vínculo en que
«Cloudflare asigna un par por cuenta», leído como si el par fuera exclusivo. Ni
la ficha ni la verificación tienen un documento de Cloudflare que lo diga, y ya
no hace falta: la persona, el teléfono, la publicidad de la casa y la cláusula
de /terminos pesan mucho más.

**No es un certificado de Cámara de Comercio**, y por eso no se afirma identidad
jurídica ni quién es el accionista. Es evidencia convergente y se publica como
tal.

#### EL CONFLICTO DE INTERÉS QUE SE DECLARA

**Corregido el 2026-10-07.** Esta ficha ponía la contraparte en «las alcaldías y
la gobernación de Boyacá», y eso no tiene respaldo en el registro. El conflicto
documentado está en SECOP, y es con **entidades nacionales y de otras
regiones**.

**Una consultora que vende servicios a entidades públicas es la dueña declarada
de un medio cuya redacción automatizada cubre esas mismas entidades en su
sección nacional.** SECOP II
([`jbjy-vk9h`](https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=id_contrato,nombre_entidad,proveedor_adjudicado,fecha_de_firma,valor_del_contrato,modalidad_de_contratacion,objeto_del_contrato,estado_contrato&$where=documento_proveedor%20like%20%27%25900143612%25%27))
registra 58 contratos con el NIT 900143612. Desde el 2025-10-07 son **12, por
COP 70 386 247**. Entre ellos:

| Entidad | Contrato | Firma | Valor (COP) |
|---|---|---|---|
| Consejo Nacional Electoral | CPS-CNE-025-2025 | 2025-10-17 | 9 789 456 |
| Ministerio de Transporte | 722-2025 | 2025-11-25 | 3 645 200 |
| Fondo de Previsión Social del Congreso | MC-014-2025 | 2025-11-21 | 3 940 000 |
| Fondo Rotatorio de la Policía | CTO 075-2-26 | 2026-07-30 | 13 840 000 |
| Departamento de Policía Vichada (sanidad) | 44-7-20006-26 | 2026-08-25 | 8 800 000 |
| Corporación Autónoma Regional de Risaralda (CARDER) | CO1.PCCNTR.9864279 | 2026-08-28 | 3 808 664 |
| Politécnico Jaime Isaza Cadavid | 55285-2026 | 2026-09-15 | 15 856 742 |

- **Tres son posteriores al 07-08-2026**, ya con el nuevo gobierno.
- Antes de esa ventana: Secretaría General de la Alcaldía Mayor de Bogotá
  (4232000-708-2025, 2025-06-12, COP 78 410 640), ICBF, Aerocivil, Supersalud.
- **En Boyacá, solo Nobsa:** concurso de méritos de 2016, contrato
  16-15-5596405, COP 100 000 000, «Liquidado», a nombre de «FUNDACION HOLDING
  CONSULTANTS DE COLOMBIA» (SECOP integrado,
  [`rpmr-utcd`](https://www.datos.gov.co/resource/rpmr-utcd.json?$select=nombre_de_la_entidad,nom_raz_social_contratista,numero_del_contrato,fecha_de_firma_del_contrato,valor_contrato,objeto_del_proceso,origen&$where=documento_proveedor%20like%20%27%25900143612%25%27)).
  Por la regla del presente no es conflicto vigente. En SECOP II hay **cero**
  contratos en Boyacá.
- El medio cubre a esas entidades: tenía en portada «Congreso elegirá el 25 de
  agosto a los nuevos magistrados del CNE» y piezas sobre la Policía.
- Que algo no aparezca en SECOP no significa que no exista: el registro abierto
  no recoge contratos fuera de SECOP ni subcontratos.

Se declara siguiendo la regla que ya gobierna el resto del catálogo: **no se
afirma que haya influido en ninguna pieza** —eso no consta y no se publica—; se
expone quién está detrás, que es comprobable, y el lector saca su conclusión con
el dato delante en vez de sin él.

Y hay una consecuencia práctica: **si esa cobertura resulta sistemáticamente
favorable a las entidades que contratan con su dueña, ya no será un conflicto
potencial sino conducta medida.** Es la comprobación de nivel 2 que esta ficha
deja anotada, y en un medio automatizado debería detectarse antes que en uno
humano. **Desde el 2026-10-07 apunta a las contrapartes nacionales** (CNE,
Policía, Ministerio de Transporte, Fondo del Congreso, Politécnico JIC), no a
las alcaldías ni a la gobernación de Boyacá.

## Historial

### REVISIÓN EXTERNA

☑ **Ciclo 2 hecho** (Claude Opus 5.5, resuelto el 2026-10-07):
`revision-externa/respuestas/opus-5-5-boyaca-digital.md`. Siete objeciones,
nueve filas con la 2 partida en tres: seis aceptadas (1, 2b, 2c, 3, 4 y 7), una
aceptada en la redacción y no en el número (5), una declarada como tensión (2a)
y una aceptada como dato y rechazada como evidencia o aviso (6: «Ex Funcionario
UTL» es pasado de un columnista, no cargo vigente de quien dirige). Las
correcciones de hecho están aplicadas arriba, y las tensiones, escritas. **La
firma espera al certificado del RUES.** Su acuerdo no cuenta como aval.
