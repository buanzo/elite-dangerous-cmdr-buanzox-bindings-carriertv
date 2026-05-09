# Public Data Notes

This directory contains reviewed data derived from the recovered controller profile.

## Files

- `canonical_bindings.tsv`: tab-separated canonical table. This is the easiest file to inspect in a spreadsheet.
- `canonical_bindings.json`: JSON copy of the canonical table for tooling.
- `export_candidates.tsv`: subset or mapped rows used to generate the Frontier `.binds` files.

## Important Columns

- `section`: Elite Dangerous controls section.
- `canonical_label`: normalized binding name.
- `primary_value`: recovered primary binding value.
- `secondary_value`: recovered secondary binding value, when present.
- `binding_kind`: approximate row type, such as button, axis, or setting.
- `recovery_status`: review status from the recovery workflow.
- `pc_bind_tag`: Frontier XML action tag used when the row can be exported.
- `export_status`: whether the row was ready for export.

## Limitations

The data is a reviewed reconstruction, not an official Frontier profile export. Some rows are intentionally blank, and some visible settings do not map cleanly to a current PC `.binds` action tag.

The installable files in `../binds/` are the public release candidates. Use the tables here for audit, explanation, and future maintenance.
