---
name: openclaw-singapore-kopi
description: Teach Singapore and Malaysia kopi stall ordering shorthand, translate plain-language coffee preferences into hawker jargon, and explain modifiers like kopi, o, c, kosong, peng, gao, po, and siew dai.
---

# How to Order Kopi Like a Pro

Translate what the user wants into the shortest kopi-stall order that a hawker or kopitiam server would expect. Default to common Singapore usage unless the user explicitly asks for Malaysia or another local variation.

## Core rule

Build the order in this sequence:

1. Base drink
2. Milk style
3. Sweetness modifier
4. Strength modifier
5. Temperature

When the user gives plain English, convert it into the shortest natural phrase instead of explaining first. Then provide a one-line gloss if helpful.

Example:

- User intent: `iced coffee with evaporated milk, less sweet, extra strong`
- Say: `kopi c siew dai gao peng`
- Gloss: `iced coffee with evaporated milk, less sugar, extra strong`

## Base vocabulary

Use these defaults:

| Term | Meaning |
| --- | --- |
| `kopi` | coffee with condensed milk and sugar |
| `kopi o` | coffee with sugar, no milk |
| `kopi c` | coffee with evaporated milk and sugar |
| `teh` | tea with condensed milk and sugar |
| `teh o` | tea with sugar, no milk |
| `teh c` | tea with evaporated milk and sugar |

`kosong` means no sugar. `peng` means iced.

## Common modifiers

| Term | Meaning |
| --- | --- |
| `kosong` | no sugar |
| `siew dai` or `siu dai` | less sugar |
| `gah dai` | extra sweet |
| `gao` | extra strong |
| `po` | weaker |
| `peng` | iced |

If the user asks for black coffee with no sugar, prefer `kopi o kosong`.

If the user asks for iced black coffee with no sugar, prefer `kopi o kosong peng`.

If the user asks for evaporated milk and no sugar, prefer `kopi c kosong`.

## Translation patterns

Use these direct conversions:

| User says | Convert to |
| --- | --- |
| `coffee` | `kopi` |
| `black coffee` | `kopi o` |
| `coffee with evaporated milk` | `kopi c` |
| `no sugar` | `kosong` |
| `less sugar` | `siew dai` |
| `extra strong` | `gao` |
| `weaker` | `po` |
| `iced` | `peng` |

Examples:

- `hot black coffee no sugar` -> `kopi o kosong`
- `iced black coffee less sweet` -> `kopi o siew dai peng`
- `iced coffee with evaporated milk no sugar` -> `kopi c kosong peng`
- `iced black coffee no sugar` -> `kopi o kosong peng`
- `extra strong hot coffee` -> `kopi gao`

## Response style

When the user asks what to say at the stall:

1. Lead with the exact phrase to say.
2. Keep it short.
3. Add a plain-English gloss only if the shorthand is non-obvious.

Preferred format:

```text
Say: kopi c kosong peng
Meaning: iced coffee with evaporated milk, no sugar
```

When the user asks for a lesson or cheat sheet, give a compact table and 3 to 5 useful examples.

When the user sounds unsure, mention that wording can vary a bit by stall and region.

## Regional caution

Treat these terms as common hawker shorthand, not a rigid universal standard. Some stalls use slightly different spellings or default sweetness. If accuracy matters, tell the user to confirm with the stall.
