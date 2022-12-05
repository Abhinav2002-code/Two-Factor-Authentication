# Two-Factor-Authentication


 The main component in the circuit is 8051 microcontrollers. This controls
everything in the device.

We connected LCD to the 8051 and configured it to display a welcome message
at first and then it waits for input from the keypad

We connected the 4x3 keypad with the microcontroller. In the keypad there are 4
rows which indicate the letters (A-D) and the 3 columns which indicate the
number (1-3).

In the 8051 controller, pin P0.0 to P0.3 are connected to the keypad rows and pin
P0.4 to P0.6 are connected to the keypad columns.

If password is correct for specific user, then one factor of authentication is done
for that user which will be shown on LCD as “WELCOME USER”.

If user input wrong password it will give another chance to input the password
again with an error message.

Then for the second RFID authentication the LCD display “SCAN YOUR
CARD”.

RFID reader is connected to TX and RX pins of MCU.

When the specific user card is tapped to the reader then only it gives access.

We connected the door lock motor pins in the P2.3 and P2.4. This motor only
works when the right user’s card is tapped.

LCD’s points are connected with P3.5 to P3.7 in 8051. LCD helps us to show the
inputs and error messages.

All devices are connected with each other. In the simulation we use the hex code
to run the program. The hex code is generated from the embedded C code. This
code only works on any 8051-microcontroller system.

To run the simulation, we set the clock frequency at 11.0592 MHZ for 8051. This
has allowed us to run the simulation without getting any errors.

![Screenshot (72)](https://user-images.githubusercontent.com/74583384/205563442-612b903c-d86e-4d0d-bc0a-3a4f16dd2294.png)

The code for above process is uploaded in the repository.

Done By- 

Abhinav Putrevu

Geda Siva Ram Chowdary

Saicharan Anipakala

Saicharan Pendyala
