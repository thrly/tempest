# Change list

## V2 major changes

The shape of the pcb has changed slightly in v2:

- optional snap-off pcb for extra key (a la TOTEM) to make 36/38-key layouts
- fixed display connections (currently uses non-standard display pins on the nice!nano, so see the [ZMK config](https://github.com/thrly/tempest-zmk) for pin details)
- slightly less aggressive middle-column stagger (friendlier for `hjkl` on vim!)
- fractionally less offset on thumb-cluster for comfort
- improved spacing on mcu to fix collision with inner key column on the top plate
