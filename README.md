
# VolvoMagicTunerStudio - release

## Supported car platforms:

 - [x] **Volvo ME7 P80, P2** - ECU OBD in-car reading/writing.
 - [x] **Volvo ME9 P1** - ECU OBD in-car reading/writing.
 - [x] **Ford ME9** with Volvo 2.5T engine - ECU bench writing/reading - (in-car OBD read/write probably works too - not
       tested yet).

_If you own Ford 2.5T ME9 car like Focus, Mondeo, S-Max, Kuga and would like to help with in-car tests - let me know :)_

## Supported interfaces:

 - [x] DICE
 - [x] Mongoose

Support for reading/clearing diagnostic trouble codes (DTCs), including detailed error descriptions.

* Writing to the flash memory is free and unrestricted.
* Reading from the flash memory is encrypted.
* Please contact me if you wish to decrypt the read content.

## How to use the app

### Select interface and car platform.  

Select you interface and your car platform. Then hit Connect. The Status bar at the top will turn green and display the message "Connected".

**WARNING** Make sure you select proper car platform!

<img width="755" height="491" alt="image" src="https://github.com/user-attachments/assets/e6106982-336e-45d4-81f3-566583c79b4f" />

### Reading flash:  
Hit _Flash read_ button.  
Next, in the newly opened window _Read flash_ and confirm.  
Leave default settings for standard ECU reading.  
Reading takes around 90-120s depending on the platform.

<img width="431" height="374" alt="image" src="https://github.com/user-attachments/assets/2b26a95f-f28c-4650-a983-ce70a114c5a8" />

### Writing flash:  
Hit _Write flash_ button.  
Next, in the newly opened window select the file you want to flash.  
Then _Write flash_ and confirm.
Leave default settings for standard ECU writing.  
Writing takes around 2-4mins depending on the platform. 

**WARNING** If you select a file that is not compatible with the car ECU, the application will most likely display a warning. Even so, ensure 100% that you are uploading the correct file for the appropriate platform. Do not flash random files found on the internet—even ones you have modified yourself—unless you are 100% certain of what you are doing. It is very easy to “brick” ECU, and an incorrect or poorly tuned file can even lead to damage to the engine itself.

<img width="422" height="473" alt="image" src="https://github.com/user-attachments/assets/d4502fa7-b0dd-44c1-9dee-7b138b86d3a6" />

### Reading/clearing errors:
Hit _Trouble codes_ button.
A new window will open, in which the automatic identification and scanning of all hi-speed CAN modules will begin.  
Vehicles typically feature two separate CAN networks. A low-speed network handles "internal" modules, such as door control units, the radio, the air conditioning system, airbags, etc. A high-speed network, on the other hand, is responsible for modules located in the engine compartment, for example, the engine control unit (ECU), the transmission control module (TCM), or the ABS system.
Currently, the application supports only the high-speed network.

<img width="641" height="392" alt="image" src="https://github.com/user-attachments/assets/76c6a5bf-6b74-45d9-b450-75d0af5cac4c" />

You can click on an error to open a window containing additional details and a snapshot of the state at the time the error occurred (a so-called "freeze frame").

<img width="501" height="548" alt="image" src="https://github.com/user-attachments/assets/b78c01f7-857b-40b3-babc-5fc68fee1136" />

**WARNING** Before clearing any error codes, be sure to take a screenshot of the codes and their associated freeze frames—that way, you can show them to your tuner!

---

Where to find me:
YT: volvome7magic
IG: volvoecutune
