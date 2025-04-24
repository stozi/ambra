# Ambra
A [Kalmar](https://github.com/aroum/kalmar)/[A. Dux](https://github.com/tapioki/cephalopoda/tree/main/Architeuthis%20dux)-based 34-key split ortho keyboard. [ZMK shield](https://github.com/stozi/zmk-keyboard-ambra)

### Included from Kalmar

- power switch
- reset button
- solder jumpers to keep the MCU upright
- perforations on the tab for the connector between the right & left boards

### Changes from Kalmar

- thumb keys mount at 90° with pogo pins and 3D-printed magnet brackets
- besides Kailh Choc, support for Gateron KS-33, both hotswap only
- JST PH battery connector
- Switched the TRRS jack to the same pogo pin connector used for the thumb keys to prevent shorting
- ground plane for some ESD protection, new pinout

Thumb keys are mounted at 90° magnetically on 3D printed brackets. Alternatively, you can run a 9mm or longer M2.5 bolt through both brackets if you don't need fold-down packability.

Better epoxy a piece of plastic to overhang the connectors on both ends of your daughter-board wire to prevent connecting it upside-down on either side. Also, put a non-conductive coating over the JST connector's mount points and reenforce the pogo-pin units with a smidgen of epoxy putty just to relieve the pins of any leverage. In testing.

![Alt text](https://github.com/stozi/ambra/blob/main/ambra.png?raw=true)
![Alt text](https://github.com/stozi/ambra/blob/main/ambra-back.png?raw=true)
![Alt text](https://github.com/stozi/ambra/blob/main/brackets.png?raw=true)

## BOM

Item     | Qty   | Notes 
----------|-------|-------
[SuperMini NRF52840 MCU](https://www.aliexpress.com/item/1005008099333183.html) | 2 | inc. sockets
[Kailh Choc V1](https://a.aliexpress.com/_EGNqHgc) | 34 | key switches
[Keycaps](https://a.aliexpress.com/_EGNqLfE) | 34 | 1U
[Magnets](https://www.aliexpress.com/item/1005006788058856.html) | 2 | D6×3mm annular cylinder
[RTLECS MG03254 3-pin](https://a.aliexpress.com/_Ev5QIZa) | 4 90°, 2 straight, 2 wires | pogo-pin connectors, solder and shrink-tube the two wires together 
[MSK-12CO2](https://aliexpress.ru/item/1005001398386692.html) | 2 | power switch
[SMD button 3×4×2](https://aliexpress.ru/item/1005003812819985.html) | 2 | reset switch
[301230 li-po](https://aliexpress.ru/item/32732458079.html) | 2 | battery
[JST PH right-angle 2-pin](https://www.aliexpress.com/item/1005008131930144.html) | 2 | battery connector
[JST wire](https://www.aliexpress.com/item/1005001649158434.html) | 2 | solder & shrink tube to battery wires, no crimping needed
[M3 machine screws, 3mm](https://www.aliexpress.com/item/1005006662972635.html) | 2 | flathead, couples with magnet
[M3 thin hex nuts](https://a.aliexpress.com/_EvCkuwM) | 2 |
[M2 tapered head machine screws, 7mm](https://a.aliexpress.com/_EzeQ9lA) | 2 | holds magnet
[M2 flat head machine screws](https://www.aliexpress.com/item/1005006662972635.html) | 4×5mm, 2×8mm | for brackets
[M2 thin hex nuts](https://a.aliexpress.com/_EvCkuwM) | 8 |
[Choc hotswap sockets](https://a.aliexpress.com/_Eu2JK5E) | 34 |
