# Pulse-Sensor-with-Arduino

# What is a Pulse Sensor?
The heart rate sensor measures your heart rate in Beats per Minute using an optical LED light source and an LED light sensor.

BPM:Beats Per Minutes 💓

Componet requirement:
1. Pulse sensor 
2. Arunio Nano/uno....
3. hook and loop for fasten(optinal)


**Please take a look a t the circuit diagram in  "Pulse Sensor_cd.jpg"

# SETUP:  
If you take look at the sensor , there are three wires with different colors ,  S means signal , positive (+) and negative(-)


S--> connect to A0 
+--> 5V 
---> GND


# Let's CODE:

STEP 1: add the library to your Arduino IDE ----> Pulse-Sensor.zip
 # HOW: GO TO SKTECH --> ICLUDE LIBRARY --> Add .zip library


A brief explanation of the three values you see in the Serial Plotter with the PulseSensorPlayground library:



# Value 1: Raw Pulse Signal   --->NOISE
Description: This is the raw data from the Pulse Sensor.

Purpose: Represents changes in light intensity caused by blood flow, creating a waveform.


# Value 2: Threshold  --->The PulseSensor Playground library uses the Threshold to filter out this noise.
Description: A static or nearly static value (e.g., 550) that the library uses to detect heartbeats.


# Value 3: Heartbeat Indicator
Description: A spike (e.g., 1000) that occurs each time a heartbeat is detected.


