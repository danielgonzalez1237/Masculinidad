# Lluvia de ideas v1 y preguntas para los socios

**Fecha:** 2026-10-26
**Autor:** Claude, en rol de advisor jurídico y cofundador.
**Regla de lectura:** lo marcado **(verificado)** sale de `01-marco-juridico.md` o
`02-benchmark.md` con fuente. Lo demás son **hipótesis de Claude** para discutir. Nada
de esto reemplaza el concepto de un abogado financiero colombiano antes del primer peso.

---

## 1. La idea en una frase

Una **gestora** de los tres socios que estructura proyectos inmobiliarios en el
Oriente Antioqueño y los financia con capital de terceros a través de un vehículo
**administrado por una fiduciaria vigilada**, cobrando honorarios por el trabajo y una
participación en la utilidad, sin prometer rentas fijas.

Lo de "sin prometer rentas fijas" no es un detalle: es la diferencia entre un negocio
y un delito en Colombia.

## 2. La línea roja jurídica (verificado)

Dos normas mandan en todo el diseño:

1. **Captación masiva y habitual** (Decreto 1981 de 1988; art. 316 del Código Penal).
   Hay captación cuando se recibe dinero *con obligación de devolverlo* de más de 20
   personas o en más de 50 obligaciones, y además el total supera el 50 % del
   patrimonio líquido del que recibe **o** se ofreció a personas indeterminadas.
   - Pena: 120 a 240 meses de prisión y multa hasta 50.000 SMMLV (unos COP 87.500
     millones en 2026). Se agrava si se usan redes o medios masivos. El verbo
     "colabore" alcanza a quien estructura o promueve, no solo a quien recibe.
   - No cuentan el cónyuge, parientes hasta 4.º grado ni socios con más del 5 % y
     seis meses de antigüedad. **Los "conocidos" sí cuentan como público.**
   - Un aporte a riesgo (equity, derecho fiduciario, participación en un fondo) no es
     "pasivo" y por tanto no es captación. Pero la Superfinanciera mira la sustancia:
     si hay **rentabilidad fija prometida o recompra obligatoria**, el aporte se vuelve
     deuda y es captación aunque se llame "participación" o "derecho fiduciario".
   - Casos que lo prueban: Home Capital (Medellín, 2024: COP 20.070 millones de 202
     personas, "compra y venta de inmuebles" con utilidad fija); Orión y Luxury House
     (3 % a 4,7 % mensual); Fundación FG (2026: "certificados de derechos fiduciarios"
     sin fiduciaria, 318 personas).
2. **Oferta pública de valores** (Decreto 2555 de 2010, art. 6.1.1.1.1). Ofrecer
   participaciones a 100 o más personas determinadas, o a personas indeterminadas, es
   oferta pública y exige registro y autorización. **Es regla de oferta, no de
   aceptación**: un deck en un grupo de WhatsApp de 150 personas o un post en Instagram
   ya es oferta pública aunque solo inviertan 10. Una SAS no puede ofrecer acciones al
   público (Ley 1258, art. 4; la Corte tumbó en 2025 el intento de cambiarlo).

Consecuencia práctica: hay dos caminos legales.

- **Camino A, privado.** Menos de 100 personas identificadas, sin publicidad abierta,
  aporte a riesgo, sin retorno fijo. Sirve para arrancar, no para escalar.
- **Camino B, regulado.** El dinero entra a un fondo o patrimonio autónomo administrado
  por una entidad vigilada. Nosotros somos el **gestor**, no el custodio. Es el único
  camino para llegar a "gente que no conozcamos" y a una plataforma abierta.

**Sobre Estados Unidos o Caimán (verificado):** no resuelven nada si los inversionistas
son residentes colombianos. La captación se juzga por la conducta de captar en
Colombia; la Superfinanciera sanciona a los promotores locales aunque el vehículo sea
extranjero (caso Stone Eagle). Solo tendría sentido si una parte relevante de los
inversionistas vive fuera del país y quiere invertir en dólares. Recomendación: Colombia.

## 3. Corrección importante frente a la idea inicial (verificado)

- **El Fondo de Capital Privado (FCP) queda descartado con tickets de COP 100 millones.**
  El mínimo legal por inversionista es 600 SMMLV, es decir, **COP 1.050 millones en
  2026**. Solo serviría si el perfil cambia a inversionistas de mil millones o más.
- **La ruta para abrir al público es el FIC inmobiliario** (fondo de inversión
  colectiva), administrado por una fiduciaria, comisionista o SAI, que por norma puede
  contratar un **gestor externo no vigilado** (art. 3.5.1.1.8 del Decreto 2555). Ese
  gestor puede ser la SAS de los tres. Ya hay un precedente real: Visum Capital es
  gestor externo de un FIC inmobiliario. El ticket mínimo lo fija el reglamento, no la
  ley; en el mercado se ven desde COP 1 a 10 millones. Sus participaciones pueden
  inscribirse y listarse en la BVC.
- **La titularización tipo PEI o TIN no es para empezar.** PEI administra más de COP 10
  billones y nació con un portafolio ya estabilizado. Es la meta de largo plazo, no la
  etapa 1.
- **El referente argentino** que Daniel recuerda es el REIT Ciclo Nova, el primer fondo
  cerrado inmobiliario de desarrollo listado en la bolsa de Buenos Aires (junio de
  2026, unos US$45 millones de 3.500 inversionistas, ticket mínimo simbólico), **no
  una emisión en Estados Unidos**. Es el caso más parecido a lo que queremos: desarrollo,
  no renta, con oferta minorista.
- **Cardone Capital** paga mensual como práctica comercial, no como obligación; se queda
  con el 35 % de la utilidad sin retorno preferente al inversionista; y tiene un juicio
  colectivo en 2027 por proyecciones en videos de redes sociales. Lección: la marca
  personal vende, pero cada afirmación pública es una representación legal.

## 4. Arquitectura propuesta (hipótesis central, ajustada a lo verificado)

Tres capas separadas. La separación es lo que blinda a los socios como personas.

```
[Inversionistas]
      │ aportan dinero (o tierra)
      ▼
[VEHÍCULO] ── administrado por fiduciaria vigilada
      │        · Etapa 0: patrimonio autónomo por proyecto, derechos fiduciarios a riesgo
      │        · Etapa 1: FIC inmobiliario; la gestora como gestor externo
      │        · Etapa 2: familia de fondos o compartimentos por tipo = "la plataforma"
      ▼
[SPV por proyecto] ── un patrimonio autónomo por cada lote o desarrollo
      ▲
      │ estructura, gerencia, propone al comité de inversiones
[LA GESTORA] ── SAS de los tres socios. Cobra honorarios + participación en utilidad.
                NUNCA recibe el dinero de los inversionistas en su cuenta.
```

Por qué:
- La plata nunca pasa por nosotros. Eso elimina de raíz el riesgo de captación y es el
  argumento que convence a un inversionista desconfiado.
- La gestora es el negocio de los tres: marca, equipo, honorarios y utilidad. Si un
  proyecto sale mal, pierde el vehículo, no la casa de los socios (mientras no firmemos
  garantías personales).
- La "plataforma donde cada quien elige su *allocation*" tiene forma legal: una familia
  de fondos (la Superfinanciera autoriza la familia y el primer fondo; los siguientes
  solo se informan) o compartimentos dentro de un fondo (los usa, por ejemplo, el FCP
  Cattleya de Aval Fiduciaria). Un compartimento de engorde (largo plazo, alto riesgo),
  uno de desarrollo (mediano plazo) y uno de renta (flujo periódico, bajo riesgo).
- Advertencia verificada: la fiducia no protege sola. En Bosques de la Luz (Envigado,
  2025) condenaron a Alianza Fiduciaria por aprobar un constructor sin capital y girar
  más de lo recaudado. Las fiduciarias ahora filtran más y exigen capital propio al
  gestor. Hay que llegar con músculo y con un constructor serio.

## 5. La escalera: tres etapas

### Etapa 0 — Club de fundadores (meses 0 a 9)
- Un solo proyecto, pequeño y claro.
- Entre 10 y 20 inversionistas de la red de los tres, ticket de COP 100 millones.
  Nunca más de 99 destinatarios de la oferta; nada en redes ni en grupos abiertos.
- Vehículo: patrimonio autónomo con fiduciaria. Los inversionistas reciben derechos
  fiduciarios **a riesgo**, sin retorno fijo ni recompra. Contrato con reglas claras de
  salida, avalúo independiente y auditoría.
- Alternativa: SAS por proyecto con acuerdo de accionistas. Tiene doble tributación
  (35 % renta más dividendos) frente a la transparencia fiscal de la fiducia (art. 102
  ET). Recomendación: fiducia.
- Descartar cuentas en participación: es la figura favorita de los esquemas sancionados.
- Objetivo real: **historial y aprendizaje**, no la utilidad.

### Etapa 1 — FIC inmobiliario (meses 9 a 24)
- Fondo administrado por fiduciaria, comisionista o SAI, con la gestora como gestor
  externo, reglamento, comité de inversiones y reporte periódico.
- Permite llegar a inversionistas desconocidos sin violar la ley.
- Hipótesis de costo y tiempo (sin fuente pública): 4 a 9 meses y COP 150 a 400
  millones de estructuración; las administradoras suelen pedir un monto objetivo de
  COP 50.000 millones o más para que les interese. Esto hay que confirmarlo con dos o
  tres fiduciarias en Medellín.

### Etapa 2 — Plataforma (año 2 en adelante)
- Familia de fondos o compartimentos por horizonte y riesgo; reporte abierto; canal
  minorista cuando haya historial auditado (listado en BVC, crowdfunding regulado, y
  mucho después titularización).

## 6. Cómo gana plata la gestora (calibrado con el benchmark)

| Concepto | Referencia colombiana verificada | Propuesta inicial (hipótesis) |
|---|---|---|
| Honorario de estructuración | 1 % sobre compromisos (FCP Valor Inmobiliario, Fiducentral) | 1 % a 2 % al cierre |
| Comisión de administración/gestión | 1,25 % a 2 % anual (Sura Rentas); 1,5 % (Davivienda); tope 1,9 % (Nexus) | 1,5 % a 2 % anual sobre activos |
| Participación en utilidad (*carry*) | 15 % sobre el exceso de 12 % anual (Fiducentral); 10 % sobre IPC + 5,5 % (Sura) | 20 % sobre el exceso de un retorno preferente de 10 % a 12 % EA |
| Gerencia de proyecto y ventas | Sin fuente publicada | 3 % a 5 % de costos; 3 % a 4 % de ventas si somos promotora |

El inversionista recibe capital y utilidad **al cierre de cada proyecto o hito**
(punto de equilibrio, escrituración), no por calendario. Un compartimento de renta sí
distribuye periódicamente. Esto responde a "sin dividendo mensual".

## 7. Ideas que pueden hacer la diferencia (hipótesis para discutir)

1. **Tierra como aporte, no solo plata.** En Llanogrande lo escaso es la tierra, y la
   red del tercer socio es de dueños de tierra. El patrimonio autónomo acepta aportes
   en especie (práctica habitual, con tratamiento fiscal favorable: el derecho
   fiduciario conserva el costo del bien aportado). El dueño pone el lote, los
   inversionistas el dinero de desarrollo, y todos son beneficiarios en proporción.
   Convierte terratenientes en aliados en vez de vendedores.
2. **No montar constructora al principio.** Aliarse con una constructora grande como
   socio constructor. Arquitectura y Concreto tiene 18 proyectos y COP 2,1 billones en
   el Oriente. El riesgo de obra lo lleva quien sabe construir.
3. **Pagar el lote contra hitos** (licencia, punto de equilibrio), como hacen las
   constructoras grandes con quien aporta lote. Nunca comprar tierra sin disponibilidad
   de agua y concepto de uso del suelo por escrito.
4. **Derecho de preferencia para los inversionistas:** compran unidades del proyecto
   con descuento antes del lanzamiento. Convierte inversionistas en vendedores.
5. **Transparencia como producto:** ficha de una página con retorno objetivo (nunca
   garantizado), riesgos, fees y fechas; reporte trimestral; avalúos independientes;
   auditoría desde el primer proyecto. En PEI la emisión de 2025 tuvo demanda de tres
   veces lo ofrecido; la transparencia vende.
6. **Tesis clara de zona y producto.** No "Antioquia en general". El Oriente ya iguala
   a Medellín en ventas de vivienda no VIS (2026), El Retiro y La Ceja lideran
   valorización en Antioquia (11,6 % y 7,1 % en 2025) y los lotes urbanizados son el
   25 % de la oferta.
7. **Compartimento de renta como puerta de entrada:** un activo en renta (coliving,
   bodegas, hotelería pequeña) con flujo mensual atrae al conservador y financia la
   operación de la gestora mientras maduran los proyectos largos.
8. **"Skin in the game" real.** Yellowstone comprometió el 5 % de su fondo; a Cardone lo
   critican por poner 1 % a 5 %. Propongo que los gestores aporten entre 5 % y 10 % del
   capital de cada vehículo, y si aportan lote, que valga al avalúo y no con prima.

## 8. Riesgos que hay que mirar de frente

- **POT de Rionegro en revisión** (2026-2027): la norma de suelo suburbano y rural
  puede cambiar. Un engorde comprado con la norma de hoy puede quedar congelado años.
- **CORNARE manda sobre el POT:** densidades de 1 a 4 viviendas por hectárea en suelo
  rural y unidad mínima de actuación de 2 hectáreas en suburbano (verificado).
- **Agua:** CORNARE suspendió concesiones en sequía y hay zonas de Rionegro con déficit
  de caudal; en junio de 2026 hubo 1.400 personas sin agua en El Retiro y Rionegro.
  La disponibilidad de agua es hoy el cuello de botella de un lote rural.
- **Valorización moderada:** 6,2 % promedio del suelo en 2024, frente al 14 % a 17 % de
  2023. "Comprar y esperar" rinde poco; el retorno real del engorde viene del cambio de
  uso, que depende del POT.
- **Iliquidez.** El inversionista de 100 millones no puede salir cuando quiera. Hay
  que decírselo de frente y por escrito.
- **Conflicto de interés.** Si el tercer socio o su red le venden tierra al vehículo:
  avalúo independiente y aprobación del comité sin él. Se define antes del primer peso.
- **Reputación cruzada.** Los primeros inversionistas serán amigos y comunidad. Un mal
  primer proyecto cuesta más que la plata.
- **Partes iguales.** Si uno pone red y capital inicial y los otros el trabajo, "partes
  iguales" puede ser justo o fuente de conflicto en dos años. Hay que escribir qué
  aporta cada uno y qué pasa si alguien deja de aportar.
- **Tiempo de Daniel.** Este negocio y el de masculinidad compiten por las mismas horas.

## 9. Preguntas para Daniel

**Sobre los socios**
1. ¿Qué aporta exactamente cada uno de los tres? ¿Alguien pone capital semilla para
   montar la gestora, pagar abogados y fiduciaria (hipótesis: COP 80 a 200 millones
   para la etapa 0)?
2. ¿Cuánto tiempo semanal puede dedicar cada uno? ¿Quién sería el gerente de tiempo
   completo?
3. ¿El tercer socio quiere ser gestor operativo o inversionista ancla con red? Son
   roles distintos y se remuneran distinto.
4. ¿Alguno tiene experiencia directa en desarrollo inmobiliario, obra o ventas de
   vivienda? ¿O habría que contratar a alguien que sí?

**Sobre los inversionistas**
5. ¿Cuántas personas de su red pondrían 100 millones en 12 meses, siendo honestos?
   ¿Y cuántas 1.000 millones o más? (Esto decide si el FCP vuelve a ser opción.)
6. ¿Qué buscan esas personas: rentabilidad, proteger patrimonio en tierra,
   diversificar, o confiar en ustedes?
7. ¿Hay ya un lote o proyecto concreto sobre la mesa?
8. ¿Alguien de su red vive fuera de Colombia y querría invertir en dólares? (Única
   razón para pensar en un vehículo offshore.)

**Sobre el producto**
9. De las cuatro modalidades (engorde, desarrollo propio, aporte a constructora,
   integral), ¿cuál es la más natural para el primer proyecto y por qué?
10. ¿Aceptan que el primer proyecto sea pequeño y "aburrido" para construir historial?
11. ¿Qué horizonte es vendible a su red: 3 años, 5 años, más?

**Sobre el riesgo personal**
12. ¿Firmarían garantías personales con bancos o constructoras? (Recomendación: no en
    etapas 0 y 1.)
13. ¿Hay en su red gente que perdió plata en "proyectos de inversión" en la zona (Home
    Capital, Bosques de la Luz)? Cambia cómo hay que presentar el producto.

## 10. Siguiente paso que propone Claude

1. Daniel responde las preguntas (en el orden que quiera, por nota de voz).
2. Con eso, Claude redacta la **v1 del plan de negocios** (modelo económico de la
   gestora, proyecto piloto, cronograma) y un **memorando para un abogado financiero**
   en Medellín con las preguntas exactas por confirmar antes de recibir el primer peso.
3. En paralelo, los socios agendan reuniones exploratorias con dos o tres fiduciarias
   (Alianza, Fiduciaria Bancolombia, Acción) para conocer costos reales de un
   patrimonio autónomo y de un FIC con gestor externo.
