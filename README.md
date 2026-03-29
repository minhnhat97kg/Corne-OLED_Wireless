# Mini Corne — ZMK Keymap Config

Corne split keyboard (5-column, wireless) running ZMK firmware on Nice!Nano v2.

## Flash Firmware

Go to **Actions** tab → download the latest build → flash the `.uf2` file to each half.

- [Keymap Editor (visual)](https://nickcoutsos.github.io/keymap-editor/)

---

## Keymap Overview

**Keyboard name (BT):** `Mini Corne`
**Layers:** 4 (Base, Nav/Num, Symbol, Adjust)
**Active keys:** 5 columns per hand + 3 thumb keys per side

### Home Row Mods (Layer 0)

Hold the home row keys to activate modifiers:

| Key | Hold |
|-----|------|
| `A` | GUI |
| `S` | ALT |
| `D` | CTRL |
| `F` | SHIFT |
| `J` | SHIFT |
| `K` | CTRL |
| `L` | ALT |
| `;` | GUI |

### Thumb Keys (Layer 0)

| Thumb | Tap | Hold |
|-------|-----|------|
| Left outer | `TAB` | `ESC` |
| Left middle | `MO1` (Nav/Num) | — |
| Left inner | `SPACE` | — |
| Right inner | `RET` | `CTRL` |
| Right middle | `MO2` (Symbol) | — |
| Right outer | `BSPC` | `DEL` |

### Combos

| Keys | Output |
|------|--------|
| `W` + `V` | `ESC` |

---

## Layer 1 — Nav & Number (hold MO1)

```
·   1    2    3    4    5      6    7    8    9    0    ·
·  TAB  ESC   ·    ·    ·    HOME PgDn PgUp END  DEL   ·
·   ·    ·    ·    ·    ·      ←    ↓    ↑    →   ·    ·
        ____  ____  ____    RET  MO3  BSPC
```

- Numbers on left top row
- Nav cluster (Home/PgDn/PgUp/End/Del) on right home row
- Arrow keys on right bottom row — mirrors Vim `h j k l`

---

## Layer 2 — Symbol (hold MO2)

```
·    !    @    #    $    %      ^    &    *    (    )   ·
·    '    "    ~    `    ·      -    =    [    ]    \   ·
·    <    >    ·    ·    ·      _    +    {    }    |   ·
        ____  MO3  ____    ____  ____  ____
```

- Quotes `' "` and `` ` `` `~` on left home row
- `< >` on left bottom (Z/X positions)
- Brackets `[ ] { }` and operators on right

---

## Layer 3 — Adjust (hold MO1 + MO2)

```
·   F1   F2   F3   F4   F5     F6   F7   F8   F9  F10  ·
·  F11  F12   ·    ·    ·    MUTE VolDn VolUp Prev Next ·
·  BT0  BT1  BT2  BT3  BT4  Play   ·    ·    ·  BTCLR ·
              ·    ·    ·       ·    ·    ·
```

- F1–F12 on top two rows (left side)
- Media controls on right home row: Mute / Vol- / Vol+ / Prev / Next
- Play/Pause on right bottom
- Bluetooth device select (BT0–BT4) on left bottom
- `BT_CLR` on right bottom corner (safe — requires Layer 3 to reach)
