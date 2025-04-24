# ESPHome-FoxESS-modbus

This repo is a store for ESPHome modbus configurations for various devices.

It was started to store the configuration for my FoxESS H1-5.0-E inverter.

I use the circuit depicted here to connect to my inverter with ESPHome: https://github.com/assembly12/Foxess-T-series-ESPHome-Home-Assistant/wiki/Hardware-setup Though I have switched the temperature sensor module from an AHT10 to a bme280 which seems much better at functioning and uses the same connector on the circuit board.

When I first started I had a 4 metre ethernet cable between the ESP32 and the inverter, this worked perfectly. However, after I configured the modbus settings in a way that the inverter did not like I got a lot of CRC errors and so cut the cable. This made no difference and it was only after making changes to what registers I was reading and when I was reading them that the CRC errors all went away.

Please note that this was all put together with information gleaned from various places and may or may not be entirely correct or safe to use. I have been using it for about a year without any issues so hopefully it is all good.
