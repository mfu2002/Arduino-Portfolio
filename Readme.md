# Hero Projects

**IMU-based Wheelchair Navigation**
Default Password: EEE20003
Implements interrupt driven programming to collect, compute and indicate wheelchair movement direction.
proximity sensor feature to indicate when wheelchair is too close to an obstacle.
Saves and read sensor data to EEPROM.
https://wokwi.com/projects/346652160874775122
**Clock/Timer/Alarm Project**
Enter A or D (UpperCase) to switch between Analogue or Digital, respectively.
This can be done at any stage of the solution; it can be changed later.
default is the digital clock.
Hold the button (or key 5 on your keyboard) for 5 seconds to swtich between
display screen (Clock, Timer, Alarm).
On the Clock screen, short press (<5 sec) the button to toggle the temp display.
On the Timer screen, short press (<5 sec) the button to start and stop the timer
On the Alarm scree, hold the button for 2sec but less than 5sec to switch
between set hour, set minute and display alarm time state.
short press (<2 sec) on the set hour state will increment the alarm hour.
short press (<2 sec) on the set minute state will increment the alarm minute.
short press (<2 sec) on the display alarm state will toggle the alarm on and off.
the alarm hour and minute are saved in the EEPROM.
The temp is also indicated using LEDs. For temp >25, it is treated as hot therefore,
the red led will turn on. Temp that is >18 and <=25 is taken as warm and the amber
light will be on. For temps <= 18, the green light will be on.
https://wokwi.com/projects/343190939116765779

**LED Matrix Text Display**
Enter text in the serial monitor to display on the LED matrix.
This text can be changed at any time from the serial monitor.
press the button (or key 5 on your keyboard) for <=1 sec, to move the
text from left to right.
press the button for > 2 to move the text from right to left.  
 press the button >1 and <= 2, to change between three speed modes.
Constraint:
Only one button allowed.

https://wokwi.com/projects/344174393136513619

# Other Projects

Pass Borderline Task 1
Q1. Briefly describe what is the different between the void setup (), the void loop () and the main () function?

In C/C++ main is the entry point of the program. It is the function that is called when the application is started, and all other functions are called from there. In Arduino Programming language, the main function is not available. Instead, we have the setup and loop functions. Setup is called once at the start. It is used to set up all the program such as setting the input and output pins. Loop is called repeatedly. It is where the crux of the code is.

Q2. Write a program that will display your name and the ID number once in the serial monitor

void setup() {
// put your setup code here, to run once:
Serial.begin(9600);
Serial.println("Faisal - 103603923");

}
void loop(){

}

https://wokwi.com/projects/343940427983880788

Q3. Briefly describe the functions delay (), Serial.println(), Serial.begin(), pinMode().

Delay(x) pauses the program for x number of milliseconds.
Serial.println(str) prints the input to the serial monitor
Serial.begin(rate) sets the baud rate. It is the rate at which the data is communicate to the serial in bits per second.
pinMode(pin, mode) sets the pin to either input or output mode.

Q4. Write a program that will display the unit number and the unit's name at the beginning of the application and then repeatedly print (“Welcome to the lab session”) in every 2 seconds. (Require Demonstration)

https://wokwi.com/projects/340947330902524498

Q5. Write a program that will blink the inbuilt LED every 1 second.

void setup() {
Serial.begin(9600);
pinMode(LED_BUILTIN, OUTPUT);
}
void loop(){
digitalWrite(LED_BUILTIN, HIGH);
delay(50); // 0.05 seconds
digitalWrite(LED_BUILTIN, LOW);
delay(1000); // 1 second
}

https://wokwi.com/projects/340947344796156498

Q6. Write a program that will On the LED for 1 second and off the LED for 2 seconds. Make sure that the LED is connected to pin 7. (Require Demonstration)

https://wokwi.com/projects/343197471376147026

Q7. Briefly explain the common data types used in Arduino

void – means nothing.
Boolean – Saves true/false, 1/0.
Byte – store a value between 0 to 255 (inclusive).
Char – a single character such as ‘a’, ‘1’ or ‘)’.
Int – stores a numeric whole number between -32,768 to 32,767. However the range is different of different boards.
Unsigned Int – stores a number whole number between 0 to 65,535.
Float – stores a numeric decimal value between 3.4028235E+38 and -3.4028235E+38.

Q8. Write a simple program to find out the students mark (x) belongs to Higher Distinction, Distinction, Credit, Pass or fail. Add the screenshot for the following marks x= 45,55,60,80 (please use switch statements) (Require Demonstration)

https://wokwi.com/projects/343197540587405907

Q9. Write a simple program that will print the values from 1 to 10 in the serial monitor using a while loop. (Require Demonstration)

https://wokwi.com/projects/340947472817848915

Q10.Write a program that will print your name and the student ID three times in the serial monitor (Use for loop) (Require Demonstration)

https://wokwi.com/projects/340947532151521875

Q11. Write a program that will generate a random number under 300 for ten time and if the generated number is between 0-100 print A, if the generate number is 101-200 print B and if the generated number is 201-300 print C in the serial monitor. (Use if else if statements and for loop) (Require Demonstration)

https://wokwi.com/projects/340948025305203282

Q12 Write a function to for multiplication, Values needed to multiply be the inputs to the function and function should output the correct value. using the function multiply 16 x 15 and print the correct value in the serial monitor. (Require Demonstration)

https://wokwi.com/projects/343197903272018516

Pass Borderline Task 2
Q1. Connect the Arduino, write a program that will display your name and the ID number once in the serial monitor.

void setup() {
Serial.begin(9600);
Serial.println("Faisal Karim - 103603923");
}

void loop() {
// put your main code here, to run repeatedly:

}
https://wokwi.com/projects/340946529507344979

Q2. Connect 2 LEDs (remember to use 270 Ohm resistors). Write code to flash LED1 every 1 second and LED2 every 2 seconds. Flashing LED duration is 50 ms.

#define LED_1_PIN 13
#define LED_2_PIN 12

void setup() {
pinMode(LED_1_PIN, OUTPUT);
pinMode(LED_2_PIN, OUTPUT);
}

void loop() {
// put your main code here, to run repeatedly:
digitalWrite(LED_1_PIN, HIGH);
delay(50);
digitalWrite(LED_1_PIN, LOW);
delay(1000);

digitalWrite(LED_1_PIN, HIGH);
digitalWrite(LED_2_PIN, HIGH);
delay(50);
digitalWrite(LED_1_PIN, LOW);
digitalWrite(LED_2_PIN, LOW);
delay(1000);

}

https://wokwi.com/projects/340946455920378452

Q3. Connect 5 LEDs (remember to use 270 Ohm resistors). Write code to take input (a single number ranging from 1 to 5) from Serial monitor and light up the corresponding LED. Only one LED lit up at a time. (Require Demonstration)

https://wokwi.com/projects/340947043202630227
Q4. Write code to toggle the LED when the button is pressed. (Require Demonstration)

https://wokwi.com/projects/343942283332158036

Q5. Write code to dim the LED until off and then glow the LED to fully bright (Use PWM).

#define LED_PIN 9

void setup() {
pinMode(LED_PIN, OUTPUT);
Serial.begin(9600);
}

void loop() {
for(int i = 255; i >=0; i--){
analogWrite(LED_PIN, i);
Serial.println(i);
delay(5);
}
delay(100);
for(int i =0; i <= 255; i++){
analogWrite(LED_PIN, i);
Serial.println(i);
delay(5);
}
}

https://wokwi.com/projects/340951381173076564
Q6. Write code to change the volume of the piezo buzzer based on input from Serial monitor (Use PWM). (Require Demonstration)

https://wokwi.com/projects/341580495925019218

Q7. Connect the seven segment LED display, write code to display number from 9 to 0 (change every 1 second). (Require Demonstration)

https://wokwi.com/projects/343941839800238676

Pass Borderline Task 3&4
Q1. Connect OLED display to Arduino Mega. Write code to draw Olympic Rings symbol at centre of the OLED display. (require demonstration)

https://wokwi.com/projects/343942668086149715

Q2. Connect OLED display and HC-SR04 Ultrasonic Distance Sensor to Arduino Mega. Write a code to present the distance value from Ultrasonic sensor as a rectangle (height of the rectangle will be the same while the width of the rectangle will be changed based on the distance value). Display a certain simple text on OLED display based on the distance value: “Safe” when the distance >= 200, “Careful” when 80 <= distance < 200 and “Too Closed” when distance < 80. (require demonstration)

https://wokwi.com/projects/343198180525998674

Q3. Connect DS1307 RTC and LED Matrix with “chain” attribute is 5 to Arduino Mega. Write a code to display the current time from DS1307 RTC to LED Matrix with the speed value is 10, pause value is 100, and text alignment is PA_CENTER. (require demonstration)

https://wokwi.com/projects/343943407626879572

Pass Borderline Task 5
Q1. Write a program that displays the correct reading of the temperature in the immediate surrounding of the temperature sensor in Celsius and Fahrenheit using appropriate calibration steps on the serial monitor. (Require demonstration)

https://wokwi.com/projects/341394269421961812

Q2. Write a program that displays the correct voltage reading from the potentiometer as you dial it on the serial monitor. (Require demonstration)

https://wokwi.com/projects/343943615846810194

Q3. Store input from the serial monitor using EEPROM and only print from EEPROM if the single input contains exactly 9 integers every time some new characters are typed into the serial monitor. (Require demonstration)

https://wokwi.com/projects/341581323721245266

Q4. Write a program that turns on the LED when the push button is pressed and turns it off when the push button is pressed again and so on. Every time the push button is pressed, the state of LED is changed between ON and OFF. You are required to store this state of change with EEPROM so that in the rare event of a power reset, the previous state of LED can be restored. (Require demonstration)

https://wokwi.com/projects/343943891868713554 
Pass Borderline Task 6
Q1.Write a simple program to blink the LED every 5 second using timer interrupts (Do not use delay, millis, micros ) . (Require demonstration)

https://wokwi.com/projects/342036030090642003

Q2. Write a simple program to blink the inbuilt LED every 500 milliseconds. Connect two buttons to the Arduino (Button A & Button B) When A is pressed millis value should be printed in the serial monitor and when the B is pressed micros value should be printed in the serial monitor. (Use hardware interrupts) . (Require demonstration)

https://wokwi.com/projects/342041673518285395

Q3. Write a program to display “I love Swinburne” in the LED matrix. When the external button is pressed it should display your name. The text should move from left to right continuously.(Use LED Dot Matrix MA7219 and interrupts). (Require demonstration)

https://wokwi.com/projects/343198469386666580

Pass Plus Task
Q1. To design digital clock with few features. Connect OLED display to Arduino. Write program to display analog and digital clocks. At the beginning, the clock is set up using serial. A real time clock (RTC) module can be added as well. (Require demonstration)

https://wokwi.com/projects/343196788796162642

Q2. To design LED matrix with few features. Make a proper connection for 8×8 LED Matrix with resistors to the microcontroller. The LED matrix have to be constructed manually by using 64 units of LED as 8×8 LED Matrix. Display your name and scroll from right to left continuously. (Require demonstration)

https://wokwi.com/projects/344174479409152596

Credit Task
Q1. Continuing from Pass Plus Task 1 for designing digital clock with few features. Connect to a push button. Use the hardware interrupt to detect the button. If the button is pressed for certain seconds, it will convert to a stopwatch or back to be digital clock. While as stopwatch, the same button is used to start/stop the stopwatch (Require demonstration)
// Enter A or D (UpperCase) to switch between Analogue or Digital, respectively.
// This can be done at any stage of the solution; it can be changed later.
// default is the digital clock.
// Hold the button (or key 5 on your keyboard) for 5 seconds to swtich between
// display screen (Clock, Timer).
// On the Timer screen, short press (<5 sec) the button to start and stop the timer

https://wokwi.com/projects/344170889218097746

Q2. Continuing from Pass Plus Task 2 for designing LED matrix with few features. Use the serial for allowing change the text of the display and save it to memory. (Require demonstration)
// Enter text in the serial monitor to display on the LED matrix.
// This text can be changed at any time from the serial monitor.

https://wokwi.com/projects/344174457615549011

Distinction Task
Q1. Continuing from Credit Task 1 for designing digital clock with few features. Using the same button to have additional feature to set alarm system. Connect to a speaker for the output of the alarm. (Require demonstration)
// Enter A or D (UpperCase) to switch between Analogue or Digital, respectively.
// This can be done at any stage of the solution; it can be changed later.
// default is the digital clock.
// Hold the button (or key 5 on your keyboard) for 5 seconds to swtich between
// display screen (Clock, Timer, Alarm).
// On the Timer screen, short press (<5 sec) the button to start and stop the timer
// on the Alarm scree, hold the button for 2sec but less than 5sec to switch
// between set hour, set minute and display alarm time state.
// short press (<2 sec) on the set hour state will increment the alarm hour.
// short press (<2 sec) on the set minute state will increment the alarm minute.
// short press (<2 sec) on the display alarm state will toggle the alarm on and off.
// the alarm hour and minute are saved in the EEPROM.

https://wokwi.com/projects/343196064828883538

Q2. Continuing from Credit Task 2 for designing LED matrix with few features. Connect the pushbutton to the embedded system. Add additional feature with the button. If button press for 1 second or less, the text will moving from left to right. If press for button press more than 2 seconds, the text will move from right to left. . (Require demonstration)
// Enter text in the serial monitor to display on the LED matrix.
// This text can be changed at any time from the serial monitor.
// press the button (or key 5 on your keyboard) for <=1 sec, to move the
// text from left to right.
// press the button for > 2 to move the text from right to left.

https://wokwi.com/projects/344174422163194451 
High Distinction Task
Q1. Continuing from Distinction Task 1 for designing digital clock with few features. Connect the temperature sensor to the microcontroller. Using previous button to have additional feature to turn on/off displaying temperature on the OLED display. If it is activated, read temperature sensor and display on OLED display. Apply three threshold (cold, medium and hot) and connect to LEDs for RGB LED as the output (Require demonstration)
// Enter A or D (UpperCase) to switch between Analogue or Digital, respectively.
// This can be done at any stage of the solution; it can be changed later.
// default is the digital clock.
// Hold the button (or key 5 on your keyboard) for 5 seconds to swtich between
// display screen (Clock, Timer, Alarm).
// On the Clock screen, short press (<5 sec) the button to toggle the temp display.
// On the Timer screen, short press (<5 sec) the button to start and stop the timer
// on the Alarm scree, hold the button for 2sec but less than 5sec to switch
// between set hour, set minute and display alarm time state.
// short press (<2 sec) on the set hour state will increment the alarm hour.
// short press (<2 sec) on the set minute state will increment the alarm minute.
// short press (<2 sec) on the display alarm state will toggle the alarm on and off.
// the alarm hour and minute are saved in the EEPROM.
// The temp is also indicated using LEDs. For temp >25, it is treated as hot therefore,
// the red led will turn on. Temp that is >18 and <=25 is taken as warm and the amber
// light will be on. For temps <= 18, the green light will be on.

https://wokwi.com/projects/343190939116765779

Q2. Continuing from Credit Task 2 for designing LED matrix with few features. Additional features is need to be added with the same pushbutton to change up to 3 modes for speed of the moving text includes slow, medium and fast. (Require demonstration)

// Enter text in the serial monitor to display on the LED matrix.
// This text can be changed at any time from the serial monitor.
// press the button (or key 5 on your keyboard) for <=1 sec, to move the
// text from left to right.
// press the button for > 2 to move the text from right to left.  
// press the button >1 and <= 2, to change between three speed modes.

https://wokwi.com/projects/344174393136513619
