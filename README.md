# GMAX4002 breakout board
A basic minimum GMAX4002 (1/1.7" 2048x1200 Global shutter) breakout board for Raspberry Pi
<img width="1891" height="1687" alt="image" src="https://github.com/user-attachments/assets/1bac498b-cdf8-45dd-bca5-283d80d76c7a" />

In general this is a simple breakout board for GMAX4002 sensor, see [here](https://github.com/will127534/gmax4002-v4l2-driver) on the driver side of things.
The caveat is that you will need to supply trigger pulses to the TEXP test point in order to trigger a new frame from the sensor and the board will not generate that signal for you, as such this is not really a complete board in my opinion but it might be easier for those who are taking this to integrate in their project.  

![_DSC9919](https://github.com/user-attachments/assets/c9388c6a-6204-44b7-9cee-850f717b9454)  
![_DSC0018](https://github.com/user-attachments/assets/8da226fc-3622-45d8-8cc0-da0c6635e797)  
![_DSC0022-2](https://github.com/user-attachments/assets/e122bc15-ab60-4fb7-ba24-ce8556489d06)  
See the action in video here: [Youtube](https://youtu.be/cdhxaaCYhbM).  
Note that the decoupling capacitor requirements from the leaked pre-released datasheet is a bit... over spec in my opinion(There is no F-way you need 2 x 22uF, 10uF and 100nF for each pixel voltage regulator), the board is deisgned following the datasheet but you can see in the board photos I've omitted some of the capacitors when soldering and it work just fine (I guess).  

At the very least this board has been tested on RPI5 with analog discovery 2 as pulse generating source. Currently I have no plan to continuing develop this board as a raspberry pi camera module but it might be useful for someone looking at this sensor also. Lastly, this project is released as MIT license, do what ever you want with that.
