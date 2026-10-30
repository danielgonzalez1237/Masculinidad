# Portal financiero de Daniel

Carpeta aparte del proyecto de masculinidad. Guarda el portal de mercados que Daniel
pidió el 30 de octubre de 2026 y las notas necesarias para actualizarlo en sesiones
futuras.

## Qué hay aquí

| Archivo | Qué es |
|---|---|
| `portal-mercados.html` | Fuente del portal publicado como artefacto en claude.ai. Se republica al mismo enlace con este archivo. |
| `README.md` | Este archivo: contexto, fuentes y cómo actualizar. |

## Los tres frentes (dicho por Daniel el 30 oct 2026)

1. **Metales preciosos de DEXTRUM**, su proyecto minero. En Kubera aparece capital de
   trabajo en Bolivia asociado a estaño; falta confirmar con Daniel qué metal es el foco
   de DEXTRUM (hipótesis: oro/plata por el nombre "metales preciosos").
2. **Portafolio personal** en Interactive Brokers: índices (VOO, QQQ, VXUS), SGOV,
   acciones (ORCL, AMZN, BRK-B, META, NU, UBER), MSTR y GLD, con margen.
3. **Cripto en inversiones de TUO**: WBTC como colateral en Aave V3 (Arbitrum) con
   préstamo en USDC en dos billeteras, WETH en Aave, Pendle PT que vence el 5 nov 2026,
   Nexo, ETH en varias redes, Hyperliquid. Falta que Daniel explique qué es TUO.

Listas de TradingView de Daniel (no se pueden abrir desde el entorno de Claude; pedirle
los tickers si hacen falta):
- https://es.tradingview.com/watchlists/321093314/
- https://es.tradingview.com/watchlists/320772800/
- https://es.tradingview.com/watchlists/317651462/

## Voces que sigue en X

Michael Saylor, Tom Lee, Felipe Campos (Alianza Valores, USD/COP), Juan Rodríguez
(YouTube "Bitcoin y Criptos") y Jack Garzón (cripto, Colombia).

## Cómo actualizar el portal

1. Leer este README y la última entrada de `03-ruta/bitacora.md` sobre el portal.
2. Traer posiciones de Kubera (conector) y noticias del día (búsqueda web): Fed y datos
   de EE. UU., oro/plata/estaño y mineras, BTC/ETH y custodios, petróleo y geopolítica,
   USD/COP y Banco de la República, resultados de las empresas de su IBKR.
3. Editar `portal-mercados.html` (subir el número de edición y la fecha de corte) y
   republicar al mismo enlace del artefacto.
4. Reglas: montos absolutos de Kubera fuera de la página (solo porcentajes y niveles);
   marcar siempre "Lectura de Claude" lo que sea interpretación; distinguir fechas
   confirmadas de "por confirmar".
