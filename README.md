# GTA-PS2-Modern-Controls

Modern controller layouts for the original PlayStation 2 versions of:

- *Grand Theft Auto III*
- *Grand Theft Auto: Vice City*
- *Grand Theft Auto: San Andreas*
- *Grand Theft Auto: Liberty City Stories*
- *Grand Theft Auto: Vice City Stories*

These PNACH patches are designed for PCSX2 and ARMSX2 and use each game's original PS2 default control scheme as the base.

The **Definitive Edition-style controls** move common driving, aiming, firing, weapon-selection, and camera actions to more familiar modern-controller positions while preserving game-specific functions where necessary.

## Purpose of the patches

The original PS2 games were designed around the DualShock 2 controller, which had pressure-sensitive face buttons. Cross and Square could detect how hard they were pressed, allowing gradual acceleration and braking instead of simple on/off input.

Modern controllers normally place analog acceleration and braking on R2 and L2. These patches move the games' native pressure-sensitive acceleration and braking actions to those triggers. When the controller and emulator provide analog trigger values, a light press can produce gentle input and a full press can produce full acceleration or braking. A controller configured for digital-only trigger input will still behave like an on/off button.

*Vice City Stories* also supports analog acceleration and braking on PS2, so its R2/L2 trigger mappings preserve that analog behavior. *Liberty City Stories* currently uses digital acceleration and braking in the released patch. A separate **analog acceleration/braking WIP build** is available for testing in the [`WIP`](WIP) folder.

## Coming soon / work in progress

Additional mods still being developed are kept in the [`WIP`](WIP) folder. These builds are unfinished and may change as development continues.

### Available now as WIP builds

- **Grand Theft Auto: Liberty City Stories — Analog acceleration/braking controls** — [download WIP build](WIP/7EA439F5_GTA_Liberty_City_Stories_Definitive_Edition_Controls_Analog_Acceleration_Braking_WIP.pnach)
- **Grand Theft Auto: San Andreas — First-person mod** — [download WIP build](WIP/399A49CA_GTA_San_Andreas_First_Person_WIP.pnach)

The WIP folder is kept separate from the finished releases in the repository root.

### Additional released patches

- **Grand Theft Auto III — HUD + radar removal** — [download release](5E115FB6_GTA3_No_Hud.pnach)
- **Grand Theft Auto III — Map Toggle 1.0** — [download release](5E115FB6_GTA_3_Map_Toggle.pnach)
- **Grand Theft Auto III — Right Stick Camera and First Person 1.0** — [download release](5E115FB6_GTA_3_Right_Stick_Camera_and_First_Person.pnach)
- **Grand Theft Auto: Vice City — Right Stick Camera and First Person 1.02** — [download release](20B19E49_GTA_Vice_City_Right_Stick_Camera_and_First_Person.pnach)

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

## Released additional patch documentation

### GTA III HUD + radar removal

File: [`5E115FB6_GTA3_No_Hud.pnach`](5E115FB6_GTA3_No_Hud.pnach)

Enable **No HUD + Radar > Enable** to hide the GTA III HUD and minimap/radar.

After turning the removal cheat off, use **Restore HUD + Radar** once if you want the HUD and radar back without restarting the game. Leave the restore option off during normal use.

### GTA III Map Toggle 1.0

File: [`5E115FB6_GTA_3_Map_Toggle.pnach`](5E115FB6_GTA_3_Map_Toggle.pnach)

This patch adds an in-game GTA III map display using the game's original map assets.

Usage and notes:

- Press **D-pad Down** to open or close the map.
- While the map is open, press **Cross** to hide or show the **location icons**.
- The optional **Map on Pause Menu Background** group moves the pause-map background upward. It requires the main Map Toggle group; restart the game after changing this option.
- A **cold boot** is required.
- The release is designed around a **4:3 display**.
- It uses the game's original radar/map tiles and HUD sprites; no ISO modification is required.

### GTA III Right Stick Camera and First Person 1.0

File: [`5E115FB6_GTA_3_Right_Stick_Camera_and_First_Person.pnach`](5E115FB6_GTA_3_Right_Stick_Camera_and_First_Person.pnach)

Target: **NTSC-U SLUS-20062 / CRC `5E115FB6`**

This patch adds a **right-stick Orbit camera** and an **on-foot first-person camera** to GTA III.

Controls and notes:

- Press **Select + D-pad Down** to toggle the alternate-camera set on or off.
- While enabled and on foot, press **Select** to cycle **Orbit Far → Orbit Medium → Orbit Near → First Person**.
- In vehicles, **Select** cycles the three Orbit distances only; First Person remains on-foot only.
- **R3** temporarily looks behind.
- Hold the game's native **L1 camera-center action** to smoothly center the view; with the Zeroable modern on-foot controls, that action is on **R1**.
- Includes an optional **Inversion OFF** group. GTA III's default vertical look is inverted; enable this option for non-inverted vertical look in the alternate cameras, native first-person view, sniper aiming, and bazooka aiming.
- Supports stock controls, the Zeroable modern-controls patch, and the released GTA III Map Toggle.
- A **cold boot and memory-card load** are required.

#### Demonstration video

This video demonstrates the **GTA III Right Stick Camera and First Person** mod:

https://github.com/user-attachments/assets/60f1e004-d828-4671-b8e2-57960329ffde

### GTA Vice City Right Stick Camera and First Person 1.02

File: [`20B19E49_GTA_Vice_City_Right_Stick_Camera_and_First_Person.pnach`](20B19E49_GTA_Vice_City_Right_Stick_Camera_and_First_Person.pnach)

Target: **NTSC-U Day 1 SLUS-20552 / CRC `20B19E49`**

This patch adds a **right-stick Orbit camera** and an **on-foot first-person camera** to Vice City.

Controls and notes:

- Press **D-pad Down** to toggle the camera mod on or off. This works with either stock controls or the Zeroable modern-controls patch.
- While enabled and on foot, press **Select** to cycle **Orbit Far → Orbit Medium → Orbit Near → First Person**.
- In vehicles, **Select** cycles the three Orbit distances only; First Person remains on-foot only.
- **R3** temporarily looks backward.
- Hold the game's native **L1 camera-center action** to smoothly center the view; with the Zeroable modern on-foot controls, that action is on **R1**.
- Stock controls are supported. The Zeroable modern-controls patch is optional and no controller remapping is bundled into this mod.
- A **full restart and memory-card load** are required.

#### Demonstration video

This video demonstrates the **Vice City Right Stick Camera and First Person** mod:

https://github.com/user-attachments/assets/647da0ea-b225-4436-82e1-7636dfb32a2c

## WIP patch documentation

### GTA Liberty City Stories Analog Acceleration/Braking

File: [`WIP/7EA439F5_GTA_Liberty_City_Stories_Definitive_Edition_Controls_Analog_Acceleration_Braking_WIP.pnach`](WIP/7EA439F5_GTA_Liberty_City_Stories_Definitive_Edition_Controls_Analog_Acceleration_Braking_WIP.pnach)

Target: **NTSC-U SLUS-21423 / CRC `7EA439F5`**

This WIP keeps the current Liberty City Stories modern-control layout while adding full-range analog vehicle acceleration and braking.

Current behavior and notes:

- **R2** provides analog acceleration and **L2** provides analog braking/reverse.
- The analog pedal hooks bypass the game's normal 4× Cross/Square pressure gain and minimum-throttle behavior while driving.
- Stock controller processing is retained **on foot**, **while paused**, and for the **second controller**.
- Requires analog trigger bindings in PCSX2 to get proportional input.
- The existing released Liberty City Stories control patch remains unchanged and continues to use digital acceleration/braking.
- This build is being kept in WIP while it receives additional testing.



The remaining WIP patch is unfinished and may change as development continues.

### GTA San Andreas First-person mod

File: [`WIP/399A49CA_GTA_San_Andreas_First_Person_WIP.pnach`](WIP/399A49CA_GTA_San_Andreas_First_Person_WIP.pnach)

Target: **NTSC-U SLUS-20946 / CRC `399A49CA`**

The current San Andreas WIP uses the closest on-foot camera to provide a first-person-style view with free vertical look.

Current behavior and options:

- **First Person - Free Vertical Look** is the main group.
- The current camera defaults use a distance of **-2.35** and a height adjustment of **+0.65**.
- Other camera cheats should be disabled while testing it.
- **First Person - Hide Body** is an optional group that requires the main first-person group.
- Hide Body removes CJ's body from the closest on-foot first-person view while leaving weapons on their normal draw path.
- Switching camera restores the body.
- To fully undo the instruction patch or uninstall the Hide Body hooks, restart the game with the relevant cheat disabled.

## Cheat groups and pause-menu behavior

All five control patches use two selectable groups:

- **Group 1 — Required:** enables the modern vehicle controls and required controller hooks.
- **Group 2 — Optional:** enables the modern on-foot controls. Leave this disabled to keep the game's original on-foot layout.

For the complete modern control layout, enable both groups.

The **pause-menu guard is built directly into every patch**. While the pause/menu screen is open, the game automatically receives the original stock controller input. There is no separate pause-menu cheat or additional group to enable.

---

# Controls

The tables below describe the **complete physical controller layout while the patch is active**, not just the buttons that were changed. When a button is unchanged, it is marked **Native** and its normal game function is shown.

## GTA III, Vice City, Liberty City Stories, and Vice City Stories

These four games use the same modernized on-foot layout and the same overall vehicle layout.

### On foot

| Physical control | Action with patch | Notes |
| --- | --- | --- |
| Left Stick | Move | **Native** |
| Right Stick | Camera / look | **Native**; exact camera behavior remains game-specific |
| Cross | Sprint / run | **Native** |
| Square | Jump | **Native** |
| Triangle | Enter vehicle | **Native** |
| Circle | Attack / fire | **Native** |
| L2 | Aim / target | Remapped from the game's native R1 targeting function |
| R2 | Attack / fire | Additional fire button |
| L1 | Next weapon | Remapped to the game's native R2 / next-weapon function |
| R1 | Center / reset camera | Remapped to the game's native L1 camera-center function |
| D-pad Left | Previous weapon | Remapped to the game's native L2 / previous-weapon function |
| D-pad Right | Next weapon | Remapped to the game's native R2 / next-weapon function |
| R3 | Look behind | **Native** |
| Select | Change camera mode | **Native** |
| Start | Pause menu | **Native** |
| L3 | Original game function | **Native**; this differs by game (for example crouch or free aim where supported) |

The core on-foot layout is therefore the same in **GTA III, Vice City, Liberty City Stories, and Vice City Stories**: L2 aims, R2 fires, R1 centers the camera, L1 selects the next weapon, and the D-pad left/right directions cycle weapons.

For the remaining D-pad directions, the current GTA III and Vice City patches suppress D-pad Up while the on-foot remap is active, but D-pad Down passes through natively. Liberty City Stories and Vice City Stories leave those directions native.

### In vehicles

| Physical control | Action with patch | Notes |
| --- | --- | --- |
| Left Stick | Steer | **Native** |
| Right Stick | Vehicle camera / turret / other vehicle-specific function | **Native** |
| L2 | Brake / reverse | Moved from native Square |
| R2 | Accelerate | Moved from native Cross |
| L1 | Vehicle fire | Moved to the left shoulder |
| R1 | Handbrake | Same gameplay function as stock |
| Cross | Handbrake | Second handbrake button |
| Square | Look left | Moved from native L2 |
| Circle | Look right | Moved from native R2 |
| Triangle | Exit vehicle | **Native** |
| L3 | Horn / siren where supported | **Native** |
| R3 | Look behind | Mapped to the game's native left+right look input |
| D-pad Up | Vehicle sub-mission / special action | GTA III / Vice City: moved from native R3; Stories titles retain their current patch behavior |
| D-pad Right | Next radio station | Moved from the game's native radio control |
| D-pad Left | Unassigned by the modern layout | Native direction is suppressed while driving |
| D-pad Down | Original game function | GTA III / Vice City: **Native**; Stories titles retain their current patch behavior |
| Select | Change camera mode | **Native** |
| Start | Pause menu | **Native** |

Cross is intentionally available as a second handbrake button alongside R1. In GTA III and Vice City, D-pad Down now passes through natively in vehicles so it remains available for game functions or external mod shortcuts, while D-pad Up still triggers the mapped vehicle sub-mission/special action.

### Pause menus

For **GTA III** and **Vice City**, the pause guard is integrated directly into the existing control groups. While the pause/menu screen is open, the game automatically receives completely stock controller input; there is no separate pause-menu cheat option.

For **Liberty City Stories** and **Vice City Stories**, the pause guard is built directly into the patch. The pause menu automatically receives completely stock controller input.

### Analog acceleration and braking

GTA III, Vice City, and Vice City Stories retain the original PS2 analog / pressure-sensitive acceleration and braking behavior when those actions are moved to R2/L2.

Liberty City Stories currently uses digital acceleration and braking in this patch. Analog acceleration support for LCS is in progress.

---

## San Andreas

San Andreas uses the same general modern layout, but its original controls are more complex, so the patch has separate handling for on-foot play, standard vehicles, bikes, and aircraft.

### On foot

| Physical control | Action with patch | Notes |
| --- | --- | --- |
| Left Stick | Character movement | **Native** |
| Right Stick | Camera movement | **Native** |
| Cross | Run / sprint | **Native** |
| Square | Jump / climb / block | **Native** |
| Triangle | Enter vehicle / game-specific interaction | **Native** |
| Circle | Attack / fire | **Native** |
| L2 | Aim / target | Remapped from native R1 |
| R2 | Fire | Remapped from native L1 fire function |
| L1 | Previous weapon | Remapped from native L2 |
| R1 | Next weapon | Remapped from native R2 |
| L3 | Crouch | **Native** |
| R3 | Look behind | **Native** |
| D-pad Up | Gang active mode | **Native** |
| D-pad Down | Gang passive mode | **Native** |
| D-pad Left | Previous weapon | Mirrors native L2 / previous weapon; hold Select to use native D-pad Left / negative response |
| D-pad Right | Next weapon | Mirrors native R2 / next weapon; hold Select to use native D-pad Right / positive response |
| Select | Change camera mode / native D-pad fallback | **Native** by itself; while held, D-pad Left/Right temporarily use their original game functions |
| Start | Pause menu | **Native** |

The major difference from the other four games is R1: in San Andreas it becomes **Next Weapon** instead of **Center Camera**.

D-pad Left and Right also mirror **Previous Weapon** and **Next Weapon** during normal on-foot play. To preserve the game's original directional-response functions and avoid edge cases where native Left/Right are required, hold **Select** while pressing D-pad Left or Right to temporarily pass those directions through natively.

### Standard vehicles

| Physical control | Action with patch | Notes |
| --- | --- | --- |
| Left Stick | Steering | **Native** |
| Right Stick | Manual camera / turret / vehicle-specific control | **Native** |
| L2 | Brake / reverse | Moved from native Square |
| R2 | Accelerate | Moved from native Cross |
| L1 | Main vehicle fire | Mapped to native Circle |
| R1 | Handbrake | Same gameplay function as stock |
| Cross | Handbrake | Second handbrake button |
| Square | Look left | Mapped to native L2 |
| Circle | Look right | Mapped to native R2 |
| Triangle | Exit vehicle | **Native** |
| L3 | Horn / siren where supported | **Native** |
| R3 | Look behind | Mapped to native L2+R2 |
| D-pad Up | Sub-mission / special vehicle action | Mapped to native R3 |
| D-pad Down | Alternate fire / turbo | Mapped to native L1 |
| D-pad Left | Previous radio station | Uses the game's native radio direction |
| D-pad Right | Next radio station | Uses the game's native radio direction |
| Select | **Hold to restore native D-pad only** | Other vehicle buttons keep the modern mapping while Select is held |
| Start | Pause menu | **Native** |

### Important: hold Select to temporarily restore the native D-pad

While driving in San Andreas, **hold Select to restore only the original/native D-pad directions**. Every other vehicle button keeps the modern mapping while Select is held. Release Select and the D-pad immediately returns to the modern vehicle layout.

This is not just a convenience feature. The modern vehicle layout reuses native D-pad inputs, so some original directional responses are otherwise unavailable while driving.

That can matter during dates. A girlfriend can ask CJ a question while he is in a vehicle and expect a **left/right D-pad response**. Without a way to send the original D-pad input, the interaction can become a soft lock because there is no valid way to answer.

If that happens, simply **hold Select and press the required native D-pad direction**. Acceleration, braking, firing, camera-look buttons, and the other modern vehicle mappings remain modern while Select is held.

### Bikes

| Physical control | Action with patch | Notes |
| --- | --- | --- |
| Left Stick | Steering / balance | **Native** |
| Right Stick | Camera | **Native** |
| R2 | Accelerate / pedal | Mapped to native Cross |
| L2 | Brake | Mapped to native Square |
| Cross | Accelerate / pedal | **Native** and intentionally retained |
| Square | Brake | **Native** and intentionally retained |
| D-pad Left | Look left | Mapped to native L2 |
| D-pad Right | Look right | Mapped to native R2 |
| R3 | Look behind | Mapped to native L2+R2 |
| Triangle | Exit / dismount | **Native** |
| L1 | Original bike-specific action | **Native** |
| R1 | Original bike-specific action | **Native** |
| Circle | Original bike-specific vehicle action | **Native** |
| L3 | Original bike-specific action | **Native** |
| D-pad Up | Original bike/vehicle action | **Native** |
| D-pad Down | Original bike/vehicle action | **Native** |
| Select | **Hold to restore native D-pad only** | All other vehicle buttons remain on the modern mapping |
| Start | Pause menu | **Native** |

Cross and Square remain usable for their original bike actions in addition to the trigger mappings. On bicycles, tapping Cross can still be useful for faster pedaling.

### Aircraft

Aircraft preserve physical L1 and R1 as native inputs because aircraft use those shoulders for important game-specific functions.

| Physical control | Action with patch | Notes |
| --- | --- | --- |
| Left Stick | Pitch / roll | **Native** |
| Right Stick | Camera / turret where supported | **Native** |
| L1 | Native L1 aircraft function | **Native** |
| R1 | Native R1 aircraft function | **Native** |
| L2 | Native Square function | Descend / aircraft-specific braking function |
| R2 | Native Cross function | Thrust / ascend depending on aircraft |
| Cross | Native Circle / main fire | Extra aircraft fire mapping |
| Square | Native L2 | Rudder / look left |
| Circle | Native R2 | Rudder / look right |
| Triangle | Exit aircraft | **Native** |
| L3 | Native aircraft function | **Native**; for example hover where supported |
| R3 | Look behind | Mapped to native L2+R2 |
| D-pad Up | Native R3 / special action | Landing gear, sub-mission, or aircraft-specific action |
| D-pad Down | Native L1 / alternate fire | Aircraft-specific secondary function |
| D-pad Left | Native D-pad Up | Previous-direction function used by the original aircraft controls |
| D-pad Right | Native D-pad Down | Next-direction function used by the original aircraft controls |
| Select | **Hold to restore native D-pad only** | All other vehicle buttons remain on the modern mapping |
| Start | Pause menu | **Native** |

This aircraft layout applies to planes, helicopters, and the Hydra while keeping native L1/R1 functions available.

### Pause menu

The San Andreas pause guard is integrated directly into the existing control groups. While the pause/menu screen is open, the game automatically receives completely stock controller input; there is no separate pause-menu cheat option.

---

## Summary of the main game-to-game differences

| Game(s) | On-foot R1 | On-foot L1 | Vehicle Select override | Pause-menu handling |
| --- | --- | --- | --- | --- |
| GTA III / Vice City | Center camera | Next weapon | No | Automatic / built in |
| Liberty City Stories / Vice City Stories | Center camera | Next weapon | No | Automatic / built in |
| San Andreas | Next weapon | Previous weapon | **Hold Select for native D-pad only** | Automatic / built in |

## Credits

- Project, control layouts, testing, and public release: **Zeroable**
- Shared controller-hook foundation: **PS2 Controller Remapper by pelvicthrustman**
- Assembly/debugging assistance: **ChatGPT**

## Disclaimer

This is an unofficial community project.

No game files, ISOs, BIOS files, or Rockstar assets are included. The project is not affiliated with or endorsed by Rockstar Games, Take-Two Interactive, Sony, PCSX2, or ARMSX2.
