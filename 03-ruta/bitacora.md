# Bitácora

Registro de sesiones de trabajo y decisiones, de la más reciente a la más antigua.

---

## 2026-10-30 — Portal financiero de Daniel (aparte del proyecto)

**Qué pidió Daniel:** un portal personal para seguir noticias y datos del mercado
financiero de EE. UU. con explicaciones de términos y efectos, orientado a sus tres
frentes: metales preciosos de DEXTRUM (su proyecto minero), portafolio personal en IBKR
y cripto en inversiones de TUO. Quiere ver los mayores impactos (guerras, EE. UU.) y lo
que se espera a 7 días, un mes y un trimestre. Sigue en X a Michael Saylor, Tom Lee,
Felipe Campos, Juan Rodríguez y Jack Garzón.

**Qué se hizo:**
- Se creó la carpeta `04-finanzas/` con el portal (`portal-mercados.html`) y un README
  con contexto y pasos para actualizarlo. Está publicado como artefacto privado en
  claude.ai; se republica al mismo enlace desde ese archivo.
- Posiciones tomadas de Kubera (conector). Las listas de TradingView no se pudieron
  abrir desde el entorno de Claude.

**Segunda parte de la sesión:** Daniel aclaró que DEXTRUM es su comercializadora minera en
Bolivia (estaño primero; oro y plata en seguimiento) y que TUO es la gestión/hedge de
cripto. Pidió que el portal se actualice solo, como un diario. Decisiones: lunes a viernes,
listo a las 8:00 a. m. Colombia, aviso push, montos en dólares con interruptor para
ocultarlos. Se creó la rutina "Diario financiero Daniel" (7:37 a. m. Colombia, sesión nueva
cada día, conector Kubera) que sigue `04-finanzas/rutina.md`; el portal pasó a formato diario
(bloque de estaño, "qué cambió", archivo de ediciones). Daniel autorizó que la rutina haga
push a la rama por defecto del repositorio.

**Pendiente de Daniel:** pegar los tickers de TradingView en `04-finanzas/README.md` (o
permitir tradingview.com en la red del entorno) y decidir si desactiva la rutina anterior
"Daily portfolio briefing" para no recibir dos avisos.

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
