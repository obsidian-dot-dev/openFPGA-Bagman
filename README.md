# openFPGA-Bagman

Bagman-compatible openFPGA core for Analogue Pocket. Ported directly from the 
[MiSTer core](https://github.com/MiSTer-devel/Arcade-Bagman_MiSTer)
by [Dar](https://darfpga.blogspot.com/) and ported by Sorgelig. 

## Notes

Supports multiple games:
-  Bagman, Super Bagman, Botanic, Pickin', and Squash

Input and Interact menus supporting dip switches and control configurations are provided for each game.

Games can be paused by entering the OSD.

## Known Limitations

* High Score saving unimplemented.

## License

Source code for the openFPGA integration of this core is provided under the
terms of GPLv3. Please see the component repositories for licensing details
of individual modules. 

## Attribution

All credits for the Bagman-compatible FPGA core are due the original authors
and contributors, without which this port would not have been possible. Credits
for the original work (taken from the original 
[core documentation](https://github.com/MiSTer-devel/Arcade-Bagman_MiSTer?tab=readme-ov-file))
are as follows:

```
---------------------------------------------------------------------------------
-- 
-- Arcade: Bagman port to MiSTer by Sorgelig
-- 24 October 2017
-- 
---------------------------------------------------------------------------------
-- Bagman (STERN) FPGA - DAR - 2014
-- http://darfpga.blogspot.fr
---------------------------------------------------------------------------------
-- T80/T80se - Version : 0247
-----------------------------
-- Z80 compatible microprocessor core
-- Copyright (c) 2001-2002 Daniel Wallner (jesus@opencores.org)
---------------------------------------------------------------------------------
```

## Installation

Copy the contents of the "dist" folder to the root of the SD card, along with the converted ROM file as described below.

### ROM Instructions

ROM files are *not included*, you must use [mra-tools-c](https://github.com/sebdel/mra-tools-c/)
along with the provided `*.mra` files to convert a MAME-compatible romset to singular
`*.rom` file compatible with this core.  This ROM file should be placed under
`/Assets/bagman/obsidian.Bagman`.
