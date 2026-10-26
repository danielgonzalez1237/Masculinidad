# Arquitectura operativa del vehículo como fondo

**Fecha:** 2026-10-26
**Autor:** Claude, en rol de cofundador y advisor.
**Qué es este documento:** el esquema de cómo funciona el vehículo *como fondo*: piezas,
roles, ciclo de vida, flujo del dinero, reparto, reporte, liquidez y método de
levantamiento de capital. No es el análisis de un proyecto (eso queda como anexo en
`05-piloto-llanogrande.md`). Lo marcado **(verificado)** sale de los informes
`01`, `02` y `06`; el resto son propuestas de Claude para que los socios decidan.

---

## 1. Principio de diseño: cuatro funciones, cuatro manos distintas

Todo fondo serio separa cuatro funciones. Cuando una sola mano las concentra, aparece
el problema (Cardone concentra las cuatro y por eso enfrenta juicio; Bosques de la Luz
falló porque nadie controló la tercera).

| Función | Quién la hace en nuestro diseño | Referente que lo hace así (verificado) |
|---|---|---|
| **Relación con inversionistas y marca** | La gestora (los tres socios) | Cardone: la marca es el canal. PEI: Pei Asset Management da la cara, la fiduciaria firma |
| **Custodia y administración del dinero** | Fiduciaria o administradora vigilada | PEI: Fiducoldex/Aval como vocera. TIN: Titularizadora Colombiana. Yellowstone: fiduciaria administradora |
| **Decisión de inversión** | Comité de inversiones (gestora + independientes) | PEI: comité asesor. FCP: comité de inversiones del gestor + comité de vigilancia de inversionistas |
| **Ejecución de proyectos** | Patrimonio autónomo por proyecto + constructora y promotora contratadas | Toda la industria colombiana: fiducia por proyecto con punto de equilibrio |

La regla que resume todo: **el dinero del inversionista nunca pasa por la cuenta de la
gestora.** Entra a un vehículo administrado por una vigilada y sale de ahí a los
proyectos. Esto es lo que nos diferencia de Home Capital, Lazza y compañía, y es lo
primero que diremos en cualquier reunión.

## 2. El mapa de piezas

```
                      ┌──────────────────────────────────┐
                      │        INVERSIONISTAS            │
                      │ Colombia (COP) · Exterior (USD   │
                      │ girado y registrado en Banrep)   │
                      └───────────────┬──────────────────┘
                                      │ aportes / compromisos
                                      ▼
┌──────────────┐   reglamento   ┌──────────────────────────────────┐
│  LA GESTORA  │◄──────────────►│   EL FONDO (vehículo regulado)    │
│  SAS de los  │  gestor externo│   Etapa 0: patrimonio autónomo    │
│  tres socios │                │   Etapa 1: FIC inmobiliario       │
│              │  honorarios +  │   administrado por fiduciaria     │
│ · origina    │  participación │   o sociedad administradora       │
│ · estructura │◄──────────────│   · custodia · contabilidad       │
│ · gerencia   │                │   · valoración · SARLAFT          │
│ · reporta    │                │   · unidades en Deceval           │
└──────┬───────┘                └───────┬──────────┬───────────────┘
       │ propone                        │          │
       ▼                                ▼          ▼
┌──────────────┐              ┌────────────┐ ┌────────────┐
│ COMITÉ DE    │   aprueba    │ COMPARTI-  │ │ COMPARTI-  │  ... (la "plataforma")
│ INVERSIONES  │─────────────►│ MENTO A    │ │ MENTO B    │
│ 3 socios +   │              │ Desarrollo │ │ Renta      │
│ 2 externos   │              └─────┬──────┘ └─────┬──────┘
└──────────────┘                    │              │
                                    ▼              ▼
                         ┌────────────────┐ ┌────────────────┐
                         │ PA PROYECTO 1  │ │ PA ACTIVO 1    │
                         │ lote + obra +  │ │ inmueble en    │
                         │ ventas         │ │ arriendo       │
                         └───┬────────┬───┘ └────────────────┘
                             │        │
                     ┌───────▼──┐ ┌───▼────────┐
                     │CONSTRUC- │ │ PROMOTORA  │  contratos a precio de mercado,
                     │TORA      │ │ (ventas)   │  aprobados por el comité sin el
                     └──────────┘ └────────────┘  socio relacionado
```

Piezas de control alrededor (todas estándar en PEI, TIN y los FCP):
- **Asamblea de inversionistas** y, en etapa FIC, **comité de vigilancia** (se reúne al
  menos cada tres meses, verificado para FCP).
- **Revisor fiscal / auditoría externa** del fondo y de cada patrimonio autónomo.
- **Avaluador independiente** registrado, con avalúo al entrar y al menos anual.
- **Representante de los inversionistas** cuando el fondo se liste (PEI lo tiene).
- **Póliza D&O** para los administradores de la gestora.

## 3. Ciclo de vida del fondo

Propongo un **fondo cerrado de desarrollo con compromisos de capital**, el modelo de
los FCP inmobiliarios y de Yellowstone, adaptado al FIC. Razón: en desarrollo el dinero
se necesita por hitos, no todo el día uno. Recibirlo todo de entrada diluye el retorno
(*cash drag*) y, peor, pone plata ociosa en manos de un gestor sin historial.

| Fase | Duración (hipótesis) | Qué pasa | Referente |
|---|---|---|---|
| **Levantamiento** | 6 a 12 meses | Periodo de suscripción; los inversionistas firman compromisos; primer cierre cuando se alcanza el monto mínimo; cierres sucesivos hasta el máximo | FIC cerrado: debe alcanzar monto objetivo en 1 año, prorrogable 6 meses (verificado) |
| **Inversión** | años 1 a 3 | Llamados de capital por proyecto aprobado; cada proyecto en su patrimonio autónomo | Yellowstone, Cattleya (compartimentos con rendición separada) |
| **Desarrollo y desinversión** | años 2 a 7 | Obra, ventas, escrituración; distribución al cierre de cada proyecto | Ciclo Nova: fondo de desarrollo a 10 años con distribución discrecional |
| **Liquidación o renovación** | año 7 a 9 | Se liquida el compartimento o se abre uno nuevo con el mismo reglamento | Sura Rentas: 99 años con ventanas; nosotros preferimos plazo definido |

**Plazo propuesto:** 7 años, prorrogable dos veces por un año. Un plazo definido vende
mejor que un fondo "perpetuo" cuando no hay historial.

## 4. Los compartimentos: así se vuelve real la "plataforma de allocation"

La idea de Daniel (elegir por temporada, riesgo y horizonte) tiene forma legal: una
familia de fondos o un fondo con compartimentos, cada uno con política, plazo, riesgo y
regla de distribución propias (verificado que existen; Cattleya de Aval Fiduciaria
opera cinco). El inversionista elige su mezcla y recibe un solo extracto.

| Compartimento | Qué compra | Horizonte | Riesgo | Cómo distribuye | Cuándo abrirlo |
|---|---|---|---|---|---|
| **Desarrollo** | Lotes para construir y vender (casas, lotes urbanizados) | 3 a 5 años | Medio-alto | Al cierre de cada proyecto | Desde el inicio (es el negocio central) |
| **Renta** | Inmuebles terminados en arriendo (coliving, bodegas, comercio en Rionegro) | 5 a 10 años | Bajo-medio | Trimestral, con regla publicada | Año 1 o 2: es la puerta de entrada del inversionista conservador y la caja de la gestora |
| **Tierra** | Engorde con tesis de cambio de uso | 5 a 10 años | Alto | Al vender | Solo con POT de Rionegro aprobado (2027) y agua resuelta |

"Por temporada" se traduce en **cierres**: cada compartimento abre ventanas de
suscripción (por ejemplo, dos al año) y el inversionista entra en la que le convenga.

## 5. Flujo del dinero, paso a paso

1. El inversionista firma el reglamento y el documento de vinculación con la
   fiduciaria (KYC, origen de fondos, perfil de riesgo). Transfiere **pesos** desde una
   cuenta a su nombre. Si vive afuera, gira dólares por un intermediario cambiario y la
   declaración de cambio registra su inversión en el Banco de la República (verificado).
   Nunca USDT, nunca efectivo, nunca cuentas de terceros.
2. La fiduciaria recibe, emite unidades a nombre del inversionista y las anota en
   Deceval (etapa FIC).
3. La gestora presenta cada proyecto al comité con un **expediente estándar**: título,
   uso del suelo y agua por escrito, avalúo, presupuesto con dos cotizaciones externas,
   modelo financiero con tres escenarios, estrategia de salida, conflictos de interés
   declarados.
4. El comité aprueba; la fiduciaria hace el llamado de capital o gira al patrimonio
   autónomo del proyecto, siempre contra hitos (compra del lote, licencia, punto de
   equilibrio, avance de obra certificado por interventor).
5. El patrimonio autónomo paga a constructora, promotora, diseñadores y al municipio.
   Las ventas entran al mismo patrimonio (encargo de preventas con punto de equilibrio,
   la figura estándar verificada).
6. Al escriturar, el patrimonio devuelve capital y utilidad al fondo; el fondo aplica
   la cascada de reparto (sección 6) y distribuye a los inversionistas y a la gestora.
7. Todo queda en el reporte trimestral y en la asamblea anual.

## 6. Economía del fondo y cascada de reparto

Referencias colombianas verificadas: Fiducentral cobra 1 % de estructuración y 15 % de
éxito sobre el exceso de 12 % anual; Sura Rentas 1,25 % a 2 % de administración y 10 %
sobre IPC + 5,5 %; Nexus tope 1,9 %; Davivienda 1,5 % más 1 % de colocación. Cardone
cobra 1 % de adquisición más fees anuales y se queda con el 35 % sin retorno preferente
(lo que no vamos a copiar).

**Propuesta inicial (hipótesis para negociar con la fiduciaria y con los primeros
inversionistas):**

| Concepto | Quién lo cobra | Cuánto | Sobre qué |
|---|---|---|---|
| Comisión de administración fiduciaria | Fiduciaria | 0,3 % a 0,6 % anual (hipótesis) | Activos administrados |
| Honorario de gestión | Gestora | 1,5 % anual | Compromisos durante inversión; activos después |
| Honorario de estructuración | Gestora | 1 % | Capital comprometido, una vez |
| Gerencia de proyecto | Gestora | 3 % a 5 % | Costos directos de cada proyecto (sustituye parte de la gestión si se prefiere no apilar) |
| Participación en utilidad | Gestora | 20 % | Utilidad por encima del retorno preferente |

**Cascada de reparto por proyecto o compartimento:**
1. Devolver el 100 % del capital aportado al inversionista.
2. Pagar un **retorno preferente del 10 % a 12 % efectivo anual** al inversionista.
3. Del excedente, 80 % al inversionista y 20 % a la gestora.

Sin *catch-up* para la gestora en el primer fondo: es más simple de explicar y es lo
que un inversionista desconfiado quiere oír. **Aporte de los socios:** entre 5 % y 10 %
del capital de cada compartimento, al mismo precio que todos (Yellowstone puso 5 %).

Regla de distribución: **cuando hay caja realizada, no por calendario.** El
compartimento de renta sí tiene fecha (trimestral) y una tasa objetivo publicada que se
recalibra cada trimestre según la caja real, nunca garantizada. Es la parte rescatable
de la idea de STRC.

## 7. Valoración, reporte y transparencia

- **Valoración:** la fiduciaria calcula el valor de la unidad según su metodología
  (obligación regulatoria de los FIC); los inmuebles con avalúo independiente anual y
  los proyectos en curso a costo más avance certificado.
- **Reporte trimestral** por compartimento: avance de cada proyecto con fotos y
  porcentaje de obra, ventas, caja, valor de la unidad, hitos del próximo trimestre,
  riesgos. Una página por proyecto, estilo PEI.
- **Ficha de una página del fondo**, actualizada cada trimestre: retorno objetivo
  (nunca garantizado), plazo, fees, riesgos, fecha del próximo reporte. La transparencia
  radical de la ficha de STRC y de Fundrise, aplicada a ladrillo.
- **Asamblea anual** presencial en Llanogrande, con visita a los proyectos. Es reporte
  y es marketing al mismo tiempo.
- **Portal del inversionista** (etapa 1): extracto, documentos, reportes. Al principio
  basta la plataforma de la fiduciaria.

## 8. Liquidez y salida

Desarrollo es ilíquido y hay que decirlo. Opciones en escalera:
- **Etapa 0:** sin liquidez hasta el cierre del proyecto. Cesión de derechos entre
  inversionistas permitida con aprobación de la fiduciaria.
- **Etapa 1:** ventanas de redención limitadas (Sura ofrece 5 % a 10 % cada tres años,
  verificado), financiadas con caja de ventas, no con nuevos aportes.
- **Etapa 2:** inscribir las unidades del FIC en el Registro Nacional de Valores y
  listarlas en la BVC (permitido para FIC inmobiliarios, verificado). Es como PEI y TIN
  dan liquidez. Requiere historial auditado y tamaño.

## 9. Método de levantamiento de capital

Aquí la palabra "captación" se queda en el documento jurídico; hacia afuera es
**"invitación a invertir"** en un fondo administrado por una fiduciaria. El método tiene
tres círculos y una regla por círculo.

| Círculo | Quiénes | Cómo se les llega | Regla legal (verificado) |
|---|---|---|---|
| **1. Núcleo** | Los tres socios, sus familias cercanas, socios de la gestora con más del 5 % y seis meses | Conversación directa | No cuentan para los umbrales de captación |
| **2. Red directa** | Conocidos de Hernán, Julián y Daniel | Reunión uno a uno o en grupos pequeños, con el mismo documento para todos y lista de destinatarios con fecha ("libro de oferta") | Menos de 100 destinatarios por ronda; nunca mensajes a grupos abiertos ni redes; aporte a riesgo, sin retorno fijo |
| **3. Público** | Inversionistas que no conocemos | Solo a través del FIC: la fiduciaria y los comisionistas lo distribuyen; nuestra marca atrae | Oferta regulada; admite más de 100 inversionistas |
| **Exterior** | Colombianos afuera y extranjeros | Giro de divisas registrado; opcionalmente un vehículo agrupador fuera del país solo para no residentes, sin promoción en Colombia | Inversión extranjera registrada en Banrep; nunca USDT a la fiducia |

**Qué sí se puede comunicar públicamente desde el día uno:** la marca de la gestora, la
tesis de zona (por qué el Oriente), contenido educativo, el historial de proyectos
cerrados con cifras reales y auditadas, y el nombre de la fiduciaria que administra.
**Qué no:** proyecciones de rentabilidad, "cupos", "tickets", invitaciones a invertir a
personas indeterminadas. Cardone muestra las dos caras: la marca le levantó más de
US$1.600 millones de 20.000 inversionistas y sus videos con proyecciones lo llevaron a
juicio (verificado).

**Lo que enseña el benchmark sobre cómo se levanta plata (verificado):**
- PEI emite por tramos en la BVC a través de comisionistas y tuvo demanda de tres veces
  lo ofrecido en 2025; su activo de venta es el historial y la calificación AAA.
- REIT Ciclo Nova (Argentina) colocó US$45 millones a 3.500 inversionistas con ticket
  simbólico en horas, a través de la plataforma de la administradora y las sociedades
  de bolsa: canal regulado más relato de desarrollo premium.
- Fundrise levantó US$3.300 millones de 400.000 cuentas con ticket de US$10 y
  plataforma digital propia bajo un régimen de oferta simplificada que Colombia no tiene.
- Lokl (Medellín) reúne más de 2.000 inversionistas con tickets de un millón vía
  fiducia y plataforma propia; funciona pero no escala a oferta pública.
- Yellowstone levantó US$500 millones de fondos de pensiones con un gestor de cinco
  años de historial. Es la liga a la que se llega con historial, no al empezar.

**Recomendación:** etapa 0 con el círculo 2 (12.000 millones son 120 participaciones;
con varios inversionistas de 50 participaciones, la lista de destinatarios cabe de
sobra bajo 100); etapa 1 con el FIC distribuido por la fiduciaria y uno o dos
comisionistas de Medellín, apoyado en nuestra marca; etapa 2 listar en la BVC.

## 10. Gobierno y blindaje de los socios

- **Comité de inversiones:** los tres socios más dos independientes con experiencia
  inmobiliaria o financiera. Decisiones por mayoría; en partes relacionadas (lote de la
  red de Hernán, constructora de Hernán, promotora de Julián) el socio relacionado no
  vota y se exige avalúo o cotización externa.
- **Límites de política de inversión** escritos en el reglamento: máximo 30 % del
  compartimento en un solo proyecto; endeudamiento máximo del 35 % de los activos (PEI
  bajó su tope a 35 %, verificado); sin garantías personales de los socios.
- **Separación contable y societaria:** gestora, fondo y cada patrimonio autónomo con
  contabilidad propia y auditor.
- **Acuerdo de socios de la gestora:** aportes, dedicación, vesting, honorario del socio
  operativo, salida, no competencia en la zona.
- **Cumplimiento:** SARLAFT lo lleva la fiduciaria; la gestora adopta su propio manual
  de prevención de lavado aunque no esté obligada, porque los inversionistas lo preguntan.

## 11. Cómo se compara con los referentes

| Pieza | Cardone | PEI | FIC Sura Rentas | Yellowstone (FCP) | Ciclo Nova (ARG) | **Nosotros (propuesta)** |
|---|---|---|---|---|---|---|
| Vehículo | LLC por fondo, oferta Reg A+ / Reg D | Titularización listada en BVC | FIC inmobiliario cerrado | FCP con gestor profesional | Fondo cerrado listado en BYMA | Fiducia → FIC inmobiliario con gestor externo → listado |
| Quién custodia | El propio manager | Fiduciaria vocera | Fiduciaria Bancolombia | Fiduciaria | Administradora regulada | Fiduciaria vigilada |
| Activo | Multifamily en renta | Renta comercial | Renta | Desarrollo de vivienda | Desarrollo premium | Desarrollo + renta + tierra, por compartimentos |
| Ticket | US$5.000 / US$250.000 | 1 título (~COP 64.000) | COP 5 millones | Institucional | AR$1.000 | COP 100 millones al inicio; menor al listar |
| Distribución | Mensual (práctica) | Trimestral | Según reglamento | Al cierre | Trimestral discrecional | Por hito; renta trimestral |
| Fees y reparto | 1 % + fees; 65/35 sin pref | Admin + titularización | 1,25 % a 2 %; 10 % sobre IPC+5,5 | Sin dato público | Sin dato | 1,5 %; 20 % sobre pref 10 % a 12 % |
| Liquidez | Ninguna | BVC diaria | Ventanas cada 3 años | Ninguna | BYMA diaria | Ninguna → ventanas → BVC |
| Canal | Marca personal, directo | Comisionistas | Fiduciaria | Institucional | Plataforma + bolsa | Red directa → fiduciaria y comisionistas → bolsa |

## 12. Decisiones que los socios deben tomar (en este orden)

1. Confirmar la arquitectura de tres capas y el camino fiducia → FIC → listado.
2. Plazo del fondo (propuesta: 7 + 1 + 1) y si arranca con un compartimento o dos.
3. Compromisos con llamados de capital (propuesta) o aporte total al inicio.
4. Retorno preferente (10 % o 12 %), participación de la gestora (20 %) y honorario de
   gestión (1,5 %).
5. Aporte de los socios al fondo (5 % o 10 %) y cómo se financia.
6. Fiduciarias a visitar: propuesta Alianza, Fiduciaria Bancolombia y Acción, con una
   misma lista de preguntas (costos, monto mínimo para un FIC, tiempo, requisitos al
   gestor externo, experiencia en el Oriente).
7. Nombre y marca de la gestora, y quién es el vocero público.

Con esas siete respuestas, Claude redacta el borrador de reglamento comercial (lo que
después un abogado convierte en reglamento del fondo) y el memorando para la fiduciaria.
