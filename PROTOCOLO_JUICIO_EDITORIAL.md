# Protocolo del juicio editorial de orientación

**Fijado el 2026-08-08, ANTES de examinar ningún medio.** El orden importa y es
comprobable en el historial de git: este archivo se confirma en un commit propio,
y las fichas de cada medio vienen después. Si los criterios se escribieran
mirando ya el resultado, serían una racionalización con aspecto de método.

---

## 0. Por qué existe

La calibración por documentos de partido falló (§24 de
`DISENO_ALGORITMO_SESGO.md`): el RILE de programas municipales no reproduce el
orden de los registros de expertos, y publicar un número apoyado en una
correlación de 0,39 con n=7 sería el aparato estadístico alrededor de una
opinión.

El diseño previó esta salida desde su sección 0: **el juicio editorial declarado,
argumentado y sujeto a réplica es un resultado aceptable**. Este protocolo lo
convierte en un procedimiento en vez de en una excusa.

**Lo que cambia respecto a hoy no es que haya juicio —los 43 valores actuales ya
lo son— sino que deja de ser invisible.** Hoy cada medio tiene un número con una
frase de justificación y `reviewedAt: null`. Después de esto, cada número tendrá
evidencia citada, un argumento, su mejor contra-argumento, la condición que lo
refutaría y **un nombre y una fecha**.

---

## 1. Qué se está juzgando, y qué no

Se juzga la **ORIENTACIÓN del medio**: estructural, permanente, de la casa. No el
sesgo de una pieza concreta, que es otra cosa y todavía no se mide (ver la nota
de `SPECTRUM_LABEL` en `shared/biasAnalysis.js`).

Escala existente, sin cambios: **−1,0 a +1,0**, con las cinco bandas de
`SPECTRUM_BANDS`. El 0,0 es **orientación mixta**: la del medio no se sitúa en el
eje izquierda-derecha, no que no tenga.

### REGLA DEL POLO FIJO (añadida el 2026-08-18 por el responsable editorial, tras el ciclo 1 de revisión externa)

**El eje mide la posición del medio respecto de un polo fijo, no su postura
frente a quien gobierne.**

Izquierda y derecha son posiciones ideológicas. No son «a favor del gobierno» y
«en contra del gobierno»: si lo fueran, el mismo medio cambiaría de signo cada
cuatro años sin haber cambiado de línea, y el eje mediría al gobierno de turno en
vez de al medio.

**Consecuencia directa: fiscalizar al poder NO es evidencia de orientación**, ni
en un sentido ni en el otro. Denunciar la corrupción de quien manda es el oficio.
Un medio no se desplaza a la izquierda por investigar a un gobierno de derecha,
ni a la derecha por investigar a uno de izquierda.

**La prueba, y es la misma forma que la regla del presente.** Si el gobierno
cambiara mañana y el medio mantuviera exactamente la misma conducta, ¿cambiaría
su clasificación? Si la respuesta es sí, no se está midiendo al medio: se está
midiendo contra quién le tocó ejercer.

Excepción escrita: los medios del Gobierno nacional sin línea propia toman la
dirección del gobierno que los controla (ver «Medios del Gobierno nacional», más
abajo; 2026-10-10).

#### Lo que sí sigue siendo evidencia, y es la parte que hay que saber leer

La regla **no** deja sin clasificar a los medios beligerantes. Lo que descarta es
la crítica al gobierno de turno; lo que admite es **la asimetría sostenida a
través de un cambio de gobierno**:

- Un medio que fiscaliza con dureza a quien manda, y sigue haciéndolo cuando
  manda el otro lado, está haciendo periodismo. Eso es **mixta**.
- Un medio que fiscalizaba con dureza y pasa a celebrar cuando llega su lado
  —o al revés— ha revelado una posición. **Eso sí es orientación, y se mide.**

Por eso el criterio no puede aplicarse sobre una foto de un solo gobierno. Y por
eso mismo **la transición de agosto de 2026 es la ocasión más limpia que va a
tener este catálogo en años**: cualquier medio clasificado por su dureza con el
gobierno saliente queda ahora sujeto a la única comprobación que vale, que es
cómo trata al entrante. Está calendarizado en las fichas afectadas.

#### Qué NO toca esta regla

Un **endoso editorial** no es fiscalización: es tomar partido, y sigue siendo
evidencia de primer orden. Lo mismo vale para el encuadre asimétrico entre
candidatos, la cobertura del propio accionista y la línea declarada por la casa.
Esta regla acota una sola cosa —la crítica al poder vigente— y no las demás.

### EVIDENCIA EDITORIAL HISTÓRICA (añadida el 2026-10-09 por el responsable editorial, ciclo 2, tanda 5)

**La asimetría sostenida en la voz de la casa, medida con un barrido del
archivo del propio medio, cuenta como conducta medida y puede mover el
número sin esperar 90 días de corpus.**

**Por qué.** La compañía media de nuestro corpus no llegaba a 90 días, porque la
base no los guarda, y además está saturada (`revision-externa/CONDUCTA-MEDIDA.md`).
Entretanto, el archivo de cada medio guarda años de piezas fechadas. En las
tandas 4 y 5, un barrido de ese archivo situó a varios medios con más claridad
que la compañía media, y lo hizo leyendo lo que el medio escribe con su propia
voz. Esperar 90 días de una métrica que no discrimina, teniendo esa evidencia
delante, no tenía sentido.

**Cuándo cuenta.** Hacen falta las cinco condiciones a la vez:

1. **Voz de la casa.** Cuentan los editoriales sin firma o firmados por la
   casa o su director, y los titulares, entradillas y análisis propios no
   atribuidos a una fuente. **No mueven el número:**
   - las columnas firmadas por terceros;
   - las reimpresiones de otros medios;
   - los comunicados reescritos;
   - la propaganda o el contenido pagado.

   Todo eso se declara, pero no cuenta.
2. **A los dos lados de un cambio de gobierno**, dentro de los últimos 12
   meses (regla del presente). Es la prueba del polo fijo: hoy, el cambio del
   07-08-2026. Fiscalizar a quien manda sigue sin contar. Lo que cuenta es la
   asimetría: fiscalizar a un lado y celebrar o disculpar al otro.
3. **Sostenida, no anecdótica.** El barrido es sistemático, sea por sección o
   por términos sobre todo el archivo de 12 meses, y no una selección de
   ejemplos. El mínimo:
   - al menos **10 piezas con postura** en voz de la casa;
   - con **al menos 3 a cada lado** del cambio de gobierno;
   - y una proporción de **al menos 3 a 1** en la misma dirección.

   Por debajo de eso es nivel 5 y no mueve el número, salvo lo que dispone la
   precisión del 2026-10-10 (más abajo).
4. **Contrapesos escritos.** La ficha dice qué contradice la dirección y
   cuánto pesa.
5. **Reproducible.** La resolución lista las piezas del barrido con URL, fecha
   y clasificación, para que cualquiera pueda recontarlas y llegar o no al
   mismo número.

**Precisiones del responsable editorial (2026-10-09 y 2026-10-10):**
- **Fiscalizar no cuenta para el mínimo por lado.** Para llegar a 3 piezas a
  cada lado del cambio de gobierno solo cuentan los elogios, las disculpas y los
  rótulos. Una pieza que solo fiscaliza a quien manda se declara, pero no suma,
  igual que en el polo fijo.
- **Un barrido que no llega a los mínimos no deshace nada.** La ficha conserva el
  valor que tenía. La regla añade una vía para mover el número; no retira
  valores puestos por otras razones.
- **Salvo que el valor solo se apoye en los niveles 4 y 5** (precisión del
  2026-10-10, tandas 8 y 9). Si el número salió de la misión declarada, de
  la comparación con otros medios o de una frase sin fuente, el barrido manda:
  - si **cumple** las cinco condiciones → el valor del barrido, con el tope de
    abajo;
  - si **no llega** pero documenta **la misma conducta con los dos
    gobiernos** —al menos 3 piezas de fiscalización o postura a cada lado del
    cambio, y la postura por debajo de 3:1— → **0,00 con evidencia**;
  - si **no llega** y la dirección es **clara** (la postura va en un solo
    sentido pero sin los mínimos) → **«sin medir»** (`bias: null`), con la
    dirección declarada como tensión;
  - si **no llega** y no hay piezas suficientes a cada lado para juzgar →
    **«sin medir»** (`bias: null`).

  Aplicado el mismo día: Las2Orillas y CasaMacondo, 0,00 con evidencia; Razón
  Pública, Vorágine y Cuestión Pública, sin medir; Revista RAYA y Volcánicas,
  por el barrido (ver DECISIONES.md, tandas 8 y 9).

  Sin esta salvedad, un número sin evidencia sobrevivía a un barrido que no
  llegaba, y quedaba más lejos del centro que uno con evidencia que sí llegaba
  y topaba en ±0,30.

**Endoso explícito** (definido el 2026-10-10, Cuestión Pública): que **el medio**
pida el voto por un candidato con nombre o declare su apoyo a él, en su voz
(editorial o pieza sin firma, o de quien lo dirige en un espacio que lo
compromete). Una columna firmada que encuadra con dureza a un candidato pero
niega el apoyo, o que va en una sección que «no compromete al medio», no es
endoso: entra en el barrido como pieza con postura.

**Cuánto mueve.** Sin propiedad documentada con posición conocida (nivel 1) ni
endoso explícito, **la magnitud no pasa de ±0,30**, la banda moderada. El valor
exacto es un **juicio declarado**: se razona contra los medios vecinos de la
escala y se escribe así. La regla 2 sigue en pie: ante la duda entre dos
bandas, la más cercana a la mixta.

**Lo que también hace: el 0,00 con evidencia.** Un barrido que muestra la
misma conducta con los dos gobiernos sostiene el 0,00 como evidencia, y ya no
como valor por defecto. La ficha lo dice así.

**Medios del Gobierno nacional: excepción al polo fijo (decisión del responsable editorial,
2026-10-10, RTVC).** Un medio que depende del Gobierno nacional y cuya línea
sigue a la del gobierno de turno —oficialismo con los dos gobiernos, sin línea
propia— **toma la dirección del gobierno que lo controla**, con la magnitud
tope (±0,30) y la marca «gubernamental» en su ficha. Se revisa en cada cambio
de gobierno, y el número cambia de signo si el gobierno lo hace. El lector ve
así hacia dónde empuja hoy ese medio, y la ficha dice por qué. Los canales
regionales de gobiernos locales (Telecafé, Telemedellín, Canal Capital,
Telecaribe) siguen en 0,00: la excepción cubre solo al Gobierno nacional; los
canales de gobiernos locales se miden por la regla general.

**Lo que NO cambia.**
- La compañía media sigue sin poder mover un número.
- La firma sigue pidiendo lo que pedía. Mover el valor no hace firmable la
  ficha.
- La regla se aplica a la vez a todas las fichas afectadas. Las ya cerradas
  que se quedaron quietas por la regla 3 teniendo una dirección declarada
  (Proclama del Pacífico, El Pilón, El Diario de Pereira, Diario La Libertad y
  Seguimiento) se reexaminan con el mismo barrido el mismo día. Así no hay una
  regla para unos medios y otra para otros.

### DATOS PERSONALES (añadida el 2026-10-08 por el responsable editorial, ciclo 2, tanda 3)

**Nunca se escriben, ni en las fichas ni en las respuestas de revisión, los
números de cédula, los teléfonos ni las direcciones particulares de personas
naturales.** Basta con el nombre, su papel en el medio y el enlace a la fuente
pública donde consta (SECOP, RUES, el propio medio).

**Por qué.** El responsable editorial es el responsable del tratamiento de datos (Ley 1581;
`/transparencia/datos`). Que un dato sea consultable en SECOP no lo convierte
en algo que este repositorio necesite copiar: nada de lo que el lector tiene
que saber depende de un número de documento. En la tanda 3, dos revisores
copiaron cédulas para identificar a dueños que operan como persona natural.

**Si un revisor las copia**, se sustituyen en la respuesta literal por «[número
de cédula omitido: dato personal de una persona natural, Ley 1581]», y la
sustitución se declara al principio de la resolución. Es la única edición
permitida de una respuesta literal.

**Lo que no cubre:** los NIT de sociedades y los datos de contacto que un
medio publica como empresa para sus lectores. Aun así, cuando el dueño es una
persona natural, ni su teléfono ni su dirección pasan a la ficha.

**Tampoco se enlaza una página que los muestre (2026-10-10, tandas 6 y 7).**
No basta con no escribir el número: una URL de SECOP, del RUES o de
contratos.gov.co puede abrir una página o un JSON con la cédula de quien
contrató a su nombre, o con la del representante legal de una sociedad. Por
eso:

- Las consultas a datos.gov.co se enlazan **con `$select`**, limitado a los
  campos que se citan (p. ej. `?$select=razon_social,estado_matricula,...
  &nit=...`). La fuente sigue siendo auditable y no devuelve documentos de
  identidad. Se comprueba antes de escribirla.
- Las constancias de contratos.gov.co y los procesos de SECOP II se citan como
  **texto** (entidad, fecha, valor, número), sin enlace.
- Los PDF que publica el propio medio con documentos de identidad (estatutos,
  informes, estados financieros) no se enlazan: se nombra el documento y se
  enlaza la página del medio de la que cuelga.
- Tampoco pasan a la ficha la nacionalidad, el origen étnico ni el lugar de
  nacimiento de una persona natural.

Rige para todo el catálogo, también para las fichas ya cerradas.

---

### CONTRATACIÓN PÚBLICA (añadida el 2026-10-07 por el responsable editorial, ciclo 2, tanda 2)

**Cada ficha de propiedad declara la contratación pública del medio y de su
sociedad editora.** Salió de la tanda 2: cuatro de cinco medios regionales
tenían contratos con los gobiernos locales que cubren, y ninguna de sus fichas
lo decía (Pereira, Ibagué, Santa Marta y el Huila).

**Qué se consulta.** SECOP I y SECOP II por el NIT de la sociedad editora,
en datos.gov.co, con la fecha de consulta.

**Qué se escribe, siempre con el mismo formato:**

> Contratación pública (SECOP I y II, NIT X, consultado AAAA-MM-DD): N contratos
> por $V **contratados** en los últimos 12 meses; N′ por $V′ en total desde AAAA.
> Principales contratantes: … . [Si alguno es un gobierno que el medio cubre, se
> dice.]

- **«Contratado», nunca «cobrado» ni «pagado».** SECOP no registra los pagos de
  forma fiable (`valor_pagado` suele estar en 0). Decir «cobró» sería afirmar más
  de lo que consta.
- **Sin NIT conocido**, se escribe «NIT no localizado; contratación pública sin
  consultar» y se deja como laguna declarada.
- **Cero contratos** también se escribe: «0 contratos en SECOP I y II a
  AAAA-MM-DD». Una ausencia comprobada es un dato.

**Qué es y qué no es.** Es **desvelamiento, no acusación**, igual que el aviso
de propiedad. No mueve la clasificación por sí sola. Si los editoriales
elogian a quien contrata, eso se declara como tensión en la ficha de sesgo, y
el número se sigue moviendo solo con corpus (regla 3).

---

### DOCUMENTO DE PROPIEDAD Y FUENTES FIDEDIGNAS (añadida el 2026-10-11 por el responsable editorial; ajustada el mismo día)

> Rige desde el 2026-10-11 (ver `DECISIONES.md`, dos entradas de ese día). La
> primera versión pedía un certificado de Cámara de Comercio por cada medio
> colombiano del catálogo. El ajuste del mismo día lo reserva para cuando cierra
> una pregunta concreta: en S.A. y S.A.S. el certificado no trae a los
> accionistas, y el RUES abierto ya prueba gratis casi todo lo demás. La lista de
> compra que resulta está en `docs/certificados-camaras.md`.

**La propiedad de un medio se documenta con fuentes fidedignas, cada una por lo
que prueba y citada con fecha.** Ninguna fuente lo prueba todo, y la ficha no
finge que alguna lo haga.

**Las fuentes fidedignas, y qué prueba cada una.**

1. **El RUES abierto** de datos.gov.co (conjunto `c82u-588k`), consultado con
   `$select` y sin campos de identificación (ver DATOS PERSONALES). Prueba la
   razón social, el NIT, la organización jurídica (S.A., S.A.S., Ltda., ESAL,
   persona natural), la cámara y la matrícula, el estado, las fechas de
   matrícula, renovación y cancelación, la actividad registrada y, cuando el
   registro lo trae, el nombre del representante legal. Cualquiera puede repetir
   la consulta gratis, y por eso es la fuente de base. **No prueba** socios,
   accionistas, junta directiva ni capital.
2. **SECOP I y II**, con el formato de CONTRATACIÓN PÚBLICA. Prueba qué contrató
   la sociedad o la persona, con quién, por cuánto y cuándo, y quién firmó por
   ella en cada contrato. **No prueba** propiedad, y el perfil del proveedor
   puede estar desactualizado: el representante legal que da SECOP vale para la
   fecha del contrato, no para hoy.
3. **Lo que el medio declara de sí mismo** (su página de quiénes somos, su
   política editorial, sus informes, su perfil autodeclarado en un directorio),
   marcado siempre **«según el propio medio»**, con la URL y la fecha de lectura.
   Prueba lo que el medio afirma y lo compromete en público. **No basta** si otra
   fuente lo contradice ni si hay un conflicto de interés: que el medio, sus
   dueños o quien lo dirige contraten con quien cubren, tengan un cargo o una
   candidatura, o se anuncie un comprador con intereses en lo que el medio
   cubre. En esos casos la autodeclaración se cita, pero no cierra la pregunta.
4. **Prensa de terceros y monitores** (Media Ownership Monitor, SembraMedia),
   atribuidos: «según X, fecha». Prueban lo que dicen a la fecha en que lo
   dicen. Un perfil «elaborado a partir de información proporcionada por el
   propio medio» es autodeclaración y se marca como tal.
5. **Registros oficiales de otros países**, para los medios internacionales, por
   lo que cada registro inscribe.

**Lo que no prueba ninguna, y la ficha lo dice siempre.** Cada ficha de
propiedad termina con lo que ninguna de sus fuentes prueba. El caso general: en
una S.A. o una S.A.S., **nadie de esas fuentes prueba los accionistas
actuales**, y tampoco el certificado de la Cámara, porque las acciones se
transfieren en el libro de accionistas de la sociedad, que no se inscribe. La
ficha no escribe «lo diría el certificado» cuando el certificado no lo diría:
escribe «accionistas actuales: no constan en ninguna fuente pública», y al lado
lo que sí consta (lo que declara el medio, lo que publicó la prensa, quién lo
representa).

**El certificado de pago de la Cámara de Comercio se compra SOLO cuando cierra
una pregunta concreta**, en uno de estos cuatro casos:

- **(a)** Sociedades limitadas, ESAL (fundaciones, corporaciones, asociaciones)
  y otras cuyo certificado lista socios, fundadores o junta que el RUES abierto
  no muestra (también la empresa asociativa de trabajo).
- **(b)** Contradicción entre fuentes: por ejemplo, un representante legal
  distinto en el RUES y en SECOP, o una forma jurídica distinta según quién la
  nombre.
- **(c)** S.A. en la que la junta directiva importa para la historia: quién la
  preside, si en ella se sienta quien tiene un cargo público o la autoridad
  editorial por estatuto (REGLA DE QUIEN DIRIGE).
- **(d)** Medio con contratos públicos relevantes con gobiernos que cubre,
  cuando la propiedad está en duda.

La pregunta se escribe en `docs/certificados-camaras.md` **antes** de comprar,
con el caso que la justifica. Se pide el certificado de existencia y
representación legal (el de ESAL para una entidad sin ánimo de lucro; el de
matrícula mercantil para una persona natural). La **copia de la constitución**
se pide solo si aporta los accionistas fundadores y la historia lo pide, y la
ficha dice lo que prueba y lo que no: quién suscribió al constituir, no quién
posee hoy. Si el certificado no cierra la pregunta, se dice así.

**Fuera de esos casos no se compra nada.** Basta el RUES abierto más lo que el
medio declara de sí mismo, y lo que falte queda escrito como laguna. Las fichas
que tenían en `falta` un certificado que no cae en (a)-(d) cambian esa línea, en
su próxima revisión, por la laguna declarada con la fórmula de arriba.

**El PDF no se publica nunca.** Trae números de cédula de representantes,
miembros de junta y revisores fiscales: la regla DATOS PERSONALES (§1) lo
excluye del repositorio, de las fichas y de los enlaces. Se guarda en una
carpeta privada **fuera del repositorio y sin versionar**, con copia de
respaldo bajo el control del responsable del tratamiento (el responsable editorial), con el nombre
`<id-del-medio>_<camara>_<AAAA-MM-DD>.pdf`. Ruta: una carpeta hermana del
repositorio, `../doblefoco-privado/certificados/` (fuera de `doblefoco/`, sin
git). Un `.gitignore` no bastaría: un `git add -f` o una copia del árbol la
arrastraría; la carpeta no cuelga del repositorio. Las copias de constitución
siguen la misma regla.

**Se cita así:** «certificado de la Cámara de Comercio de X, expedido el
AAAA-MM-DD», con el código de verificación si lo trae. Con ese código
cualquiera puede ver en el sitio de la cámara la imagen del certificado tal
como se expidió, sin pagar, **pero solo durante 60 días calendario desde la
expedición** (así lo imprimen los certificados de las cámaras de Bogotá,
Medellín y Cúcuta; para las demás, por confirmar). Pasado ese plazo, lo que
sigue haciendo verificable la cita es que el registro mercantil es público:
cualquiera puede comprar hoy el mismo certificado por 1 UVB y contrastarlo. La
ficha no promete más que eso. El RUES abierto y SECOP se citan con su enlace con
`$select` y la fecha de consulta; la autodeclaración, con la URL y la fecha de
lectura.

**Registro versionado, sin datos personales:** `docs/certificados-registro.md`,
una fila por certificado:

| Medio | Cámara | Expedido | Código de verificación | Pedido por |
|---|---|---|---|---|

«Pedido por» es el cargo o el nombre de quien lo pidió en DobleFoco, no el de
nadie del medio. No se anotan el número de recibo, el PIN de descarga ni nada
que el PDF diga de personas.

**Qué pasa a la ficha desde un certificado** (`mediaOwnership.js` y
`fichas/<id>.md`), citado con la fórmula de arriba:

- razón social, NIT, tipo de sociedad, cámara y matrícula, estado (activa, en
  liquidación, cancelada), fecha de constitución y de la última renovación;
- capital autorizado, suscrito y pagado;
- objeto social o actividad registrada, cuando dice algo del medio (una
  sociedad de publicidad que edita un periódico);
- la junta directiva y la representación legal **por cargo**. El nombre solo
  cuando su papel es la historia: si es socio o accionista, si dirige la
  redacción, si representa también a otra sociedad del caso o si dispara la
  REGLA DE QUIEN DIRIGE. Es la misma línea que la cabecera de
  `mediaOwnership.js`: cuando la persona manda, se dice quién es; cuando solo
  firma, basta el cargo;
- los socios, asociados o fundadores con nombre, si el documento los trae: son
  la propiedad, que es lo que la ficha existe para decir.

**Qué no pasa:** cédulas y demás números de documento; domicilios y teléfonos
de personas naturales; suplentes, revisores fiscales y apoderados, salvo que su
papel sea la historia; embargos, medidas o anotaciones sobre personas; el PDF y
cualquier enlace a él.

**Vigencia.** El certificado que se tenga se renueva cada 12 meses, con la
revisión ordinaria (§7), y siempre que haya cambio de propiedad o de
representación legal (revisión extraordinaria, §7). Un certificado de más de 12
meses se sigue citando, con su fecha, pero la ficha queda marcada para
renovarlo. Las consultas al RUES abierto y a SECOP se repiten en cada revisión
ordinaria, con la fecha nueva. Si al renovar la pregunta ya está cerrada por
otra fuente fidedigna, el certificado no se renueva y se dice por qué.

**Si no hay sociedad identificable**, o la búsqueda en el RUES no da matrícula,
no se compra nada a ciegas: el medio queda en **ausencia declarada**
(`ownerType: null`, con `consultadoEl`, `buscadoEn` y `falta`; ver
`mediaOwnership.js` y la decisión del 2026-08-12 en `DECISIONES.md`), y en
`buscadoEn` se anota qué se buscó en el RUES, por razón social y por nombre de
establecimiento. Si el medio lo explota una persona natural, la matrícula y sus
establecimientos se buscan primero en el RUES; el certificado de matrícula
mercantil, solo si además cae en (a)-(d).

**Cómo encaja con lo que ya rige.**

- **DATOS PERSONALES:** el certificado y las copias son fuente, no texto que se
  publica. Lo que pasa a la ficha pasa por esa regla; el PDF no se enlaza por la
  misma razón que una consulta de datos.gov.co sin `$select`, y del RUES
  abierto nunca se pide el campo del documento del representante.
- **CONTRATACIÓN PÚBLICA:** SECOP es fuente de esta regla con el formato de
  aquella. El caso (d) usa sus números: «relevantes» quiere decir que el medio
  vive en parte de ese dinero o que el contratante es un gobierno que el medio
  cubre a diario.
- **Ausencia declarada:** las fuentes fidedignas la cierran cuando existe la
  sociedad; cuando no existe, la ausencia sigue siendo el estado correcto, con
  la búsqueda en el RUES dentro de `buscadoEn`. Que un certificado no se compre
  no es una ausencia: es una laguna declarada con lo que sí consta.
- **Firma (§6):** quien firma la ficha ha visto el certificado que cita y ha
  hecho o repetido la consulta del RUES abierto. Un certificado de más de 12
  meses no invalida una firma, pero la revisión ordinaria no se da por hecha sin
  renovarlo.
- **Regla del presente** (§2): rige la orientación, no la propiedad, pero la
  idea es la misma. Cada fuente fecha lo que dice; una nota de prensa o un
  certificado de hace años es historia de la sociedad, no su presente. Si una
  fuente fidedigna de fecha posterior contradice a otra, se declara la tensión
  y, si cae en (b), se compra el certificado.

---

### REGLA DE QUIEN DIRIGE (añadida el 2026-09-02 por el responsable editorial, en la sesión de decisiones)

**La política de quien DIRIGE la redacción es materia de aviso cuando es una
candidatura o un cargo público vigente. Nada más lo es.**

El mapa de propiedad nombra a quien posee. Pero quien decide qué se publica es
quien dirige, y cuando esa persona compite por un cargo o lo ocupa, el lector
tiene derecho a saberlo al leer el medio. Es la misma lógica que el aviso de
propiedad: **desvelamiento, no acusación**, y no mueve la clasificación.

**Qué dispara el aviso.** Una candidatura anunciada o inscrita, o un cargo
público en ejercicio, de quien dirige la redacción —directora, director,
editor general—, **con fecha y con fuente consultable**. La fuente tiene que
estar en la lista de fuentes de la ficha, que es lo que el lector ve.

**AMPLIADA el 2026-10-07 (el responsable editorial): también quien tiene la autoridad editorial por
estatuto.** Si los estatutos o un documento del propio medio dan la máxima
autoridad editorial a otro cargo —presidencia de la junta, presidencia del
grupo— y no a la dirección de la redacción, el aviso se dispara igual por la
candidatura o el cargo público vigente de esa persona. Salió de Semana: su
estatuto da esa autoridad a la presidenta de la junta, Vicky Dávila, y la regla
tal como estaba miraba solo la redacción. Lo que cuenta es dónde reside la
decisión editorial, no el nombre del cargo. La autoridad estatutaria se
acredita con fuente consultable, igual que la candidatura.

**Qué NO lo dispara.** Afinidad, militancia pasada, opinión publicada, parentesco
con un político, o un dueño que hace política: lo del dueño ya tiene su
instrumento en la ficha de propiedad, y lo demás es orientación —y la
orientación se mide con corpus, no con biografía—.

**Cuándo caduca.** Con la candidatura o con el cargo. Se anota `hasta` y el
aviso deja de mostrarse **sin borrarse**: es historia de la ficha.

**Los casos del 2026-09-02.** Diario La Libertad: la directora anunció su
candidatura en su propio periódico el 12-10-2025, sin decir a cuál; se comprobó
ese día que **no se inscribió a la Cámara en marzo de 2026**, y el anuncio no
consta retirado. Aviso publicado **como anuncio**, que es lo que es, y con esa
comprobación escrita: un aviso que afirmara más de lo que consta sería la
misma falta que este protocolo persigue en los medios. La Nación
(Neiva) se había citado como caso hermano, y al aplicar la regla **no la
cumple**: la ficha documenta que el diario cubre a su dueño, que es asunto de
propiedad, y no consta candidatura ni cargo de quien la dirige. No se publica
aviso sin el hecho.

**2026-10-07 (el responsable editorial): el aviso de La Libertad se cerró con `hasta`
2026-06-21.** El anuncio era condicional, se apoyaba en «fuentes cercanas» y no
nombraba cargo ni partido, y la contienda a la que apuntaba terminó ese día sin
que conste inscripción. El componente lo titulaba en presente —«Quien lo dirige
es candidata»—, que era afirmar más de lo que consta: la falta de arriba. Sigue
en la ficha como historia; si se inscribe en 2027, aviso nuevo.

---

## 2. Jerarquía de la evidencia

Ordenada de más a menos fuerte. **Una ficha no puede apoyarse solo en niveles 4
y 5.**

| | Nivel | Qué vale | Dónde está |
|---|---|---|---|
| 1 | **Propiedad documentada** | Quién controla la empresa, con fuente citable y persona natural | `shared/mediaOwnership.js` |
| 2 | **Conducta medida en nuestro corpus** | Qué cubre, con quién coincide, qué omite, cuánto publica | base de datos, `scripts/coCoverage.mjs` |
| 3 | **Registros externos** | MOM/RSF, Observatorio de Medios de la MOE, ColombiaCheck, sentencias | enlace directo |
| 4 | **Declaraciones del propio medio** | Su manifiesto, su línea declarada, su historia institucional | enlace directo |
| 5 | **Hechos editoriales notorios** | Portadas, coberturas o decisiones que tuvieron consecuencia pública verificable | enlace directo |

### REGLA DEL PRESENTE (añadida el 2026-08-08 por el responsable editorial, tras la primera ficha)

**Toda evidencia de orientación tiene que ser sobre el presente. Estrictamente.**

Un hecho del pasado —por notable, heroico o infame que sea— no dice nada de la
línea de hoy. El caso que zanja la discusión es **Semana**: destapó las chuzadas
del DAS bajo el gobierno de Uribe, y hoy está clasificada en **+0,45**. Misma
cabecera, línea opuesta. Si el pasado contara como evidencia, Semana tendría que
estar a la izquierda.

Lo que esto excluye, aunque esté bien documentado y sea cierto:

- fundaciones, efemérides y «tradiciones» («diario de tradición liberal»)
- hechos editoriales notables de otra época —premios, denuncias, atentados
  sufridos, directores asesinados—
- la línea de un dueño o un director **anteriores**
- la afirmación de un registro externo cuando esa afirmación es histórica: MOM
  dice que El Espectador «ha estado asociado **desde su fundación** a la defensa
  de ideas liberales», y eso describe 1887, no 2026

**Esto invalidó las dos mitades de la primera ficha**, la que apoyaba la
propuesta y la que la atacaba. La regla no se aplica solo cuando incomoda al
argumento contrario.

**Lo que sí sobrevive del pasado**: un hecho antiguo que además **sea una
estructura vigente**. «Fundado en 1957» no vale; «es el órgano del Partido
Comunista, que hoy lo posee» sí, porque la propiedad es comprobable hoy. La
prueba: si el hecho dejara de ser cierto mañana, ¿cambiaría la clasificación? Si
la respuesta es no, es historia y no evidencia.

**Consecuencia para el nivel 5** de la tabla de arriba: «hechos editoriales
notorios» solo cuenta si son **de los últimos 12 meses**.

### Lo que NO cuenta como evidencia

- **El juicio de un modelo de lenguaje sobre la posición del medio.** Es una
  compresión de texto de internet que probablemente incluye especulación sobre
  esta misma pregunta. Rompe la procedencia y no es reproducible entre versiones.
- **La coincidencia entre varios modelos.** Mide fiabilidad, no validez:
  comparten datos de entrenamiento y se equivocan de forma correlacionada.
- **La reputación** («todo el mundo sabe que…»). Si no hay dónde consta, no entra.
- **El volumen de reportes de lectores.** Un recuento de quejas no es una fuente.

---

## 3. El papel de la IA, invertido

**El modelo no dictamina: redacta y ataca.**

1. **Redacción.** Compone el borrador de la ficha a partir de la evidencia de los
   niveles 1-5, con cada afirmación enlazada. No añade nada que no pueda enlazar.
2. **Ataque.** A cada modelo consultado se le pide **argumentar EN CONTRA** de la
   clasificación propuesta, con evidencia. No se le pregunta si está de acuerdo.

**El acuerdo no se registra como validación.** Si los modelos coinciden, la ficha
no gana nada: puede ser el mismo prejuicio repetido. **Lo que se publica es el
desacuerdo**, con el nombre del modelo, su versión y la fecha — porque las
versiones cambian y una revisión de agosto de 2026 no es repetible en 2027.

Si una objeción resulta sólida, **se cambia el número o se declara la tensión en
la ficha**. Una objeción que se ignora sin motivo escrito invalida la firma.

---

## 4. Forma de la ficha

```
MEDIO · valor propuesto · firma · fecha
├─ EVIDENCIA     por niveles, cada punto con su enlace
├─ ARGUMENTO     por qué ese valor y no el contiguo
├─ CONTRA        el mejor caso en contra que se encontró
├─ REFUTACIÓN    qué observación concreta cambiaría el número
└─ REVISIÓN      qué objetó cada modelo · versión · fecha
```

**El campo REFUTACIÓN es obligatorio y no admite fórmulas vagas.** «Si cambiara
su línea» no vale. Vale: «si en tres meses su cobertura de X deja de coincidir
con Y», o «si se documenta que Z entró en el capital».

---

## 5. Reglas de decisión

1. **El dueño no determina la orientación, pero se declara siempre.** Un medio
   puede tener línea distinta de los intereses de su propietario; afirmar lo
   contrario por defecto sería determinismo, no evidencia. Lo que no se admite es
   omitir de quién es. Excepción: los medios del Gobierno nacional sin línea
   propia (§1, 2026-10-10).
2. **Ante la duda entre dos bandas, se elige la más cercana a la mixta.** El
   error de clasificar de más es más caro que el de clasificar de menos: acusa.
3. **Sin evidencia de nivel 1-3, no se mueve el número.** Se deja el actual y se
   marca la ficha como incompleta.
   **Excepción (2026-10-09):** la asimetría sostenida en la voz de la casa,
   medida con un barrido histórico, cuenta como nivel 2 si cumple las cinco
   condiciones de «Evidencia editorial histórica» (§1), y mueve como mucho
   hasta ±0,30, **salvo endoso explícito o nivel 1 con posición conocida**,
   que levantan el tope como dice el §1 (precisión del 2026-10-10, El
   Informador: el resumen omitía la salvedad y contradecía al §1).
   **Y la precisión del 2026-10-10** (§1): si el valor solo se apoya en los
   niveles 4 y 5, el barrido manda aunque no llegue, y lo pasa a 0,00 con
   evidencia o a «sin medir».
4. **Un medio puede quedar sin firmar.** Es mejor que firmarlo sin fundamento.
5. **La ficha se publica entera**, incluido el contra-argumento. Publicar solo la
   conclusión convertiría el ejercicio en autoridad, que es lo contrario de lo
   que busca.

---

## 6. Quién firma y qué significa

Firma **el responsable editorial**, como responsable editorial de DobleFoco. La firma
significa: *he leído la evidencia, el argumento y la objeción, y sostengo este
número públicamente y sujeto a réplica.*

No significa que el número sea correcto. Significa que **hay alguien a quien
preguntarle por qué**, que es exactamente lo que hoy no hay.

---

## 7. Revisión

- **Ordinaria**: cada 12 meses.
- **Extraordinaria**: cambio de propiedad, cambio de dirección, o cumplimiento de
  la condición escrita en REFUTACIÓN.
- **Por réplica**: cualquier lector puede impugnar una ficha aportando evidencia
  de nivel 1-3. Una impugnación con fuente obliga a responder por escrito.
- **Por objeción del medio** (añadido el 2026-09-02 por el responsable editorial, duda 12): si el
  propio medio objeta su clasificación, su ficha o un aviso, escribiendo desde
  una cuenta suya a `doblefoco.co@gmail.com`, **se acusa recibo en 5 días y se
  responde por escrito en 15**. La objeción y la respuesta **se publican junto a
  la ficha, con fecha**, cambie o no la clasificación —como una `note` de
  `mediaOwnership.js`, con la fecha de recepción y, si el medio publicó su
  objeción, el enlace—. La reclasificación, si la hay, sigue este protocolo
  entero: evidencia de nivel 1-3, regla del presente, refutación. Un dato de
  hecho demostrado errado —dueño, fecha, cargo— se corrige siempre. La
  insistencia no es evidencia. El procedimiento está publicado en
  `/transparencia/limitaciones`; si los plazos cambian, cambian en los dos sitios.

**El caso previsto**: la ficha de RTVC ya lleva anotado que su gerencia depende
del gobierno de turno y que el período cambió el 7 de agosto de 2026. Fue la
primera revisión extraordinaria, y se hizo el 2026-10-10 (ciclo 2, tandas 8 y 9): el
barrido confirmó que sigue a quien gobierna, y RTVC pasó a **+0,30
«gubernamental»** por la excepción de los medios del Gobierno nacional (§1).
