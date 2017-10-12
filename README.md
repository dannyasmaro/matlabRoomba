# matlabRoomba
Digital Controls - Roomba Project 1
For the project, I created three Simulink library blocks: one ton initilizae the connection
between the roomba nad the rooWifi, onefor the Range Sensor State, and one for Left and Right 
Wheel Control. With these two Simulink blocks created, you can place them into navigation control based on the input to the
Roomba from sensor input, and output velocity requirements to the wheels of the
Roomba. I made use of the ```presistant``` Simulink Code to reference the same serialport
object for two of the Simulink blocks. 

