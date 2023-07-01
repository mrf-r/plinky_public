# plinky

an 8 voice touch synth - https://plinkysynth.com

I apologise, its been so long since I looked at this, I am releasing a snapshot of what I had on my harddrive after a couple of years of barely being touched. while I am not actively developing plinky, I hope that by open sourcing it I can stimulate the wonderful community who collaborate on the plinky discord. I also hope to help iterate on some of the more obvious bugs, both hardware and software. 

If you are interested in plinky, please feel free to join our discord community. More information at https://plinkysynth.com


LICENSE
==
Logos & Design
---
The plinky logo and the design of the front panel design and all other graphic elements (both in code and in the documentation and hardware design) are CC BY-SA 4.0. Full text available at https://creativecommons.org/licenses/by-sa/4.0/

Third party elements
--
This repository is still somewhat disorganised, and includes some third party code. This includes (but may not be limited to), code generated by the [STM32 Cube IDE](https://www.st.com/en/development-tools/stm32cubeide.html) default project generator; [tinyusb](https://github.com/hathach/tinyusb); [dear imgui](https://github.com/ocornut/imgui) (which in turn uses [gl3w](https://github.com/skaslev/gl3w) and [glfw](https://github.com/glfw/glfw)), [portaudio](https://github.com/PortAudio/portaudio). These projects remain under their original licenses.

Software
--
The rest of the software of plinky is licensed under the MIT License https://opensource.org/licenses/MIT

Hardware
--
The hardware design is licensed under the permissive CERN open hardware license, CERN-OHL-P v2. Full text is available at https://cern.ch/cern-ohl.

Derived works & Commercial Products
--
If you make something with this, I'd love to know! Let me know on [twitter](https://twitter.com/mmalex) 

If you sell or distribute something based on this repo, please make it clear that it is distinct from the original plinky design, and abide by the licenses above.
My main concern is that the small plinky community, who are focused on discussion of creative audio hardware in general, become burdened with support or other work for a product they didn't actively get involved with. We don't want that! So please be respectful.

Building and stuff
==
you need [STM32 cube ide](https://www.st.com/en/development-tools/stm32cubeide.html), its basically the default project so most of the code is in `sw/Core/Src`, most of the rest of the `sw/` folder is just the usual auto generated boilerplate mess.

It would be a useful project to update the firmware to build with a more minimal setup; the only significant middleware used relates to USB; while I lean on the STM default project a little, I imagine that the peripheral code could be modified fairly easily.

it should also compile as an emulator for mac and windows, using portaudio and dear imgui. it also compiles for wasm, somehow... I imagine that following the path of the WASM emulator, it would be relatively easy to port plinky to software plugin type platforms.

there is also a bootloader project... I forget exactly how it relates to the final build process. Consider that a TODO to document :)

the hardware is mostly in the `hw/` folder, but I was new to kicad so I am not sure if all the library stuff is in the right place.

if there is something missing or something in there that you think shouldn't be in there, let me know and I can sort it out


Will there still be kit plinkys? eg from Thonk?
==
I havent spoken to steve about it, but I don't see why not!

Thanks!
==
Many thanks to the plinky community, who have helped plinky evolve and kept the dream alive over a few years. 

Thanks to Steve from https://thonk.co.uk who encouraged plinky into existence and helped produce the kits; to Kay from https://leipzigwest.org/ for tireless hardware help, encouragment and pre-made plinkys! To Stijn from http://www2.thisisnotrocketscience.nl/ for support, hardware help, and the impetus to opensource this.

Cheers all! 

-- [mmalex](https://twitter.com/mmalex)

