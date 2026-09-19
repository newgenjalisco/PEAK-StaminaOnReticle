# Stamina On Reticle

A lightweight, client-side PEAK mod that draws your stamina as a circular ring
right around the crosshair, so you never have to look away to check it.

## Features

- Full circular ring centred on the crosshair that drains as stamina is spent.
- Active status effects are represented using each status in-game color.
-  Additional outer ring for the extra stamina.
- Configurable diameter, thickness, colours and screen offset.

## Configuration

Everything is configured from one plain text file, so you can change the mod
with Notepad (or any text editor): open the file, change a value, save it and
start the game. No extra tools are needed.

The mod ships with a ready-to-edit default config that mod managers copy to the
`BepInEx\config` folder:

```
com.staminaonreticle.peak.cfg
```

On a manual install it is located in the game's folder:

```
<PEAK install folder>\BepInEx\config\com.staminaonreticle.peak.cfg
```

Mod managers such as Gale or r2modman keep it inside their profile instead, for
example `%APPDATA%\r2modmanPlus-local\PEAK\profiles\Default\BepInEx\config\`.

The file uses simple `key = value` lines, with comments explaining each option
and the defaults. It can also be edited live in-game with ConfigurationManager.

Key options:

| Setting | Default | Description |
| --- | --- | --- |
| `Enabled` | `true` | Show the ring. |
| `Show Stats` | `true` | Draw active status effects as coloured arcs. |
| `Show Extra Stamina` | `true` | Draw the outer extra-stamina ring. |
| `Hide When Full` | `false` | Fade the ring out at full stamina. |
| `Diameter` / `Thickness` | `46` / `3.5` | Ring size in pixels at 1080p. |
| `Full Color` / `Low Color` | `#4CD137` | Ring colour. |
| `Offset X` / `Offset Y` | `0` | Fine-tune the position. |

## Installation

Install with Gale, r2modman, or any Thunderstore mod manager. The mod depends on
`BepInEx-BepInExPack_PEAK`.
