# Killzones & Levels — TradingView Indicator

Indicador profesional de sesiones con ajuste automático de DST y niveles clave.

## Sesiones

| Sesión | Tu hora (UTC-3) | Zona horaria nativa | Color |
|--------|-----------------|---------------------|-------|
| 🇬🇧 London | 05:00 - 07:00 | Europe/London 08:00-10:00 | Azul |
| 🇺🇸 New York | 10:00 - 12:30 | America/New_York 08:00-10:30 | Naranja |
| 🇯🇵 Asia | 20:00 - 22:30 | Asia/Tokyo 08:00-10:30 | Púrpura |

### Sesiones Completas (fondo ultra-suave)

| Sesión | Horario completo (UTC-3) | Zona Nativa |
|--------|--------------------------|-------------|
| 🇬🇧 London | ~05:00 - 14:00 | Europe/London 08:00-17:00 |
| 🇺🇸 NY | ~10:00 - 19:00 | America/New_York 08:00-17:00 |
| 🇯🇵 Asia | ~20:00 - 06:00 | Asia/Tokyo 09:00-18:00 |

> Las sesiones completas se muestran como un fondo casi invisible (97% transparencia) para dar contexto de cuándo el mercado está activo. Los killzones (boxes) se dibujan encima con más visibilidad.

## Niveles

- **PDH / PDL** — Previous Day High / Low (ámbar, línea discontinua)
- **PWH / PWL** — Previous Week High / Low (rosa, línea punteada)
- **Session Hi / Lo** — Máximo y mínimo de cada sesión (color de sesión, discontinua)
- **Session Mid** — Punto medio de cada sesión (color de sesión, punteada)

## DST Automático

Las sesiones se definen en su **zona horaria nativa** usando nombres IANA:
- `Europe/London` ajusta automáticamente entre GMT y BST
- `America/New_York` ajusta automáticamente entre EST y EDT
- `Asia/Tokyo` no tiene DST

**No necesitás cambiar nada cuando cambia el horario.**

## Cómo instalar

1. Abrí TradingView → Pine Script Editor (pestaña inferior)
2. Borrá el contenido por defecto
3. Copiá y pegá el contenido de `Sessions_Indicator.pine`
4. Hacé clic en **Add to chart**

## Configuración

En el panel de settings del indicador, podés:

- **Activar/desactivar** cada sesión y cada nivel
- **Cambiar colores** de fondo, borde, líneas y labels
- **Ajustar** la extensión de líneas (en barras)
- **Modificar horarios** de sesión si necesitás rangos diferentes

## Timeframes recomendados

- **M1, M5, M15** — Ideal para ver las sesiones con detalle
- **H1** — Se ven las sesiones como bloques compactos
- **H4+** — Las sesiones pueden no ser visibles (pocas barras por sesión)
