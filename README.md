# Project 1: Simulink Library for Roomba

Danny Asmaro 
Digital Controls - Dr. Li Bai 
Temple University

For this project, we created three Simulink library blocks:
![capture](https://user-images.githubusercontent.com/31410235/33971098-c02a1df8-e044-11e7-95e3-d50d142bc554.PNG)

- First block for initializing the Roomba.
![capture2](https://user-images.githubusercontent.com/31410235/33971178-2ab6973c-e045-11e7-8706-8c12045e1d6e.PNG)
- Second block for the Range Sensor State (refer to RangeStateRoomba.m).
![irsensor](https://user-images.githubusercontent.com/31410235/33971181-2cededac-e045-11e7-8f2c-b411aac762fd.PNG)
- Third block for Left and Right Wheel Control (refer to SetWheelVelRoomba.m). 
![wheels](https://user-images.githubusercontent.com/31410235/33971184-2fd3a48a-e045-11e7-81f1-14b9746faad8.PNG)

Using these two Simulink blocks created, we place them into navigation control based on the input to the Roomba from sensor input, and output velocity requirements to the wheels of your Roomba. We were required to create a serialport object which needs to be the same for both Simulink blocks.We made use of the ```presistant``` Simulink Code to reference the same serialport
object for two of the Simulink blocks. 


