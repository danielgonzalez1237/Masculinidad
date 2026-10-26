# Bitácora

Registro de sesiones de trabajo y decisiones, de la más reciente a la más antigua.

---

## 2026-10-26 — Nueva idea: vehículo de inversión inmobiliaria (Oriente Antioqueño)

**Contexto que compartió Daniel:**
- Un tercer socio de Llanogrande, con red de personas de alto patrimonio, propuso
  asociarse con Daniel y Julián. Proporciones sin discutir; Daniel propone partes iguales.
- Idea: recaudar de conocidos (y luego del público) con tickets de ~COP 100 millones
  para invertir en real estate del Oriente Antioqueño: engorde de tierra, desarrollo,
  aporte de lotes a constructoras, proyectos integrales. Operar como "desarrolladora".
- Pidió a Claude rol de advisor jurídico y cofundador, benchmark con agentes y
  construir el plan de negocios de forma continua.

**Qué se hizo:**
- Se creó la carpeta `04-fondo-inmobiliario/` con la idea original en sus palabras.
- Dos agentes de investigación produjeron `01-marco-juridico.md` (captación, oferta
  pública, FIC, FCP, fiducia, titularización, crowdfunding, SAS, offshore, suelo del
  Oriente) y `02-benchmark.md` (Cardone, STRC, REIT, PEI, TIN, FIC bancarios, Lokl,
  casos de fraude, mercado del Oriente), con fuentes y marcas de verificación.
- Claude escribió `03-brainstorm-y-preguntas.md`: línea roja legal, arquitectura de
  tres capas (gestora SAS + vehículo con fiduciaria + SPV por proyecto), escalera de
  tres etapas, modelo de ingresos de la gestora, ideas diferenciales, riesgos y 13
  preguntas para Daniel.

**Hallazgos clave (verificados):**
- El FCP queda descartado con tickets de 100 millones: mínimo legal 600 SMMLV
  (COP 1.050 millones en 2026).
- La ruta para abrir al público es un FIC inmobiliario con la gestora como gestor
  externo no vigilado (art. 3.5.1.1.8 del Decreto 2555).
- Prometer rentabilidad fija o recompra convierte cualquier figura en captación
  (casos Home Capital en Medellín, Orión, Luxury House, Fundación FG).
- Un vehículo en EE. UU. o Caimán no resuelve la captación con inversionistas residentes.
- El referente argentino es el REIT Ciclo Nova, listado en Buenos Aires, no en EE. UU.

**Segunda ronda (misma sesión):** Daniel respondió las preguntas clave. Socios:
Hernán (lotes, constructora, inversionistas), Julián (promotora, inversionistas),
Daniel (administración, finanzas, jurídico, contable); partes iguales probables.
Piloto: lote de 18.000 m² detrás del Bancolombia de Llanogrande para cuatro casas
luxury, recaudo objetivo COP 12.000 millones en participaciones de 100 millones.
Daniel planteó además tokenizar las participaciones (emisor extranjero que contrate a
la SAS colombiana como operadora) y recibir aportes en USDT. Claude creó
`04-socios-y-roles.md` y `05-piloto-llanogrande.md` (alertas: unidad mínima de 2 ha
en suburbano frente a 1,8 ha del lote, agua, POT en revisión, constructora como parte
relacionada, modelo de servilleta con tres escenarios) y lanzó un agente sobre
tokenización y cripto en Colombia.

**Tercera ronda (misma sesión):** llegó el informe de tokenización y cripto
(`06-tokenizacion-y-cripto.md`): no hay ley de criptoactivos ni régimen de
tokenización en Colombia; las fiduciarias no pueden recibir cripto; el modelo "emisor
extranjero de tokens + operadora colombiana vendiendo a residentes" es el patrón del
caso Lazza Capital (Medellín, 2024) y se descarta; la tokenización queda como opción
futura vía sandbox o representación digital de una participación ya regulada. Daniel
aclaró que no busca que Claude evalúe la viabilidad del proyecto sino que esquematice
la arquitectura del vehículo como fondo y el método de levantamiento de capital, con
base en el benchmark. Claude escribió `07-arquitectura-del-fondo.md` (cuatro funciones
separadas, mapa de piezas, ciclo de vida, compartimentos, flujo del dinero, cascada de
reparto, reporte, liquidez, método de levantamiento por círculos, gobierno, comparación
con referentes y siete decisiones pendientes).

**Decisiones:** ninguna todavía. Recomendación de Claude: Colombia, fiducia con
derechos fiduciarios a riesgo para el primer proyecto, FIC inmobiliario para escalar.

**Nota técnica:** el push por git fue bloqueado por permisos de la sesión; los
archivos se publicaron en la rama con la herramienta de GitHub de la sesión.

**Próximo paso:** los socios responden las siete decisiones de la sección 12 de
`07-arquitectura-del-fondo.md`.

---

## 2026-10-08 — Inicio del proyecto

**Contexto que compartió Daniel:**
- Idea conjunta con un amigo exseminarista del Regnum Christi; ambos pertenecen a la
  comunidad en Medellín.
- Perciben un interés amplio, tanto católico como social, por la masculinidad y su
  significado en la sociedad.
- Daniel: emprendedor joven, esposo, formado desde su hogar en caballerosidad,
  respeto a la mujer y roles del hogar.
- Objetivo doble: ayudar y formar personas de verdad, y construir un negocio con
  imagen personal para los dos.

**Qué se hizo:**
- Se creó este repositorio como memoria del proyecto: perfiles de fundadores,
  acuerdos de sociedad, visión, audiencia, oferta y hoja de ruta.

**Decisiones:** ninguna todavía.

**Próximo paso:** cada fundador responde los bloques 1, 4 y 5 de su perfil.
