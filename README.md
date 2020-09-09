# Visitor-Counter-using-LPC2148-and-SSD
***
## Problem Statement
A C code and Proteus simulation to count number of persons entering a door of auditorium via an IR sensor connected and display count on seven segment using LPC2148


## Visitor Counter Application
1)The Visitor Counter using LPC Microcontroller circuit can be used domestically to get an indication of number of persons entering a restricted areas.

      a)Private Office/ Clinics.

      b)Social Events.

      c)Residential Apartments( having separate for visitors).

2)Further automation can be done to trigger an operate other energy equipment like lights, fans, AC units based on the counts.



## Components and Specifications
1) LPC 2138
2) Seven Segment Display CC
3) Resistor 10k
4) Capacitor 22pF
5) Battery 3.3V
6) Crystal
Button
7) Switch


## Functional Flow Diagram
https://github.com/NehaNevrekar/Visitor-Counter-using-LPC2148-and-Seven-Segment-Display/issues/1#issue-696531157


## Visitor Counter – Control Philosophy
1) The circuit works on the principle of IR sensing.

2) IR sensor detect presence of visitor & trigger input to LPC microcontroller.(Here, Push button is used in place of IR sensor to simulate the condition)

3) Based on the output from IR sensor, the microcontroller triggers output LOW or HIGH.

          a) In normal operation, the output from IR sensor is logic LOW(0v).

          b) In case of any interruption (detect person while crossing the IR beam), output from IR sensor is logic HIGH(+3.3v).

4) The transition from low to high, for each sensor pair is detected by the microcontroller and generates output to change the count on SSD.

5) A switch is used to ON/OFF the circuit as well as to RESET the SSD



## Algorithm
Step1: Start.

Step2: Switch ON the SSD.

Step3: Check for External interrupt at EINT3 using External interrupt button.

Step4: If there exist an interrupt, increment the count.

Step5: Display the count on SSD.

Step6: When count becomes 10, clear the interrupt.

Step7: Reset the Seven segment & end the interrupt.

Step8: Stop.


## Simulation



## Conclusion
-> We were successfully able to design and simulate a Visitor Counter using LPC Microcontroller.

-> The result hence obtained from the microcontroller was displayed on the SSD.

-> Resetting of the SSD was done using the switch which was also used to ON/OFF the circuit.

