# GTA-PS2-Modern-Controls

Modern controller layouts for the original PlayStation 2 versions of:

- *Grand Theft Auto III*
- *Grand Theft Auto: Vice City*
- *Grand Theft Auto: San Andreas*
- *Grand Theft Auto: Liberty City Stories*
- *Grand Theft Auto: Vice City Stories*

These PNACH patches are designed for PCSX2 and ARMSX2 and use each game's original PS2 default control scheme as the base.

The **Definitive Edition-style controls** move common driving, aiming, firing, weapon-selection, and camera actions to more familiar modern-controller positions while preserving game-specific functions where necessary.

## Emulator testing

These layouts have been tested on:

- **PCSX2 2.8.0**
- **ARMSX2**

## Supported game versions

| Game | Region and release | PCSX2 CRC | Patch file |
| --- | --- | --- | --- |
| Grand Theft Auto III | NTSC-U, SLUS-20062 | `5E115FB6` | [`5E115FB6_GTA_3_Definitive_Edition_Controls.pnach`](5E115FB6_GTA_3_Definitive_Edition_Controls.pnach) |
| Grand Theft Auto: Vice City | NTSC-U Day 1, SLUS-20552 | `20B19E49` | [`20B19E49_GTA_Vice_City_Definitive_Edition_Controls.pnach`](20B19E49_GTA_Vice_City_Definitive_Edition_Controls.pnach) |
| Grand Theft Auto: San Andreas | NTSC-U, SLUS-20946 | `399A49CA` | [`399A49CA_GTA_San_Andreas_Definitive_Edition_Controls.pnach`](399A49CA_GTA_San_Andreas_Definitive_Edition_Controls.pnach) |
| Grand Theft Auto: Liberty City Stories | NTSC-U, SLUS-21423 | `7EA439F5` | [`7EA439F5_GTA_Liberty_City_Stories_Definitive_Edition_Controls.pnach`](7EA439F5_GTA_Liberty_City_Stories_Definitive_Edition_Controls.pnach) |
| Grand Theft Auto: Vice City Stories | NTSC-U, SLUS-21590 | `4F32A11F` | [`4F32A11F_GTA_Vice_City_Stories_Definitive_Edition_Controls.pnach`](4F32A11F_GTA_Vice_City_Stories_Definitive_Edition_Controls.pnach) |

These files are CRC-specific. A patch for one CRC should not be used with a different game revision.

## Installation

1. Download the PNACH file for your game.
2. Drag or copy it directly into PCSX2's `cheats` folder.
3. Enable cheats in PCSX2.
4. Open the game's cheat list and enable the desired groups.
5. Leave the game on its **original/default PS2 control scheme**.

No renaming or editing of the PNACH file is required.

## Cheat groups and pause-menu behavior

### GTA III, Vice City, and San Andreas

These games use three groups:

- **Group 1 — Required:** vehicle controls and the shared controller hook.
- **Group 2 — Optional:** modern on-foot controls. Leave this disabled to keep the original on-foot layout.
- **Group 3 — Optional:** native pause/menu controls.

For the complete layout, enable all three groups.

### Liberty City Stories and Vice City Stories

These use two groups:

- **Group 1 — Required:** vehicle controls.
- **Group 2 — Optional:** modern on-foot controls.

The native pause-menu guard is built into these patches. While the pause menu is open, the game automatically receives the original stock controller input; no separate pause-menu group is required.

---

# Controls

## Common vehicle layout

*GTA III*, *Vice City*, *Liberty City Stories*, and *Vice City Stories* use the same overall vehicle layout:

| Button | Action |
| --- | --- |
| L2 | Brake / reverse |
| R2 | Accelerate |
| L1 | Vehicle fire |
| R1 | Handbrake |
| Cross | Handbrake |
| Square | Look left |
| Circle | Look right |
| R3 | Look behind |
| D-pad Up | Vehicle sub-mission or special action |
| D-pad Right | Next radio station |

Native D-pad Left and Down are suppressed while the vehicle remap is active.

Cross is used as a second handbrake button alongside R1, giving the driving layout a feel closer to later GTA games.

### Analog acceleration and braking

The original PS2 versions of *GTA III*, *Vice City*, and *San Andreas* used the DualShock 2's pressure-sensitive face buttons for driving. The patches move those native acceleration/braking inputs to R2 and L2 while preserving pressure values.

When the controller and emulator expose analog trigger input, light trigger presses can produce lighter acceleration or braking and full presses can produce full input.

*Liberty City Stories* and *Vice City Stories* use digital acceleration and braking by default, so their R2/L2 driving controls remain digital.

---

## GTA III and Vice City — on foot

These two games use the same on-foot layout:

| Button | Action |
| --- | --- |
| L2 | Target / aim |
| R2 | Attack / fire |
| Circle | Attack / fire |
| L1 | Next weapon |
| R1 | Reset / center camera |
| D-pad Left | Previous weapon |
| D-pad Right | Next weapon |
| R3 | Native action |

The important camera difference compared with San Andreas is **R1**: in GTA III and Vice City it is used to reset/center the camera.

Native D-pad Up and Down are suppressed while the on-foot group is active. Enable Group 3 so pause/menu navigation always uses the game's native controls.

---

## Liberty City Stories and Vice City Stories — on foot

LCS and VCS use a slightly different version of the GTA III-style layout because both games have a freely moving right-stick camera.

| Button | Action |
| --- | --- |
| L2 | Aim |
| R2 | Fire |
| Circle | Native fire |
| R1 | Center camera |
| L1 | Next weapon |
| D-pad Left | Previous weapon |
| D-pad Right | Next weapon |
| D-pad Up | Native |
| D-pad Down | Native |
| R3 | Native |

Both **L1** and **D-pad Right** select the next weapon.

The pause menu always uses completely stock controls automatically.

---

## San Andreas

San Andreas uses separate handling for standard vehicles, bikes, and aircraft.

It also has a temporary native-input override for situations where a gameplay prompt requires the original D-pad.

### Important: hold Select for native controls while in a vehicle

While in any vehicle, hold **Select** to temporarily restore the original vehicle controls.

This is especially useful for prompts that require a directional Yes/No response, such as date interactions. Release Select to return immediately to the modern layout.

### On foot

| Button | Action |
| --- | --- |
| L2 | Aim |
| R2 | Fire |
| L1 | Previous weapon |
| R1 | Next weapon |
| D-pad | Native actions |
| R3 | Native |

The important difference from GTA III and Vice City is **R1**: instead of resetting the camera, it selects the **next weapon**.

### Standard vehicles

| Button | Action |
| --- | --- |
| L2 | Brake / reverse |
| R2 | Accelerate |
| L1 | Main fire |
| R1 | Handbrake |
| Cross | Handbrake |
| Square | Look left |
| Circle | Look right |
| R3 | Look behind |
| D-pad Up | Sub-mission, landing gear, or special vehicle action |
| D-pad Down | Alternate fire / turbo |
| D-pad Left | Previous radio station |
| D-pad Right | Next radio station |

Cross is also available as a second handbrake button alongside R1.

### Bikes

| Button | Action |
| --- | --- |
| R2 | Accelerate |
| L2 | Brake |
| Cross | Native accelerate action |
| Square | Native brake action |
| D-pad Left | Look left |
| D-pad Right | Look right |
| R3 | Look behind |

Cross and Square remain available for their original bike actions. On bicycles, repeatedly tapping Cross may still be preferable when pedaling hard or building speed quickly.

### Aircraft

Aircraft preserve physical L1 and R1 as native inputs so their original special functions remain available.

| Button | Action sent to the game |
| --- | --- |
| L1 | Native L1 |
| R1 | Native R1 |
| R2 | Native Cross |
| L2 | Native Square |
| Cross | Native Circle / main fire |
| Square | Rudder / look left |
| Circle | Rudder / look right |
| R3 | Look behind |
| D-pad Up | Native R3 / landing gear or special action |
| D-pad Down | Native L1 / alternate fire |
| D-pad Left | Native D-pad Up |
| D-pad Right | Native D-pad Down |

This applies to aircraft with and without weapons, including planes, helicopters, and the Hydra.

---

## Why some controls differ between games

The goal is not to force every game into one identical layout. The patches keep the controls as consistent as possible while respecting differences in the original games.

Examples:

- **GTA III / Vice City:** R1 resets or centers the camera on foot.
- **San Andreas:** R1 selects the next weapon on foot.
- **Liberty City Stories / Vice City Stories:** R1 centers the camera, while L1 and D-pad Right both select the next weapon.
- **San Andreas vehicles:** holding Select temporarily restores the original controls for prompts that need the stock D-pad.
- **San Andreas bikes and aircraft:** receive their own layouts so vehicle-specific functions remain usable.
- **LCS / VCS:** pause-menu stock controls are automatic and built into the patch.

## Credits

- Project, control layouts, testing, and public release: **Zeroable**
- Shared controller-hook foundation: **PS2 Controller Remapper by pelvicthrustman**
- Assembly/debugging assistance: **ChatGPT**

## Disclaimer

This is an unofficial community project.

No game files, ISOs, BIOS files, or Rockstar assets are included. The project is not affiliated with or endorsed by Rockstar Games, Take-Two Interactive, Sony, PCSX2, or ARMSX2.
