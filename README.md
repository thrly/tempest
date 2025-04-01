# TEMPEST

_a 36-key split ergonomic wireless keyboard._

![Tempest Image](/tempest-pcb-v01.png)

> [!CAUTION]
> v.0.1 : Currently awaiting PCB to tests. There are some potential collisions on the board design which may cause issues.

## Design

- Five columns, three rows, three thumb keys.
- Column stagger and splay on the pinky and ring columns.
- Powered by nice!nano microcontroller / pro micro (and optional nice!view display).
- Low profile Choc switches.
- Reversible PCB.
- Uses some components from the Typeractive Corne design.
- Layout with Ergogen (see [config.yaml](./ergogen/config.yaml)).

## Using this repo

The ergogen files are contained in the ergogen/ folder.

Gerber files for PCB fabrication (i.e. JLPCB) can be found in /tempest-gerbers/ for ordering.

Latest KiCad PCB is included, but files can be generated using Ergogen.

> [!IMPORTANT]
> Some of the ergogen/ceoloide footprint files have been modified slightly from the [originals](https://github.com/ceoloide/ergogen-footprints).

## Influences

TEMPEST takes influence from:

- [Temper](https://github.com/raeedcho/temper) by raeedcho
- [Bad Temper](https://github.com/essFitt/Bad-Temper/tree/main) by essFitt
- [TOTEM](https://github.com/GEIGEIGEIST/TOTEM) by GEIST
- [FORAGER](https://github.com/carrefinho/forager) by carrefinho
- also Chocofi, Sweep, Corne
