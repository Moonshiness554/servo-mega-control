servo-mega-control
==================

Edit this file and see how to create syntax highlighting for the Arduino.

Note that Arduino code is really just `C`.

Three backticks (a key often tucked away beneath the ESC key), will signify the start.
Then place the language type (e.g. "C" or "Java")

```C
#include<Servo.h>

Servo myservo;

int potpin = 0;
int val;

void setup(){
  myservo.attach(9);
}

void loop(){
  val=analogRead(potpin);
  val=map(val, 0, 1023, 0, 179);
  myservo.write(val);
  delay(15);
}
```
finally end the code block with three back ticks, commit, and enjoy the :cool: syntax highlighting.
