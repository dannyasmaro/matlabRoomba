Danny Asmaro 
Digital Controls - Dr. Li Bai - Temple University

## Project 1: Simulink Library for Roomba

## Instructions on Adding Roomba Libraries to Simulink library
1. Download Roomba libraries (including multiple .m files) to the MATLAB document folder
2. Locate the "slblocks.m" file
3. In MATLAB command window, enter addpath('directory') in which directory is the directory of the slblocks.m file
4. In MATLAB command window, enter savepath
5. In MATLAB command window, enter path to make sure that the MATLAB path includes the path to these directories
6. Open Simulink library browser and refresh the browser. The Roomba library should be seen in the browser, and blocks can be dragged or copied into Simulink models like the inherent blocks

The model for this project should have two constants connected to the left wheel and right wheel inputs as shown below:
![model](https://user-images.githubusercontent.com/31410235/33971660-a37662f4-e047-11e7-8f3c-27a6feced935.PNG)

For this project, we created three Simulink library blocks:
![capture](https://user-images.githubusercontent.com/31410235/33971098-c02a1df8-e044-11e7-95e3-d50d142bc554.PNG)

### First block for initializing the Roomba.
![capture2](https://user-images.githubusercontent.com/31410235/33971178-2ab6973c-e045-11e7-8706-8c12045e1d6e.PNG)
### Second block for the Range Sensor State (refer to RangeStateRoomba.m).
![irsensor](https://user-images.githubusercontent.com/31410235/33971181-2cededac-e045-11e7-8f2c-b411aac762fd.PNG)
### Third block for Left and Right Wheel Control (refer to SetWheelVelRoomba.m). 
![wheels](https://user-images.githubusercontent.com/31410235/33971184-2fd3a48a-e045-11e7-81f1-14b9746faad8.PNG)

Using these three Simulink blocks created, we place them into navigation control based on the input to the Roomba from sensor input, and output velocity requirements to the wheels of your Roomba. We were required to create a serialport object which needs to be the same for both Simulink blocks.We made use of the ```presistant``` Simulink Code to reference the same serialport
object for two of the Simulink blocks. 

