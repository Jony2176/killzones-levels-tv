# Killzones & Levels — TradingView Indicator

Professional forex session indicator with automatic DST adjustment and key levels.

## Features

- **3 Session Boxes** — London, New York, Asia with full market hours
- **Killzone Highlights** — Subtle bgcolor for your specific trading windows within each session
- **Session Hi/Lo/Mid** — Extension lines from the full session range
- **PDH/PDL & PWH/PWL** — Previous Day and Week High/Low levels
- **Automatic DST** — Uses IANA timezones, no manual adjustment needed

## Sessions

| Session | Full Session (UTC-3) | Killzone (UTC-3) | Native TZ | Color |
|---------|---------------------|------------------|-----------|-------|
| 🇬🇧 London | 05:00 - 09:00 | 05:00 - 07:00 | Europe/London | Green |
| 🇺🇸 New York | 10:00 - 15:00 | 10:00 - 12:30 | America/New_York | Orange |
| 🇯🇵 Asia | 20:00 - 04:00 | 20:00 - 22:30 | Asia/Tokyo | Purple |

## Key Levels

- **PDH / PDL** — Previous Day High / Low (amber, dashed)
- **PWH / PWL** — Previous Week High / Low (pink, dotted)
- **Session Hi / Lo** — Session high and low (session color, dashed)
- **Session Mid** — Session midpoint (session color, dotted)

## DST Auto-Adjustment

Sessions are defined in their **native timezone** using IANA names:
- `Europe/London` auto-adjusts between GMT and BST
- `America/New_York` auto-adjusts between EST and EDT
- `Asia/Tokyo` has no DST

**No manual changes needed when clocks change.**

## Installation

1. Open TradingView → Pine Script Editor (bottom tab)
2. Delete the default content
3. Copy and paste the content of `Sessions_Indicator.pine`
4. Click **Add to chart**
5. Click **Save** (disk icon) to save to your My Scripts

## Configuration

In the indicator settings panel:

- **Toggle** each session and level on/off
- **Change colors** for each session
- **Adjust** line extension length (in bars)
- **Modify** session times if you need different ranges

## Recommended Timeframes

- **M1, M5, M15** — Ideal for detailed session view
- **H1** — Sessions appear as compact blocks
- **H4+** — Sessions may not be visible (few bars per session)

> **Note:** On timeframes below 5 minutes, session boxes may end 1-2 minutes early. This is a Pine Script limitation.

## License

MIT
