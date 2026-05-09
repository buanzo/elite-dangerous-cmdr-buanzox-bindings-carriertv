# Release Checklist

Run this from the repository root before committing or publishing.

## Content

- `binds/BUANZOFAOFF.binds` exists and its root preset name is `BUANZOFAOFF`.
- `binds/BUANZOFAOFFXINPUT.binds` exists and its root preset name is `BUANZOFAOFFXINPUT`.
- `README.md` and `docs/install.md` describe GitHub as the primary public download/source location.
- `CONTRIBUTORS.txt` reflects the current human and Codex contributions.

## Privacy

```bash
find . -type f -size +25M -print
find . -type f \( -iname '*.mp4' -o -iname '*.mkv' -o -iname '*.mov' -o -iname '*.jpg' -o -iname '*.jpeg' -o -iname '*.png' -o -iname '*.zip' \) -print
rg -n "Frontier ID|FID|CMDR DARK|HIP 2453|778,855,379|BuanzoPS4Recovered|BuanzoPS4RecoveredXInput|/home/buanzo|/mnt/" .
```

Expected result: no output, except matches inside checklist files that intentionally name blocked patterns.

## Final Video

- Final upload render uses human English voiceover, not the silent smoke audio.
- Install scene uses the sanitized NVIDIA Controls snippet from `4.0s` for `27.5s`.
- Top-right account HUD is covered by the solid privacy mask in every scene.
- Install preset-list area is covered during the install snippet.
- Contact sheets for install and outro scenes show no readable account, Frontier ID, legacy preset, or local-system details.

## Git

- Review `git status --short`.
- Commit only public-safe files.
- Push only after the checklist above is clean.
