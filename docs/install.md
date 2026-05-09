# Installation Guide

## Which File To Use

The GitHub repository is the primary public download/source location for the first release.

- Use `BUANZOFAOFF.binds` first if Elite Dangerous detects the controller as `DualShock4`.
- Use `BUANZOFAOFFXINPUT.binds` if Steam Input or Windows exposes the controller as an Xbox-style gamepad.

## Install Steps

1. Close Elite Dangerous.
2. Open the Windows run dialog with `Win + R`.
3. Paste this path and press Enter:

```text
%LOCALAPPDATA%\Frontier Developments\Elite Dangerous\Options\Bindings
```

4. Copy one or both `.binds` files from the `binds/` directory into that folder.
5. Start Elite Dangerous.
6. Open `Options > Controls`.
7. Select `BUANZOFAOFF` or `BUANZOFAOFFXINPUT`.
8. Apply the preset.

If Elite was already open when the file was copied, restart the game so it reloads the bindings folder.

## Optional StartPreset File

Elite can be nudged toward a preset by creating or editing this file in the same `Bindings` folder:

```text
StartPreset.start
```

The file should contain only the preset name, without `.binds`:

```text
BUANZOFAOFF
```

or:

```text
BUANZOFAOFFXINPUT
```

This is optional. Selecting the preset inside Elite is the preferred visible confirmation.
