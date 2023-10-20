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

TODO
- Add hardware shopping list
- Improve the schematic.
- Replace the protoboard with a "proper" PCB.
- Install it all.
