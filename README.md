# CHEP Ender 3 Bed Level Code

This repository contains the original, and modified versions of the CHEP bed level gcode for the Ender 3 3D printer.

## Variations
Some modified versions of the code fix specific problems.

### Slow Execution
Because the original gcode does not specify a travel speed, the Ender 3 will default to whatever speed was previously specified (probably from a previous gcode.) This may cause the printer to move improperly slow during execution.<br><br>
The modified gcode is [here](CHEP_Ender_3_bed_level_fast.gcode).

### Heat-Sensitive Bed
If you are using the (cheap) stock bed surface that ships with the printer, the material is susceptable to slight warping during warming that can affect your bed level calibration. In order to calibrate with proper bed temperature, we've modified the code to run with the bed at 45C.<br><br>
The temperature modified gcode is [here](CHEP_Ender_3_bed_level_hotbed.gcode).

### Hot and Fast Version
Gcode that combines the two previous modifications is  [here](CHEP_Ender_3_bed_level_hot_fast.gcode).
