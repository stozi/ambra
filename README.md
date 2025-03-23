# ambra
A [Kalmar](https://github.com/aroum/kalmar)/[A. Dux](https://github.com/tapioki/cephalopoda/tree/main/Architeuthis%20dux)-based 34-key split ortho keyboard

## Changes from Kalmar

- thumb keys mount at 90° with pogo pins and 3D-printed magnet brackets
- JST PH battery connector
- ground plane for some ESD protection, new pinout

Thumb keys are mounted at 90° magnetically on 3D printed brackets. Alternatively, you can run a 9mm or longer M2.5 bolt through both brackets if you don't need fold-down packability.


Better put a non-conductive coating over the JST connector's mount points and reenforce the pogo-pin units with a little epoxy putty just to relieve the pins of any leverage. In testing.

![Alt text](https://github.com/stozi/ambra/blob/main/ambra.png?raw=true)
![Alt text](https://github.com/stozi/ambra/blob/main/ambra-back.png?raw=true)
![Alt text](https://github.com/stozi/ambra/blob/main/brackets.png?raw=true)

## BOM

Item     | Qty   | Notes 
----------|-------|-------
[SuperMini NRF52840 MCU](https://www.aliexpress.com/item/1005008099333183.html) | 2 | inc. sockets
[Kailh Choc V1](https://aliexpress.ru/item/32959996455.html) | 34 | key switches
[Keycaps](https://aliexpress.ru/item/33026798318.html) | 34 | 1U
[Magnets](https://www.aliexpress.com/item/1005006788058856.html) | 2 | D6×3mm annular cylinder
[RTLECS MG03254 3-pin](https://sl.aliexpress.ru/p?key=pW35Gta) | 2 pairs | pogo-pin connectors, straight + 90°
[MSK-12CO2](https://aliexpress.ru/item/1005001398386692.html) | 2 | power switch
[SMD button 3×4×2](https://aliexpress.ru/item/1005003812819985.html) | 2 | reset switch
[301230 li-po](https://aliexpress.ru/item/32732458079.html) | 2 | battery
[JST PH right-angle 2-pin](https://www.aliexpress.com/item/1005008131930144.html) | 2 | battery connector
[JST wire](https://www.aliexpress.com/item/1005001649158434.html) | 2 | solder & shrink tube to battery wires, no crimping needed
[M3 bolts, 3mm](https://www.aliexpress.com/item/1005006662972635.html) | 2 | flathead, couples with magnet
M3 nuts, 1.8mm (ISO 4035) | 2 |
M2.5 bolts, 4mm | 2 | tapered head, holds magnet
M2.5 nuts, ~1.35mm (ISO 4035)| 2 |
M2 bolts, 3.5mm | 4 | for board bracket
M2 bolts, 7.5mm | 2 | for thumb key bracket
M2 nuts, ~1.1mm (ISO 4035) | 6 | 

The pinout has been optimized so, until this gets accepted to ZMK, for QWERTY, set up your ZMK keymap for A. Dux as follows:

```
     X E D G T  Y H K I .
lthumb S V C W  O , M L rthumb
rthumb Z Q A F  J ; P ? lthumb
           R B  N U
```
