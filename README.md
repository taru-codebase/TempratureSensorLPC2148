# OBJECTIVE


The primary objective of this project is to design, develop, and implement a low-cost, reliable, and real-time temperature monitoring and alert system using an Arduino microcontroller and a SIM900A GSM module.
The specific objectives to achieve this aim are:
•
To interface a temperature sensor (such as the LM35 or DHT11) with the Arduino UNO to accurately read ambient temperature data.
•
To establish stable communication between the Arduino microcontroller and the SIM900A GSM module.
•
To program the Arduino to continuously compare the measured temperature against predefined minimum and maximum threshold values.
•
To automatically trigger and send an SMS alert to a pre-programmed mobile number via the SIM900A module when the temperature violates these thresholds.
•
To test and validate the complete system for reliability, accuracy, and timely alert transmission.


# METHODOLOGY



This project will be implemented in three main phases: system design, hardware integration, and software development.
First, the system architecture will be designed, defining the connections between the Arduino UNO, the temperature sensor (e.g., LM35/DHT11), and the SIM900A GSM module.
Second, the hardware will be assembled. The temperature sensor will be connected to an Arduino input pin, and the SIM900A module's TX/RX pins will be interfaced with the Arduino's serial pins. A valid SIM card will be inserted into the GSM module, and both modules will be connected to appropriate power supplies.
Third, the software will be developed using the Arduino IDE. The code will be written to:

1.Initialize and read data from the temperature sensor.

2.Continuously compare the temperature reading against preset maximum and minimum thresholds.

3.Send specific AT commands to the SIM900A module to send an SMS alert if a threshold is breached.

4.Listen for incoming SMS messages and reply with the current temperature upon receiving a "STATUS" command.
Finally, the integrated system will be tested to ensure sensor accuracy and reliable SMS communication before deployment.

# COMPONENTS USED
Hardware Components

•Arduino UNO

•SIM900A GSM/GPRS Module

•Temperature Sensor (LM35)

•SIM Card

•Jumper Wires

•Breadboard,Software Components

•Arduino IDE


# EXPECTED RESULTS 
Upon successful completion and testing of the project, the system will demonstrate the following functional outcomes:

•Successful Initialization: When powered on, the Arduino will initialize, the temperature sensor will provide stable readings, and the SIM900A module will successfully register with the 2G cellular network.

•Continuous Monitoring: The system will accurately read the ambient temperature from the sensor at regular, programmed intervals.

•Automated SMS Alert (Threshold Breach): If the measured temperature exceeds the predefined maximum (e.g., 30°C) the Arduino will automatically trigger the SIM900A module to send an alert SMS to the user's phone.

•SMS Status Reply: In response to the "STATUS" command, the system will read the current temperature and successfully send an SMS back to the user with the real-time data.

•Stable Operation: The system will run continuously without freezing, providing reliable monitoring as long as it has power and a cellular connection.
