# Las fichas de orientación — qué hay en esta carpeta

Una ficha por medio, con la evidencia que sostiene su valor de sesgo y el
argumento en contra. El protocolo que las gobierna es
`../PROTOCOLO_JUICIO_EDITORIAL.md`; el circuito que las cierra,
`../revision-externa/`.

## Aquí hay DOS cosas distintas, y confundirlas hace mal las cuentas

**Esto se escribe porque ya pasó** (2026-08-18): al contar las fichas contra el
registro salieron **siete que no corresponden a ningún medio del catálogo**, y se
leyeron como huérfanas —medios dados de baja, o altas que nunca llegaron al
registro—. No era ninguna de las dos cosas. Son una categoría propia que existía
de hecho y no estaba escrita en ninguna parte.

### 1 · Fichas de medio

De un medio que **está en `shared/mediaRegistry.js`** y que el lector ve en el
sitio. Llevan valor, `reviewedAt` y firma pendiente o puesta. Son las que entran
al circuito de revisión externa.

### 2 · Fichas de candidatura

De un medio que **se evaluó para entrar y no entró**. No están en el registro, y
eso es el resultado del trabajo, no un olvido. Se reconocen por la cabecera:

```
| **Valor propuesto** | **ninguno** — … |
| **Firma**           | ☐ no procede … |
```

**Por qué se conservan en vez de borrarlas.** Es la misma regla que rige todo lo
demás aquí: *un hueco declarado se puede leer; uno escondido vuelve como
objeción.* Un departamento sin medio en el mapa es una afirmación —«aquí no
encontramos ninguno admisible»— y esa afirmación necesita su expediente. Sin
estas fichas, la ausencia parecería descuido y nadie sabría qué se miró ya.

Las de hoy, con su motivo:

| Ficha | Por qué no entró |
|---|---|
| `diario-de-cundinamarca.md` | Inactivo desde el 22-07-2026; su director es contratista de difusión de la Alcaldía de Soacha |
| `diario-del-sur.md` | El alta no se recomienda todavía |
| `ecos-del-combeima.md` | Sin alta: pauta informativa pagada por la Alcaldía de Ibagué y la Gobernación del Tolima, y control sin documentar tras la muerte de su fundador (ciclo 2, 2026-10-10). La afiliación a Blu es de programación, no de propiedad |
| `cordoba-narino-segunda-vuelta.md` | **Ficha conjunta de cuatro candidatos**: los cuatro tienen la misma evidencia —ninguna— y el mismo siguiente paso |

## Cómo contar bien

```
archivos en fichas/*.md        = fichas de medio + fichas de candidatura + este LEEME
fichas de medio               = las que corresponden a un id de MEDIA_REGISTRY
```

Al 2026-08-18: **57 archivos**, de los cuales **50 son fichas de medio** y 7 de
candidatura. Los medios del registro son **76**, así que **26 siguen sin ficha** —
y entre ellos están los que calibran los extremos del eje: el Semanario VOZ
(−0,80) y El Nuevo Siglo (+0,55).

Al 2026-10-10, tras las altas de `el-informador.md`, `el-isleno.md` y
`sucre-noticias.md` (ciclo 2, tanda 7), que pasan de candidatura a ficha de
medio: **68 archivos**, de los cuales **63 son fichas de medio**, 4 de
candidatura y este LEEME. Los medios del registro son **82**, así que **19
siguen sin ficha**.

Cualquier frase del tipo «hay N fichas» tiene que decir de cuál de las dos habla.
