# ESPHome-AUXswitcher
Built a AUX switcher for my desktop to switch between the headphones and speakers automatically through Home Asisstant using ESPHome.

The basic idea is that a 2-channel relay board switches between the two AUX ports by connecting the incoming audio signal to the COM of the relays, and then connecting one of the outgoing signals to NC, while the other outgoing signal is connected to NO. By turning both the relays on or off, the signal will then switch between the outgoing signals.

I also built a spool attached to a stepper motor that could pull the headphone cable in from under the table. The idea was that the cable should be pulled in before our robotic vacuum cleaner started cleaning to avoid her being caught up in the cable. This feature turned out to be a gimmick and not very practical. I ended up just finding the perfect length for the headphone cable, so that it reached my head perfectly fine, and don't go onto the floor when it's on its hook. 

The box are prepared for M3 screw inserts that can be melted into place using a soldering iron. I also glued a piece of rubber band to where the lip of the lid will be to make the lid be a more snug fit, while still have the possibility of being compressable so that the lid can be removed easily if wanted.
![box_preparations](https://github.com/petrepa/ESPHome-AUXswitcher/blob/master/Photos/box_preperations.jpg)
Every component can then be screwed to its place in the box. 
From left to right we have: voltage regulator (used to step down 12V to 5V for the components needing this voltage), stepper motor driver (which is not really needed, so this can be dropped), a perfboard for the NODEMCU-32S so that the MCU can be switched easily (also makes it easier to solder on the underside of the perfboard) and lastely the 2-channel relay board controlling where the audio signal goes.
![box_components](https://github.com/petrepa/ESPHome-AUXswitcher/blob/master/Photos/box_components.jpg)
Fully assembled box with all its connections. I forgot to design a opening for the stepper motor wires, so I just used a file to make a notch in the space between the box and the lid. Since I wouldn't recommend using a stepper motor at all, this won't be a problem.
![assembled_box](https://github.com/petrepa/ESPHome-AUXswitcher/blob/master/Photos/assembled_box.jpg)
The headset holder is meant to be placed under your desk onto a drawer or something. It uses a large push switch.
![assembled_headset_holder](https://github.com/petrepa/ESPHome-AUXswitcher/blob/master/Photos/assembeld_headset_holder.jpg)
The headset fits nicely and can easily be plugged into the box using banana plugs. 
![headset_holder](https://github.com/petrepa/ESPHome-AUXswitcher/blob/master/Photos/headsett_holder.jpg)
