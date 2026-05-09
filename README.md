# CMDR Buanzox Elite Dangerous Controller Bindings

Public release data for the CarrierTV tutorial about CMDR Buanzox's recovered Elite Dangerous controller profile.

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

## Privacy Boundary

This repo is private while it is being reviewed, but it should already be treated as public. Anything committed here should be safe to publish later.

Before publishing or adding new data, run [RELEASE_CHECKLIST.md](RELEASE_CHECKLIST.md) and the detailed privacy checks in [docs/privacy-checklist.md](docs/privacy-checklist.md).
