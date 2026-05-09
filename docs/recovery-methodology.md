# Recovery Methodology

The public files here come from a reviewed recovery workflow:

1. Source control-menu footage was analyzed frame by frame.
2. OCR and manual review were used to extract visible rows.
3. Obvious OCR corruption and duplicate rows were normalized into canonical labels.
4. Manual supplements were added only when a row was confidently recovered from the source material.
5. Export-ready rows were mapped to Frontier `.binds` XML action tags.
6. Two installable release candidates were generated:
   - `BUANZOFAOFF.binds` from a native DualShock4-style template.
   - `BUANZOFAOFFXINPUT.binds` from an XInput-style template.

## What Is Not Included

This repository does not include:

- raw videos
- screenshots
- frame dumps
- OCR review sheets
- local run manifests with absolute paths
- generated tutorial videos
- personal identifiers or game-account metadata

Those materials are intentionally kept out of the public-data repo.
