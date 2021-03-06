# Why ESP8266?
A Wemos D1 Mini Pro is being used for the rapid prototyping of AAL solutions. The board is based in the ESP8266 chip with 16MB of on-board flash memory.

Some of its advantaged over other platforms include:
*  Cheap. These boards can be found for around 4$ from different manufacturers. There are other variants (D1 Mini) with less memory but the same capabilities for around 2$, but these were the ones we had around.
*  Open-source software. All the ecosystem is public and being actively developed in GitHub. It has a very big community made up of manufacturers and makers that has developed libraries for every imaginable hardware. This makes development cycles a breeze.
*  Libraries are available for different programming languages. The most used ones come from Arduino environment which is written in C++ but there's also the option to use MicroPython or even LUA by using the NodeMCU firmware. 
*  Open-source hardware. Schematics and PCB designs are also available in easy-to-modify standard formats able to be opened from KiCAD or EAGLECAD. There are all kind of derived products: Some have built-in battery controllers, others have the option of adding an external antenna... There are also shields to allow adding external hardware without the need to use any cables.
*  32-bit microcontroller, much more powerful than typical Arduino-compatibles which use ATMEGA's 8-bit architecture. They are not as powerful as to allow a Linux kernel inside, but this is usually not needed for Cloud-based IoT. 
*  Full Wifi stack. The board can act as an Access Point or as a Station and can switch from one mode to another while running with no external hardware needed. Other wifi-related advantages are the ability to do Over The Air programming or the rapid deployment of Mesh Networks.
*  Low-power consumption. [Real-world tests](https://openhomeautomation.net/esp8266-battery) measure less than 90mA while sending data over wifi and can go lower than 10mA while using the included sleep modes.
*  On-board USB to UART converter, so no external programmers are required. This also allows to easily debug over serial while prototyping.
*  Actively used by the industry in real-world scenarios. The prime example is iTead's sonoff line which is based on this chipset, but there are a million chinese and occidental manufacturers which are basing their IoT developments around it. This allows [community-made firmwares](https://github.com/xoseperez/espurna/wiki/Hardware) to be deployed in actual commercial products.

Once the rapid prototyping phase is over, the ESP8266 is available in other formats, like the ESP12, which allow direct deployment into final PCB's with little to none modifications to the schematics. 

They are also prepared to be soldered as a SMD component directly into PCB's, so no external headers are needed.

They are typically sold for around 1,5$, much less if bought in bulk. The cost-reduction comes from the fact that some components are removed, like the USB-UART converter which is typically not needed in a final product.