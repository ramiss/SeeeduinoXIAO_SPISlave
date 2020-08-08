# SeeeduinoXIAO_SPISlave

This repository provides a working Arduino SPI Slave example for the Seeeduino XIAO board. http://wiki.seeedstudio.com/Seeeduino-XIAO/) (ATSAMD21G18A). 

Thanks goes out to:
- jeremyherbert - https://github.com/jeremyherbert/playful-turtle-xiao
- The atmel SAMD21 library
- everyone at https://forum.arduino.cc/index.php?topic=360026.0
 
**Important notes:**

- The seeeduino xiao supports 0V to 3.3V digital signals. Connecting signals outside this range will likely cause permanent damage to the device.
- We are NOT using the default SPI pins per the Seeeduino documentation - we are reassigning these pins to SERCOM0.
- MOSI and MISO should be connected direct to the SPI master device - do not reverse/swap them. 
- If you are only receiving/listening, then you can leave pin MISO pin 4 disconnected.
- You can use Serial for USB and Serial1 for UART TX/RX
 
**Connection information:**

WARNING: Do not use the pinout information provided by seeedstudio. 

- SPI_MOSI  - Board Pin: 2 - Connect to MOSI on master
- SPI_SCK   - Board Pin: 3
- SPI_MISO  - Board Pin: 4 - Connect to MISO on master
- SPI_CS    - Board Pin: 5

![SeeeduinoXIAO_SPISlave_Wiring](https://i.imgur.com/GB6cOee.png)
