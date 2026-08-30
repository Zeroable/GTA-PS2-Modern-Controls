# GTA-PS2-Modern-Controls

Modern controller layouts for the original PlayStation 2 versions of *Grand Theft Auto III*, *Grand Theft Auto: Vice City*, and *Grand Theft Auto: San Andreas* when played through PCSX2 or ARMSX2.

The **Definitive Edition Controls** layouts move common driving, aiming, firing, weapon-selection, and camera actions to more familiar modern-controller positions while preserving game-specific actions where needed.

The original PS2 games were designed around the DualShock 2 controller, which had pressure-sensitive face buttons. Cross and Square could detect how hard they were pressed, allowing gradual acceleration and braking instead of simple on/off input.

Modern controllers normally place analog acceleration and braking on R2 and L2. These patches move the games' native pressure-sensitive acceleration and braking actions to those triggers. When the controller and emulator provide analog trigger values, a light press can produce gentle input and a full press can produce full acceleration or braking. A controller configured for digital-only trigger input will still behave like an on/off button.

The patches automatically change control behavior when entering or leaving a vehicle. San Andreas also selects the appropriate vehicle layout for standard vehicles, bikes, and aircraft. No manual controller-profile switching is required during play.

## Emulator testing

These layouts have been tested on:

- **PCSX2 2.8.0**
- **ARMSX2**

## Supported game versions

| Game | Region and release | PCSX2 CRC | File |
| --- | --- | --- | --- |
| Grand Theft Auto III | NTSC-U, SLUS-20062 | `5E115FB6` | `5E115FB6.pnach` |
| Grand Theft Auto: Vice City | NTSC-U, SLUS-20552 | `20B19E49` | `20B19E49.pnach` |
| Grand Theft Auto: San Andreas | NTSC-U, SLUS-20946 | `399A49CA` | `399A49CA.pnach` |

These files are CRC-specific. PCSX2 will not apply a file to a different game revision with another CRC.

## Installation

1. Download the `.pnach` file matching your game and CRC from `Definitive Edition Controls`.
2. Place it in PCSX2's `cheats` folder.
3. Enable cheats in PCSX2.
4. Open the game's cheat list and enable the desired groups.
5. Use the game's original PS2 default control scheme. A different in-game control type can change the results.

For the complete layout, enable all three groups:

- **Group 1 — required:** modern vehicle controls and the shared control hook.
- **Group 2 — optional:** modern on-foot controls. Leave this off to keep the original on-foot layout.
- **Group 3 — optional:** restores native input while the pause/menu screen is open. This group requires Group 1.

## GTA III and Vice City

These two games use the same overall layout.

### On foot

| Button | Action |
| --- | --- |
| L2 | Target / aim |
| R2 | Attack / fire |
| Circle | Attack / fire |
| L1 | Next weapon |
| R1 | Reset camera |
| D-pad Left | Previous weapon |
| D-pad Right | Next weapon |

Native D-pad Up and Down are suppressed while the on-foot group is active. Group 3 keeps pause and menu navigation native.

### In vehicles

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

Native D-pad Left and Down are suppressed while the vehicle group is active. In case you are asked a Yes or No question while in a car. Prevents softlock.

Cross has no vehicle assignment in the Definitive Edition layout. It is mapped here as a second handbrake button alongside R1, keeping the driving layout consistent with *Grand Theft Auto IV*.

## San Andreas

San Andreas uses separate handling for standard vehicles, bikes, and aircraft. It also provides a native-input override for interactions that require the original D-pad.

### Important: hold Select for native vehicle controls

While in any vehicle, hold **Select** to temporarily restore the original controls. This restores native D-pad input for prompts that require a directional answer, including date prompts that ask for a yes/no response.

Release Select to return to the modern layout.

### On foot

| Button | Action |
| --- | --- |
| L2 | Aim |
| R2 | Fire |
| L1 | Previous weapon |
| R1 | Next weapon |
| D-pad | Native actions |

The most important difference from GTA III and Vice City is **R1**: it resets the camera in those games, but selects the **next weapon** in San Andreas.

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

Cross has no vehicle assignment in the Definitive Edition layout. It is mapped here as a second handbrake button alongside R1, keeping the driving layout consistent with *Grand Theft Auto IV*.

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

Bike controls intentionally take a small liberty with the standard layout. R2 and L2 provide pressure-sensitive acceleration and braking when analog trigger values are available, while Cross and Square remain usable for their native bike actions. For bicycles, repeatedly tapping Cross may still be preferable when pedaling hard or building speed quickly.

### Aircraft

Aircraft preserve native L1 and R1 so their original special functions remain available.

| Button | Action sent to the game |
| --- | --- |
| L1 | Native L1 |
| R1 | Native R1 |
| R2 | Native Cross |
| L2 | Native Square |
| Cross | Native Circle / main fire |
| Square | Rudder left |
| Circle | Rudder right |
| R3 | Look behind |
| D-pad Up | Native R3 / landing gear or special action |
| D-pad Down | Native L1 / alternate fire |
| D-pad Left | Native D-pad Up |
| D-pad Right | Native D-pad Down |

This layout applies to aircraft with and without weapons, including planes, helicopters, and the Hydra.

## Credits

- Project, configurations, testing, and public release: **Zeroable**
- Shared hook foundation: **PS2 Controller Remapper by pelvicthrustman**

This is a community project and is not affiliated with Rockstar Games, Sony, or the PCSX2 project.
