# TEMPEST

_a 36-key split ergonomic keyboard_

![Maintenance](https://img.shields.io/maintenance/yes/2025) ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/thrly/tempest)

![TEMPEST keyboard](images/tempest-white.jpg)

## Design

- Five columns, three rows, three thumb keys
- Column stagger and splay on the pinky and ring columns
- Powered by nice!nano / pro micro microcontroller
- Designed for wireless use + battery
- Low profile v1 Choc switches + hotswap sockets
- Reversible PCB
- Uses some components (JST plug, power switch, reset) from the Typeractive Corne design
- Layout designed with [Ergogen](https://ergogen.ceoloide.com/) (see [config.yaml](./ergogen/config.yaml))
- PCB designed with [KiCad](https://www.kicad.org/) (v 9)
- Simple 3D-printable case

> [!NOTE]
> Despite the footprint for it, there is **no working display** on the current version (1.1). The display header pins are not connected correctly. See issue [#7](https://github.com/thrly/tempest/issues/7). You could probably hand-wire the holes to the microcontroller pins to fix though...

![TEMPEST keyboard](images/tempest.jpg)

## Firmware

TEMPEST was designed to be used with ZMK. [You can find the ZMK-config repository and a keymap here.](https://github.com/thrly/tempest-zmk)


## Build Guide

[Details on the build and case can be found here.](/build-guide.md)

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

<img src="https://github.com/thrly/tempest/blob/8db28c0fb310842e8c9dc7b95e4b05a694a6e47c/images/wave.png" width=50%>

<a href="https://ko-fi.com/C0C22GIO8" target="_blank"><img height="42" alt="Buy Me a Coffee at ko-fi.com" src="https://storage.ko-fi.com/cdn/kofi1.png?v=6"></a>
