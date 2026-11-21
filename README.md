# Nivel — robotic arm 5+1

Nivel is a robotic arm with five joints and a gripper, for personal and scientific use. It is
[Makedona](https://makedona.com)'s first open source and open hardware project.

**Status:** in development. The models, STEP files, bill of materials, wiring, build instructions
and firmware will be published here in January 2027. Until then this repository holds the
announcement below.

## Announcement

Makedona is to publish its first open source and open hardware project in January: Nivel, a
robotic arm 5+1 for personal and scientific use.

We built it to validate how accurate and mature Makedona's integrated design process is for
industrial-grade work. And because everyone should have their own robotic arm.

### The arm

- Five joints and a gripper. Reach 110–348 mm on the work plane, the base turning ±150°
  (model: reach analysis).
- NEMA 17 stepper motors through belts and planetary gearboxes. A BigTreeTech Octopus running
  Marlin 2.1 moves the joints; an ESP32 host serves its controls over WLAN and turns a drawing's
  G-code into joint moves.
- 16 printed parts in PETG, about 23.5 hours and 830 g of filament on a Prusa CORE One L
  (model: virtual print).
- Holds about 500 g in its gripper (model estimate; the friction is assumed, and the grip will be
  measured on the built arm).

The figures come from the Makedona model of the arm and its analyses. They will be checked on
the built arm, and this page will say how they compared.

### How the film was made

Nothing in the film is animated by hand. The arm runs the same joint G-code its Marlin
controller will run, planned at the controller's limits and checked against the arm's dynamics.
Every frame is rendered from the Makedona model: its geometry, its motion and its wiring, with
the firmware for both the ESP32 host and the Octopus controller built and ready to flash into
real chips.

Stay tuned for project updates.

## Licences

When the files are published:

| | Licence |
|---|---|
| Hardware: models, STEP files, BOM, wiring | [CERN-OHL-S-2.0](https://ohwr.org/cern_ohl_s_v2.txt) |
| Software: ESP32 host, Marlin configuration | [GPL-3.0-or-later](https://www.gnu.org/licenses/gpl-3.0.txt) |
| Instructions and images | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |

## Contact

Jan Landén, jan.landen@alpha-advisors.fi
