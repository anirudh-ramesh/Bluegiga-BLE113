MPU6050_raw contains firmware for accessing raw data from InvenSense’s MPU6050 over BLE.

References:
Firmware - http://www.sureshjoshi.com/development/ble112-communicating-with-mpu6050/
Hardware - http://invensense.com/mems/gyro/documents/PS-MPU-6000A-00v3.4.pdf

Hardware:
In the original scenario, the MPU6050 is connected to the DKBLE113, which has labelled pins for the I2C interface.

Software:
Set "Client Characteristc Configuration" to a value of 0100 using "Write" to begin accessing raw data on the BLEGUI2.
The raw data will be displayed in 12 bytes. The first 6 bytes is from the accelerometer and the next 6 bytes is from the gyroscope. Within each, there are 2 bytes from X, Y and Z in order.
Or, simply, raw data will be of the format Ax AY AZ GX GY GZ [spaces absent].
AX, AY and AZ are in two's complement format.
