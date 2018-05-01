# Arduino C

## About
I used Arduino C to program my Arduino.

## Setup
Download Arduino IDE https://create.arduino.cc/ or use online IDE

## The stack
Can be used to make and recieve HTTP requests
    - uses Ethernet.h library
    - need either an ethernet shield, wifi board or Arduino Yun

## Next Steps
- Explore other electronics that can be used with the arduino (motors, sensors, etc.)
- Program Arduino in C++ (extention to the C language, adds object orientation)

## Hello World

#include <LiquidCrystal.h>

LiquidCrystal lcd(12, 11, 5, 4, 3, 2);      // put your pin numbers here

void setup()
  {
  // setup code here, to run once:
  lcd.begin(16, 2);                 //LCD parameters
  lcd.print("hello, world!");
  }

void loop()
  {
  lcd.setCursor(0, 1);
  // print the number of seconds since reset
  lcd.print(millis() / 1000);
  delay(1000);
  }
