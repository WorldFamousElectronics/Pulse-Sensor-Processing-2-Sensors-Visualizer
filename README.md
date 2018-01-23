# Multiple Pulse Sensor Visualizer  

This processing sketch will display data from two Pulse Sensors.

Processing is a creative coding language. If you don't have Processing on your computer, you can download it [here](www.processing.org).

First, follow [this tutorial](https://pulsesensor.com/pages/two-or-more-pulse-sensors) to familiarize yourself with the Arduino code.
## Modify Arduino Sketch
You will have to make one change to the example Arduino code. Near the top of the main page in the Arduino sketch TwoPulseSensors_On_OneArduino.ino there is the line

    const int OUTPUT_TYPE = SERIAL_PLOTTER;

Change that line to

    const int OUTPUT_TYPE = PROCESSING_VISUALIZER;

That will change the Serial output of the Arduino so that it can talk to this Processing sketch.

## Works with more than 2 Pulse Sensors
This sketch is set to process signals from 2 Pulse Sensors. If you would like to use more than 2 Pulse Sensors, you will have to adjust the variable `numSensors` at the top of the main code page to the number that you want to work with.

  **NOTE:** We don't make any guarantees for the functionality of this code with higher numbers of Pulse Sensors! 
