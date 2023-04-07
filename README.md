# Indoor-air-quality-control

This is an Arduino code that detects using MQ-135 and DHT-11 sensors the amount of carbon dioxide and water vapour in air and triggers a buzzer alarm when their concentration passes safe levels

The code first checks if the concentration of  harmful gases is not safe, if so, it gives a fast buzzer warning (250 ms between sound warnings) . If not, it checks if the level is close to being harmful if so, it gives a slower buzzer warning (500 ms between sound warnings).
The loop of the code is infinite as when any order is executed, or a value check finishes it goes back to reading the values from sensors.


The circuit is made using "Circuito.io" site 

MQ-135 sensor which calculates the amount of carbon dioxide in ppm is connected to an Analog pin in Arduino (sends readings).

DHT 11 sensor which calculates the water vapor percentage is connected to a Digital pin (sends readings).

The buzzer is connected to a digital pin (receives commands).
