# nanoleaf-canvas-NL29

Pictures from Inside of a Controller Panel of Nanoleaf Canvas NL29

I uploaded these pictures of the inside of a Controller Panel of Nanoleaf Canvas
type NL29.

https://nanoleaf.me/en-EU/products/nanoleaf-canvas/index.html?category=canvas&pack=smarter-kit&size=4

I did not find any pics on the internet, that's why I'm putting them here.

Why I opened it - it was the second time one of these controllers died, and now it's impossible
buy a replacement.
To preserve my 20 Panels I got desperate enough to try to fix it by myself.

First Cut:

Cut it open -- I started with dremeling the inner square in the middle of the backside.
I cut from the side --- and the plastic i very strong.
But to cut it out does not make sense. Yes, the main PCB the green one, gets accessible.
You could easily cut into the PCB i got lucky and only hit the ram chip slightly, and don't destroy
it. You don't need to do it the first time.

Second Cut:

The second cut is around all corners around 5mm in. That allows you to the PCB. But don't cut too deep
you could cut into the PCB and more easily on the 4 led leaf’s(see pictures). To get it disassembled you
need screwdrivers and knives and a lot of patience. But you will be able to get into it.

The PCB:

![alt text](https://github.com/mabels/nanoleaf-canvas-NL29/blob/main/pcb-to-frontside.jpg?raw=true)
![alt text](https://github.com/mabels/nanoleaf-canvas-NL29/blob/main/pcb-to-backside.jpg?raw=true)

Recovery

I found out. If I supply the hole PCB with the 42Volt, the central CPU starts and resets in the boot
phase. But If I only supply 3.3V behind(green wire) the 3.3Volt regulator the CPU starts without any problem
and runs stable for days. If you want to connect the panels, only connect the GND and Signal lane
from any edge. The slider with the 3 pins uses the slightly longer pin is GND and on the other outer side,
that's signal. Solder two cables on it and connect it to one of the edge connectors, on some, there is
also some text on the PCB needed to the connector.

Todo:

3d print a new housing and add a step-down converter from 42V to 3.3V. The touch sensors should work also,
there are texts on the PCB, and if you touch the PCB, something happens.


Wishes:

Find the root cause – I tried to understand the PCB design but didn’t understand it completely.
There are four channel mosfet drivers for the LEDs. But where are the constant power coils and the 5-volt power supply?
Any ideas that could help to fix the panel?

