# CMDR Buanzox Elite Dangerous Controller Bindings

Public release data for the CarrierTV tutorial about CMDR Buanzox's Elite Dangerous controller profile.

Español: [README.es.md](README.es.md). This is the only translated asset in the repository; data tables, detailed docs, filenames, and binding names remain in English.

This repository is intended to contain only public-safe data: installable `.binds` files, reviewed control tables, and documentation. It intentionally does not contain source videos, screenshots, raw captures, review sheets, local run folders, personal identifiers, or generated tutorial videos.

## Presets

- `binds/BUANZOFAOFF.binds`: native DualShock4 profile. Try this first if Elite Dangerous detects the controller as `DualShock4`.
- `binds/BUANZOFAOFFXINPUT.binds`: XInput fallback. Use this if Steam Input or Windows exposes the controller as an Xbox-style gamepad.

## Install

1. Close Elite Dangerous.
2. Download the `.binds` file you want to use.
3. Copy it to:

```text
%LOCALAPPDATA%\Frontier Developments\Elite Dangerous\Options\Bindings
```

4. Start Elite Dangerous.
5. Go to `Options > Controls`.
6. Select `BUANZOFAOFF` or `BUANZOFAOFFXINPUT`.
7. Apply the preset.

See [docs/install.md](docs/install.md) for the longer install notes. This GitHub repository is the primary public download/source location for the first release.

## Data

- [data/canonical_bindings.tsv](data/canonical_bindings.tsv): reviewed canonical binding table.
- [data/canonical_bindings.json](data/canonical_bindings.json): same canonical table in JSON form.
- [data/export_candidates.tsv](data/export_candidates.tsv): rows that were mapped to Frontier XML action tags for export.

See [data/README.md](data/README.md) for column notes and limitations.

## Tutorial Context

The video explains the profile as a control grammar, not just a button list:

- Alternate Controls is the normal flight layer.
- Regular controls are kept for temporary lateral-thrust work.
- Flight Assist Off is treated as a deliberate combat posture.
- Button families are used for memory: Cross for extremes and targeting, Circle for approach/utilities, Square for weapons/panels, Triangle for travel/maps/ship state.

## Full Binding List

This is the practical assigned-button list from the public data tables. The TSV and JSON files also include blank, default, axis, and evidence rows for audit.

### Flight Layers and Movement

| Action | Binding |
| --- | --- |
| Yaw left | `L1` |
| Yaw right | `R1` |
| Alternate Controls toggle | `CIRCLE+D-PAD LEFT` |

### Throttle Doctrine

| Action | Binding |
| --- | --- |
| Set speed to -100% | `X+L1` |
| Set speed to 0% | `L1+R1` |
| Set speed to 25% | `SQUARE+D-PAD DOWN` |
| Set speed to 50% | `SQUARE+R1` |
| Set speed to 75% | `CIRCLE` |
| Set speed to 100% | `X+R1` |

### Combat and Flight Assist

| Action | Binding |
| --- | --- |
| Primary fire | `R2` |
| Secondary fire | `L2` |
| Deploy hardpoints | `SQUARE` |
| Cycle next fire group | `SQUARE+L1` |
| Toggle Flight Assist | `TRIANGLE+R1` |
| Engine boost | `CIRCLE+L1` |
| Silent running | `TRIANGLE+L1` |
| Toggle orbit lines | `R3` |

### Targeting

| Action | Binding |
| --- | --- |
| Select target ahead | `X` |
| Cycle next target | `X+D-PAD LEFT` |
| Select highest threat | `X+D-PAD DOWN` |
| Select wingman's target | `X+D-PAD RIGHT` |
| Cycle next subsystem | `X+D-PAD UP` |
| Target next system in route | `CIRCLE+R1` |

### Power and Ship Utilities

| Action | Binding |
| --- | --- |
| Divert power to engines | `D-PAD UP` |
| Divert power to weapons | `D-PAD RIGHT` |
| Divert power to systems | `D-PAD LEFT` |
| Balance power distribution | `D-PAD DOWN` |
| Cargo scoop | `CIRCLE+D-PAD UP` |
| Landing gear | `CIRCLE+D-PAD DOWN` |
| Ship lights | `TRIANGLE+R3` |
| Night vision | `TRIANGLE+L3` |

### Panels, Maps, and Headlook

| Action | Binding |
| --- | --- |
| External panel | `SQUARE+D-PAD LEFT` |
| Comms panel | `SQUARE+D-PAD UP` |
| Internal panel | `SQUARE+D-PAD RIGHT` |
| Open galaxy map | `TRIANGLE+D-PAD LEFT` |
| Open system map | `TRIANGLE+D-PAD RIGHT` |
| Supercruise | `TRIANGLE+D-PAD DOWN` |
| Hyperspace jump | `TRIANGLE+D-PAD UP` |
| Switch cockpit mode | `TOUCHPAD` |
| Enter FSS mode | `TOUCHPAD` |
| Headlook | `R3+L3` |

Bottom/role panel note: the expected-looking `SQUARE+D-PAD DOWN` is not a bottom-panel binding in this profile; it sets speed to 25%. To use the bottom/role panel, toggle headlook with `R3+L3`, look down until the panel focuses, then press `R3+L3` again to exit. If you want a direct bottom-panel shortcut, `SQUARE+X` is a clean optional candidate to add manually, but it is not included in these released `.binds` files.

## Privacy Boundary

This repo is private while it is being reviewed, but it should already be treated as public. Anything committed here should be safe to publish later.

Before publishing or adding new data, run [RELEASE_CHECKLIST.md](RELEASE_CHECKLIST.md) and the detailed privacy checks in [docs/privacy-checklist.md](docs/privacy-checklist.md).
