# Smart Module 1
### By Tinker Valley

## About
This configuration includes the following:

### Garage Door
I have a basic Mastercraft garage door opener from Canadian Tire. The door can be controlled by simply shorting the two wires for the wall panel together. I have a relay connected to these two wires to control opening/closing. 
I only have one contact sensor for the garage door. The sensor is only able to see whether the garage door is fully closed or not.
The configuration contains two binary_sensor entities that both receive input from the same contact sensor, but one is set to inverted. That way, when the closed sensor is on (door is closed), the open sensor will display off (because the door is not open). 
The cover entity uses these two sensors to display the door open/close status in Home Assistant.

### Front Door Contact Sensor
This one is a simple contact sensor in the frame of my door. I can see when the door is open and closed.

### Doorbell
My house did not have a doorbell wired when I moved in, so this is another simple binary_sensor that detects the button press. I have these setup with an automation in Home Assistant that plays a doorbell sound on all my Nest minis.

### HVAC Fan
I sometimes like to be able to turn on my furnace fan to recirculate air in the house, but my Ecobee makes this more complicated than it should be. I have this connected to a relay that's connected to the FAN wire on ny furnace board.
