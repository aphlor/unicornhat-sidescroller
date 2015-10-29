A sidescroller for the Unicorn HAT
----------------------------------

This is a simple sidescroller demo for the Unicorn HAT by the lovely [Pimoroni](https://shop.pimoroni.com/). It uses the Sinclair ZX Spectrum character bitmap (yoinked from a 48KB ROM at ```$3D00``` to ```$3FFF```).

It uses a virtual framebuffer of 24x8 pixels and draws the area from 9-16 on the X axis to the Unicorn HAT (no consideration for colours per se). 1-8 and 17-24 are kept for offscreen drawing, as I intend to use some left/right swipe effects in future. New letters are drawn into the 17-24 area and left shifted into the visual area, then left shifted out to the offscreen area left of the visual display. By default, ```unicornhat.rotation``` is set to 180 so that the display is the right way up when the "UNICORN HAT" logo is to the left of the LED-matrix and the chips on the right side.

There's no license for the code, just pick it up and use it. It would be nice if you retained a notice stating I wrote it, but this is something trivial I wrote for python practice.

Requires the ```unicornhat``` library for Python. Install with:

    pip install unicornhat

Rob Andrews ([rob@aphlor.org](mailto:rob@aphlor.org))
