# LiFi-based-communication-between-two-stm32-boards


## OBJECTIVE
This project aims to build a light-based communication system using a laser module to transmit data patterns to a receiver equipped with an LDR (Light Dependent Resistor) module and LEDs. The goal is to send patterns as digital pulses and synchronize the transmitter and receiver systems for accurate data transfer.

## CONCEPTS USED
LiFi <br/>
•	Light Fidelity, a wireless method of communication using light instead of radio waves. The transmitter sends data in the form of laser light, which is received by the receiver’s LDR. The receiver captures the data and displays it via the LEDs.

## SYSTEM DESIGN
![WhatsApp Image 2024-11-04 at 23 15 11_34c0807c](https://github.com/user-attachments/assets/f275717b-6545-488a-a0f5-f89879a35cd9)

## Transmitter
•	GPIO Configuration: PA0 is configured to control the laser (ON/OFF), while PA1 serves as the synchronization pulse output. Buttons connected to PA2 and PA3 are used to select transmission patterns.<br/>
•	Two distinct patterns are defined (Button 1: 1001, Button 2: 0101)<br/>
•	Synchronization Pulse: A pulse on PA1 signals the start of each bit transmission, helping the receiver to know when to read each bit.

## Receiver
•	LDR Module: Connected to PA2, the LDR reads digital signals from the laser module to detect transmitted patterns.<br/>
•	LED Indicators: LEDs are connected to GPIO pins PA3-PA6 to represent each bit in the received pattern.

## Working Video
[![19CSE303 | Wireless Communication using LiFi | Group 15](https://i9.ytimg.com/vi/TGA5QlxO-nM/mqdefault.jpg?sqp=CICJyLkG-oaymwEmCMACELQB8quKqQMa8AEB-AH-CYAC0AWKAgwIABABGCogXyhlMA8=&rs=AOn4CLDkvAOuAPJJTiirA0nVo8pYbM6Ljw)](https://youtu.be/TGA5QlxO-nM)

## GROUP MEMBERS
•	CB.EN.U4CSE22412 – Charu Nethra<br/>
•	CB.EN.U4CSE22437 – Sarath Chandra<br/>
•	CB.EN.U4CSE22443 – Shaun Sunny<br/>
•	CB.EN.U4CSE22452 – Vaibhav V Shekar<br/><br/>

19CSE303 - Embedded Systems<br/>
Department of Computer Science and Engineering<br/>
Amrita School of Computing,<br/>
Amrita Vishwa Vidyapeetham, Coimbatore, India
