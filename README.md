# USB-Ravenna-AES-67-Audio-Interface
A 2 in - 8 out Audio interface based on a CH32H417. With Mic/Line/Instrument input, and Headphone + 4 x symmetric or 4 x AES/EBU output.

The core of this audio interface is a CH32H417. 
It features 2 RISC-V cores running at 400 and 144 MHZ.
USB 3.2 Gen1 controller and transceiver, 
100M Ethernet MAC and PHY,
high-speed isolated transceiver, 
Type-C/PD controller and PHY.
So everything needed for multichannel Audio over Ethernet.

But it would get to its limits with all the output features i wanted.
So it has a RP2354 on its board to manage the audio streams.
The CH32H417 handles usb + ethernet communication and also all the gpio + GUI.
The RP2354 handles AES/EBU signal and the ADC + DAC.
