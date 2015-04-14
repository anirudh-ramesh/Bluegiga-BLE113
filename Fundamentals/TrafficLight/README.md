TrafficLight contains firmware for controlling the BLE113 through signal events on the GATT database.

Pins P0_3, P0_5 and P0_7, respectively, on the DKBLE113, are connected to Red, Amber and Green LEDs. The signal events are updated on the GATT database using BLEGUI2 and BLED112.
Signals can be sent using the "Write Command" option once you input signal code (0:Red, 1:Amber, 2:Green) into a characteristic.
