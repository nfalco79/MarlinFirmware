This repository represent an example of Marlin 2.x configuration for a Flyingbear Ghost 5.

# Hardware configuration
This configuration has been designed using the following mods:
* Robin Nano V3.1
* 4x TMC2226 (it's the same for 2209)
* UART mode
* printer head dual fan (https://www.thingiverse.com/thing:6162681)
* direct drive LDO Orbiter V2.0 (https://www.thingiverse.com/thing:6175743)
* 3D Touch V3.2 Pro (non BLTouch) -- not yet ready

# Wiring
The Ghost 5 originally controls the 3010 (heater fan) together with the controller 6010 fan that blows on the mosfet and TMC driver. Marlin 2.x has an indipendent logic on how to control this particular fan than I had change controller 6010 fan connection. I removed the controller 6010 fan from Base PCB (red connection) connecting it into the motherboard FAN2 connector (PB1)