# TEMPEST

_a 36-key split ergonomic keyboard_

![TEMPEST keyboard](images/tempest.jpg)

## Design

- Five columns, three rows, three thumb keys.
- Column stagger and splay on the pinky and ring columns.
- Powered by nice!nano / pro micro microcontroller.
- Designed for wireless use + battery.
- Low profile v1 Choc switches.
- Reversible PCB.
- Uses some components (JST plug, power switch, reset) from the Typeractive Corne design.
- Layout designed with [Ergogen](https://ergogen.ceoloide.com/) (see [config.yaml](./ergogen/config.yaml)).
- PCB designed with [KiCad](https://www.kicad.org/) (v 9).

> [!NOTE]
> Despite the footprint for it, there is no display on the current version (1.1). The display header pins are not connected correctly. See issue [#7](https://github.com/thrly/tempest/issues/7). You could probably hand-wire the holes to the microcontroller to fix though.

![TEMPEST keyboard](images/tempest-2.jpg)

## Bill of Materials (BOM)

| Quantity | Part                                                                             | Notes                                                                                                            |
| -------- | -------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 2        | TEMPEST PCBs (reversible) from [gerbers .zip file](/tempest%201-1%20gerbers.zip) | order from [JLCPCB](https://jlcpcb.com/) or similar                                                              |
| 2        | nice!nano                                                                        | or other Pro Micro controller (see note about spring headers)                                                    |
| 2        | [LiPo battery](https://typeractive.xyz/products/lithium-battery-110mah)          | see nice!nano documentation for reccomendations, with 2-pin JST plug                                             |
| 2        | 2-pin JST plug                                                                   | 2.0mm pin spacing, black are annoyingly harder to find than white                                                |
| 2        | Miniature Alps SPDT switch (7 pin)                                               | Power on/off                                                                                                     |
| 2        | Miniature momentary button (side mount)                                          | Reset                                                                                                            |
| 4        | 12-pin headers (5mm height)                                                      | MAC8 XB-3-5 from [Typeractive](https://typeractive.xyz/products/no-solder-spring-headers?variant=47196312502503) |
| 36       | 1N4148W SMD diodes                                                               |
| 36       | Kailh choc switches (v1)                                                         |
| 36       | Kailh choc hotswap sockets                                                       |
| 36       | Choc keycaps                                                                     |

### Optional: Display

| Quantity | Part                      | Notes                                                                                                            |
| -------- | ------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 2        | nice!view display         |
| 2        | 5-pin header (7mm height) | MAC8 XB-3-7 from [Typeractive](https://typeractive.xyz/products/no-solder-spring-headers?variant=47196312535271) |

### Optional: Case

| Quantity | Part                 | Notes                                                         |
| -------- | -------------------- | ------------------------------------------------------------- |
| 2        | case .stl            | Mirror for right side; PLA; 0.12 mm layer height; >50% infill |
| 2        | key plate STL        | Mirror for right side; PLA; 0.12 mm layer height; >50% infill |
| 2        | stick-on rubber feet | or tenting legs from aliexpress                               |
| 10       | M2 standoffs         | height: 4 mm                                                  |
| 20       | M2 bolts             | height: 4 mm                                                  |

## Build guide

The build for the TEMPEST is simple and broadly follows the same steps outlined in [Typeractive's Corne build](https://docs.typeractive.xyz/build-guides/corne-wireless). Theirs is well-written and documented, so read that for now.

Some important notes, however:

> [!IMPORTANT]
> Microcontroller should be placed **facing DOWN** (i.e. facing the board).

> [!NOTE]
> The microcontroller pin holes on the board have been narrowed (to 0.85mm) to enable the use of no-solder spring headers (MAC8 XB-3-5, as found from [Typeractive](https://typeractive.xyz/products/no-solder-spring-headers?variant=47196312502503)). These headers will fit the nice!nano, but other Pro Micro controllers may have pin holes that are too wide for these spring headers.

> [!IMPORTANT]
> Ensure that you solder the jumper pads for microcontroller, display, and battery plug closed **on the BACK side of the board** (i.e. the same side you're soldering your hotswap switch plugs and diodes).

## Other Information

### Ergogen

The ergogen files are contained in the ergogen/ folder. See [here](https://docs.ergogen.xyz/usage) for guidance on building from ergogen.

Ergogen was used mainly as a layout tool for the keys and wiring nets. Some of the footprints for things like MCU, switches, plugs, etc. may have been manually tweaked in the KiCad PCB editor, so don't expect the Ergogen render to be completely the same as the final PCB version.

> [!NOTE]
> Some of the ergogen/ceoloide footprint files used here have been modified slightly from the [originals](https://github.com/ceoloide/ergogen-footprints). Run locally, not on the ergogen web app.

### Ordering the PCB

Use the Gerber .zip file for PCB fabrication (i.e. JLPCB, PCBWay).

#### Suggested fabrication options

- FR-4 PCB, 1.6 mm
- LeadFree HASL

Latest KiCad PCB is included, or files can be generated using Ergogen.

![TEMPEST PCB Image](images/tempest-pcb-v1-1.png)

> Tempest PCB v1.1

### Case

Files for a simple 3D-printed case included. Pictured case was printed in Matte PLA, with 0.12 layer height and 100% infill.

> [!TIP]
> Alternatively, use the back-plate and top-plate exports from ergogen to order FR-4 plates along with your PCB. You can also use the DXF exports to design your own 3D-printed case/plates easily.

## Influences

TEMPEST is inspired by and takes influence from:

- [Temper](https://github.com/raeedcho/temper) by raeedcho
- [Bad Temper](https://github.com/essFitt/Bad-Temper/tree/main) by essFitt
- [TOTEM](https://github.com/GEIGEIGEIST/TOTEM) by GEIST
- [FORAGER](https://github.com/carrefinho/forager) by carrefinho
- [Corne](https://github.com/foostan/crkbd) by foostan (and the [Typeractive](https://typeractive.xyz/) version)
- also [Chocofi](https://github.com/pashutk/chocofi), [Sweep](https://github.com/davidphilipbarr/Sweep), and others.

## Thanks

If you build Tempest, I'd _love_ to hear how you get on with it. Please say hello via [thrly.com](https://www.thrly.com) or [instagram](https://www.instagram.com/thrly.xy/).

![Tempest Wave](/images/wave.png)

<a href="https://ko-fi.com/C0C22GIO8" target="_blank"><img height="42" alt="Buy Me a Coffee at ko-fi.com" src="https://storage.ko-fi.com/cdn/kofi1.png?v=6"></a>
