STARPHEUS BOT
----

(foto proyecto completo)

Orpheus Bot It's a robot inspired by the Hack Club mascot (Orpheus).
Starpheus is a Wall-E type robot.
You can control it with a LogiTECH controller (you control its neck with an MG996R servo motor and the TT motors). 
It has 3 OLEDs that make up its eyes and mouth, simulates emotions with basic state machines (scared, happy, sleepy, neutral),
and uses an HC ultrasonic sensor to avoid collisions.
NOTE: this is a rlly full demo jsjjs 

Design
-------
The complete BOT is 31 cm tall, and 31 cm long counting the arms, its designed to look cool (idk if it is,for me it is), i wanted it to be like a Walle-E type.


<img width="1583" height="1025" alt="Captura de pantalla 2026-06-25 231214" src="https://github.com/user-attachments/assets/5b45980b-86ec-43b7-99fd-ab6a43da7123" />
The design was made so that our little Starpheus isn't heavy and has good mobility.

It has details to be able to put our components and hollow parts so that the chassis isn't heavy and has more mobility, as I already mentioned.

details:

holes for 3 OLED screens (2x 0.96 & 0.91 )
a reset button at the back
the ESP32-S3 connector at the back
the ultrasonic sensor in the front
and spots to attach the motors.

I'm an amateur, this is my biggest solo project so far, and I like to challenge myself.
Honestly, I struggled a lot with this project. I changed everything from one moment to the next thousands of times. It was going to have computer vision and an infrared sensor so you could pet it, it was going to be semi-autonomous, but it was very ambitious. This is the beginning of Starpheus; in the future, I’ll improve it and all these ideas will be more than just ideas. 


foto proyecto completo) 

Gallery 
--

PCB
---
<img width="650" height="642" alt="esquema" src="https://github.com/user-attachments/assets/c567d5f9-156c-44a7-b191-5b3382d18e65" />


<img width="1277" height="881" alt="esq" src="https://github.com/user-attachments/assets/304f0cc7-0606-48bf-84ae-abe0fbb28c1d" />


<img width="1918" height="1198" alt="Captura de pantalla 2026-06-24 214031" src="https://github.com/user-attachments/assets/6bb2b666-d774-465c-a368-070cd27421a1" />

CAD
---
<img width="751" height="978" alt="Captura de pantalla 2026-06-25 231259" src="https://github.com/user-attachments/assets/6189a05b-a693-42e1-bee5-32ee504c322e" />
<img width="1551" height="993" alt="Captura de pantalla 2026-06-25 225029" src="https://github.com/user-attachments/assets/bb8e06e1-9721-43c4-82b5-8ffb87222979" />
<img width="822" height="742" alt="Captura de pantalla 2026-06-25 231134" src="https://github.com/user-attachments/assets/3e80a1ba-ec18-4bc6-8048-4add605c5daa" />


Wiring Table 
<img width="1252" height="727" alt="image" src="https://github.com/user-attachments/assets/2af0afb4-d7e8-444b-a53e-8a248546cdf7" />

I made this EXCEL with all the connections :B

BOM 
--
| Component         | Description                                | Unit | Cost    | Distibutor    | Link                                                                                                                                                                        |
|-------------------|--------------------------------------------|------|---------|---------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ESP32-S3          | Micro Controler, send code to components   | 1    | $34.91  | Amazon        | LIANXUE Potente ESP32S3-DevKitC-1 Placa de desarrollo WiFi Microcontrolador Procesador ESP32S3-WROOM-1-N16R8 Placa de desarrollo de repuesto : Amazon.com.mx: Electrónicos  |
| DRV8833           | H bridge for motors and control PWM        | 1    | $111.00 | Amazon        | EC Buying DRV8833 - Módulo de driver de motor de doble puente H compatible con TB6612FNG PCB rojo : Amazon.com.mx: Herramientas y Mejoras del Hogar                         |
| OLED.96           | Display, shows data (orpheus eyes)         | 2    | $4.49   | Mercado Libre | https://articulo.mercadolibre.com.mx/MLM-705156753-display-pantalla-oled-128x64-096-para-arduino-_JM?searchVariation=63044404311                                            |
| OLED.91           | Display, shows data (orpheus mouth)        | 1    | $1.31   | AlliExpress   | Módulo OLED de 0,91 pulgadas 0,91 ""Blanco Azul 128X32 Pantalla LED LCD 0,91"" IIC Comunicar para Arduino - AliExpress 502                                                  |
| HC-SR04           | Ultra sonic sensor, meausres distance      | 1    | $2.96   | Mercado Libre | Sensor De Distancia Hc-sr04 Ultrasónico | Meses sin interés                                                                                                                 |
| IR                | infrared sensor, orpheus detects touch     | 1    | $4.88   | AlliExpress   | Módulo de Sensor Infrarrojo IR para Evitar Obstáculos, para Arduino, Coche Inteligente, Robot, Fotoeléctrico Reflectante de 3 Cables, Nuevo                                 |
| MG-996R           | Servo Motor, orpheus neck                  | 1    | $7.33   | Mercado Libre | Servomotor Mg996r / Mg995 Servo Motor | Envío gratis                                                                                                                        |
| dc engines        | Movement or orpheus bot                    | 2    | $4.00   | AlliExpress   | Motorreductor TT 1:48 3 a 6 V DC 200 RPM : Amazon.com.mx: Deportes y Aire Libre                                                                                             |
| buck converters   | For Voltage Protecction of the components  | 3    | $6.76   | AlliExpress   | Regulador de Voltaje LM2596 Buck Converter 3-40V a 1.5-35V 3A : Amazon.com.mx: Electrónicos                                                                                 |
| Resistors 1k      | Kit of resistores, It helps with voltages  | 3    | $1.67   | AlliExpress   | 100 piezas de resistores de película metálica de 1/4W, 1R ~ 1M ohmios, 100R, 220R, 330R, 1K, 1.5K, 2.2K, 3.3K, 4.7K, 10K, 22K, 47K, 100K, 100, 220, 330, 1K5, 2K2, 3K3, 4K7 |
| Capacitores 470uf | Kit of Capacitores, It helps with voltages | 3    | $1.21   | AlliExpress   | 5 uds 35V 470uF condensador electrolítico de aluminio 4V 10V 16V 25V 35V 100UF 220UF 330UF 470UF 680UF 1000UF 47UF 1500UF 10UF 22UF - AliExpress 502                        |
| Potobard          | Helps With the wiring                      | 1    | $3.41   | AlliExpress   | Destec Protoboard MB-102, 830 Puntos de Conexión, Placa de Pruebas Electrónicas : Amazon.com.mx: Industria, Empresas y Ciencia                                              |
| Wires Dupont      | Kit, Conects the components                | 1    | $1.79   | AlliExpress   | Cable Dupont macho a macho, 10CM, 40 piezas, fila de 2,54 MM, Cable de puente de placa de pruebas para cables eléctricos Arduino - AliExpress 13                            |
| Push Botton       | I added for a RST button of ESP32 ()       | 1    | $3.35   | Mercado Libre | Switch De Push, De Boton Redondo, Normalmente Abier | Au-105 Rojo | Envío gratis                                                                                            |

There are a lot of components, it's a bit tedious but worth it. I will implement an ESP32 Cam in the future and they cost 3 bucks because I have a spare one. I recommend buying lots of batteries!!

ASSEMBLY 
---
LICENSE
---
MIT license 

PS:(sorry for some gramatic errors and bad spelling, enlish is not my best lenguage)
thank you a lot hack club staff and people looking at this <3
