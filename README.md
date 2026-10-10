# Corne Wireless — ZMK Keymap Config

Three split Corne keyboards running ZMK firmware on Nice!Nano v2. All three use
the same [keymap](config/corne.keymap), including the gaming layer. The 5-column
keyboard has no physical keys at the outer positions used by the 6-column boards.

| Device | Columns | Bluetooth name |
|--------|---------|----------------|
| Mini Corne | 5 | `Mini Corne` |
| Corne 6 Big | 6 | `Corne 6 Big` |
| Corne 6 Pro | 6 | `Corne 6 Pro` |

## Flash Firmware

One run in **Actions** builds all three devices. Download the 5-column, 6-column,
and third-keyboard artifacts, then flash the matching left and right `.uf2` files
to each device. The 5-column artifact also includes `settings_reset.uf2`.

- [Keymap Editor (visual)](https://nickcoutsos.github.io/keymap-editor/)

---

## Keymap Overview

**Layers:** 5 (Base, Nav/Num, Symbol, Adjust, Game)
**Active keys:** 5 or 6 columns per hand + 3 thumb keys per side

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
| `J` + `K` | `ESC` |

---

## Layer 1 — Nav & Number (hold MO1)

```
·   1    2    3    4    5      6    7    8    9    0    ·
·  TAB  ESC   ·    ·    ·     ←    ↓    ↑    →    ·    ·
·   ·    ·    ·    ·    ·     HOME PgDn PgUp END  DEL   ·
        ____  ____  ____    RET  MO3  BSPC
```

- Numbers across the top row
- Arrow keys on the right home row; Home/PgDn/PgUp/End/Del below them

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
·  BT0  BT1  BT2  BT3  BT4  Play BriDn BriUp GAME BTCLR ·
              ·    ·    ·       ·    ·    ·
```

- F1–F12 on top two rows (left side)
- Media controls on right home row: Mute / Vol- / Vol+ / Prev / Next
- Right bottom row: Play/Pause, Brightness Down/Up, Game toggle, Bluetooth clear
- Bluetooth device select (BT0–BT4) on left bottom
- `BT_CLR` on right bottom corner (safe — requires Layer 3 to reach)

---

## Layer 4 — Game

Hold Nav/Num and Symbol, then tap the right-hand `.` position to enable Game.
Tap that same position again to return to the normal layout. In Game, the left
hand's QWERT/ASDFG/ZXCVB keys send letters directly, without home-row mods.
The left thumbs are **Ctrl**, **Shift**, and **Space**; the other right-hand keys
keep their normal behavior.
