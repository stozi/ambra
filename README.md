# ambra
A [Kalmar](https://github.com/aroum/kalmar)/[A. Dux](https://github.com/tapioki/cephalopoda/tree/main/Architeuthis%20dux)-based 34-key split ortho keyboard

Thumb keys are mounted at 90° with a [RTLECS MG03254](https://sl.aliexpress.ru/p?key=pW35Gta) magnet pogo-pin unit and held in place with the 3D printable brackets and a D6x3mm cylindrical neodymium magnet on a 4mm M2.5 tapered-head bolt. The magnet couples with a steel 3mm M3 bolt with an unbeveled flathead (D6mm) in the other bracket. The brackets are held on with three M2 bolts, one about 7.5mm, two 3.5mm. Alternatively, you can run a 9mm or longer M2.5 bolt through both brackets if you don't need fold-down packability.

2mm-pitch JST PH connector added for the battery, you can get a male end pre-crimped to wires and easily solder the wires to your battery wires. I added a ground plane for ESD protection. This involved optimizing the pinout. So, until this gets accepted to ZMK, for QWERTY, set up your ZMK keymap for A. Dux as follows:

```
     X E D G T  Y H K I .
lthumb S V C W  O , M L rthumb
rthumb Z Q A F  J ; P ? lthumb
           R B  N U
```

Better put a non-conductive coating over the JST connector's mount points and reenforce the pogo-pin units with a little epoxy putty. In testing.

![Alt text](https://github.com/stozi/ambra/blob/main/ambra.png?raw=true)
![Alt text](https://github.com/stozi/ambra/blob/main/ambra-back.png?raw=true)
![Alt text](https://github.com/stozi/ambra/blob/main/brackets.png?raw=true)
