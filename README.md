# TEMPEST

_a 36-key split ergonomic wireless keyboard._

![TEMPEST Image](/tempest-pcb-v01.png)

> [!CAUTION]
> v.0.1 : Error in circuit layout: ring, middle, index keys do NOT work. DO NOT BUILD THIS VERSION.

## Design

- Five columns, three rows, three thumb keys.
- Column stagger and splay on the pinky and ring columns.
- Powered by nice!nano microcontroller / pro micro (and optional nice!view display).
- Designed for wireless use / battery.
- Low profile v1 Choc switches.
- Reversible PCB.
- Uses some components (JST plug, power switch, reset) from the Typeractive Corne design.
- Layout with Ergogen (see [config.yaml](./ergogen/config.yaml)).

## Build guide

The build for the TEMPEST is simple, and broadly follows the same steps outlined in [Typeractive's Corne build](https://docs.typeractive.xyz/build-guides/corne-wireless). Theirs is well-written and documented, so read that for now.

## Using this repo

### Ergogen / design

The ergogen files are contained in the ergogen/ folder. See [here](https://docs.ergogen.xyz/usage) for guidance on building from ergogen.

> [!IMPORTANT]
> Some of the ergogen/ceoloide footprint files have been modified slightly from the [originals](https://github.com/ceoloide/ergogen-footprints).

### PCB
Gerber and drill files for PCB fabrication (i.e. JLPCB) can be found in /tempest-gerbers/ for ordering.

Latest KiCad PCB is included, but files can be generated using Ergogen.

### Case
Plates and case 3D printed (STLs included). Printed in Matte PLA, with 0.12 layer height and 100% infill.
Alternatively, you can use the back-plate and top-plate exports from ergogen to order FR-4 plates along with your PCB.

## Influences

TEMPEST takes influence from:

- [Temper](https://github.com/raeedcho/temper) by raeedcho
- [Bad Temper](https://github.com/essFitt/Bad-Temper/tree/main) by essFitt
- [TOTEM](https://github.com/GEIGEIGEIST/TOTEM) by GEIST
- [FORAGER](https://github.com/carrefinho/forager) by carrefinho
- [Corne](https://github.com/foostan/crkbd) by foostan (and the [Typeractive](https://typeractive.xyz/) version)
- also Chocofi, Sweep, etc.