# Rutina diaria: Diario financiero de Daniel

Este archivo es el manual que sigue la sesión automática de cada día hábil (rutina
"Diario financiero Daniel", 7:37 a. m. Colombia, lunes a viernes). Daniel la pidió el
30 de octubre de 2026. Si algo falla o Daniel pide cambios, se corrige **este archivo**,
no la rutina.

## Permisos que Daniel dio explícitamente (30 oct 2026)

- Publicar cada edición al **mismo artefacto**: https://claude.ai/artifact/SLAz28JYah7jirnuFYeL1H
- Hacer commit y push directamente a la **rama por defecto** del repositorio
  (`claude/keen-mendel-nhfjp1` hoy; si la renombra a `main`, usar `main`). Si el push a esa
  rama es rechazado, hacer push a la rama asignada a la sesión y decirlo en el resumen final.
- Leer su portafolio en Kubera (conector) y mostrar montos en dólares en el diario (el portal
  tiene un interruptor para ocultarlos).

## Resultado esperado de cada corrida

1. `04-finanzas/diario/AAAA-MM-DD.md`: la edición del día en Markdown.
2. `04-finanzas/ediciones/AAAA-MM-DD(anterior).html`: la portada anterior archivada.
3. `04-finanzas/portal-mercados.html`: la nueva portada.
4. Artefacto republicado con la portada y la edición archivada como archivo adjunto.
5. Commit + push.
6. Mensaje final de **dos líneas** (es lo que llega como notificación push): titular con los
   dos o tres datos que más le importan y el enlace del artefacto.

## Pasos

### 1. Contexto (5 min)
- `git pull` de la rama por defecto.
- Leer `04-finanzas/README.md` (frentes, voces, reglas), la **edición anterior** en
  `04-finanzas/diario/` (la más reciente) y el `portal-mercados.html` actual.
- Fecha de corte: la hora de ejecución en ET (normalmente ~7:40 a. m. ET, antes de la apertura).

### 2. Posiciones en Kubera
- `get_default_portfolio` (el resultado se guarda en un archivo largo de una sola línea:
  leerlo por tramos de ~18.000 caracteres con Python `-I` y `read()[a:b]`).
- `get_top_movers` con el `portfolioId` para el cambio del día y del mes.
- Extraer: patrimonio neto, activos, deuda, cambio del día y del mes; IBKR (valor, margen,
  posiciones); Aave por billetera (colateral WBTC/WETH y deuda USDC) → **LTV = deuda /
  colateral** y precio de liquidación de BTC ≈ deuda / (0,78 × WBTC en unidades), restando el
  WETH si lo hay. Umbral 0,78 es el histórico de Aave V3 Arbitrum; decir siempre "verificar
  health factor en Aave". Vencimientos (Pendle PT) y partidas de DEXTRUM (Bolivia, estaño).
- **Si en la sesión no existen herramientas `mcp__Kubera__*`** (hoy la rutina corre sin el
  conector, decisión de Daniel del 30 oct 2026) o si Kubera falla: tomar las posiciones de la
  **última edición** en `04-finanzas/diario/` (cantidades de WBTC/WETH, colateral, deuda USDC,
  valor de IBKR y margen, partidas de DEXTRUM), recalcular LTV y precio de liquidación con el
  precio de BTC del día, y escribir en la portada (semáforo o "qué cambió") y en el Markdown:
  "Posiciones al DD/MM según Kubera; hoy no se refrescaron". No omitir las tablas de
  posiciones: se conservan con esa marca. Cuando Daniel adjunte Kubera a la rutina desde
  claude.ai (Rutinas → "Diario financiero Daniel" → conectores), este paso vuelve a ser
  automático sin cambiar nada más.

### 3. Noticias y datos (12–16 búsquedas en paralelo, modo extended para lo de hoy)
Priorizar lo fechado hoy y ayer. Cubrir siempre:

| Frente | Buscar | Fuentes que funcionan |
|---|---|---|
| Macro EE. UU. | Fed (decisión, discursos, FedWatch probabilidad próxima reunión), empleo, CPI/PCE, PIB, S&P/Nasdaq cierre | CNBC, Yahoo Finance, FXStreet, Kiplinger, Newsquawk ("week ahead") |
| Geopolítica/petróleo | Irán–Ormuz, Rusia–Ucrania, aranceles, Brent/WTI | OilPrice, FinanceFeeds, CNBC, TradingEconomics |
| Estaño (DEXTRUM) | LME cash y 3M, inventarios LME, SHFE, demanda China | Westmetall (tabla oficial), Metal.com / SMM, Mysteel, Sucden |
| Oro y plata | spot, ratio oro/plata, mineras (Newmont, Barrick, GDX, GDXJ), bancos centrales | Kitco, USAGold, Rio Times, Investing.com, BullionVault |
| IBKR | ORCL, AMZN, META, BRK-B, NU, UBER, MSTR, QQQ/VOO/VXUS; fechas de resultados | CNBC, Yahoo, TheStreet, 24/7 Wall St, MarketBeat, IR de las empresas |
| Cripto (TUO) | BTC/ETH precio y niveles, flujos ETF, custodios (Binance, Nexo), Aave, Pendle, MSTR, Saylor, Tom Lee | CoinDesk, CryptoTimes, Benzinga, CCN, KuCoin news, Axios |
| Colombia | USD/COP (TRM y spot), Banco de la República, inflación DANE, fiscal, Felipe Campos | Infobae Colombia, Bloomberg Línea, El Heraldo, Portafolio, XTB LatAm, banrep.gov.co |
| Voces en español | Juan Rodríguez ("Bitcoin y Criptos"), Jack Garzón | CriptoNoticias, DiarioBitcoin |

No accesibles desde el entorno: tradingview.com (bloqueado por red) y X (requiere sesión).
Si Daniel ya pegó sus tickers de TradingView en `04-finanzas/README.md`, buscarlos también.

### 4. Escribir la edición (Markdown)
Archivo `04-finanzas/diario/AAAA-MM-DD.md` con esta estructura fija:

```
# Edición N — día, D de mes de AAAA (corte HH:MM ET)
## Semáforo        (Metales/DEXTRUM, IBKR, Cripto/TUO, Dólar COP: estado + 1 frase)
## Qué cambió desde la edición anterior   (3–6 líneas; precios, LTV, calendario, patrimonio)
## Los impactos que más pesan             (3–5; cada uno: hecho con fuente, término explicado, efecto en lo suyo, "Lectura de Claude")
## Tus tres frentes                       (Metales/DEXTRUM con tabla de estaño; IBKR con reportes próximos; Cripto con tabla Aave)
## Qué se espera                          (7 días con fechas; mes; trimestre)
## Las voces que sigues                   (solo si hay algo nuevo fechado; si no, "sin novedades")
## Glosario                               (solo términos nuevos de esta edición)
## Fuentes                                (enlaces usados)
```

### 5. Regenerar la portada HTML
- Copiar el `portal-mercados.html` actual a `04-finanzas/ediciones/AAAA-MM-DD.html` con la
  fecha de **esa** edición, anteponiendo este encabezado (los archivos adjuntos se sirven sin
  esqueleto):
  `<!doctype html><html lang="es"><head><meta charset="utf-8"><meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover"></head><body>` … `</body></html>`.
- Reescribir `portal-mercados.html` con la nueva edición **manteniendo el mismo CSS, la misma
  estructura de secciones, el interruptor de montos (`.money`, script al final) y el `<title>`**.
  Cambiar: número de edición, fecha de corte, textos y tablas. Mantener los nombres de clases.
- Actualizar la lista `#ediciones` del pie: una `<li>` por edición archivada, la más reciente
  primero, con enlace relativo `ediciones/AAAA-MM-DD.html`. Máximo 30 ediciones listadas.

### 6. Publicar
- `Artifact` acción `read` de la URL del artefacto (obligatorio antes de publicar desde una
  conversación nueva).
- `Artifact` publicar con `file_path` = `04-finanzas/portal-mercados.html`, `url` = la URL,
  `root` = `04-finanzas`, `files` = `{"ediciones/AAAA-MM-DD.html": "ediciones/AAAA-MM-DD.html"}`
  (solo la nueva; las anteriores se conservan). Ediciones con más de 30 días: pasar `null`
  en `files` para quitarlas del artefacto (siguen en el repo). No pasar `icon`.
- `label`: "Edición N · D mmm AAAA".

### 7. Guardar
- `git add 04-finanzas && git commit -m "Diario financiero: edición N (AAAA-MM-DD)"` y push a
  la rama por defecto (ver permisos). Mensaje de commit sin identificadores de modelo.
- `03-ruta/bitacora.md` solo si hubo una decisión o cambio de alcance (no cada día).

### 8. Cerrar
Mensaje final de dos líneas, por ejemplo:
"Oro −3 % (3.890), BTC 76.500 tras hack de Binance; tu LTV secundario 54 %. Empleo EE. UU. el viernes.
https://claude.ai/artifact/SLAz28JYah7jirnuFYeL1H"

## Reglas de estilo (no negociables)
- Español, cercano, colombiano neutro. Punto de miles y coma decimal (US$3.890, 12,50 %).
- Explicar cada término la primera vez (una frase). Glosario solo con términos nuevos.
- Separar hechos (con fuente y fecha) de interpretación ("Lectura de Claude"). Fechas de
  calendario: "confirmado" o "por confirmar". Nunca recomendaciones de compra/venta ni asesoría.
- No inventar cifras. Si una fuente no se encuentra, decir "sin dato hoy".
- Los precios son instantáneas: anotar la hora aproximada cuando importe.
- No incluir direcciones de billeteras, números de cuenta ni nombres de terceros que aparezcan
  en Kubera (préstamos personales, familiares).

## Fin de semana y festivos
La rutina corre lunes a viernes. El lunes, cubrir también lo ocurrido sábado y domingo
(cripto y geopolítica). Si Wall Street estuvo cerrado el día anterior, decirlo en el semáforo.
