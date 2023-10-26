# Robot Vacuum Garage door

ESP+Nema17 Stepper controlled.


Hardware based on: 
* https://hackaday.io/project/178993-space-saving-robot-vacuum-cleaner-garage, where I've added open and close limit switches.

5 minutes after I finally made my own simple code, which runs the motor a set amount of steps, I found this great inspiration from

* https://github.com/NeilDuToit92/ESPHome_Garage/blob/master/ESPHome.yml


## Functionality:
A limit switch will be mounted next to the robot while docked, signaling Docked/Leaving. Two limit switches are mounted on the gear, to stop it at upper and lower limit.
When the robot leaves, it will open straight away, and stay open until the robot docks, then waits 5 seconds until closing.
This gives me the DUMB mode, which I am happy with leaving in the house if we move out.
When combining this with Home Assistant, etc, a simple automation can close the door and reopen it when done vacuuming.

## Shopping list: (some in norway, decent priced, quick shipping)
- Nema 17 motor 42BYGH 1.5A: * https://www.aliexpress.com/item/32665922113.html
- L298N Motor Driver Controller Board: * https://www.aliexpress.com/item/1005004431531794.html
- A4988 Stepper Motor Driver: * https://artigereliv.no/produkt/elektronikk/mikrokontrollere/sensorer-og-tilbehor/a4988-stepper-motor-driver-med-heatsink
- ESP8266 NodeMCU V2: * https://artigereliv.no/produkt/elektronikk/mikrokontrollere/nodemcu/nodemcu-v2
- Prototype board (to be replaced): * https://artigereliv.no/produkt/elektronikk/mikrokontrollere/sensorer-og-tilbehor/7x9cm-dobbeltsidig-prototype-pcb
- HC-SR04 ultrasonic distance sensor: (not yet integrated) * https://www.fibel.no/product/hc-sr04-ultralyd-avstandssensor/
- 6.3V1000UF capacitors from Ali: * https://www.aliexpress.com/item/1005004524280300.html
- Mini Screw Terminal Blocks Connector, 2P and 4P: * https://www.aliexpress.com/item/1005001677869988.html
- Micro switches: * https://www.kjell.com/no/produkter/elektro-og-verktoy/elektronikk/electromechanics/strombryter-for-elektronikk/mikrobrytere/mikrobryter-1-pins-arm-p36031
- Cable shoes for the switches: * https://www.kjell.com/no/produkter/elektro-og-verktoy/biltilbehor/kabelsko/flatstifthylse-bla-10-pk.-48-mm-p67203

TODO
- Improve the schematic.
- Replace the protoboard with a "proper" PCB.
- Install it all.
- Replace switch for docked position with ultrasonic sensor.
- Maybe add lighting when open, I have spare led strip pieces available.
