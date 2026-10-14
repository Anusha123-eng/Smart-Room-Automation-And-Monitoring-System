Smart room systems communicate on a network of smart devices such as lights, fans, security cameras, and appliances, all of which can be controlled remotely. These devices communicate with each other using protocol like Wi-Fi enabling seamless interaction and automation. The primary benefits of smart home automation is convenience.

# Problem Statement
With the increasing demand for convenience and security in modern living, traditional home management systems often lack the integration and responsiveness required for effective automation. Homeowners face challenges such as the inability to remotely monitor and control devices, manage energy consumption efficiently, and ensure comprehensive security against unauthorized access. This project aims to develop a smart home automation and security system that seamlessly integrates various home devices, provides real-time monitoring and alerts, enhances energy efficiency, and offers robust security features to enhance the overall living experience.

# SYSTEM REQUIREMENTS

## Software Requirements
Software requirements describe the software and applications needed to run the Smart IoT Home Automation System.

The software requirements are:

**Laptop:** Used to write, edit, and upload the program.

**Android Phone:** Used to monitor and control home appliances.

**Blynk App:** Used to control appliances and receive notifications remotely.

## Hardware Requirements
The main hardware components required for the project are:

- **ESP8266:** A Wi-Fi-enabled microcontroller that connects the system to the internet and controls home appliances.
- **Relay:** An electrically operated switch used to turn appliances such as lights and fans ON or OFF.
- **Buzzer:** Produces an audible alarm when high temperature or unsafe conditions are detected.
- **DHT11 Sensor:** Measures temperature and humidity inside the home.
- **Servo Motor:** Controls door locking and unlocking by moving to specific positions.
- **GSM Module:** Sends SMS alerts and enables communication through a mobile network.
- **LED:** Provides lighting that can be controlled remotely using the mobile application.
- **Switches:** Allow users to control electrical appliances manually or through the automation system.
- **Light and Fan:** These appliances can be switched ON or OFF remotely to improve convenience and save energy.

**- SYSTEM DESIGN**

The  system  design for this includes two modules: 

• Home Appliances System 

• Security System 

• Circuit Diagram

<img width="319" height="272" alt="image" src="https://github.com/user-attachments/assets/34c118bc-1389-4b03-b507-8dcb2f10aa93" />

In this Figure firstly we should check the sensor value which are already uploaded in the cloud. If the temperature  value is above the threshold value, then the buzzer activates through this we can control and monitor the home appliances.   

<img width="335" height="368" alt="image" src="https://github.com/user-attachments/assets/29fe93ea-ca15-4ff5-8e51-211de7d1b5cf" />

In this figure  ESP8266 camera is on preview mode. If the person is detected then it will recognize the person face. If not detected then it will return switch to preview mode. After recognizing persons face if the person is known and authorized or owner, he can directly enter the password if it is valid, it opens the door. If the person is authorized but he is not the owner then he can get the password from the owner through communication. If the person is unknown and unauthorized the link will be sent to owner which in real time he can see the face of unauthorized person who is trying to enter the room and he can take security measures. 

**Home Appliances System**

The home appliances system is implemented using the ESP8266 microcontroller. It uses IoT technology to control and monitor home appliances such as lights and fans. The appliances can be controlled remotely using a smartphone through the Blynk application. Users can switch appliances ON or OFF from anywhere with an internet connection. Sensors can also help monitor home conditions and support automatic actions. This system improves convenience, saves energy, and makes home management easier.

<img width="296" height="151" alt="image" src="https://github.com/user-attachments/assets/eb39aed9-bb1d-4f1f-b6d0-0b77ef2ec143" />

# 4.2 Security System

The security system is implemented using the ESP32-CAM. The camera continuously monitors the entrance and detects people. If a person is detected, the system checks their face. If no person is detected, the camera returns to preview mode.

If the person is the owner, they can enter the correct password to unlock the door. If an authorized visitor arrives, they can request the password from the owner. If an unknown person tries to enter, the system sends a notification and a link to the owner to view the person's image in real time. This helps the owner monitor visitors and improve home security.

<img width="310" height="172" alt="image" src="https://github.com/user-attachments/assets/396df998-14f5-4d31-aade-88cc5accd7d0" />

**RESULT AND IMPLMENTATION**

<img width="288" height="135" alt="image" src="https://github.com/user-attachments/assets/24838fe6-b45a-4ff9-ad6a-88390839a64a" />

Shows the dashboard of the Blynk application in which it is connected to the ESP8266 sensor, it contains home appliances switches like LED, Fan. It also shows the value of current  temperature and humidity. 

<img width="295" height="148" alt="image" src="https://github.com/user-attachments/assets/a87e951a-500d-4c75-aa94-5abb15f92265" />

shows that both the switches are activated. It turns on both light and fan through Blynk app.

<img width="292" height="174" alt="image" src="https://github.com/user-attachments/assets/bea30618-12d9-493a-ad66-22b4d0b3004e" />

states that camera recognizes the authorized person and allow user to enter the room. 

<img width="309" height="188" alt="image" src="https://github.com/user-attachments/assets/20a59b95-69f2-4c5f-96fb-11e22252c131" />

shows that if authorized person trying to enter the room the door is automatically opened. 

<img width="317" height="183" alt="image" src="https://github.com/user-attachments/assets/df7bb73b-7c6f-4e19-b1c4-7fc7e7bcabad" />

states that camera detects the unauthorized person and the door remains unlock.

<img width="310" height="173" alt="image" src="https://github.com/user-attachments/assets/389ae6f9-5f2c-4ec9-aa5b-8a69446a182d" />

states that when unauthorized person entered the room it sends the alert message to owner. 

<img width="328" height="207" alt="image" src="https://github.com/user-attachments/assets/c7160432-1973-430a-ab6b-3d14769a484d" />

unauthorized person but he is known person.

<img width="311" height="171" alt="image" src="https://github.com/user-attachments/assets/616bd272-6c9a-4cea-9e20-445efb56a462" />

shows that if any unauthorized person trying to enter the room but he is known person. 

<img width="320" height="176" alt="image" src="https://github.com/user-attachments/assets/a9a7ef3b-4c6d-4001-971c-40c2bc351cd5" />

shown that Owner activates password to enter the room for known person.

<img width="297" height="177" alt="image" src="https://github.com/user-attachments/assets/1238c945-9b6b-4743-85ca-253229b64811" />

shows that if authorized person trying to enter the room the door is automatically opened.









