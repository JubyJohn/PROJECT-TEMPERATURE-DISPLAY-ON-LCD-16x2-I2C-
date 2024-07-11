# PROJECT TEMPERATURE DISPLAY ON LCD 16x2 I2C


## AIM
To display the temperature and humidity reading of DHT11 on LCD 16x2 I2C.


## COMPONENTS

1.	ESP8266 NodeMCU
2.	LCD 16x2 I2C
3.	DHT11
4.	Jumper Wire
5.	USB cable

## CONNECTION

### LCD16x2 I2C Module Pin Diagram
 
<br> VCC = power supply ---->  3V3
<br> GND = ground          ---->  GND
<br> SDA = serial data line   ---->  D2
<br> SCL = serial clock line   ---->  D1

### Push Button Pin Diagram

 

<br> VCC    = power supply  ---->  3V3
<br> DATA  = Output     ---->  D6
<br> GND   = ground   ---->  GND


## PROCEDURE

<br> Step 1 : Interface ESP8266 microcontroller to Arduino IDE using port.
<br> Step 2: Interface ESP8266 microcontroller with DHT11 and print temperture and humidity values on serial monitor.
<br> Step 3 : Interface ESP8266 microcontroller with LCD 16x2 I2C to display HI on LCD
<br> Step 4 : Interface ESP8266 microcontroller with LCD 16x2 I2C and DHT11 by modifying both the programs.


## PROBLEMS FACED

### Error 1 -   DHT_sensor library installation
#### How to rectify:
(1)  Need to find suitable library
https://chem.libretexts.org/Courses/Intercollegiate_Courses/Internet_of_Science_Things/7%3A_Appendix_5%3A_Microcontollers/2%3A_Read_Temperature_and_Humidity_with_DHT22
(2)  Open above link address -> download ZIP file
(3)  Go to Arduino IDE -> sketch -> include library -> add ZIP file -> downloads -> select downloaded zip file -> close
### Error 2 -   Not getting DHT22 sensor reading 
#### How to rectify:
(1)  On serial monitor it prints like
              Humidity: nan %  Temperature : nan*C      // not getting the readings 
(2)  Changed sensor , this error shows because of sensor complaint.


## OUTPUT
C:\Users\JUBY JOHN\Desktop\Projects\prjt 2 i2c&dht11\images

## REFERENCES
LiquidcrystalI2C- library : http://easycoding.tn/index.php/resources/
LiquidcrystalI2C- code : http://easycoding.tn/tuniot/demos/code/
Adafruit_Sensor library : https://github.com/adafruit/Adafruit_Sensor
DHT_Sensor library  :
 https://www.arduinolibraries.info/libraries/dht-sensor-library
DHT11 -code : https://chem.libretexts.org/Courses/Intercollegiate_Courses/Internet_of_Science_Things/7%3A_Appendix_5%3A_Microcontollers/2%3A_Read_Temperature_and_Humidity_with_DHT22


