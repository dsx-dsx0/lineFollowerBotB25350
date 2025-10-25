# lineFollowerBotB25350
HELLO!
## WHAT HAS BEEN DONE:
This code used the PID algorithm for a line follower robot.
## HOW IT HAS BEEN DONE:
The algorithm was implimented by first calculating the relative position of the bot to the line using the weighted average of the 5 readings (giving one direction a higher value than the other).
The PID constants were set in such a way that the final correction_value (summation of P, I and D terms), is added to the right motor and subtracted form the left motor, to make the bot turn.
## RESOURCES:
1) All the links provided in the group.
2) LLMs (some details about their usage is given in the .ino file)
3) https://www.youtube.com/watch?v=fv6dLTEvl74&t=197s
4) https://www.youtube.com/watch?v=dQw4w9WgXcQ&list=RDdQw4w9WgXcQ&start_radio=1
## WHAT I HAVE LEARNED:
1) How PID algorithms work.
2) Why the 'D' part of PID is important, and 'PI' alone is not often enough.
3) Certain details about the hardware like, motors cant directly be connected to arduino, Basic physical design of a Line Follower (no application in the code, but i was curious, so i looked it up)
   , application of void setup() and void loop() and Serial.begin(),
   1)  motors cant directly be connected to arduino
   2)  Basic physical design of a Line Follower (no application in the code, but i was curious, so i looked it up)
   3)  application of void setup(), void loop(). Serial.begin(), Serial.println(), Serial.print(), pinMode(), digitalWrite(), analogWrite(), map()
4) Importance of sensor calibration irl.
5) Devices that give analog output (like the rpm of a motor), need to be connected to a pin with PWM capabilities (like ~5 and ~6 in arduino UNO).
6) How breadboards work, and their applications.
## PROBLEMS FACED:
1) My lack of deep knowledge on cpp.
2) Lack of testing capabilities of IR sensors in tinkercad left me unable to test and tune the PID algo.
3) The code may be inefficient in certain places.
4) It took my a while to understand PID.
## WHAT COULD HAVE BEEN DONE BETTER:
1) The code could have been much more cleaner.
2) No actual testing of the bot has been done. Therefore, the speed and accuracy could have been better.
3) I dont know what the actual base speed of the motor is. (although these details can be altered in the code).
