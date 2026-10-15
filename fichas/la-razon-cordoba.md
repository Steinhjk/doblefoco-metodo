# LA RAZÓN.CO (Montería) — ficha de orientación

| | |
|---|---|
| **Medio** | La Razón.co (Montería) · `la-razon-cordoba` · larazon.co |
| **Valor vigente** | **0,00** — orientación mixta, provisional |
| **Firma** | ☑ **FIRMADA el 2026-10-10 — el responsable editorial** (firma en bloque tras el ciclo 2; ver DECISIONES.md. Lo que más abajo dice «sin firmar», «no se firma» o «provisional» es el estado anterior a esta firma y se conserva como historia) |
| **Alta** | 2026-08-09 (candidatura) · **2026-08-11 (alta)** · 2026-10-07 (correcciones del ciclo 2, tanda 2) |
| **Última revisión** | — |
| **Departamento / ámbito** | Córdoba |
| **Fuentes de propiedad** | `shared/mediaOwnership.js` (`la-razon-cordoba`): 7 fuentes<br>**Propiedad:** **ausencia declarada de los socios**: constan la sociedad y su representante legal — ver `shared/mediaOwnership.js` |
| **Recogida** | `https://larazon.co/feed/` · vía `direct` |
| **Protocolo** | `PROTOCOLO_JUICIO_EDITORIAL.md` |

## Estado

**0,00, orientación mixta, provisional**, por
ausencia de evidencia y no por evidencia de equilibrio. **Firmada el 2026-10-10**
en la firma en bloque del catálogo (cabecera, «Firma»). La cabecera no da fecha
de última revisión («—»); la última corrección es la del ciclo 2, tanda 2
(2026-10-07), que cambió la descripción de la propiedad y del método, no el
número.

**Pendiente:**

- los socios de A & J Medios S.A.S.: constan la sociedad y su representante
  legal, no los accionistas (ausencia declarada en `shared/mediaOwnership.js`);
- la prueba del polo fijo a los dos lados del 07-08-2026 (tensión 1);
- medir su encuadre, que es lo único que puede mover el 0,00 con evidencia
  propia.

## Evidencia

### Nivel 1 — Hay sociedad y representante legal; no hay socios

| Dato | Valor | Fuente |
|---|---|---|
| Sociedad | **A & J MEDIOS S.A.S.**, NIT **900773173** | SECOP I (`f789-7hwg`) y SECOP II (`jbjy-vk9h`), consultados el 2026-10-07; la nombra el propio medio en [`/anuncia-con-nosotros/`](https://larazon.co/anuncia-con-nosotros/), página modificada el 2025-01-21 |
| Representante legal | **Luis Darío Díaz Cárdenas** | SECOP I; último contrato firmado el 2026-04-24, constancia 26-4-14713277 |
| Director | **Luis Darío Díaz**, autodeclarado por el medio el 2025-04-30 | [`/larazon-co-celebra-11-anos-de-liderazgo-informativo-en-cordoba/`](https://larazon.co/larazon-co-celebra-11-anos-de-liderazgo-informativo-en-cordoba/) |
| Socios | **no constan** | — |
| Establecimiento | **Larazon.co Diario Digital**, constituido el **24-09-2014** | DataCrédito Empresas, consulta manual del 2026-08-09 |
| Dirección registrada | Carrera 5 n.º 68-09, Montería, Córdoba | DataCrédito (2026-08-09) y el pie de la portada (2026-10-07) |
| Contacto de gerencia | `[correo omitido]` | DataCrédito y `/anuncia-con-nosotros/` |

**DataCrédito dio el 2026-08-09 el establecimiento, la constitución, la
dirección y el correo, y nada más**: ni representante legal ni socios. Su
servidor responde **403 a las consultas automatizadas** —se probó con un
navegador completo, no es el caso de la tilde en el User-Agent—, así que ese
dato se cita con la fecha de la consulta manual.

La página `/anuncia-con-nosotros/` dice literal: «Bienvenidos a A & J MEDIOS
S.A.S.» y «Desde 2014, A & J MEDIOS S.A.S. se ha dedicado a fortalecer la imagen
de marcas y empresas a través de sus servicios publicitarios.» En SECOP I, los
42 registros del NIT nombran como representante legal a Luis Darío Díaz
Cárdenas en 41, con variantes de tecleo. Uno de 2019 (constancia 19-4-8984250)
une la sociedad al medio de forma expresa: «A TRAVeS DEL DIARIO DIGITAL LA
RAZoN.CO».

**SECOP da el representante legal, no los accionistas.** Por eso `ownerType`
sigue en `null` y la ausencia declarada se mantiene, ahora acotada a los socios:
quien representa una sociedad no es por eso su dueño.

**Las páginas institucionales.** `/nosotros/` y `/contacto/` **redirigen con 301
a noticias antiguas** (comprobado el 2026-10-07 con `curl -sIL`): la primera, a
una pieza sobre la JEP y los falsos positivos; la segunda, a una sobre un caso
de covid-19 en la DIAN. Es la redirección por coincidencia de slug de WordPress.
La comprobación del 2026-08-11, que decía que esas páginas no publicaban mástil
y que la presentación estaba maquetada como imagen, se hizo sobre esas dos
noticias. **Las páginas institucionales reales son `/contactenos/` y
`/anuncia-con-nosotros/`**, la segunda con texto legible. El pie de la portada
dice «© 2026 Todos los derechos reservados. . Dirección: Carrera 5 # 68 – 09
—Barrio El Recreo— Montería, Córdoba.» y no trae NIT ni director.

**Regla de quien dirige.** No consta candidatura ni cargo público vigente de
Luis Darío Díaz (comprobado el 2026-10-07). No hay aviso.

### Nivel 2 — Conducta medida, 2026-08-31 a 2026-10-07

```
artículos ............................ 1023
en alguna historia ................... 299
historias ............................ 344  ·  compartidas 293
agenda propia ........................ 15 %
compañía media ....................... +0,145
coincide más con ..................... El Heraldo 91 · Caracol Radio 75 · Infobae 66
```

Medición del 2026-10-07. **Son 37 días y el protocolo pide 90**: no valida el
número, y la compañía media no se usa para moverlo. Ingerido desde el
2026-08-11; agenda de Montería y el resto de Córdoba —Chinú, Sahagún, Lorica—.

## Argumento

### POR QUÉ 0.00 Y NO «SIN NÚMERO»

Mismo criterio que Proclama del Pacífico, Chocó 7 Días y MiPutumayo: **nada de la
evidencia lo sitúa en el eje**, y la regla del protocolo manda entonces la banda
más cercana a la mixta.

Conviene decirlo sin adornos: **es orientación mixta por ausencia de evidencia,
no por evidencia de equilibrio.** No hemos medido su encuadre; hemos comprobado
que no tenemos con qué moverlo del centro. Son cosas distintas y la ficha pública
lo dice.

## El mejor caso en contra

- **Hacia «sin medir», o hacia un barrido ya (el más fuerte).** El 0,00 no sale
  de ninguna lectura de su voz: «No hemos medido su encuadre» (Argumento). La
  ficha remite la prueba del polo fijo al barrido de 12 meses (REFUTACIÓN,
  5 y 6): desde el 2026-10-09 el protocolo deja barrer el archivo del
  propio medio sin esperar, y nadie lo ha hecho. Mientras tanto, el número que ve
  el lector no tiene una pieza detrás.
- **Hacia la derecha, por la compañía.** Su compañía media es de +0,145 en 37
  días, y coincide sobre todo con El Heraldo, Caracol Radio e Infobae. El
  protocolo no deja que la compañía media mueva un número.
- **Hacia ninguna dirección, por lo que sí se ve.** Con Petro y con De la
  Espriella domina el titular-cita del poder de turno, con una pieza crítica por
  periodo, las dos atribuidas a terceros (aeropuerto Golfo de Morrosquillo,
  02-08-2026; vuelos del presidente, 18-09-2026). Es poco para un 0,00 con
  evidencia —la precisión del 2026-10-10 pide al menos 3 piezas a cada lado— y
  nada para una dirección.
- **Hacia una dirección, por el dinero.** Pauta de la Cámara de Comercio de
  Montería hasta mayo de 2026, contenido político vendido en la campaña local de
  2023, y un departamento «con condenas por parapolítica y una elite regional
  estrecha» (REFUTACIÓN, 4). Nada de eso tiene signo en el eje, y el capital de
  los socios no consta.

**Lo que no hay:** ninguna pieza con postura en voz propia que la ficha cite.

## Qué cambiaría el número

### REFUTACIÓN — qué reabriría el expediente

1. **Certificado de Cámara de Comercio de Montería** de A & J Medios S.A.S.
   **Cumplido a medias** el 2026-10-07: el representante legal ya consta por
   SECOP; los socios no. El certificado sigue haciendo falta para ellos y
   retiraría la ausencia declarada.
2. ~~**Leer su mástil** abriendo la imagen de «Nosotros» en un navegador y
   transcribirla.~~ **Obsoleto:** no había mástil en imagen; era la redirección
   de `/nosotros/` a una noticia.
3. ~~**Confirmar o descartar A&J Medios S.A.S.** con una fuente que se pueda
   abrir.~~ **Cumplido** el 2026-10-07.
4. **Si aparece capital ligado a la política cordobesa** —departamento con
   condenas por parapolítica y una elite regional estrecha— se declara antes que
   cualquier número.
5. **Medir su encuadre** con el barrido de 12 meses del archivo del propio medio
   (evidencia editorial histórica, desde el 2026-10-09; ya no se esperan 90 días
   de corpus): es lo único que puede mover el 0,00 con evidencia propia.
6. **La prueba del polo fijo**, en ese mismo barrido, a los dos lados del
   2026-08-07.

## Tensiones declaradas

### COLISIÓN DE NOMBRE — LA TERCERA DEL CATÁLOGO

No tiene ninguna relación con **La Razón de Madrid** (Grupo Planeta, director
Francisco Marhuenda), ni con La Razón de México, ni con La Razón de Buenos Aires.

Va después de los dos Caracol y los dos El País. Por eso el `name` lleva la
ciudad: `La Razón.co (Montería)`.

### TENSIONES DECLARADAS (2026-10-07)

1. **La prueba del polo fijo está pendiente.** En el periodo de Petro y en el de
   De la Espriella domina el titular-cita del poder de turno. Hay una pieza
   crítica por periodo, las dos atribuidas a terceros: el aeropuerto Golfo de
   Morrosquillo (2026-08-02) y los vuelos del presidente (2026-09-18). No hay
   medición de dureza relativa. Se hace con el barrido de 12 meses del archivo del
   propio medio (desde el 2026-10-09 ya no se esperan 90 días de corpus).
2. **Conflicto vigente con la Cámara de Comercio de Montería.** Pauta mensual en
   sus redes hasta mayo de 2026, y es la entidad que previsiblemente lleva su
   registro mercantil, aunque no se ha comprobado con certificado. Se declara
   como desvelamiento para la cobertura de esa entidad, no como vínculo
   partidista, y no mueve el número.
3. **Contrato con la Defensoría del Pueblo (2024).** La delegada de Libertad de
   Expresión contrató a un medio por $72.000.000 para producir contenidos. Es
   historia por la regla del presente (ejecución hasta el 2024-12-31), aunque el
   registro aún lo marca «En ejecución». Contexto de la relación con el Estado,
   no evidencia.
4. **Contenido político vendido.** Las categorías «contenido-patrocinado» (2
   entradas, ambas de septiembre de 2023) y «larazonpolitica» (14 entradas, de
   la campaña local de 2023) son historia. Se vigila en las locales de 2027.
5. **Los socios siguen sin documentar.** Hasta tener el certificado mercantil,
   la ficha dice quién representa la sociedad, no de quién es.

## Contratación pública

> Contratación pública (SECOP I y II, NIT 900773173, consultado 2026-10-07): 6
> contratos por $15.300.000 **contratados** en los últimos 12 meses; 43 por
> $227.850.000 en total desde 2018. Principales contratantes: Cámara de Comercio
> de Montería, Defensoría del Pueblo y E.S.E. CAMU El Amparo (Montería). Entre
> los que el medio cubre están la Alcaldía de Sahagún (2019) y la Personería de
> Montería (2018); no consta ninguno con la Gobernación de Córdoba ni con la
> Alcaldía de Montería bajo este NIT.

| Entidad | Contratos | Suma contratada | Firmas |
|---|---|---|---|
| Cámara de Comercio de Montería (SECOP I) | 32 | $66.350.000 | 2021-09-14 → 2026-04-24 |
| E.S.E. CAMU El Amparo, Montería (SECOP I) | 8 | $61.500.000 | 2018-04-30 → 2022-01-28 |
| Alcaldía de Sahagún (SECOP I) | 1 | $24.000.000 | 2019-07-10 |
| Personería de Montería (SECOP I) | 1 | $4.000.000 | 2018-08-21 |
| Defensoría del Pueblo, CD-813-2024 (SECOP II) | 1 | $72.000.000 | 2024-04-22 |
| **Total** | **43** | **$227.850.000** | 2018-04-30 → 2026-04-24 |

- **Lo vigente son los 6 contratos con la Cámara de Comercio de Montería**:
  dos de $2.450.000 (31-10 y 02-12-2025) y cuatro de $2.600.000 (enero a abril
  de 2026). Son pauta en sus redes: el último, firmado el 2026-04-24, es el
  «SERVICIO DE PUBLICIDAD DURANTE EL MES DE MAYO DE 2026 -30 PUBLICACIONES EN
  LAS REDES SOCIALES DE LARAZON.CO». No consta ninguno firmado después.
- SECOP I no registra adiciones: el valor con adiciones es el mismo.
- El de la Defensoría es por contratación directa, para la Delegada para la
  Protección de Derechos en Ambientes Digitales y Libertad de Expresión
  («producción y difusión de contenidos y piezas pedagógicas…»), con ejecución
  del 2024-05-09 al 2024-12-31.

Es **desvelamiento, no acusación**, y no mueve el número.

## Propiedad y lo que no consta

### UNA PISTA QUE NO SE PUBLICÓ, CONFIRMADA EN PARTE EL 2026-10-07

Una búsqueda del 2026-08-11 devolvió que el medio pertenecería a **«A&J Medios
S.A.S.»**, dirigido por el periodista **Luis Darío Díaz** con su esposa **Ana
Carolina Buitrago** en la gerencia general, y que el establecimiento figura con
CIIU 7310 (publicidad). Entonces no entró en la ficha: DataCrédito devolvía 403,
el perfil de infoperiodistas era el de **La Razón de Madrid** y la única
corroboración era el resumen de un buscador.

El 2026-10-07 se confirmó en parte, con fuentes que se pueden abrir:

- **A & J Medios S.A.S. y Luis Darío Díaz quedan confirmados**: la sociedad la
  nombra el propio medio y la registra SECOP; él figura como representante legal
  en SECOP y como director en la pieza del 2025-04-30 (ver nivel 1).
- **Ana Carolina Buitrago solo consta como gerente general en 2016**, en una
  pieza del propio medio
  ([`/la-razon-co-ya-es-el-segundo-diario-nativo-digital-mas-leido-en-la-costa/`](https://larazon.co/la-razon-co-ya-es-el-segundo-diario-nativo-digital-mas-leido-en-la-costa/)):
  «LA RAZÓN.CO, Pertenece a la empresa A&J Medios S.A.S. que surgió por
  iniciativa de su director, el Periodista Luis Darío Díaz y su esposa Ana
  Carolina Buitrago (hoy Gerente General).» Es historia por la regla del
  presente. **No se publica como gerente actual.**
- **El CIIU 7310 y la constitución del 24-09-2014 siguen sin fuente abrible**:
  Empresite responde 429 y DataCrédito, 403.

La lección del 11 de agosto se mantiene: un resumen de buscador no es fuente, y
aquí señalaba a dos personas naturales. Lo que entra hoy entra porque hay
documento, y solo hasta donde llega el documento.

## Historial

### QUÉ CAMBIÓ EL 2026-10-07

La revisión externa del ciclo 2 (tanda 2,
`revision-externa/respuestas/opus-5-5-la-razon-cordoba.md`) tumbó la
descripción de la propiedad y del método, **no el número**. El responsable editorial decidió aplicar
las correcciones y no firmar todavía (DECISIONES.md, 2026-10-07):

- **La sociedad y el representante legal sí constan**, en fuentes que se pueden
  abrir: la página institucional del propio medio y SECOP. Lo que sigue sin
  documentar son **los socios**.
- **La comprobación del 2026-08-11 se hizo sobre dos noticias.** `/nosotros/` y
  `/contacto/` redirigen con 301 a piezas antiguas; las páginas institucionales
  son otras.
- **Tiene contratación pública**, y la ficha no la mencionaba.
- **El nivel 2 ya no está vacío**, aunque la medición no llega a los 90 días.

El 0.00 no cambia: sigue siendo ausencia de evidencia en el eje.

### QUÉ CAMBIÓ ENTRE EL 9 Y EL 11 DE AGOSTO

No apareció ningún dato nuevo sobre sus dueños. **Cambió la regla.**

La versión anterior de esta ficha no proponía número y lo argumentaba así: «hay
sociedad y no hay persona; declarar un `ownerType` obliga a afirmar de quién es
el medio». El argumento era correcto y la conclusión —dejarlo fuera— era la que
el catálogo permitía entonces.

El 2026-08-11 el responsable editorial pidió que la ausencia de información se declarara con su fecha
de consulta en vez de resolverse no publicando. Eso convierte `ownerType: null`
en un estado de primera clase: se publica **la búsqueda** cuando no hay
**resultado**. Con esa vía, la objeción que dejaba fuera a este medio deja de
aplicar, porque ya no hay que afirmar de quién es para darlo de alta.

Es el primer medio del catálogo que entra por ahí. Detrás vienen **EL DIARIO de
Boyacá, Vive el Meta y Lente Regional**, que están fuera por exactamente el mismo
motivo y hoy podrían reevaluarse.
