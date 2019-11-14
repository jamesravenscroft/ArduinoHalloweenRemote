# ArduinoHalloweenRemote

/*
  Blink is a necessary command to test out if the Arduino connection works.

  Turns an LED on for one second, then off for one second, repeatedly.

  Most Arduinos have an on-board LED you can control. On the UNO, MEGA and ZERO
  it is attached to digital pin 13, on MKR1000 on pin 6. LED_BUILTIN is set to
  the correct LED pin independent of which board is used.
  If you want to know what pin the on-board LED is connected to on your Arduino
  model, check the Technical Specs of your board at:
  https://www.arduino.cc/en/Main/Products

  modified 8 May 2014
  by Scott Fitzgerald
  modified 2 Sep 2016
  by Arturo Guadalupi
  modified 8 Sep 2016
  by Colby Newman

  This example code is in the public domain.

  http://www.arduino.cc/en/Tutorial/Blink
*/

// the setup function runs once when you press reset or power the board
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(LED_BUILTIN, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(1000);                       // wait for a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(1000);                       // wait for a second
}


From there we need to import the remote Data (coming soon).
I plugged in the props to a breadboard and assigned a pin to start and electrical charge when Button 1 was pressed, and Turn off when Button 2 was pressed. 

So there was a bit of learning in the electrical field that had to happen:
Arduino USB ports burn out under very little electrical overload. 
![Image of Yaktocat](https://github.com/jamesravenscroft/ArduinoHalloweenRemote/blob/master/IMG_7736.jpeg)
![Image of Yaktocat](https://github.com/jamesravenscroft/ArduinoHalloweenRemote/blob/master/arduinoElec.jpg)

  I got really excited when I had the code and the props and the breadboard, I had the Arduino running power off the USB connection, I press the remote button and suddenly the port isn't recongizable. I wasn't sure what the issue was, the driver had given me some issues before so I thought that was it.
  I just bought another Arduino, similar problem. I figured it out and ordered some more boards and transistors.
