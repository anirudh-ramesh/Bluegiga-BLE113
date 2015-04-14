ArduinoUART contains firmware for accessing data over UART using an Arduino from InvenSense’s MPU6050 and for updating the GATT database.

References:
Firmware - http://www.sureshjoshi.com/development/ble112-uart-watermarks-example/
Hardware - http://invensense.com/mems/gyro/documents/PS-MPU-6000A-00v3.4.pdf

Hardware:
In the original scenario, UART1 had been chosen on the DKBLE113, without loss of generality.
There needs to be a logic level converter between the Arduino and the DKBLE113. (Schematic.jpg)
The sensor data is retrieved by the Arduino from InvenSense’s MPU6050.
