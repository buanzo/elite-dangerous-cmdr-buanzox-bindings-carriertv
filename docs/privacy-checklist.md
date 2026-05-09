# Privacy Checklist

Use this checklist before committing or publishing new files.

## Allowed

- `.binds` files that contain only public preset data.
- Reviewed TSV/JSON binding tables.
- Documentation written for public readers.
- Small metadata files that do not contain local paths, account identifiers, or raw capture references.

## Not Allowed

- Source videos or rendered tutorial videos.
- Screenshots, thumbnails, extracted frames, or contact sheets.
- Raw OCR dumps and review sheets.
- Local manifests containing absolute paths.
- Frontier ID, account IDs, email addresses, local usernames, or private commander/account details.
- Any file copied directly from a raw run folder without review.

## Quick Checks

Run these from the repo root before publishing:

```bash
git status --short
find . -type f -size +25M -print
rg -n "Frontier ID|FID|CMDR DARK|HIP 2453|778,855,379" .
rg -n -g '!docs/privacy-checklist.md' '@' .
find . -type f \( -iname '*.mp4' -o -iname '*.mkv' -o -iname '*.mov' -o -iname '*.jpg' -o -iname '*.png' -o -iname '*.zip' \) -print
```

If any command returns a suspicious result, review it before committing.
