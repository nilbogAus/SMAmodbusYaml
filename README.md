# SMAmodbusYaml
Home Assistant Modbus yaml for SMA inverter

Putting this together from whatever sources I can find.

add the file modbus.yaml to config folder (where configuration.yaml is)

then add this into configuration.yaml to reference it:
> modbus: !include modbus.yaml

To get this working you may have to activate Madbus TCP for the inverter. I had to do this using SMA's Sunny Explorer software. 
