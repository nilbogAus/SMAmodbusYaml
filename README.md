# SMAmodbusYaml
Home Assistant Modbus yaml for SMA inverter

Putting this together from whatever sources I can find.

To get this working you may have to activate Modbus TCP for the inverter. I had to do this using SMA's Sunny Explorer software. 

NB: At night some SMA inverters go into low power mode when not generating and some Modbus registers become nonsensical. It is probably best to try to get this working the first time in daylight.

# Setup

add the file modbus.yaml to config folder (where configuration.yaml is)

then add this into configuration.yaml to reference it:
> modbus: !include modbus.yaml <br>
> homeassistant: <br>
>&nbsp; packages: <br>
>&nbsp;&nbsp; modbustemplate: !include modbus_template.yaml  

