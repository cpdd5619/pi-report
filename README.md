# pi-report
#Introduction
Fire is the big problem in the word.It can cause property damage, casualties and health problems.According to the UNDR(United Nations Disaster Reduction) Programme,the direct economic losses caused by fires in 2022 alone exceeded $128 billion worldwide, with nearly 35% of cases failing to effectively contain the disaster due to delayed response or functional limitations of traditional smoke alarm systems.So the smoke alarm is a must in every building, it can effectively avoid the occurrence of fire and remind people to pay attention to refuge.Raspberry PI is an open source hardware platform with low cost (€35-75), low power consumption (5V/3A) and high scalability (GPIO, Wi-Fi/ Bluetooth).

#Target
1.Smoke can be accurately detected
2.Raspberry PI can run automatically

#System design
-Fittings
1. Smoke sensor
2. Buzzer
3. Dupont line
4. Lighter
-Operating system: Raspberry Pi OS Lite
-Core language: Python 3.9

#Implementation
Key Functionalities
Real-time monitoring
The MQ-2 sensor samples every 10 seconds with an adjustable threshold (default: concentration >300ppm triggers an alarm)
Local alarm
Buzzer sounds (85dB) + LED flashing red

#test experiment
Background of experiment design
1.In the dormitory room(10m**2)
2.clean air
experimental procedure
First we ues the pi to connect hotspot,then log in the pi,because there is no other gas in the room, the words "normal air" can be seen on the screen, which will appear every 10 seconds, then turn on the lighter to release the gas, and then slowly approach the smoke sensor, and then the words "sos, smoke detected" will appear on the screen, and then the buzzer will sound. Moving the lighter away from the screen will be followed by the words "normal air," which will cycle every ten seconds

#Application
1.Home security:When it rings, tell the family they need to escape
2.Factory monitoring:When it rings, you need to stop the production line and let the workers come to repair it
3.preservation of cultural relics:When it rings,notify relevant personnel to protect cultural relics
#Challenge and improvement
1.Smoke sensors are not very sensitive ,but it cannot detect smoke if it is too far
2.The buzzer is not very loud
3.The appearance is too simple

1.It can later be connected to 5g for the Internet of Things
2.It can be detected in milliseconds
3.It will send a message when it detected the smoke
4.It can analyze the situation and decide whether to call the fire

#conclusion
In this experiment, the system is designed to continuously monitor air quality and trigger alarms when smoke is detected. By using a digital output sensor, we eliminate the need for an analog-to-digital converter (ADC), simplifying the circuit and software implementation.This product is only suitable for small environments like dormitories, and when it comes to the big environment, it needs to be adjusted more. It provides a safe guarantee for small and medium-sized places and lays the foundation for subsequent products.It makes a big effect in a lot of little thingsEven though it has many limitations, it will become more and more perfect with the progress of Times.
