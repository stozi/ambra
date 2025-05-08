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
- Switched the TRRS jack to the same pogo pin connector used for the thumb keys to prevent shorting (VCC/power is the middle pin so mounting one side backwards won't cause damage)
- ground plane for some ESD protection, new pinout

If you don't need fold-down packability or can't get the magnets, you can run a 9mm or longer M2 bolt through both brackets. However, any fall will then be more likely to cause damage.

Consider putting a non-conductive coating between the JST connector's mount points and the battery. Remove remnants of perforations on the thumb-key board before attaching the bracket.

Passed basic testing.

![Alt text](https://github.com/stozi/ambra/blob/main/prototype.jpg?raw=true)
![Alt text](https://github.com/stozi/ambra/blob/main/brackets.jpg?raw=true)

## BOM

Item     | Qty   | Notes 
----------|-------|-------
[SuperMini NRF52840 MCU](https://www.aliexpress.com/item/1005008099333183.html) | 2 | inc. sockets. Alternatively, ProMicro/Elite-C for a wired build
[Kailh Choc V1](https://a.aliexpress.com/_EGNqHgc) | 34 | key switches. Alternatively, [Gateron KS-33](https://a.aliexpress.com/_EuUuYVU)
[Choc hotswap sockets](https://a.aliexpress.com/_Eu2JK5E) | 34 | Alternatively, [Gateron KS-33 hotswap sockets](https://a.aliexpress.com/_EGlN42e)
[Keycaps](https://a.aliexpress.com/_EGNqLfE) | 34 | 1U. If using KS-33 switches, STL files are provided to print your own 'MX stem, Choc-1U-spaced' caps
[Magnets](https://a.aliexpress.com/_EGMQ442) | 2 | D6×3mm annular cylinder
[RTLECS MG03254 3-pin](https://a.aliexpress.com/_Ev5QIZa) | 2 straight m, 2 90° f | magnetic pogo-pin connectors
[MSK-12CO2](https://aliexpress.ru/item/1005001398386692.html) | 2 | power switch
[SMD button 3×4×2](https://aliexpress.ru/item/1005003812819985.html) | 2 | reset switch
[301230 li-po](https://aliexpress.ru/item/32732458079.html) | 2 | battery
[JST PH right-angle 2-pin](https://www.aliexpress.com/item/1005008131930144.html) | 2 | battery connector
[JST wire](https://www.aliexpress.com/item/1005001649158434.html) | 2 | solder & shrink tube to battery wires, no crimping needed, or [battery already with connector](https://a.aliexpress.com/_EJkhjGm) 
[M3 machine screws, 3mm](https://www.aliexpress.com/item/1005006662972635.html) | 2 | flathead, couples with magnet
[M3 thin hex nuts](https://a.aliexpress.com/_EvCkuwM) | 2 |
[M2 tapered head machine screws, 7mm](https://a.aliexpress.com/_EzeQ9lA) | 2 | holds magnet
[M2 flat head machine screws, 8mm](https://www.aliexpress.com/item/1005006662972635.html) | 6 | for brackets
[M2 thin hex nuts](https://a.aliexpress.com/_EvCkuwM) | 8 |
OPTIONAL: [RTLECS MG03254 cable](https://www.aliexpress.com/item/1005007988032729.html) and extra RTLECS 90° female connectors as listed above | 2 of each | For a wired build: cut, solder and shrink-tube the two wires together
