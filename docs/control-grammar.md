# Control Grammar

This profile is designed as a control grammar, not a flat button list.

## Flight Layers

- Alternate Controls is the normal flight layer.
- Regular controls are used temporarily for lateral-thrust precision work.
- Flight Assist Off is treated as a deliberate combat posture.

## Button Families

- Cross: throttle extremes and targeting root.
- Circle: approach speed and ship utilities.
- Square: weapons, fire groups, and cockpit panels.
- Triangle: travel, maps, Flight Assist, and ship state.
- D-pad: power distribution when used alone.

## Examples

- `X+R1`: set speed to 100 percent.
- `X+L1`: set speed to -100 percent.
- `L1+R1`: set speed to 0 percent.
- `CIRCLE`: set speed to 75 percent.
- `TRIANGLE+R1`: toggle Flight Assist.
- `CIRCLE+D-PAD LEFT`: toggle Alternate Controls.
- `SQUARE+D-PAD LEFT`: external panel.
- `SQUARE+D-PAD UP`: comms panel.
- `SQUARE+D-PAD RIGHT`: internal panel.
- `TRIANGLE+D-PAD LEFT`: galaxy map.

## Bottom Panel Exception

`SQUARE+D-PAD DOWN` looks like it should complete the Square-plus-D-pad panel set, but it does not. In this profile it is `SET SPEED TO 25%`.

For the bottom/role panel, use the recovered method: press `R3+L3` to enter headlook, look down until the panel focuses, then press `R3+L3` again to exit.

If you want a direct bottom-panel shortcut, `SQUARE+X` is a clean optional candidate to add manually. It is not included in the released `.binds` files.

The tutorial video highlights these combinations on a DualShock-style controller so the viewer sees both the binding and the physical button family.
